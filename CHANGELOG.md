# Changelog

All notable changes to the SocialStalker Chrome Extension are documented in this file.
This project adheres to [Semantic Versioning](https://semver.org/) and follows the [Keep a Changelog](https://keepachangelog.com/) standard.

---

## [2.1.0] - 2026-10-18

### Features & Improvements
* **Instagram (User ID Resolution)**: Added multi-strategy user ID resolver utilizing profile HTML parsing and GraphQL post lookups, ensuring reliable downloads on private or restricted profiles.
* **Instagram (Endpoints)**: Updated rotating GraphQL document IDs and query variables following Instagram web bundle updates, retaining legacy endpoints as automatic fallbacks.
* **Instagram (Story Downloads)**: Added metadata recovery fallback that extracts story identifiers directly from intercepted network payloads when username resolution is delayed.

---

## [2.0.0] - 2026-08-23

### Features & New Capabilities
* **Core Architecture**: Rebuilt extension around a platform-agnostic core layer with declarative route matching, observer lifecycle management, and typed background messaging.
* **In-Page Feedback**: Replaced OS desktop notifications with an in-page toast notification system matching the SocialStalker High-Contrast Brutalist design system.
* **Facebook**: Added context menu integration for opening full-resolution profile pictures in a new tab.
* **Facebook**: Implemented bucket query story extractor with automated session token refresh.
* **Facebook & Instagram (Seen Blocker)**: Added MAIN-world seen-state blocker that intercepts outgoing delivery receipts and story view pings before leaving the browser.
* **Instagram**: Injected native download controls directly into action rows on feed posts, reels, and story viewers.
* **Instagram**: Introduced tiered resolution fallback chain for profile pictures, guaranteeing the highest possible resolution available.
* **Observability & Privacy**: Integrated Sentry error monitoring across all three execution realms (content script, MAIN world, service worker) with strict credential scrubbing for cookies, CSRF tokens, and auth signatures.

### Bug Fixes
* **Instagram Stories**: Fixed injector failing to mount when story viewer was opened directly from the home feed tray.
* **Instagram Stories**: Fixed frame-tracking bug where paused video stories were incorrectly saved as 0-byte image files instead of streaming MP4 files.
* **Instagram**: Fixed GraphQL profile resolution failure by stripping tracking tokens appended to shortcodes.
* **Instagram**: Fixed query failures by harvesting dynamic GraphQL document IDs directly from active page bundles.
* **Instagram**: Fixed injected button positioning by anchoring buttons within native action rows rather than relative to outer container bounds.
