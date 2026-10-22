## [2.1.1](https://github.com/socialstalker/extension/compare/v2.1.0...v2.1.1) (2026-10-22)

### Features

* **background:** open changelog tab when extension updates ([52e9830](https://github.com/socialstalker/extension/commit/52e98307307f0468cac8603d92bb700378892481))
* **changelog:** add in-extension what's new page connected to GitHub releases ([20042fe](https://github.com/socialstalker/extension/commit/20042fe69be58154390e89709a16b3b4bcf7306c))
* **changelog:** overhaul changelog page with offline bundling, scope filtering, and multi-repo release workflow ([99c67f8](https://github.com/socialstalker/extension/commit/99c67f8863d5dea16c8dba013bce23aafd2645ef))

### Bug Fixes

* **instagram:** migrate stories and highlights to GraphQL and POST fallbacks ([6fea859](https://github.com/socialstalker/extension/commit/6fea8595a230cacbba4749e50acc30da426890d6))

## [2.1.0](https://github.com/socialstalker/extension/compare/v2.0.0...v2.1.0) (2026-10-18)

## [2.0.0](https://github.com/socialstalker/extension/compare/e1b9f85c9faa617a72c7becd221d04d9b32e83de...v2.0.0) (2026-08-23)

### Features

* **core:** platform-agnostic core layer ([e1b9f85](https://github.com/socialstalker/extension/commit/e1b9f85c9faa617a72c7becd221d04d9b32e83de))
* **facebook:** add context menu for opening full profile pictures and refactor related features ([c414448](https://github.com/socialstalker/extension/commit/c414448dcfa191cb1dfe304b0adc8a42ca3b0235))
* **facebook:** enhance story handling with bucket queries and session token management ([9a535d9](https://github.com/socialstalker/extension/commit/9a535d99c270497de9d69a27f792c226d23c94c2))
* in-page toast feedback, replacing OS notifications ([fbc6193](https://github.com/socialstalker/extension/commit/fbc619380c90e5d3fe0c902dbffa58c99059e163))
* **instagram:** download controls on feed posts ([4380a93](https://github.com/socialstalker/extension/commit/4380a935a23d0d651d0f460f0bbfdd5d813c9d08))
* **instagram:** implement shared injection loop for action row features ([7218b8d](https://github.com/socialstalker/extension/commit/7218b8dc0308c6106727793b1f33874f4f66c02c))
* **instagram:** implement story seen-state blocker and associated client modules ([1f4dd3e](https://github.com/socialstalker/extension/commit/1f4dd3e688960fcd5d679993282ee419b2b65c6e))
* **instagram:** port endpoints from C# and rebuild features on the registry ([8df3bbf](https://github.com/socialstalker/extension/commit/8df3bbf7c8e9cc9c55f95942377e3ed835e6cdf2))
* **instagram:** tiered resolution for full-size profile pictures ([bf373e3](https://github.com/socialstalker/extension/commit/bf373e324ab09f51979d30e0c352e5e8fbe8763e))
* **instagram:** UserIdResolver with a strategy chain ([ffde26f](https://github.com/socialstalker/extension/commit/ffde26f026390b626bf8fb4a3de076f950c9fc7e))
* **observability:** implement Sentry integration across multiple realms ([dc34d93](https://github.com/socialstalker/extension/commit/dc34d93a78627ca20ea69fe7f625d2bb9cb97a1c))
* rebuild background, Facebook platform, and extension pages ([ddd4ced](https://github.com/socialstalker/extension/commit/ddd4ced8c882d820169a402acbfc97c5d44ca004))
* **release:** add GitHub Actions workflow for extension release automation ([b32335a](https://github.com/socialstalker/extension/commit/b32335a46e78d79026ec9ffb3f50cea8e0a7bfca))
* **seen-blocker:** implement seen-state blockers for Facebook and Instagram with shared messaging ([5a32245](https://github.com/socialstalker/extension/commit/5a3224534d5bfd60286d45d1e4ceb0c3421cf255))

### Bug Fixes

* **ig-stories:** inject into the viewer when opened from the home feed ([efa1de9](https://github.com/socialstalker/extension/commit/efa1de9e0e7acb359cf8d63f5e24c5f9dae8e6e1))
* **ig-stories:** track the frame on screen and stop serving mp4s as images ([a4a9b85](https://github.com/socialstalker/extension/commit/a4a9b85432f4da2435f32f265acad376b99e930d))
* **instagram:** decode only the shortcode, not the token appended to it ([be557e4](https://github.com/socialstalker/extension/commit/be557e44ad8f5ff365b048520a245695a9ba90bc))
* **instagram:** harvest the profile GraphQL query instead of pinning it ([f1788ff](https://github.com/socialstalker/extension/commit/f1788ffa2b607f38f8b4191d78a1a236d6809bfe))
* **instagram:** inject profile buttons into the action row, not the page ([af608ae](https://github.com/socialstalker/extension/commit/af608aef3a50eb2e6eefc3484a9a4243654505b2))
* **instagram:** send the profile query the way Instagram actually accepts it ([3d59316](https://github.com/socialstalker/extension/commit/3d59316fc3d7435db5cbde7dc9ce28d92c7095f3))
* scope the web_profile_info removal to the profile-picture path ([78f7932](https://github.com/socialstalker/extension/commit/78f7932db581f72c74187d214f595dc4a2d1e4b2))
* **stories:** serve the story on screen, not the one first opened ([ed9e9a5](https://github.com/socialstalker/extension/commit/ed9e9a5e68499d32a2557823972cc1d8ce3ad2f7))
* **telemetry:** keep the first capture, and name the archived profile ([259c152](https://github.com/socialstalker/extension/commit/259c152d7c0c663436d27a01d7cff8fd46829a3d))
