# Changelog

## [0.1.8](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/compare/0.1.7...0.1.8) (2026-08-29)


### Features

* **falkordb:** Add FalkorDB source and tools ([mcp-toolbox#​3692](https://redirect.github.com/googleapis/mcp-toolbox/issues/3692)) ([a94702c](https://redirect.github.com/googleapis/mcp-toolbox/commit/a94702c13121736e0ceb05425af43a0b953ac5b5)) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))
* **mcp:** Add Secure Parameters support as Toolbox experimental extension ([mcp-toolbox#​3394](https://redirect.github.com/googleapis/mcp-toolbox/issues/3394)) ([9750d2d](https://redirect.github.com/googleapis/mcp-toolbox/commit/9750d2da4b1dc08761ab2b5510454e1a386ebce8)) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))
* **server/mcp:** Support com.google.cloud/toolbox.v1 extension in v20260728 ([mcp-toolbox#​3801](https://redirect.github.com/googleapis/mcp-toolbox/issues/3801)) ([f4f7da6](https://redirect.github.com/googleapis/mcp-toolbox/commit/f4f7da605245ff9e8d491d0c55591ba3b400623b)) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))
* **skill:** Add fix-failing-tests skill for mcp-toolbox ([mcp-toolbox#​3821](https://redirect.github.com/googleapis/mcp-toolbox/issues/3821)) ([168e69c](https://redirect.github.com/googleapis/mcp-toolbox/commit/168e69c048d65aa15b926f9dd7680245949cc57a)) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))
* **sources:** Support native read-only mode and dynamic tool annotations ([mcp-toolbox#​3872](https://redirect.github.com/googleapis/mcp-toolbox/issues/3872)) ([c257022](https://redirect.github.com/googleapis/mcp-toolbox/commit/c257022fed2cc5e9a286bf9fd78e91d76f9ff3b8)), refs [mcp-toolbox#​3615](https://redirect.github.com/googleapis/mcp-toolbox/issues/3615) [mcp-toolbox#​3816](https://redirect.github.com/googleapis/mcp-toolbox/issues/3816) [mcp-toolbox#​3618](https://redirect.github.com/googleapis/mcp-toolbox/issues/3618) [mcp-toolbox#​3851](https://redirect.github.com/googleapis/mcp-toolbox/issues/3851) [mcp-toolbox#​3619](https://redirect.github.com/googleapis/mcp-toolbox/issues/3619) [mcp-toolbox#​3617](https://redirect.github.com/googleapis/mcp-toolbox/issues/3617) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))


### Bug Fixes

* **cloud-storage:** Resolve symlinks when enforcing local path boundaries ([mcp-toolbox#​3810](https://redirect.github.com/googleapis/mcp-toolbox/issues/3810)) ([c2ada64](https://redirect.github.com/googleapis/mcp-toolbox/commit/c2ada6421f718cb861c7ccd5f0e8cd7e841a407f)) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))
* **config:** Compare env var offsets in rune space when skipping comments ([mcp-toolbox#​3856](https://redirect.github.com/googleapis/mcp-toolbox/issues/3856)) ([2e76934](https://redirect.github.com/googleapis/mcp-toolbox/commit/2e769343332cf84084a162e23f556490faa20d32)) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))
* **postgres:** Filter background processes in postgres-list-active-queries ([mcp-toolbox#​3885](https://redirect.github.com/googleapis/mcp-toolbox/issues/3885)) ([3d9e62a](https://redirect.github.com/googleapis/mcp-toolbox/commit/3d9e62a979be951bb04aeaf31aa4505598031f4a)) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))
* Merge prebuilt tools when reloading custom config ([mcp-toolbox#​3864](https://redirect.github.com/googleapis/mcp-toolbox/issues/3864)) ([5a6d865](https://redirect.github.com/googleapis/mcp-toolbox/commit/5a6d865eff939ace8c803d3ce8831aa83d00a750)) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))
* Normalize postgres UUIDs to strings ([mcp-toolbox#​3806](https://redirect.github.com/googleapis/mcp-toolbox/issues/3806)) ([3b02f1d](https://redirect.github.com/googleapis/mcp-toolbox/commit/3b02f1d86ab774c1e0fb13d0de7b6b428da78b83)) ([00b233a](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/00b233a212ca827e4de17d8cac046aff5cbee70f))

## [0.1.7](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/compare/0.1.6...0.1.7) (2026-08-20)


### Features

* **deps:** update dependency @toolbox-sdk/server to v1.9.0 ([#100](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/100)) ([03fa0a6](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/03fa0a6c0c6d3a61061c9b485f953c1e39556f51))

## [0.1.6](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/compare/0.1.5...0.1.6) (2026-01-30)


### Features

* Support custom scopes and maxQueryResultRows ([#77](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/77)) ([c38438e](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/c38438e8d4296d98ab2fa52e3b61cfe518fec3a4))

## [0.1.5](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/compare/0.1.4...0.1.5) (2026-01-28)


### Features

* add Configuration settings ([#72](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/72)) ([27a9100](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/27a9100b91b45d2dc49b48b29b7565551de21d80))
* **deps:** update dependency googleapis/mcp-toolbox to v0.26.0 ([#74](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/74)) ([124a489](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/124a4898581b220e2e0dd9772484a7808d161c84))

## [0.1.4](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/compare/0.1.3...0.1.4) (2026-01-22)


### Features

* **deps:** update dependency googleapis/mcp-toolbox to v0.25.0 ([#69](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/69)) ([bc0ac06](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/bc0ac06dd17f1bb81f47fa116ec31b67677322e6))

## [0.1.3](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/compare/0.1.2...0.1.3) (2025-12-30)


### Features

* **deps:** update dependency googleapis/mcp-toolbox to v0.24.0 ([#67](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/67)) ([888a7d7](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/888a7d7329d1027acae4743d3b84a79554383758))

## [0.1.2](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/compare/0.1.1...0.1.2) (2025-12-12)


### Features

* **deps:** update dependency googleapis/mcp-toolbox to v0.23.0 ([#63](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/63)) ([7c942a5](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/7c942a5fd79e45963db59e70d6d7c59475e6b49d))

## [0.1.1](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/compare/0.1.0...0.1.1) (2025-09-30)


### Features

* additional instructions for the context file ([#28](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/28)) ([0014c2b](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/0014c2b51e50339c3f8a551a32f2da38d3e830f9))
* standardize mcp server names ([#25](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/25)) ([c833e93](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/c833e93ceee5755da04daea4eba571e76e9e17bb))

## 0.1.0 (2025-09-22)


### Features

* add the BigQuery Conversational Analytics Extension ([#7](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/issues/7)) ([c3c552e](https://github.com/gemini-cli-extensions/bigquery-conversational-analytics/commit/c3c552e50ada6ba2dca2cbc538270a7668235a50))
