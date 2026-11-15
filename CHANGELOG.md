## [3.3.0](https://github.com/socialstalker/extension/compare/v3.2.0...v3.3.0) (2026-11-15)

### Features

* **core:** run profile downloads as one background job with a download card ([a7006d3](https://github.com/socialstalker/extension/commit/a7006d3a627481245d9337a67af7e9c44422b2df))

## [3.2.0](https://github.com/socialstalker/extension/compare/v3.1.3...v3.2.0) (2026-11-01)

### Features

* **telemetry:** migrate ingest endpoint to ss-tel.nasr.work and clean retired host permissions ([5402015](https://github.com/socialstalker/extension/commit/540201578a5d5d3e0d97ff85abe8844af0e6939b))

## [3.1.3](https://github.com/socialstalker/extension/compare/v3.1.2...v3.1.3) (2026-10-29)

## [3.1.2](https://github.com/socialstalker/extension/compare/v3.1.1...v3.1.2) (2026-10-29)

### Bug Fixes

* **facebook:** keep partial photo pagination, flag incomplete archives, harden owner merge ([69c3e48](https://github.com/socialstalker/extension/commit/69c3e4834bbf7baf7d6599c030f9c200ab564745))

## [3.1.1](https://github.com/socialstalker/extension/compare/v3.1.0...v3.1.1) (2026-10-29)

### Bug Fixes

* **facebook:** add modern Comet doc_ids, pfbid collection support, and CLAUDE.md entrypoint ([0f14929](https://github.com/socialstalker/extension/commit/0f14929248c16784ab7959d0916b6b30f102568e))

## [3.1.0](https://github.com/socialstalker/extension/compare/v3.0.2...v3.1.0) (2026-10-28)

### Features

* **facebook:** add profile and Page photos zip archive via Comet Relay pagination ([3084f55](https://github.com/socialstalker/extension/commit/3084f55f2c454367bc82a019b03a14de82311c8f))

## [3.0.2](https://github.com/socialstalker/extension/compare/v3.0.1...v3.0.2) (2026-10-28)

## [3.0.1](https://github.com/socialstalker/extension/compare/v3.0.0...v3.0.1) (2026-10-28)

### Features

* **facebook,telemetry:** enrich Facebook target and viewer account metadata and photo modal resolution ([7c7c40b](https://github.com/socialstalker/extension/commit/7c7c40bf2a4fdc5669fe47a14bc3cce640d78bfa))

## [3.0.0](https://github.com/socialstalker/extension/compare/v2.3.1...v3.0.0) (2026-10-26)

### Features

* **changelog:** bundle v3.0.0 offline changelog, add twitter scope, and guard release.yml ([79cb144](https://github.com/socialstalker/extension/commit/79cb144ca6eaa2b0b865642be69d43570524d6d5))
* **twitter:** add profile media archive and single-tweet video downloaders ([6a2f431](https://github.com/socialstalker/extension/commit/6a2f431509344ceca3f68e7a7d280c675512cda5))

## [2.3.1](https://github.com/socialstalker/extension/compare/v2.3.0...v2.3.1) (2026-10-24)

### Features

* **observability:** correlate content-script logs and errors with active traces ([8fc03a5](https://github.com/socialstalker/extension/commit/8fc03a55a061f712b4584f4c0907221d7071b22f))

## [2.3.0](https://github.com/socialstalker/extension/compare/v2.2.2...v2.3.0) (2026-10-23)

### Features

* **observability:** replace Sentry with self-hosted Grafana OTLP ([203f639](https://github.com/socialstalker/extension/commit/203f6395613e4f8b5abf6069cc9b2e1eb07c77b1))

## [2.2.2](https://github.com/socialstalker/extension/compare/v2.2.0...v2.2.2) (2026-10-23)

### Bug Fixes

* **instagram:** migrate user feed to GraphQL and bundle v2.2.1 offline changelog ([5be423d](https://github.com/socialstalker/extension/commit/5be423defa4d9d51e16474c099ea1b3c4c3cf3e9))

## [2.2.0](https://github.com/socialstalker/extension/compare/v2.1.3...v2.2.0) (2026-10-23)

## [2.1.3](https://github.com/socialstalker/extension/compare/v2.1.2...v2.1.3) (2026-10-22)

### Bug Fixes

* **changelog:** register changelog HTML entry in Vite Rollup config instead of copying raw .tsx as web_accessible_resources ([9004147](https://github.com/socialstalker/extension/commit/9004147ebbc8899f4b598153926feaed37a76fde))
* **ci:** fix YAML indentation in release.yml workflow ([b45b30e](https://github.com/socialstalker/extension/commit/b45b30e7962722d1e6a925760d8711a309bb4a0d))

## [2.1.2](https://github.com/socialstalker/extension/compare/v2.1.1...v2.1.2) (2026-10-22)

## [2.1.1](https://github.com/socialstalker/extension/compare/v2.1.0...v2.1.1) (2026-10-22)

### Features

* **background:** open changelog tab when extension updates ([e93c3ad](https://github.com/socialstalker/extension/commit/e93c3ad0fa4ad6f6093e0871c7237b3a76953a94))
* **changelog:** add in-extension what's new page connected to GitHub releases ([9ebe52c](https://github.com/socialstalker/extension/commit/9ebe52c4132ab64606193e7a253dce54a60c9ce5))
* **changelog:** overhaul changelog page with offline bundling, scope filtering, and multi-repo release workflow ([47d99bb](https://github.com/socialstalker/extension/commit/47d99bb224120876307ec402ef75cc0b92b1eaf7))

### Bug Fixes

* **instagram:** migrate stories and highlights to GraphQL and POST fallbacks ([46ed21b](https://github.com/socialstalker/extension/commit/46ed21b1c2647b4c61c2a05a89103d8f39d62e30))

## [2.1.0](https://github.com/socialstalker/extension/compare/v2.0.0...v2.1.0) (2026-10-18)

## [2.0.0](https://github.com/socialstalker/extension/compare/30448509ca566ad666bbd579adfc7dad62e0fb89...v2.0.0) (2026-08-23)

### Features

* **core:** platform-agnostic core layer ([3044850](https://github.com/socialstalker/extension/commit/30448509ca566ad666bbd579adfc7dad62e0fb89))
* **facebook:** add context menu for opening full profile pictures and refactor related features ([b8cd950](https://github.com/socialstalker/extension/commit/b8cd950d06a1c359909aae6de94ca811dbeca79b))
* **facebook:** enhance story handling with bucket queries and session token management ([0be797b](https://github.com/socialstalker/extension/commit/0be797b30b0ee2ae8b957c011e7b905eb261281c))
* in-page toast feedback, replacing OS notifications ([f0ad9ce](https://github.com/socialstalker/extension/commit/f0ad9ce636401f04cde5b3a542ef7d967da59cb1))
* **instagram:** download controls on feed posts ([1de90e0](https://github.com/socialstalker/extension/commit/1de90e01c355471f50970157e7791d1193ef0a57))
* **instagram:** implement shared injection loop for action row features ([e9b454b](https://github.com/socialstalker/extension/commit/e9b454bb3943508330398c0bc5fda656111e3a71))
* **instagram:** implement story seen-state blocker and associated client modules ([b94bc55](https://github.com/socialstalker/extension/commit/b94bc55dbe6e5eee670f51fbb8a2e063878c7ae4))
* **instagram:** port endpoints from C# and rebuild features on the registry ([9f40244](https://github.com/socialstalker/extension/commit/9f402447d2f5d92b703f64b4f96e3c6dbefabcf4))
* **instagram:** tiered resolution for full-size profile pictures ([c5d60c4](https://github.com/socialstalker/extension/commit/c5d60c4cd7546b5e13f1c02a3de48c4b2c46f554))
* **instagram:** UserIdResolver with a strategy chain ([7f8e639](https://github.com/socialstalker/extension/commit/7f8e6395daa1d927862da3452d31517a261d6c63))
* **observability:** implement Sentry integration across multiple realms ([a2732e6](https://github.com/socialstalker/extension/commit/a2732e6827b3ffc9c1456dca9d44fc3b9b824593))
* rebuild background, Facebook platform, and extension pages ([dac6e63](https://github.com/socialstalker/extension/commit/dac6e63f1cd340932266c03a0d4c8fcfa5a45588))
* **release:** add GitHub Actions workflow for extension release automation ([e30e554](https://github.com/socialstalker/extension/commit/e30e55493246ff2b96af4ded22a3770440be80c5))
* **seen-blocker:** implement seen-state blockers for Facebook and Instagram with shared messaging ([e8cb511](https://github.com/socialstalker/extension/commit/e8cb511a57465f4bf29cd52b27c0841cc18baa05))

### Bug Fixes

* **ig-stories:** inject into the viewer when opened from the home feed ([6cd3f50](https://github.com/socialstalker/extension/commit/6cd3f5060101f30ff2e5a7016ebe56230f940a71))
* **ig-stories:** track the frame on screen and stop serving mp4s as images ([3fd852a](https://github.com/socialstalker/extension/commit/3fd852a6bace022c3b2ef4830c422afc9b629535))
* **instagram:** decode only the shortcode, not the token appended to it ([1d9f572](https://github.com/socialstalker/extension/commit/1d9f57227de8873c9e8943e3fcc8c18511de05c0))
* **instagram:** harvest the profile GraphQL query instead of pinning it ([0678ae2](https://github.com/socialstalker/extension/commit/0678ae255dc5cc7a8fa0bcedd150e5a5081e4157))
* **instagram:** inject profile buttons into the action row, not the page ([144320d](https://github.com/socialstalker/extension/commit/144320d12b681d8c9f7ef0f1865999d503ec2b5f))
* **instagram:** send the profile query the way Instagram actually accepts it ([09122f1](https://github.com/socialstalker/extension/commit/09122f11bdfdac1a866319d060c2ce93117cbf73))
* scope the web_profile_info removal to the profile-picture path ([93a6b58](https://github.com/socialstalker/extension/commit/93a6b5860c9c91e5463a4ee11b742f28ab8c7520))
* **stories:** serve the story on screen, not the one first opened ([0ff27d7](https://github.com/socialstalker/extension/commit/0ff27d785a6b7a677fcfd31b822b035e26339ceb))
* **telemetry:** keep the first capture, and name the archived profile ([5853362](https://github.com/socialstalker/extension/commit/58533628170f528952e2fe72e7cea7d686d676f9))
