# Changelog

All notable changes to the SocialStalker Chrome Extension are documented in this file.
This project adheres to [Semantic Versioning](https://semver.org/) and follows the [Keep a Changelog](https://keepachangelog.com/) standard.

---

## [2.1.2](https://github.com/socialstalker/extension/compare/v2.1.1...v2.1.2) - 2026-10-22

### Features & Capabilities
* **Core (Offline-Bundled Changelog)**: Overhauled the changelog page with SocialStalker High-Contrast Brutalism, featuring version navigation, search, and platform scope filters (Instagram, Facebook, Stories, Core) that load instantly offline with zero API rate limits ([99c67f8](https://github.com/socialstalker/extension/commit/99c67f8863d5dea16c8dba013bce23aafd2645ef)).
* **Core (Multi-Repo Distribution)**: Decoupled private extension source code from public distributions. All releases, signed CRX packages, and verified unpacked ZIP archives are now published directly to the public `socialstalker/releases` repository ([99c67f8](https://github.com/socialstalker/extension/commit/99c67f8863d5dea16c8dba013bce23aafd2645ef)).

### Bug Fixes & Stability
* **Core (Changelog Compilation)**: Registered the changelog HTML entrypoint directly in Vite Rollup inputs instead of copying raw `.tsx` source files as `web_accessible_resources`, fixing the blank screen when the changelog tab opened ([68e9ff1](https://github.com/socialstalker/extension/commit/68e9ff1)).

---

## [2.1.1](https://github.com/socialstalker/extension/compare/v2.1.0...v2.1.1) - 2026-10-22

### Features & Capabilities
* **Core (Automated What's New)**: The extension now automatically opens a dedicated release notes tab upon auto-update via `chrome.runtime.onInstalled` ([52e9830](https://github.com/socialstalker/extension/commit/52e98307307f0468cac8603d92bb700378892481)).

### Bug Fixes & Stability
* **Instagram (Stories & Highlights)**: Migrated reel and story fetching from fragile REST endpoints to authenticated GraphQL document queries and POST fallbacks, preventing media resolution failures when Instagram returns 400 Bad Request on legacy query params ([6fea859](https://github.com/socialstalker/extension/commit/6fea8595a230cacbba4749e50acc30da426890d6)).

---

## [2.1.0](https://github.com/socialstalker/extension/compare/v2.0.0...v2.1.0) - 2026-10-18

### Features & Improvements
* **Instagram (User ID Resolution)**: Added multi-strategy user ID resolver utilizing profile HTML parsing and GraphQL post lookups, ensuring reliable downloads on private or restricted profiles ([40b38d9](https://github.com/socialstalker/extension/commit/40b38d941332f15257d039c350a8dcab8369a5bc)).
* **Instagram (Endpoints)**: Updated rotating GraphQL document IDs and query variables following Instagram web bundle updates, retaining legacy endpoints as automatic fallbacks ([40b38d9](https://github.com/socialstalker/extension/commit/40b38d941332f15257d039c350a8dcab8369a5bc)).
* **Instagram (Story Downloads)**: Added metadata recovery fallback that extracts story identifiers directly from intercepted network payloads when username resolution is delayed ([40b38d9](https://github.com/socialstalker/extension/commit/40b38d941332f15257d039c350a8dcab8369a5bc)).

---

## [2.0.0](https://github.com/socialstalker/extension/commits/v2.0.0) - 2026-08-23

### Features & New Capabilities
* **Core Architecture**: Rebuilt extension around a platform-agnostic core layer with declarative route matching, observer lifecycle management, and typed background messaging ([e1b9f85](https://github.com/socialstalker/extension/commit/e1b9f85c9faa617a72c7becd221d04d9b32e83de)).
* **In-Page Feedback**: Replaced OS desktop notifications with an in-page toast notification system matching the SocialStalker High-Contrast Brutalist design system ([fbc6193](https://github.com/socialstalker/extension/commit/fbc619380c90e5d3fe0c902dbffa58c99059e163)).
* **Facebook**: Added context menu integration for opening full-resolution profile pictures in a new tab ([c414448](https://github.com/socialstalker/extension/commit/c414448dcfa191cb1dfe304b0adc8a42ca3b0235)).
* **Facebook**: Implemented bucket query story extractor with automated session token refresh ([9a535d9](https://github.com/socialstalker/extension/commit/9a535d99c270497de9d69a27f792c226d23c94c2)).
* **Facebook & Instagram (Seen Blocker)**: Added MAIN-world seen-state blocker that intercepts outgoing delivery receipts and story view pings before leaving the browser ([5a32245](https://github.com/socialstalker/extension/commit/5a3224534d5bfd60286d45d1e4ceb0c3421cf255), [1f4dd3e](https://github.com/socialstalker/extension/commit/1f4dd3e688960fcd5d679993282ee419b2b65c6e)).
* **Instagram**: Injected native download controls directly into action rows on feed posts, reels, and stories ([4380a93](https://github.com/socialstalker/extension/commit/4380a935a23d0d651d0f460f0bbfdd5d813c9d08), [7218b8d](https://github.com/socialstalker/extension/commit/7218b8dc0308c6106727793b1f33874f4f66c02c)).
* **Instagram**: Introduced tiered resolution fallback chain for profile pictures, guaranteeing the highest possible resolution available ([bf373e3](https://github.com/socialstalker/extension/commit/bf373e324ab09f51979d30e0c352e5e8fbe8763e)).
* **Observability & Privacy**: Integrated Sentry error monitoring across all three execution realms (content script, MAIN world, service worker) with strict credential scrubbing for cookies, CSRF tokens, and auth signatures ([dc34d93](https://github.com/socialstalker/extension/commit/dc34d93a78627ca20ea69fe7f625d2bb9cb97a1c)).

### Bug Fixes & Stability
* **Instagram Stories**: Fixed injector failing to mount when story viewer was opened directly from the home feed tray ([efa1de9](https://github.com/socialstalker/extension/commit/efa1de9e0e7acb359cf8d63f5e24c5f9dae8e6e1)).
* **Instagram Stories**: Fixed frame-tracking bug where paused video stories were incorrectly saved as 0-byte image files instead of streaming MP4 files ([a4a9b85](https://github.com/socialstalker/extension/commit/a4a9b85432f4da2435f32f265acad376b99e930d)).
* **Instagram**: Fixed GraphQL profile resolution failure by stripping tracking tokens appended to shortcodes ([be557e4](https://github.com/socialstalker/extension/commit/be557e44ad8f5ff365b048520a245695a9ba90bc)).
* **Instagram**: Fixed query failures by harvesting dynamic GraphQL document IDs directly from active page bundles ([f1788ff](https://github.com/socialstalker/extension/commit/f1788ffa2b607f38f8b4191d78a1a236d6809bfe)).
* **Instagram**: Fixed injected button positioning by anchoring buttons within native action rows rather than relative to outer container bounds ([af608ae](https://github.com/socialstalker/extension/commit/af608aef3a50eb2e6eefc3484a9a4243654505b2)).
