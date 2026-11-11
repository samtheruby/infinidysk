# Changelog

## [2.0.0-beta.1](https://github.com/samtheruby/infinidysk/compare/v2.0.0-beta.7...v2.0.0-beta.1) (2026-11-11)


### ⚠ BREAKING CHANGES

* **api:** infinidysk no longer starts while a Readarr Arr instance is configured. Before upgrading, remove Readarr instances or change them to Chaptarr in Settings > Arr instances. If already upgraded, start the previous version to do so, or override the list with INFINIDYSK__ARR_INSTANCES.

* force next release to 1.2.5 ([#1147](https://github.com/samtheruby/infinidysk/issues/1147)) ([0c5d56b](https://github.com/samtheruby/infinidysk/commit/0c5d56b86684e525a4870ae1f6d8a1cac582e5e2))
* **release:** force next release to 1.2.6 ([#1194](https://github.com/samtheruby/infinidysk/issues/1194)) ([f559135](https://github.com/samtheruby/infinidysk/commit/f55913539b35247bbb60ebc9d3cb68646e99f32e))


### Features

* **api:** better Lidarr support: more audio formats, faster cleanup after album deletes, and a tagging warning ([#1838](https://github.com/samtheruby/infinidysk/issues/1838)) ([e138a06](https://github.com/samtheruby/infinidysk/commit/e138a062aa1df9f9a85a0aaecf532a2e060fbc98))
* **api:** support Chaptarr instead of the abandoned Readarr ([#1827](https://github.com/samtheruby/infinidysk/issues/1827)) ([24e55b5](https://github.com/samtheruby/infinidysk/commit/24e55b51b6843a7df13364c2a310d77cf36a999c))
* **api:** support pack filename shows the InfiniDysk version that generated it ([#1609](https://github.com/samtheruby/infinidysk/issues/1609)) ([0f1e775](https://github.com/samtheruby/infinidysk/commit/0f1e775bbffacdc3f0f805edbc67600fb13fccbf))
* **arr:** support Sonarr v5 ([#1833](https://github.com/samtheruby/infinidysk/issues/1833)) ([b743f54](https://github.com/samtheruby/infinidysk/commit/b743f544313a0ad447687c8bcd7a678abab56a63))
* **auth:** show your identity provider's name on the SSO sign-in button ([#1835](https://github.com/samtheruby/infinidysk/issues/1835)) ([1845fe8](https://github.com/samtheruby/infinidysk/commit/1845fe8182b8f084da671ca399a12bff028500d0))
* **auth:** sign in behind a reverse proxy via gui configuration ([#1420](https://github.com/samtheruby/infinidysk/issues/1420)) ([fbad2f0](https://github.com/samtheruby/infinidysk/commit/fbad2f0cdcc6f6b21d5671e779ddbbdb9a0f4365))
* **auth:** sign in with single sign-on (OIDC), carried over from 1.x ([#1812](https://github.com/samtheruby/infinidysk/issues/1812)) ([4fc3b6a](https://github.com/samtheruby/infinidysk/commit/4fc3b6a4e834c478313466e1af95aa9bbf0b7350))
* **db:** back up your database nightly and restore it from the Maintenance page ([#1809](https://github.com/samtheruby/infinidysk/issues/1809)) ([0c40be7](https://github.com/samtheruby/infinidysk/commit/0c40be7d06360f75e2bca544b940744212ea6357))
* **db:** choose where infinidysk keeps its database and files ([#1858](https://github.com/samtheruby/infinidysk/issues/1858)) ([c1f6f93](https://github.com/samtheruby/infinidysk/commit/c1f6f936462bd2e2a003971ff67c88dd28e331fe))
* **db:** move from SQLite to PostgreSQL from the settings page ([#1807](https://github.com/samtheruby/infinidysk/issues/1807)) ([20a87fb](https://github.com/samtheruby/infinidysk/commit/20a87fbbb770026a549acd335c350ce01cb353c6))
* **health:** add a "quick" health-check depth ([#1410](https://github.com/samtheruby/infinidysk/issues/1410)) ([89ee934](https://github.com/samtheruby/infinidysk/commit/89ee9344d55d35035b052d15df196dbf36602b85))
* **health:** add actions to resolve attention items and clarify health statistics ([#1484](https://github.com/samtheruby/infinidysk/issues/1484)) ([5b395b4](https://github.com/samtheruby/infinidysk/commit/5b395b4680635ee99037674f19bf501ea898fdfe))
* **health:** clean up mounts whose streaming payloads are missing ([#1218](https://github.com/samtheruby/infinidysk/issues/1218)) ([aa83ef3](https://github.com/samtheruby/infinidysk/commit/aa83ef32662d84bdb59cdce41bcbe7f7ea72c5f0))
* **health:** expose segment-buffer eviction causes and throttle forced GC ([#1230](https://github.com/samtheruby/infinidysk/issues/1230)) ([cbd87e5](https://github.com/samtheruby/infinidysk/commit/cbd87e5b4e760e0c274af4bd08962229b251bd4d))
* **health:** PAR2 repair now fixes missing articles inside RAR releases ([#1348](https://github.com/samtheruby/infinidysk/issues/1348)) ([5c7bf79](https://github.com/samtheruby/infinidysk/commit/5c7bf7912307fbc76a02a0c06e55441bcf1a67d0))
* **health:** parallel health checks with shared connection gate and queue coexistence ([#1208](https://github.com/samtheruby/infinidysk/issues/1208)) ([b42ac42](https://github.com/samtheruby/infinidysk/commit/b42ac422a62ae20e60b65a2b356a4b723a3dc9da))
* **health:** parallel health checks with shared connection gate and queue coexistence ([#1208](https://github.com/samtheruby/infinidysk/issues/1208)) ([9ebbe55](https://github.com/samtheruby/infinidysk/commit/9ebbe551d360782dd40ddc7e8d80fc18f8693ca9))
* **health:** re-check action-needed files from Health history ([#1336](https://github.com/samtheruby/infinidysk/issues/1336)) ([2043c96](https://github.com/samtheruby/infinidysk/commit/2043c96906fa3c44f01eb93daec7a83f744b9077))
* **health:** re-run health checks across the whole library from Settings → Maintenance ([#1203](https://github.com/samtheruby/infinidysk/issues/1203)) ([bb54a92](https://github.com/samtheruby/infinidysk/commit/bb54a92b77c6147eb547685e5f75b96ef8f089b9))
* **health:** separate active attention items from repair history ([#1463](https://github.com/samtheruby/infinidysk/issues/1463)) ([68f4d2b](https://github.com/samtheruby/infinidysk/commit/68f4d2b63f276675cc2e53ebc30a0fc3c21e6ae6))
* **health:** stop a running health check or repair from the Health page ([#1753](https://github.com/samtheruby/infinidysk/issues/1753)) ([02e9b21](https://github.com/samtheruby/infinidysk/commit/02e9b21e320e722f83224d632853a27c2a44adf3))
* **health:** turn on background repairs by default ([#1284](https://github.com/samtheruby/infinidysk/issues/1284)) ([c3229c2](https://github.com/samtheruby/infinidysk/commit/c3229c2a386e4bb678e85956aeb444788e87bbda))
* **import:** upgrade 1.x installs that keep their data in PostgreSQL ([#1815](https://github.com/samtheruby/infinidysk/issues/1815)) ([6ee6cbf](https://github.com/samtheruby/infinidysk/commit/6ee6cbfc686a4be55d4f04afcc4ce74af634d35a))
* **mount:** read history shows which app started ffmpeg or ffprobe ([#1791](https://github.com/samtheruby/infinidysk/issues/1791)) ([25e114a](https://github.com/samtheruby/infinidysk/commit/25e114ac59e4738f9594a30c4ccb30d98d945817))
* **mount:** turn off the built-in FUSE mount when you do not need it, without warnings ([#1841](https://github.com/samtheruby/infinidysk/issues/1841)) ([d721677](https://github.com/samtheruby/infinidysk/commit/d721677513bc8f0e23005450114a2a6f93ea7379))
* **nntp:** 25 more providers to pick from when adding a server ([#1880](https://github.com/samtheruby/infinidysk/issues/1880)) ([0bd13e8](https://github.com/samtheruby/infinidysk/commit/0bd13e84efacfbafafffcf32b34fda42af8a9954))
* **nntp:** add the news-central.giganews.com server to the Giganews profile ([#1824](https://github.com/samtheruby/infinidysk/issues/1824)) ([028d6fb](https://github.com/samtheruby/infinidysk/commit/028d6fb3663d9a266396ecd39cf7cc17e94bb98d))
* **nntp:** split transfer and metadata connection budgets ([#1207](https://github.com/samtheruby/infinidysk/issues/1207)) ([39e04c1](https://github.com/samtheruby/infinidysk/commit/39e04c126377be0e025c3838c0fdcc1433884506))
* **nntp:** split transfer and metadata connection budgets ([#1207](https://github.com/samtheruby/infinidysk/issues/1207)) ([a434ee2](https://github.com/samtheruby/infinidysk/commit/a434ee2308dbbbab6e19598e567f3ff193319e60))
* **queue:** create symlink and STRM outputs together ([#1146](https://github.com/samtheruby/infinidysk/issues/1146)) ([c888279](https://github.com/samtheruby/infinidysk/commit/c88827999fec100a03c4f212c04b4415322e4e29))
* **queue:** import NZBs that contain another NZB ([#1875](https://github.com/samtheruby/infinidysk/issues/1875)) ([db91586](https://github.com/samtheruby/infinidysk/commit/db915861fa075483721e9cf1fd7ef6983e7016c2))
* **queue:** name a lone imported video after its release folder ([#1149](https://github.com/samtheruby/infinidysk/issues/1149)) ([c7530c0](https://github.com/samtheruby/infinidysk/commit/c7530c0bd265852329f49d71fd5ccdea09970a73))
* **sab:** include client user agent in authentication rejection warnings ([#1179](https://github.com/samtheruby/infinidysk/issues/1179)) ([8848ad5](https://github.com/samtheruby/infinidysk/commit/8848ad517623cf892d6c464d6fb817ef35f9a523))
* **scheduling:** schedule health checks, repairs, and queue downloads by time of day ([#1153](https://github.com/samtheruby/infinidysk/issues/1153)) ([5e6a3ff](https://github.com/samtheruby/infinidysk/commit/5e6a3ff0d82187739adad227a543bbaa2128a006))
* **support:** identify stalled playback and repeated health checks in support packs ([#1482](https://github.com/samtheruby/infinidysk/issues/1482)) ([873d317](https://github.com/samtheruby/infinidysk/commit/873d317d4ecfcb6d67cf390065960debd2942ee1))
* **ui:** activity chart separates client playback reads from app-triggered reads ([#1340](https://github.com/samtheruby/infinidysk/issues/1340)) ([79ad0ef](https://github.com/samtheruby/infinidysk/commit/79ad0ef29fda9f2e72f286350e1a66cb45844ad8))
* **ui:** Activity chart shows import downloads separately from maintenance ([#1535](https://github.com/samtheruby/infinidysk/issues/1535)) ([ae7da05](https://github.com/samtheruby/infinidysk/commit/ae7da05c38c4623d1ccdae6eb79679d2a6bf5c82))
* **ui:** backups get their own settings page ([#1826](https://github.com/samtheruby/infinidysk/issues/1826)) ([343cd7f](https://github.com/samtheruby/infinidysk/commit/343cd7f3340c5a0b3320cdec91f65c8e6a54d058))
* **ui:** guide first-run setup for Plex, Emby, and Jellyfin ([#1306](https://github.com/samtheruby/infinidysk/issues/1306)) ([b31a220](https://github.com/samtheruby/infinidysk/commit/b31a22080f7615b4abf96f918ad90438563840e8))
* **ui:** inspect each provider's speed history from Overview ([#1151](https://github.com/samtheruby/infinidysk/issues/1151)) ([ea6ce14](https://github.com/samtheruby/infinidysk/commit/ea6ce1428910217442c8c10d69d5f621b5138bd8))
* **ui:** make health check depth adjustable ([#1426](https://github.com/samtheruby/infinidysk/issues/1426)) ([9c315ac](https://github.com/samtheruby/infinidysk/commit/9c315acc71618b4bccb56dfe0724c6db23f471bb))
* **ui:** manage files in compact tree and list views with health filters ([#1546](https://github.com/samtheruby/infinidysk/issues/1546)) ([d83a6c1](https://github.com/samtheruby/infinidysk/commit/d83a6c10e5f5c7102930c8d947e136d8db500711))
* **ui:** overview activity shows download speed by workload as bars ([#1810](https://github.com/samtheruby/infinidysk/issues/1810)) ([dfa8146](https://github.com/samtheruby/infinidysk/commit/dfa81468bc7504bea4c00f7c3f4c3d83849ff93b))
* **ui:** peak download now shows the true 1-second maximum and no longer shrinks when widening the time range ([#1536](https://github.com/samtheruby/infinidysk/issues/1536)) ([5b6a969](https://github.com/samtheruby/infinidysk/commit/5b6a969ace140ced0539b198f7cd219f1bb0bdb4))
* **ui:** remind you to remove 1.x data after the upgrade, with its estimated disk usage ([#1876](https://github.com/samtheruby/infinidysk/issues/1876)) ([eebad20](https://github.com/samtheruby/infinidysk/commit/eebad20e14e0e7739a50757a22e68000db5b99da))
* **ui:** setup wizard always suggests rclone RC notifications for symlink installs ([#1320](https://github.com/samtheruby/infinidysk/issues/1320)) ([502995d](https://github.com/samtheruby/infinidysk/commit/502995dd8308a83a18b14c9b855a6061690ad987))
* **ui:** show active queue jobs and history in one list ([#1286](https://github.com/samtheruby/infinidysk/issues/1286)) ([e6b2e21](https://github.com/samtheruby/infinidysk/commit/e6b2e21285a0e7c19c4910c1e3d2935f2f66e851))
* **ui:** show provider bytes fetched on the overview activity card ([#1528](https://github.com/samtheruby/infinidysk/issues/1528)) ([70a122f](https://github.com/samtheruby/infinidysk/commit/70a122f2f7954e50497f8c6288b91fadcb789696))
* **ui:** the Queue link shows when a download needs you in the Arr ([#1849](https://github.com/samtheruby/infinidysk/issues/1849)) ([2c1a095](https://github.com/samtheruby/infinidysk/commit/2c1a0953d2aa2a3c06f1044a8255c07dad959b22))
* **ui:** the queue no longer shows failed imports older than a day unless you filter for them ([#1865](https://github.com/samtheruby/infinidysk/issues/1865)) ([2db9609](https://github.com/samtheruby/infinidysk/commit/2db96096a071f31edf0ce38ee0be21bd3175b30c))
* **ui:** warn when a provider repeatedly blocks missing-article checks ([#1551](https://github.com/samtheruby/infinidysk/issues/1551)) ([612fcdb](https://github.com/samtheruby/infinidysk/commit/612fcdb995be1c3e41a70d0da31cfc9be29de8b2))
* **ui:** warn when rclone streams through port 3000 ([#1328](https://github.com/samtheruby/infinidysk/issues/1328)) ([eae59a5](https://github.com/samtheruby/infinidysk/commit/eae59a5593fbdb1f3d83297cd3d300d699acb8bb))
* **ui:** warn when Segment Cache duplicates rclone VFS read-ahead ([#1319](https://github.com/samtheruby/infinidysk/issues/1319)) ([eebc880](https://github.com/samtheruby/infinidysk/commit/eebc88029b6ee101c1475f0da2e906309999229b))
* **usenet:** add memory ownership telemetry ([#1295](https://github.com/samtheruby/infinidysk/issues/1295)) ([04cac95](https://github.com/samtheruby/infinidysk/commit/04cac95850c342b0b7ad7a86b918a6cdf5767f40))
* **usenet:** benchmark configured provider limits above 50 connections ([#1360](https://github.com/samtheruby/infinidysk/issues/1360)) ([63bde75](https://github.com/samtheruby/infinidysk/commit/63bde757cbec76584324cf5ede9c27d775aefb0f))
* **usenet:** cap total Usenet download bandwidth ([#1152](https://github.com/samtheruby/infinidysk/issues/1152)) ([ecd2193](https://github.com/samtheruby/infinidysk/commit/ecd21933df54c52f9eba93251ad48919ff6e6e4e))
* **usenet:** improve batching for short and medium range reads (opt-in) ([#1292](https://github.com/samtheruby/infinidysk/issues/1292)) ([21a499f](https://github.com/samtheruby/infinidysk/commit/21a499f5932641250ae30dd706a3cf17c85bf35f))
* **usenet:** leftover segment-cache files are cleaned up on startup when the cache is disabled ([#1321](https://github.com/samtheruby/infinidysk/issues/1321)) ([a9c69f8](https://github.com/samtheruby/infinidysk/commit/a9c69f830580f7095d2ffd53a76ad6d6982b7c9f))
* **usenet:** let long reads expand provider connections faster ([#1324](https://github.com/samtheruby/infinidysk/issues/1324)) ([9044421](https://github.com/samtheruby/infinidysk/commit/9044421ecaef71048dff09626b86afe02b4a2b7a))
* **usenet:** let segment cache writes run behind playback ([#1325](https://github.com/samtheruby/infinidysk/issues/1325)) ([5cd2aee](https://github.com/samtheruby/infinidysk/commit/5cd2aee3b70622a380ec4cd94a209ec300559523))
* **usenet:** make provider circuit-breaker cooldowns configurable ([#1118](https://github.com/samtheruby/infinidysk/issues/1118)) ([56e9415](https://github.com/samtheruby/infinidysk/commit/56e941593bb1313b2ac9757016cfe972d249084c))
* **usenet:** measure production pipelined cache bypass before the warm-read fix ([#1288](https://github.com/samtheruby/infinidysk/issues/1288)) ([a3a0d7b](https://github.com/samtheruby/infinidysk/commit/a3a0d7bf877cf65d6a86a0db4ca52edc48a8648d))
* **usenet:** segment cache is off by default for new installs; existing installs keep their current behavior ([#1322](https://github.com/samtheruby/infinidysk/issues/1322)) ([d0d18c0](https://github.com/samtheruby/infinidysk/commit/d0d18c02a672fec7c131dff6b0af80398a655a07))
* **usenet:** warm provider connections when long reads start ([#1330](https://github.com/samtheruby/infinidysk/issues/1330)) ([83a431c](https://github.com/samtheruby/infinidysk/commit/83a431cdfc21adcdb5322fd78c834688d13142d9))
* **webdav:** stream traces separate connection, permit, and failed-attempt waits per request ([#1661](https://github.com/samtheruby/infinidysk/issues/1661)) ([738a87c](https://github.com/samtheruby/infinidysk/commit/738a87cd966b6db15d87c7199da30d8a1be8b7e2))
* **webdav:** stream traces show what each playback stall was waiting on ([#1674](https://github.com/samtheruby/infinidysk/issues/1674)) ([9fd1869](https://github.com/samtheruby/infinidysk/commit/9fd1869d6d35876f71541de222383ef9dc511636))


### Bug Fixes

* **api:** an unresponsive STRM folder no longer freezes settings and the SAB API ([#1795](https://github.com/samtheruby/infinidysk/issues/1795)) ([a7eb784](https://github.com/samtheruby/infinidysk/commit/a7eb784e4e39b7db6850817a00bac2ef3b2b1332))
* **api:** Arrs that start after InfiniDysk now connect without a restart ([#1806](https://github.com/samtheruby/infinidysk/issues/1806)) ([ba4972f](https://github.com/samtheruby/infinidysk/commit/ba4972f6a813f765cb49847098e489644735b9d9))
* **api:** hide full numeric-only IPv6 addresses in support packs ([#1524](https://github.com/samtheruby/infinidysk/issues/1524)) ([181a8ae](https://github.com/samtheruby/infinidysk/commit/181a8aec2b666ec55e63d8cad6d3c32b1cd2b4dc))
* **api:** link the update notice to the release notes of the newer tag ([#1860](https://github.com/samtheruby/infinidysk/issues/1860)) ([005812a](https://github.com/samtheruby/infinidysk/commit/005812a4248f4d5685257dd76dbb429181e4aff2))
* **api:** reject invalid Warden source uploads with 400 and count UTF-8 bytes ([#1274](https://github.com/samtheruby/infinidysk/issues/1274)) ([08f5567](https://github.com/samtheruby/infinidysk/commit/08f5567271644c3044dc339922fc980cdc8e8c73))
* **archive:** malformed 7z headers can no longer hang or exhaust memory during import ([#1794](https://github.com/samtheruby/infinidysk/issues/1794)) ([7091745](https://github.com/samtheruby/infinidysk/commit/7091745063ffba6feb7826191f9fea16a219be54))
* **arr:** Arr and Prowlarr connections work with Docker hostnames behind a proxy and report timeouts clearly ([#1537](https://github.com/samtheruby/infinidysk/issues/1537)) ([d480668](https://github.com/samtheruby/infinidysk/commit/d4806683c050c8702d6fee5646e8e18090549a27))
* **arr:** Arr Health no longer shows instances offline with 'database is locked' on large installs ([#1556](https://github.com/samtheruby/infinidysk/issues/1556)) ([916b1e5](https://github.com/samtheruby/infinidysk/commit/916b1e5be7dc390eeebbc06a3be4126495a047d4))
* **arr:** files imported by a second Arr are no longer deleted by cleanup of the first ([#1802](https://github.com/samtheruby/infinidysk/issues/1802)) ([3464a0c](https://github.com/samtheruby/infinidysk/commit/3464a0c14d3f0187e113c962b132e267c42ec5de))
* **arr:** prevent overlapping Watchtower cycles after a timeout ([#1278](https://github.com/samtheruby/infinidysk/issues/1278)) ([28a9eba](https://github.com/samtheruby/infinidysk/commit/28a9ebad42149933a770e488f4fd36dbc518f631))
* **arr:** Radarr and other Arrs save the infinidysk webhook even when they cannot reach it yet ([#1861](https://github.com/samtheruby/infinidysk/issues/1861)) ([e3e0507](https://github.com/samtheruby/infinidysk/commit/e3e0507366d9e17abda275018644d3aa92f069f2))
* **arr:** reject oversized Newznab and Watchtower list responses instead of parsing them unbounded ([#1279](https://github.com/samtheruby/infinidysk/issues/1279)) ([b9be02e](https://github.com/samtheruby/infinidysk/commit/b9be02eb3db846f3a6504af92bd93c6d9817c1a6))
* **arr:** retain WebDAV items when Arr repair only partially completes ([#1381](https://github.com/samtheruby/infinidysk/issues/1381)) ([75420e9](https://github.com/samtheruby/infinidysk/commit/75420e92cbea9435d9c6d7ce1f2201f27b64c4b7))
* **arr:** skip the automatic-search wait when no release was blocklisted ([#1817](https://github.com/samtheruby/infinidysk/issues/1817)) ([23be919](https://github.com/samtheruby/infinidysk/commit/23be9194448dbb028bee7cb4c21378f2357610c2))
* **arr:** Sonarr repairs no longer resolve to a different series whose folder name shares a prefix ([#1620](https://github.com/samtheruby/infinidysk/issues/1620)) ([c4a4229](https://github.com/samtheruby/infinidysk/commit/c4a422939288bd5d523b2886f405838ded98ae5e))
* **arr:** stop false "Imports are taking longer than expected" alerts ([#1673](https://github.com/samtheruby/infinidysk/issues/1673)) ([34a32e2](https://github.com/samtheruby/infinidysk/commit/34a32e2abad8a8f23b0f2b7d03ce5d9232e0e55f))
* **arr:** stop re-importing uploads rejected by queue rules ([#1380](https://github.com/samtheruby/infinidysk/issues/1380)) ([95e9598](https://github.com/samtheruby/infinidysk/commit/95e9598bf8c6ba777a5a58a32e6b5f09b720ba15))
* **arr:** treat a connection the Arr drops mid-request as transient ([#1890](https://github.com/samtheruby/infinidysk/issues/1890)) ([766acc2](https://github.com/samtheruby/infinidysk/commit/766acc2d3aecb8a4ca50cc2e8f3654b188cb31b0))
* **auth:** direct sign-in works again when Base URL points to a reverse proxy ([#1443](https://github.com/samtheruby/infinidysk/issues/1443)) ([72a9bdb](https://github.com/samtheruby/infinidysk/commit/72a9bdb0d18e68bd662ca1fd4ab540d370ac2fb5))
* **auth:** hash the WEBDAV_PASSWORD env value once, not per request ([#1438](https://github.com/samtheruby/infinidysk/issues/1438)) ([6ae4c24](https://github.com/samtheruby/infinidysk/commit/6ae4c24050ed29b0298c43285c0031f520be51c9))
* **auth:** keep API keys and URL tokens out of frontend request logs ([#1526](https://github.com/samtheruby/infinidysk/issues/1526)) ([bfc7f20](https://github.com/samtheruby/infinidysk/commit/bfc7f2030cba9148c15f4bb9206b4f52b81dabf5))
* **auth:** recover from rejected login action origins ([#1401](https://github.com/samtheruby/infinidysk/issues/1401)) ([7895e06](https://github.com/samtheruby/infinidysk/commit/7895e06415f865acefeaec68a379edeafea7a374))
* **auth:** sign in works again behind a reverse proxy ([#1406](https://github.com/samtheruby/infinidysk/issues/1406)) ([ee0bbbd](https://github.com/samtheruby/infinidysk/commit/ee0bbbd1e4eeeba154fb3c61e4814b61161408b1))
* **ci:** anchor prerelease notes to latest stable release ([#1402](https://github.com/samtheruby/infinidysk/issues/1402)) ([bf640d2](https://github.com/samtheruby/infinidysk/commit/bf640d2800d4d50570938f1e259e558032383179))
* **db:** cleanup runs on SQLite no longer stop when other work writes to the database ([#1840](https://github.com/samtheruby/infinidysk/issues/1840)) ([6d676ab](https://github.com/samtheruby/infinidysk/commit/6d676ab28a308139bcf8c3d12e3446c91fd11837))
* **db:** container no longer dumps a stack trace per file when local streaming metadata is corrupt ([#1297](https://github.com/samtheruby/infinidysk/issues/1297)) ([cd9b120](https://github.com/samtheruby/infinidysk/commit/cd9b1205c1c8b312c3e0a14540dfa249d6ebd201))
* **db:** database backups no longer include metrics history ([#1589](https://github.com/samtheruby/infinidysk/issues/1589)) ([190eace](https://github.com/samtheruby/infinidysk/commit/190eace08a758f9af3cdcddfa38e429e99e9e479))
* **db:** failed maintenance runs and API errors now say what the database reported ([#1839](https://github.com/samtheruby/infinidysk/issues/1839)) ([43ac7fd](https://github.com/samtheruby/infinidysk/commit/43ac7fd1f399ef79ae9032c01e4276ef487a3924))
* **db:** let orphan cleanup continue through temporary locks ([#1408](https://github.com/samtheruby/infinidysk/issues/1408)) ([9c163ff](https://github.com/samtheruby/infinidysk/commit/9c163ff568b309714f96b0d2b1538dfd49556ad7))
* **db:** recheck pending history cleanup under the SQLite write lock ([#1599](https://github.com/samtheruby/infinidysk/issues/1599)) ([e3f079d](https://github.com/samtheruby/infinidysk/commit/e3f079d2ac937d4deb3eab4097ae2ec7a53fa80a))
* **db:** remove metrics integrity scans from startup ([#1512](https://github.com/samtheruby/infinidysk/issues/1512)) ([eb76ecf](https://github.com/samtheruby/infinidysk/commit/eb76ecf4434da790a72bcb773411ba8556ee4dae))
* **db:** retry backup directory initialization in the scheduler ([#1269](https://github.com/samtheruby/infinidysk/issues/1269)) ([32b07bf](https://github.com/samtheruby/infinidysk/commit/32b07bfb5aef4f836ffc498a87744a19e66bf7cf))
* **db:** skip a maintenance sweep instead of stopping the host when SQLite is busy ([#1268](https://github.com/samtheruby/infinidysk/issues/1268)) ([f846184](https://github.com/samtheruby/infinidysk/commit/f84618478024a399b0d844c3b16dce1ef621ca07))
* **db:** startup vacuum runs when enabled through NZBDAV_CONFIG__DB__IS_STARTUP_VACUUM_ENABLED ([#1450](https://github.com/samtheruby/infinidysk/issues/1450)) ([b0a5404](https://github.com/samtheruby/infinidysk/commit/b0a5404a04a9a0a0442d5d390cffae1e7f348cfc))
* **deps:** Bump @tanstack/react-query ([#1778](https://github.com/samtheruby/infinidysk/issues/1778)) ([10fba4d](https://github.com/samtheruby/infinidysk/commit/10fba4df44c845d95975ee19ab52706b5ee3536e))
* **deps:** Bump advanced-security/component-detection-dependency-submission-action ([#1395](https://github.com/samtheruby/infinidysk/issues/1395)) ([a35ffe2](https://github.com/samtheruby/infinidysk/commit/a35ffe24ac6a9850d4813936fb7210c78268f992))
* **deps:** Bump advanced-security/component-detection-dependency-submission-action ([#1682](https://github.com/samtheruby/infinidysk/issues/1682)) ([6d21118](https://github.com/samtheruby/infinidysk/commit/6d21118d4136f95784bd0743bee2e511abb671fe))
* **deps:** Bump body-parser from 2.3.0 to 2.4.0 in /frontend ([#1742](https://github.com/samtheruby/infinidysk/issues/1742)) ([a77b5ff](https://github.com/samtheruby/infinidysk/commit/a77b5ffb36a09f3de5f33e53a0a2cdc54ca13222))
* **deps:** Bump brace-expansion from 2.1.4 to 2.1.7 in /frontend ([#1603](https://github.com/samtheruby/infinidysk/issues/1603)) ([de57eb3](https://github.com/samtheruby/infinidysk/commit/de57eb3f12a07fed14ff1306a3e6a434dad2ca78))
* **deps:** Bump dotnet-stryker from 4.16.0 to 5.0.0 ([#1480](https://github.com/samtheruby/infinidysk/issues/1480)) ([a914b40](https://github.com/samtheruby/infinidysk/commit/a914b4092173632852f2a2aa80204e9d1c21253f))
* **deps:** Bump fast-uri from 3.1.5 to 3.1.7 in /frontend ([#1312](https://github.com/samtheruby/infinidysk/issues/1312)) ([219ac28](https://github.com/samtheruby/infinidysk/commit/219ac28b808483c0e6e11cb6f9fbf5cc86385b16))
* **deps:** Bump fast-uri from 3.1.8 to 3.1.9 in /frontend ([#1743](https://github.com/samtheruby/infinidysk/issues/1743)) ([ff0f4d3](https://github.com/samtheruby/infinidysk/commit/ff0f4d36391d5de58ba7ac3c87194e861bf556f9))
* **deps:** Bump fast-uri from 3.1.8 to 3.1.9 in /ui ([#1784](https://github.com/samtheruby/infinidysk/issues/1784)) ([7a4df2b](https://github.com/samtheruby/infinidysk/commit/7a4df2bb218acfb52c4473b2d7d2b0669956abba))
* **deps:** Bump fuse3 from 0.9.0 to 0.10.0 ([#1873](https://github.com/samtheruby/infinidysk/issues/1873)) ([6ef351a](https://github.com/samtheruby/infinidysk/commit/6ef351a177ab9e950ddaf4e6e8229990c56cdcf5))
* **deps:** Bump github/codeql-action ([#1629](https://github.com/samtheruby/infinidysk/issues/1629)) ([3544821](https://github.com/samtheruby/infinidysk/commit/3544821965cf2c5cb8d4d27cfe3c628eafc70223))
* **deps:** Bump github/codeql-action ([#1758](https://github.com/samtheruby/infinidysk/issues/1758)) ([0ac3c86](https://github.com/samtheruby/infinidysk/commit/0ac3c8685f0b951fff2f6b3dfbaa2b3b93f70522))
* **deps:** Bump github/codeql-action in the github-actions group ([#1256](https://github.com/samtheruby/infinidysk/issues/1256)) ([79a4861](https://github.com/samtheruby/infinidysk/commit/79a486147b178877292d8fd08363fd4117092a25))
* **deps:** Bump github/codeql-action in the github-actions group ([#1315](https://github.com/samtheruby/infinidysk/issues/1315)) ([99ec38c](https://github.com/samtheruby/infinidysk/commit/99ec38cc56c39ddf645076066c42d54843f2ed4a))
* **deps:** Bump github/codeql-action in the github-actions group ([#1478](https://github.com/samtheruby/infinidysk/issues/1478)) ([d542ca5](https://github.com/samtheruby/infinidysk/commit/d542ca55b872bd22ed9e8615797c56d5b609acc8))
* **deps:** Bump github/codeql-action in the github-actions group ([#1569](https://github.com/samtheruby/infinidysk/issues/1569)) ([ad86990](https://github.com/samtheruby/infinidysk/commit/ad86990931fad0a1233c98a97167a67b2aaab949))
* **deps:** Bump ip-address from 10.4.0 to 10.7.2 in /frontend ([#1596](https://github.com/samtheruby/infinidysk/issues/1596)) ([be46762](https://github.com/samtheruby/infinidysk/commit/be46762a65c69f7c4a41c52ff83b15adaa906f4b))
* **deps:** Bump ip-address from 10.7.2 to 10.7.5 in /frontend ([#1744](https://github.com/samtheruby/infinidysk/issues/1744)) ([6fac334](https://github.com/samtheruby/infinidysk/commit/6fac33411bcc87b06bbadd543778eeea5e007c36))
* **deps:** Bump js-yaml and @redocly/openapi-core in /frontend ([#1397](https://github.com/samtheruby/infinidysk/issues/1397)) ([5fe0a8d](https://github.com/samtheruby/infinidysk/commit/5fe0a8dc0c367740a7ef52037fe69ebe5d993f60))
* **deps:** Bump NUnit from 4.6.1 to 5.0.0 ([#1644](https://github.com/samtheruby/infinidysk/issues/1644)) ([a13d490](https://github.com/samtheruby/infinidysk/commit/a13d49088fc8534c97364badab0f38f538331750))
* **deps:** Bump proxy-addr from 2.0.7 to 2.0.8 in /frontend ([#1647](https://github.com/samtheruby/infinidysk/issues/1647)) ([a03cd96](https://github.com/samtheruby/infinidysk/commit/a03cd96e4ff4fb1f224c359e975a02ddedac174a))
* **deps:** Bump qs from 6.15.3 to 6.16.0 in /frontend ([#1316](https://github.com/samtheruby/infinidysk/issues/1316)) ([51bc1b5](https://github.com/samtheruby/infinidysk/commit/51bc1b5cd6bc500a31d3e7ec72e73910e87714dd))
* **deps:** Bump qs from 6.16.0 to 6.17.1 in /ui ([#1785](https://github.com/samtheruby/infinidysk/issues/1785)) ([d52c2fb](https://github.com/samtheruby/infinidysk/commit/d52c2fb8b10f6b305b6f19cf22cd6906a2656927))
* **deps:** Bump Scalar.AspNetCore from 2.17.1 to 2.17.2 ([#1339](https://github.com/samtheruby/infinidysk/issues/1339)) ([e3737c6](https://github.com/samtheruby/infinidysk/commit/e3737c6a45d2cf5d3ab07eb32907b4cb461ff582))
* **deps:** Bump source-map-js from 1.2.1 to 1.2.2 in /frontend ([#1648](https://github.com/samtheruby/infinidysk/issues/1648)) ([44428f2](https://github.com/samtheruby/infinidysk/commit/44428f2a76fc50b9dd2ea6e49543f61ed2b3ee33))
* **deps:** Bump systeminformation from 5.33.15 to 5.33.19 in /ui ([#1786](https://github.com/samtheruby/infinidysk/issues/1786)) ([608ade1](https://github.com/samtheruby/infinidysk/commit/608ade139964120ef798b7758b86b815e0ccb51a))
* **deps:** Bump the cargo-minor-patch group with 4 updates ([#1872](https://github.com/samtheruby/infinidysk/issues/1872)) ([fc62ad5](https://github.com/samtheruby/infinidysk/commit/fc62ad52f375ac8dd5773a977a171986c66d1cf3))
* **deps:** Bump the github-actions group across 1 directory with 2 updates ([#1722](https://github.com/samtheruby/infinidysk/issues/1722)) ([4dd62f6](https://github.com/samtheruby/infinidysk/commit/4dd62f669fdd287308f03091c8bbdf1f1c3c0124))
* **deps:** Bump the npm-minor-and-patch group ([#1202](https://github.com/samtheruby/infinidysk/issues/1202)) ([de13c67](https://github.com/samtheruby/infinidysk/commit/de13c67b5e8365bd8ab82750c511481da4058862))
* **deps:** Bump the npm-minor-and-patch group ([#1254](https://github.com/samtheruby/infinidysk/issues/1254)) ([23c7ba8](https://github.com/samtheruby/infinidysk/commit/23c7ba8e0ae753888e402c178aa73c102fbc028e))
* **deps:** Bump the npm-minor-and-patch group ([#1313](https://github.com/samtheruby/infinidysk/issues/1313)) ([484dafc](https://github.com/samtheruby/infinidysk/commit/484dafc57eb084bcd4afc8b62b05a5d96339909b))
* **deps:** Bump the npm-minor-and-patch group ([#1392](https://github.com/samtheruby/infinidysk/issues/1392)) ([b78fa73](https://github.com/samtheruby/infinidysk/commit/b78fa73da05704ab590da14abe92dd8d1e9d379c))
* **deps:** Bump the npm-minor-and-patch group ([#1422](https://github.com/samtheruby/infinidysk/issues/1422)) ([bfb2074](https://github.com/samtheruby/infinidysk/commit/bfb2074ab46d9e4c4019c8ce5774e7de0037cfd7))
* **deps:** Bump the npm-minor-and-patch group ([#1681](https://github.com/samtheruby/infinidysk/issues/1681)) ([a3c3a8b](https://github.com/samtheruby/infinidysk/commit/a3c3a8b9f3f28a6be3673e12b7eb74da4111c56c))
* **deps:** Bump the npm-minor-and-patch group ([#1757](https://github.com/samtheruby/infinidysk/issues/1757)) ([2dc8b53](https://github.com/samtheruby/infinidysk/commit/2dc8b5338a06d217159c1a0092365ad6620954b9))
* **deps:** Bump the npm-minor-and-patch group across 1 directory with 13 updates ([#1532](https://github.com/samtheruby/infinidysk/issues/1532)) ([f478af7](https://github.com/samtheruby/infinidysk/commit/f478af794abe3275a9e3078733ca7edc2d52576b))
* **deps:** Bump the npm-minor-and-patch group across 1 directory with 15 updates ([#1736](https://github.com/samtheruby/infinidysk/issues/1736)) ([af69ab9](https://github.com/samtheruby/infinidysk/commit/af69ab9a3db5d96d3e8e3a6e51b9b655fe237235))
* **deps:** Bump the npm-minor-and-patch group across 1 directory with 4 updates ([#1341](https://github.com/samtheruby/infinidysk/issues/1341)) ([4e32bb6](https://github.com/samtheruby/infinidysk/commit/4e32bb6b5368ca533efc4a96ad73c19355c53b84))
* **deps:** Bump the npm-minor-and-patch group across 1 directory with 8 updates ([#1601](https://github.com/samtheruby/infinidysk/issues/1601)) ([aec5115](https://github.com/samtheruby/infinidysk/commit/aec511538fb6e3ccc4d6abc74d5f69292dfb5745))
* **deps:** Bump the npm-minor-and-patch group across 1 directory with 9 updates ([#1642](https://github.com/samtheruby/infinidysk/issues/1642)) ([1709f13](https://github.com/samtheruby/infinidysk/commit/1709f1385702967b5d6a6f44c0c0a3160908615b))
* **deps:** Bump the npm-minor-patch group in /ui with 3 updates ([#1844](https://github.com/samtheruby/infinidysk/issues/1844)) ([ba17029](https://github.com/samtheruby/infinidysk/commit/ba17029c9e28fd63a39ec257dbbed551f71c31cb))
* **deps:** Bump the npm-minor-patch group in /ui with 4 updates ([#1869](https://github.com/samtheruby/infinidysk/issues/1869)) ([6bb8e3a](https://github.com/samtheruby/infinidysk/commit/6bb8e3a56d213f1a6e0364241e6a7b72b45e1136))
* **deps:** Bump the nuget-minor-and-patch group with 1 update ([#1423](https://github.com/samtheruby/infinidysk/issues/1423)) ([de1d6b0](https://github.com/samtheruby/infinidysk/commit/de1d6b09f3c369924b19b233b2d73e75cf483875))
* **deps:** Bump the nuget-minor-and-patch group with 1 update ([#1568](https://github.com/samtheruby/infinidysk/issues/1568)) ([90b2713](https://github.com/samtheruby/infinidysk/commit/90b27138af36e26beafe17e324e015fc2b426925))
* **deps:** Bump the nuget-minor-and-patch group with 1 update ([#1602](https://github.com/samtheruby/infinidysk/issues/1602)) ([edb7aa4](https://github.com/samtheruby/infinidysk/commit/edb7aa475cd38c35f4f158a58bde0a5e59c82168))
* **deps:** Bump the nuget-minor-and-patch group with 1 update ([#1756](https://github.com/samtheruby/infinidysk/issues/1756)) ([11de8f1](https://github.com/samtheruby/infinidysk/commit/11de8f190c5df5bb0684a508660e42ccd73ff1b7))
* **deps:** Bump the nuget-minor-and-patch group with 11 updates ([#1737](https://github.com/samtheruby/infinidysk/issues/1737)) ([635eb22](https://github.com/samtheruby/infinidysk/commit/635eb22a5c2d586ffdb40b14fc07c91857533dff))
* **deps:** Bump the nuget-minor-and-patch group with 2 updates ([#1314](https://github.com/samtheruby/infinidysk/issues/1314)) ([a0377e5](https://github.com/samtheruby/infinidysk/commit/a0377e5ccdf3681a070a5879a6418ec263764a6f))
* **deps:** Bump the nuget-minor-and-patch group with 2 updates ([#1683](https://github.com/samtheruby/infinidysk/issues/1683)) ([45f35b5](https://github.com/samtheruby/infinidysk/commit/45f35b5b300181e3df483ddb542c0bdf0b59b072))
* **deps:** Bump the nuget-minor-and-patch group with 3 updates ([#1255](https://github.com/samtheruby/infinidysk/issues/1255)) ([f8ede69](https://github.com/samtheruby/infinidysk/commit/f8ede696fd27e6e6c26c7d15748ca85a180d17ae))
* **deps:** Bump the nuget-minor-and-patch group with 9 updates ([#1533](https://github.com/samtheruby/infinidysk/issues/1533)) ([ded1d4e](https://github.com/samtheruby/infinidysk/commit/ded1d4e0734edf4d4daab46df07d619f440efe3c))
* **deps:** Bump the react-router group across 1 directory with 5 updates ([#1337](https://github.com/samtheruby/infinidysk/issues/1337)) ([11c2c02](https://github.com/samtheruby/infinidysk/commit/11c2c027d465664806a0aebc6c013a8cd6a3efbf))
* **deps:** Bump the react-router group across 1 directory with 5 updates ([#1531](https://github.com/samtheruby/infinidysk/issues/1531)) ([0d75b5d](https://github.com/samtheruby/infinidysk/commit/0d75b5d15c40c35cae092797877bc735afb94bb9))
* **deps:** Bump the react-router group in /frontend with 5 updates ([#1755](https://github.com/samtheruby/infinidysk/issues/1755)) ([10e0f7a](https://github.com/samtheruby/infinidysk/commit/10e0f7af802f01bf6f50c2920ba658747f0f1129))
* **deps:** Bump vite from 8.3.2 to 8.3.4 in /frontend ([#1727](https://github.com/samtheruby/infinidysk/issues/1727)) ([62c1458](https://github.com/samtheruby/infinidysk/commit/62c14587feac77d3ab630b960094e07e61ee067a))
* **deps:** Bump xunit.runner.visualstudio from 3.1.5 to 4.0.1 ([#1723](https://github.com/samtheruby/infinidysk/issues/1723)) ([b7f3299](https://github.com/samtheruby/infinidysk/commit/b7f3299c7a8d9a7073efc76518c0011046b8382f))
* **deps:** Bump xunit.v3 from 3.2.2 to 4.0.1 ([#1534](https://github.com/samtheruby/infinidysk/issues/1534)) ([8eea89a](https://github.com/samtheruby/infinidysk/commit/8eea89a20e5af9d05bdaa283d1b3e99d60e5ae86))
* **deps:** Bump zensical from 0.0.54 to 0.0.55 in the docs-python group ([#1155](https://github.com/samtheruby/infinidysk/issues/1155)) ([9556699](https://github.com/samtheruby/infinidysk/commit/95566994c68b7f302bb2499e56416688d567bf3d))
* **deps:** Bump zensical from 0.0.55 to 0.0.56 in the docs-python group ([#1201](https://github.com/samtheruby/infinidysk/issues/1201)) ([d5c2f23](https://github.com/samtheruby/infinidysk/commit/d5c2f23bac1f3c8b909ff7cf511003b5dc24bad3))
* **deps:** Bump zensical from 0.0.56 to 0.0.57 in the docs-python group ([#1253](https://github.com/samtheruby/infinidysk/issues/1253)) ([c9c5b97](https://github.com/samtheruby/infinidysk/commit/c9c5b97d81758ec4e7f55e79a7f85ea371a21efe))
* **deps:** Bump zensical from 0.0.57 to 0.0.59 in the docs-python group ([#1391](https://github.com/samtheruby/infinidysk/issues/1391)) ([1a98063](https://github.com/samtheruby/infinidysk/commit/1a98063c5f76aeefda74014cd1a99c2212feac45))
* **deps:** Bump zensical from 0.0.59 to 0.0.61 in the docs-python group ([#1476](https://github.com/samtheruby/infinidysk/issues/1476)) ([5b6d6ff](https://github.com/samtheruby/infinidysk/commit/5b6d6ff188b74881fe52d61eecbae97686450348))
* **deps:** Bump zensical from 0.0.61 to 0.0.62 in the docs-python group ([#1530](https://github.com/samtheruby/infinidysk/issues/1530)) ([e71d7d1](https://github.com/samtheruby/infinidysk/commit/e71d7d1316a61647609f9ace1da8a32fb078fd8e))
* **deps:** Bump zensical from 0.0.62 to 0.0.64 in the docs-python group ([#1600](https://github.com/samtheruby/infinidysk/issues/1600)) ([8064d1e](https://github.com/samtheruby/infinidysk/commit/8064d1e029d8bb5561e2ce6b259d3ab4026d2e47))
* **deps:** Bump zensical from 0.0.64 to 0.0.65 in the docs-python group ([#1626](https://github.com/samtheruby/infinidysk/issues/1626)) ([0ad6d23](https://github.com/samtheruby/infinidysk/commit/0ad6d23b82c1a578da68831febf7a1f343a1a96c))
* **deps:** Bump zensical from 0.0.65 to 0.0.66 in the docs-python group ([#1641](https://github.com/samtheruby/infinidysk/issues/1641)) ([a388993](https://github.com/samtheruby/infinidysk/commit/a3889933ca1ec87917c72ffb1f4c624d204eec90))
* **deps:** Bump zensical from 0.0.66 to 0.0.67 in the docs-python group ([#1680](https://github.com/samtheruby/infinidysk/issues/1680)) ([c1df5ae](https://github.com/samtheruby/infinidysk/commit/c1df5ae6882c6bb21a5fef0b7fd89d6f3bb5fc99))
* **docker:** ship the musl rapidyenc native in the Alpine image ([#1370](https://github.com/samtheruby/infinidysk/issues/1370)) ([5275648](https://github.com/samtheruby/infinidysk/commit/52756484649bfe974397e45dec012871af284ada))
* **health:** a provider outage no longer marks good files as damaged ([#1829](https://github.com/samtheruby/infinidysk/issues/1829)) ([e8963ed](https://github.com/samtheruby/infinidysk/commit/e8963edac9355be750a6073988403993cd3986a9))
* **health:** broken files from an Arr that cannot repair them are kept for you instead of deleted ([#1837](https://github.com/samtheruby/infinidysk/issues/1837)) ([c3bd0ba](https://github.com/samtheruby/infinidysk/commit/c3bd0baf90b13846da6aca35e26f945b106385e4))
* **health:** clarify Library Directory requirements ([#1302](https://github.com/samtheruby/infinidysk/issues/1302)) ([8843fb7](https://github.com/samtheruby/infinidysk/commit/8843fb778df74ea1ef8e3c9ae032d669076713c9))
* **health:** classify persistently missing streaming payloads as orphaned ([#1215](https://github.com/samtheruby/infinidysk/issues/1215)) ([70323ff](https://github.com/samtheruby/infinidysk/commit/70323fffaacb128d691bf24bebb6726dec27b034))
* **health:** clear stale pending repairs when recording deferred results ([#1462](https://github.com/samtheruby/infinidysk/issues/1462)) ([e51ffd8](https://github.com/samtheruby/infinidysk/commit/e51ffd8cbe78948c33910f7f6b11abcce85e72cb))
* **health:** defer contended PAR2 repairs ([#1383](https://github.com/samtheruby/infinidysk/issues/1383)) ([4bc4a21](https://github.com/samtheruby/infinidysk/commit/4bc4a212cb7e11fd71799989cb4191256283a644))
* **health:** explain blocked removals and omit file extensions from searches ([#1490](https://github.com/samtheruby/infinidysk/issues/1490)) ([e9f2734](https://github.com/samtheruby/infinidysk/commit/e9f2734558d7f88a0536826eaa33f7b10a48f5f8))
* **health:** files PAR2 cannot repair are no longer stuck behind other PAR2 repairs ([#1761](https://github.com/samtheruby/infinidysk/issues/1761)) ([afa599d](https://github.com/samtheruby/infinidysk/commit/afa599d255bc9c0751a4b3ceccaf2d91d75382e1))
* **health:** files replaced by Sonarr/Radarr upgrades no longer pile up as "Not library linked" ([#1754](https://github.com/samtheruby/infinidysk/issues/1754)) ([b1578be](https://github.com/samtheruby/infinidysk/commit/b1578be2038e97692d4c53b16c5ae2ba4c894d31))
* **health:** flag unlinked files and allow needs-attention removal with read-only WebDAV ([#1494](https://github.com/samtheruby/infinidysk/issues/1494)) ([d907cbc](https://github.com/samtheruby/infinidysk/commit/d907cbc076d84bf7fff37961f5eb73fa2db444ba))
* **health:** health checks no longer appear stuck at 0% for hours on dead releases ([#1611](https://github.com/samtheruby/infinidysk/issues/1611)) ([8927443](https://github.com/samtheruby/infinidysk/commit/89274437e7396804e7d2a3419e14927b045e02c8))
* **health:** Health page no longer reports previously scanned files as awaiting their initial scan ([#1577](https://github.com/samtheruby/infinidysk/issues/1577)) ([12a3415](https://github.com/samtheruby/infinidysk/commit/12a34153ec3cefca240119d32959209c1e344b81))
* **health:** hold the write permit only while health work writes ([#1868](https://github.com/samtheruby/infinidysk/issues/1868)) ([07a61e5](https://github.com/samtheruby/infinidysk/commit/07a61e5c2edf9b2009357f587b46fc7c841b1ee5))
* **health:** include history-linked files in routine checks ([#1466](https://github.com/samtheruby/infinidysk/issues/1466)) ([d55e941](https://github.com/samtheruby/infinidysk/commit/d55e941e7bdfcdf150c919282d49bf78578a2749))
* **health:** initialize the playback repair trigger before serving requests ([#1705](https://github.com/samtheruby/infinidysk/issues/1705)) ([18a0c4b](https://github.com/samtheruby/infinidysk/commit/18a0c4bf0448ddf02c329ac12a613fcce8b33caf))
* **health:** keep prune and unlinked-file cleanup running if progress reporting fails ([#1272](https://github.com/samtheruby/infinidysk/issues/1272)) ([d62d57e](https://github.com/samtheruby/infinidysk/commit/d62d57eb33f0661b6ac2e6d7cebad504f7da5e80))
* **health:** keep recently played files available during automatic repair ([#1713](https://github.com/samtheruby/infinidysk/issues/1713)) ([4bef51e](https://github.com/samtheruby/infinidysk/commit/4bef51e7dca75fdb16ee1e174d20f07b0064aab3))
* **health:** keep running health checks visible after starting a full scan ([#1481](https://github.com/samtheruby/infinidysk/issues/1481)) ([ab7652a](https://github.com/samtheruby/infinidysk/commit/ab7652a06c5cd74e4a1bcbd7b26a66847506eb54))
* **health:** PAR2 background repair is now off by default ([#1762](https://github.com/samtheruby/infinidysk/issues/1762)) ([d8169d4](https://github.com/samtheruby/infinidysk/commit/d8169d47771aa4b9e2720aa0d915dd385b7e2fa5))
* **health:** PAR2 repair no longer fails on multi-volume releases with an identity byte-limit error ([#1694](https://github.com/samtheruby/infinidysk/issues/1694)) ([f5bc20b](https://github.com/samtheruby/infinidysk/commit/f5bc20b93ac6f106bf3d4d7dcc1bd89e9e95883d))
* **health:** preserve urgent repairs across concurrent checks ([#1407](https://github.com/samtheruby/infinidysk/issues/1407)) ([33ebeef](https://github.com/samtheruby/infinidysk/commit/33ebeefd5504753038de7b20fc931dbef6789031))
* **health:** prevent cancellation leaving old files behind after successful Arr repairs ([#1503](https://github.com/samtheruby/infinidysk/issues/1503)) ([272d575](https://github.com/samtheruby/infinidysk/commit/272d57543205b22c79ab601bad9b7d9712d12a53))
* **health:** prevent false repairs when stored segment alternatives are available ([#1373](https://github.com/samtheruby/infinidysk/issues/1373)) ([6fb47d9](https://github.com/samtheruby/infinidysk/commit/6fb47d9fa94700a02880a2d6a4ece535708f2aaf))
* **health:** prevent health alerts timing out on large histories ([#1518](https://github.com/samtheruby/infinidysk/issues/1518)) ([37173d3](https://github.com/samtheruby/infinidysk/commit/37173d36ebf2ec6b4738d260d7d4f43804fa302d))
* **health:** prevent provider timeouts from triggering repair or blocklisting ([#1457](https://github.com/samtheruby/infinidysk/issues/1457)) ([447c2bd](https://github.com/samtheruby/infinidysk/commit/447c2bd094834d0192ef79a06485af91d9b04e29))
* **health:** recover libraries downloaded before 1.3.0 ([#1335](https://github.com/samtheruby/infinidysk/issues/1335)) ([528eca5](https://github.com/samtheruby/infinidysk/commit/528eca5f2fc2ba362441848c02cb024c994336fe))
* **health:** recover PAR2 repair after transient patch catalog load failures ([#1277](https://github.com/samtheruby/infinidysk/issues/1277)) ([f7a27f3](https://github.com/samtheruby/infinidysk/commit/f7a27f395a05bc3e76191b038425483e2a0f10bd))
* **health:** repair Arr-linked files after SAB history cleanup ([#1282](https://github.com/samtheruby/infinidysk/issues/1282)) ([e5cf9c9](https://github.com/samtheruby/infinidysk/commit/e5cf9c9295cca9c81da7f21a5afc4d6975e3d9a0))
* **health:** repairs follow the Arr's own search instead of always waiting two minutes ([#1867](https://github.com/samtheruby/infinidysk/issues/1867)) ([9b6ae7a](https://github.com/samtheruby/infinidysk/commit/9b6ae7a7758499d692d1181573784a83a5c40dec))
* **health:** repairs no longer replace a newer file the Arr imported from another download ([#1832](https://github.com/samtheruby/infinidysk/issues/1832)) ([107cabe](https://github.com/samtheruby/infinidysk/commit/107cabe2704dcb0ad23e703c4a36fc816ed64b57))
* **health:** replace releases that break during playback instead of keeping them as damaged ([#1631](https://github.com/samtheruby/infinidysk/issues/1631)) ([e250e47](https://github.com/samtheruby/infinidysk/commit/e250e478d3876486c52dafb93127e0387b3064fc))
* **health:** require a pure definitive-miss provider walk before treating a segment as missing ([9d34565](https://github.com/samtheruby/infinidysk/commit/9d345657d59952064c0b28bdf164516908e14116))
* **health:** show a complete health overview breakdown totaling 100% ([#1458](https://github.com/samtheruby/infinidysk/issues/1458)) ([207758e](https://github.com/samtheruby/infinidysk/commit/207758e85df4a81550f3bda56c74db9b330345f1))
* **health:** start orphan cleanup retry budget after contention ([#1464](https://github.com/samtheruby/infinidysk/issues/1464)) ([6d255ae](https://github.com/samtheruby/infinidysk/commit/6d255aebdfa2469a8998d156131682b2ee6032e3))
* **health:** stay idle when no usenet provider is enabled ([#1573](https://github.com/samtheruby/infinidysk/issues/1573)) ([8f67a44](https://github.com/samtheruby/infinidysk/commit/8f67a442bfe0db110d5972894cccb5ec6f9ca920))
* **health:** stop deleting linked files after inconclusive Arr lookups ([#1229](https://github.com/samtheruby/infinidysk/issues/1229)) ([997eb59](https://github.com/samtheruby/infinidysk/commit/997eb59b2c2b1a270c6f1bc3e2db3a60986c10b1)), closes [#1221](https://github.com/samtheruby/infinidysk/issues/1221)
* **health:** stop PAR2 identity probing of dead volumes with untrusted ranges ([#1752](https://github.com/samtheruby/infinidysk/issues/1752)) ([6000cd4](https://github.com/samtheruby/infinidysk/commit/6000cd49edcd5e209567c3b4a559b746e9e0ddd6))
* **health:** treat null pending multipart parts as empty during PAR2 repair ([#1740](https://github.com/samtheruby/infinidysk/issues/1740)) ([933b800](https://github.com/samtheruby/infinidysk/commit/933b800c57b6749abe93c1d55087d874530acdd7))
* **health:** urgent streaming repairs keep their failure count across restarts ([#1496](https://github.com/samtheruby/infinidysk/issues/1496)) ([a60e759](https://github.com/samtheruby/infinidysk/commit/a60e759ded0debcfb0e44d45a01050067ad72836))
* **health:** verify PAR2 slices before applying the damage cap ([#1213](https://github.com/samtheruby/infinidysk/issues/1213)) ([017eb23](https://github.com/samtheruby/infinidysk/commit/017eb23dc69381065d7549c47f9cad607117d1f1))
* **hosting:** backend exits nonzero after a hosted background service crashes ([#1273](https://github.com/samtheruby/infinidysk/issues/1273)) ([8990114](https://github.com/samtheruby/infinidysk/commit/899011478f4bbe5fa6867a4fde6e667f1a86ecbf))
* **import:** measure a pending volume when a known size cannot fit its articles ([#1878](https://github.com/samtheruby/infinidysk/issues/1878)) ([180f9ab](https://github.com/samtheruby/infinidysk/commit/180f9abf1eddd581a6257da7a5e8ca021a19ea92))
* **import:** migrate large legacy metadata without size-based skips ([#1797](https://github.com/samtheruby/infinidysk/issues/1797)) ([29f8e2f](https://github.com/samtheruby/infinidysk/commit/29f8e2f4b9eb83f4cfc41fc739b1e853321a9534))
* **import:** migration no longer follows symlinks out of the old config folder ([#1796](https://github.com/samtheruby/infinidysk/issues/1796)) ([a877923](https://github.com/samtheruby/infinidysk/commit/a877923a8bb0cbaacf7f71662bd1f8bd4747c6bf))
* **import:** reject Arr paths that climb out of a library folder ([#1800](https://github.com/samtheruby/infinidysk/issues/1800)) ([fe058ed](https://github.com/samtheruby/infinidysk/commit/fe058edfa5dcd20dc2b98ce2bce766d2ba54d053))
* **import:** the import report shows progress instead of a silent console ([#1877](https://github.com/samtheruby/infinidysk/issues/1877)) ([b29bc25](https://github.com/samtheruby/infinidysk/commit/b29bc257bd0ecf55b025fc8027f74a4e41e963ea))
* **import:** upgrading from 1.x shows progress while it checks your library instead of looking stuck ([#1799](https://github.com/samtheruby/infinidysk/issues/1799)) ([53bd352](https://github.com/samtheruby/infinidysk/commit/53bd3524485eed2339fe61669eb0985066f356d0))
* **metrics:** count shared-stream pump fetches as client reads ([#1350](https://github.com/samtheruby/infinidysk/issues/1350)) ([581833f](https://github.com/samtheruby/infinidysk/commit/581833f81d0e36035d27727201f97b98f7144d9e))
* **metrics:** Overview Backup rescues counts a retried provider once per rescued article ([#1576](https://github.com/samtheruby/infinidysk/issues/1576)) ([48d772f](https://github.com/samtheruby/infinidysk/commit/48d772fdb827c4274472a6a396c8b39cfed5a068))
* **metrics:** quarantine a corrupt metrics database and back off failed flushes ([#1435](https://github.com/samtheruby/infinidysk/issues/1435)) ([5093dd0](https://github.com/samtheruby/infinidysk/commit/5093dd0e7bb57c50e7d87f820ac197d17063bf67))
* **metrics:** retain historical statistics across backend restarts ([#1525](https://github.com/samtheruby/infinidysk/issues/1525)) ([cd638ce](https://github.com/samtheruby/infinidysk/commit/cd638ce1245f22357b7f66e9c68bcc56ea7f705f))
* **mount:** distinguish failed tuning writes from external tuning ([#1866](https://github.com/samtheruby/infinidysk/issues/1866)) ([3bee375](https://github.com/samtheruby/infinidysk/commit/3bee3758d2602bc8a003b93298c453550c114883))
* **mount:** keep files referenced by legacy library links ([#1828](https://github.com/samtheruby/infinidysk/issues/1828)) ([4e1c914](https://github.com/samtheruby/infinidysk/commit/4e1c914b7ad927bbf205126199ff9955981ef2bc))
* **nntp:** bound fresh connection acquisition ([#1409](https://github.com/samtheruby/infinidysk/issues/1409)) ([f912daa](https://github.com/samtheruby/infinidysk/commit/f912daa81d93e120ce1c214096943bc7baea878b))
* **nntp:** brief connection failures no longer shrink the provider pool ([#1883](https://github.com/samtheruby/infinidysk/issues/1883)) ([b77a82f](https://github.com/samtheruby/infinidysk/commit/b77a82f78d189065ff6ef8cc638abf291e59723e))
* **nntp:** fail over on articles that end before their announced size ([#1805](https://github.com/samtheruby/infinidysk/issues/1805)) ([27ce044](https://github.com/samtheruby/infinidysk/commit/27ce0448d4b6a27f4ffe990dadf2b195c29d72e5))
* **nntp:** handle late connection factory cancellation without stacks ([#1473](https://github.com/samtheruby/infinidysk/issues/1473)) ([13acf51](https://github.com/samtheruby/infinidysk/commit/13acf519e3b9b45a8115d521820459c0d8fbf275))
* **nntp:** keep playback working when a provider returns the wrong post ([#1357](https://github.com/samtheruby/infinidysk/issues/1357)) ([b4ede00](https://github.com/samtheruby/infinidysk/commit/b4ede004a35d47b966b3b4480167a47b9eaf9625))
* **nntp:** keep streaming when an article-completion observer throws ([#1275](https://github.com/samtheruby/infinidysk/issues/1275)) ([6cc3ee1](https://github.com/samtheruby/infinidysk/commit/6cc3ee122028c14537df804e37854d2c894d5750))
* **nntp:** normalize pooled capacity by configured connection limits ([#1491](https://github.com/samtheruby/infinidysk/issues/1491)) ([570975f](https://github.com/samtheruby/infinidysk/commit/570975f53b67888d6625aac3e9f23140bf201322))
* **nntp:** playback and imports no longer stall when a provider refuses extra connections ([#1623](https://github.com/samtheruby/infinidysk/issues/1623)) ([5b5260e](https://github.com/samtheruby/infinidysk/commit/5b5260eb60ca8ac3385fbed865dcc8fe433ac4b9))
* **nntp:** releases with obfuscated yEnc headers play instead of hanging and being removed ([#1548](https://github.com/samtheruby/infinidysk/issues/1548)) ([a40a071](https://github.com/samtheruby/infinidysk/commit/a40a07159467a286ac8291b80c492e3e0949b80a))
* **nntp:** report stalled provider connections accurately and bound login time ([#1887](https://github.com/samtheruby/infinidysk/issues/1887)) ([d1bb0af](https://github.com/samtheruby/infinidysk/commit/d1bb0afe99bf5a6d9f920e88ac2d8f4a23760e16))
* **nntp:** retry on a new connection when the server ends the session with 400 ([#1889](https://github.com/samtheruby/infinidysk/issues/1889)) ([6874a08](https://github.com/samtheruby/infinidysk/commit/6874a08c44adff6ec2a26e68f786f85366daf387))
* **nntp:** skip reconnect pacing when the caller cancels a read ([#1658](https://github.com/samtheruby/infinidysk/issues/1658)) ([6f8a40c](https://github.com/samtheruby/infinidysk/commit/6f8a40c6b654d02a23aa02b73c11b99935e6fb8a))
* **nntp:** treat 481 "maximum connections per user" as a connection limit ([#1668](https://github.com/samtheruby/infinidysk/issues/1668)) ([c50c2f9](https://github.com/samtheruby/infinidysk/commit/c50c2f9644c7b81b1de3a1e1520e3d6b76216d1b))
* **nntp:** validate article offsets after the full part header arrives ([#1886](https://github.com/samtheruby/infinidysk/issues/1886)) ([5ac1ab2](https://github.com/samtheruby/infinidysk/commit/5ac1ab2b9c5556b441e7cc117722032016a7a3e2))
* **par2:** index large PAR2 sets without quadratic lookups ([#1801](https://github.com/samtheruby/infinidysk/issues/1801)) ([8c1fdff](https://github.com/samtheruby/infinidysk/commit/8c1fdff880d8693bb1b4081580587aa209794f67))
* **queue:** accept NZBs with up to 1,302,083 segments ([#1220](https://github.com/samtheruby/infinidysk/issues/1220)) ([a7b0256](https://github.com/samtheruby/infinidysk/commit/a7b0256f4edce6a7fd0e6b091b3d1bbd977912ea))
* **queue:** add nested archive context to media validation failures ([#1516](https://github.com/samtheruby/infinidysk/issues/1516)) ([fb68a84](https://github.com/samtheruby/infinidysk/commit/fb68a8481ec818d394a6213ba2a8dfc057b3c1df))
* **queue:** allow reviewed cleanup of large orphan backlogs ([#1352](https://github.com/samtheruby/infinidysk/issues/1352)) ([b5bf01e](https://github.com/samtheruby/infinidysk/commit/b5bf01efc8364de4a8b3479fc69e4a368a225e02))
* **queue:** bound outstanding import tasks ([#1803](https://github.com/samtheruby/infinidysk/issues/1803)) ([1155315](https://github.com/samtheruby/infinidysk/commit/11553154af8a75c533527c85a6679078115a780c))
* **queue:** busy database no longer marks completed downloads as failed ([#1197](https://github.com/samtheruby/infinidysk/issues/1197)) ([63b3ddd](https://github.com/samtheruby/infinidysk/commit/63b3ddd93658b729cdccd940c6bada395ab3c886)), closes [#1180](https://github.com/samtheruby/infinidysk/issues/1180)
* **queue:** bypass packed range lookup for empty 7z members ([#1505](https://github.com/samtheruby/infinidysk/issues/1505)) ([5ac8313](https://github.com/samtheruby/infinidysk/commit/5ac83133f363ec5bf422b6e3b8d0cb85afd5b68b))
* **queue:** cancelled imports no longer keep parsing huge NZB files ([#1192](https://github.com/samtheruby/infinidysk/issues/1192)) ([946637d](https://github.com/samtheruby/infinidysk/commit/946637d42226638887fea0195f66bd80cbb5f7a4))
* **queue:** classify unsupported 7z compression before packed range lookup ([#1468](https://github.com/samtheruby/infinidysk/issues/1468)) ([f9354d4](https://github.com/samtheruby/infinidysk/commit/f9354d46816cf39ae9475ca3532894eb2f5b6f23))
* **queue:** deleting or pausing a stuck download no longer hangs forever ([#1198](https://github.com/samtheruby/infinidysk/issues/1198)) ([4df9040](https://github.com/samtheruby/infinidysk/commit/4df9040c03f25a15896f119a1f8904b0247a199a))
* **queue:** do not record inconclusive article misses as missing evidence ([#1745](https://github.com/samtheruby/infinidysk/issues/1745)) ([1db170a](https://github.com/samtheruby/infinidysk/commit/1db170a7be78a620bb9877a433bb9eea2fcac5ef))
* **queue:** explain intentional archive compression rejection ([#1470](https://github.com/samtheruby/infinidysk/issues/1470)) ([efd1368](https://github.com/samtheruby/infinidysk/commit/efd1368241e5105cfc28cbaf100fae783c987214))
* **queue:** fail over when a provider returns another post's first segment ([87a6f87](https://github.com/samtheruby/infinidysk/commit/87a6f87a37597fe88fb5f7c9cae81f7c03be2fa1))
* **queue:** failed imports no longer leave orphaned STRM files on disk ([#1196](https://github.com/samtheruby/infinidysk/issues/1196)) ([80cf116](https://github.com/samtheruby/infinidysk/commit/80cf11666ef2e41726d45174c0332894ea8b9ef7))
* **queue:** filter sample-directory videos without sibling-size comparisons ([#1475](https://github.com/samtheruby/infinidysk/issues/1475)) ([f76d460](https://github.com/samtheruby/infinidysk/commit/f76d46077de21011e80261ff5c7774b4a9095451))
* **queue:** group shuffled first RAR volumes with matching continuations ([8bc3a18](https://github.com/samtheruby/infinidysk/commit/8bc3a183c3feb1aad7671caeb30203e76588f703))
* **queue:** import independent RAR and 7z archive sets separately ([#1382](https://github.com/samtheruby/infinidysk/issues/1382)) ([c9250ba](https://github.com/samtheruby/infinidysk/commit/c9250bac749ed0c70522f6091225ee194dd74a23))
* **queue:** import logs now explain why PAR2-verified recovery was unavailable for mismatched yEnc articles ([#1519](https://github.com/samtheruby/infinidysk/issues/1519)) ([57bc644](https://github.com/samtheruby/infinidysk/commit/57bc644042d354cf1ed156aae7d1b1da56c862c0))
* **queue:** import RAR releases with individually scrambled volume names ([#1469](https://github.com/samtheruby/infinidysk/issues/1469)) ([eac163b](https://github.com/samtheruby/infinidysk/commit/eac163b6104733218342e4fb687fba1aa258a238))
* **queue:** imported files keep their Usenet post date when Queue Pipelining is enabled ([#1637](https://github.com/samtheruby/infinidysk/issues/1637)) ([036cbea](https://github.com/samtheruby/infinidysk/commit/036cbeaeeb15aac187a60e6256be6bf447dd3d22))
* **queue:** indexer watermark files no longer fail imports with 'Rar signature not found' on some providers ([#1679](https://github.com/samtheruby/infinidysk/issues/1679)) ([e1130a0](https://github.com/samtheruby/infinidysk/commit/e1130a0129fa4ffb479a0fa226b696cc575706fe))
* **queue:** keep replacement uploads within the configured queue limit ([#1527](https://github.com/samtheruby/infinidysk/issues/1527)) ([d8aaf2d](https://github.com/samtheruby/infinidysk/commit/d8aaf2d2e58970b9eda8606ea93f33ab8ba27e3f))
* **queue:** large imports of missing or corrupt Usenet articles no longer grind the server ([#1188](https://github.com/samtheruby/infinidysk/issues/1188)) ([544aa6c](https://github.com/samtheruby/infinidysk/commit/544aa6ce180c27f2fc85cb0134bc07857d343216))
* **queue:** large NZBs up to 256 MiB no longer rejected during import ([#1177](https://github.com/samtheruby/infinidysk/issues/1177)) ([3328f03](https://github.com/samtheruby/infinidysk/commit/3328f0304c0ca378bbb247b480ca22fa6ac033cb))
* **queue:** lazy RAR mounting no longer drops extra files hidden behind the first archive member ([#1453](https://github.com/samtheruby/infinidysk/issues/1453)) ([55f9b5c](https://github.com/samtheruby/infinidysk/commit/55f9b5ce044aad98a506c6d1bdeae24bce800a44))
* **queue:** leftover STRM files are cleaned up and samples in Sample folders no longer get mounted ([#1169](https://github.com/samtheruby/infinidysk/issues/1169)) ([87993e1](https://github.com/samtheruby/infinidysk/commit/87993e17a1bec27feefd4ee046aaf09536b69040))
* **queue:** limit concurrent archive key derivations ([#1804](https://github.com/samtheruby/infinidysk/issues/1804)) ([6073369](https://github.com/samtheruby/infinidysk/commit/607336974219104987752825e99fd17ba9c6ae4a))
* **queue:** NZBs with long Usenet subjects no longer rejected during import ([#1160](https://github.com/samtheruby/infinidysk/issues/1160)) ([d98be41](https://github.com/samtheruby/infinidysk/commit/d98be418345d1bcaf36d8bdf3d35bc098e3323cc))
* **queue:** preserve first-volume header ordering for stored RAR files ([#1688](https://github.com/samtheruby/infinidysk/issues/1688)) ([206b9ad](https://github.com/samtheruby/infinidysk/commit/206b9ad7e0f48c3a9147a3c88def368d23298919))
* **queue:** preserve jobs and retry delays during concurrent queue changes ([#1399](https://github.com/samtheruby/infinidysk/issues/1399)) ([8ddebd9](https://github.com/samtheruby/infinidysk/commit/8ddebd99efd860b66f452a7dac976b8fd68902d9))
* **queue:** preserve playback for NZBs with omitted interior parts ([#1594](https://github.com/samtheruby/infinidysk/issues/1594)) ([b3396fe](https://github.com/samtheruby/infinidysk/commit/b3396fe8ca57a0023cf9275638c77b91bc0e338b))
* **queue:** restart instead of serving a dead queue after processor failure ([#1287](https://github.com/samtheruby/infinidysk/issues/1287)) ([cb77327](https://github.com/samtheruby/infinidysk/commit/cb77327fd26e80bf61e64b1b5edc12e0d6135251))
* **queue:** restore a single import strategy instead of dual symlink and STRM outputs ([#1171](https://github.com/samtheruby/infinidysk/issues/1171)) ([144cac9](https://github.com/samtheruby/infinidysk/commit/144cac947fa32290d540d7d6be2e33837af12983))
* **queue:** season packs with repeated RAR/7z volume numbers import as separate archives ([#1452](https://github.com/samtheruby/infinidysk/issues/1452)) ([9b4739b](https://github.com/samtheruby/infinidysk/commit/9b4739b4ce55314943db7c0c2145136621338cb5))
* **queue:** skip unavailable optional first-segment metadata ([#1625](https://github.com/samtheruby/infinidysk/issues/1625)) ([b9604a2](https://github.com/samtheruby/infinidysk/commit/b9604a2321d71266a1d641d322fc8c78dcdd325c))
* **queue:** stop reprocessing releases that already failed health validation ([#1216](https://github.com/samtheruby/infinidysk/issues/1216)) ([a08b848](https://github.com/samtheruby/infinidysk/commit/a08b8484ce5b279d7f311634c90d9c5a4ab60cd7))
* **queue:** STRM and library files are no longer written through symlinked subfolders ([#1798](https://github.com/samtheruby/infinidysk/issues/1798)) ([b030f90](https://github.com/samtheruby/infinidysk/commit/b030f9001a1bccd85ad223533ee7c6cd10753117))
* **queue:** STRM cleanup and writes no longer follow planted paths out of the STRM folder ([#1793](https://github.com/samtheruby/infinidysk/issues/1793)) ([ce0868e](https://github.com/samtheruby/infinidysk/commit/ce0868e4175c58dba3a9611d462847938482324d))
* **rclone:** improve mount recommendations and RC connection tests ([#1311](https://github.com/samtheruby/infinidysk/issues/1311)) ([efca97d](https://github.com/samtheruby/infinidysk/commit/efca97d333bf984fc7bc5ddb5a06dc34d705178c))
* retry a busy daily maintenance slot in place instead of skipping to tomorrow ([#1747](https://github.com/samtheruby/infinidysk/issues/1747)) ([d46bf6e](https://github.com/samtheruby/infinidysk/commit/d46bf6ee74b45e90a6d5d50d1686294083a5685f))
* **sab:** accept duplicate segment fallbacks and keep validation errors bounded ([#1400](https://github.com/samtheruby/infinidysk/issues/1400)) ([11d587b](https://github.com/samtheruby/infinidysk/commit/11d587beb8523ed4ca95d04369dc59b4bff2871a))
* **sab:** deleting a queue item that is failing at the same moment no longer returns HTTP 500 ([#1309](https://github.com/samtheruby/infinidysk/issues/1309)) ([71a52c8](https://github.com/samtheruby/infinidysk/commit/71a52c878a0634c3eb72a2ea95ce498b3101795a))
* **sab:** oversize NZBs and stalled indexer fetches are rejected before they fill the disk ([#1195](https://github.com/samtheruby/infinidysk/issues/1195)) ([133cd42](https://github.com/samtheruby/infinidysk/commit/133cd4277042e78cf2bbb3b607204429b9c89b66))
* **sab:** Sonarr/Radarr no longer loop on "Download doesn't contain intermediate path" after a job folder is removed ([#1347](https://github.com/samtheruby/infinidysk/issues/1347)) ([295c4cc](https://github.com/samtheruby/infinidysk/commit/295c4cc9eb0106a3efef7cc3ec7331ef2bbdeabb))
* scheduled orphan cleanup and database backups no longer skip nights ([#1738](https://github.com/samtheruby/infinidysk/issues/1738)) ([ce51abc](https://github.com/samtheruby/infinidysk/commit/ce51abc223622c53d3e4c62623e12283b4035c6e))
* **sharpcompress:** truncate RAR passwords to 127 characters before key derivation ([#1751](https://github.com/samtheruby/infinidysk/issues/1751)) ([db347c7](https://github.com/samtheruby/infinidysk/commit/db347c75c4a32d4d029f2dfcd8839e83a8f47eff))
* **stream:** fetch a segment again when its read-ahead failed before the reader needed it ([#1888](https://github.com/samtheruby/infinidysk/issues/1888)) ([159efcb](https://github.com/samtheruby/infinidysk/commit/159efcbb1768f0d50e4b06d8e92271314ade8459))
* **ui:** align streaming bandwidth input width ([#1260](https://github.com/samtheruby/infinidysk/issues/1260)) ([ec10a5a](https://github.com/samtheruby/infinidysk/commit/ec10a5a9e4cb4d2acebfa8195d7d121e1775c2ef))
* **ui:** align the admin UI with daisyUI defaults and accessible controls ([#1206](https://github.com/samtheruby/infinidysk/issues/1206)) ([b34f994](https://github.com/samtheruby/infinidysk/commit/b34f994e416104c5b90b22146924bc87b23d57b0))
* **ui:** clarify Activity totals and make support easier to find ([#1485](https://github.com/samtheruby/infinidysk/issues/1485)) ([eaba97a](https://github.com/samtheruby/infinidysk/commit/eaba97a0a91d93b64a55205558fefb0ea3464a45))
* **ui:** cleanup shows how many empty folders it removed, and cancel stops it ([#1884](https://github.com/samtheruby/infinidysk/issues/1884)) ([6c0f572](https://github.com/samtheruby/infinidysk/commit/6c0f572741163456d5533819e4e8babe87b98fa2))
* **ui:** clearer status and failure reasons on phones, and a missing-articles rate that reflects playback ([#1874](https://github.com/samtheruby/infinidysk/issues/1874)) ([6b6dcad](https://github.com/samtheruby/infinidysk/commit/6b6dcad9092a08f0a3792e879fd27e6737fd9b7d))
* **ui:** compact idle Right now, keep Arr Health on-screen, and tooltip the rename setting ([#1265](https://github.com/samtheruby/infinidysk/issues/1265)) ([5e89125](https://github.com/samtheruby/infinidysk/commit/5e89125aac14701b68b1681e940e6a197c0b2500))
* **ui:** connect expanded provider speed paths through zero ([#1554](https://github.com/samtheruby/infinidysk/issues/1554)) ([4a50932](https://github.com/samtheruby/infinidysk/commit/4a50932365bc75bd46157b41b91cecb71c4f3a33))
* **ui:** connect sparse provider throughput graph to zero baseline ([#1553](https://github.com/samtheruby/infinidysk/issues/1553)) ([a533693](https://github.com/samtheruby/infinidysk/commit/a533693a4e3f4f290c8e66176dbcf748ffb100c5))
* **ui:** connections counter no longer flashes a spinner on the queue page ([#1154](https://github.com/samtheruby/infinidysk/issues/1154)) ([9edff32](https://github.com/samtheruby/infinidysk/commit/9edff32ab7fedebb6c4cf11121b42825b9ca18ae))
* **ui:** explain degraded Arr warnings directly on overview ([#1504](https://github.com/samtheruby/infinidysk/issues/1504)) ([23d6593](https://github.com/samtheruby/infinidysk/commit/23d6593646b835b80d31700ef18a94882bf14ffd))
* **ui:** hide all-clear alert indicator ([#1549](https://github.com/samtheruby/infinidysk/issues/1549)) ([401c8c3](https://github.com/samtheruby/infinidysk/commit/401c8c3d404d1560476ac466f159cb99b3a6485e))
* **ui:** identify active media reads with parent folder names ([#1562](https://github.com/samtheruby/infinidysk/issues/1562)) ([b81c13f](https://github.com/samtheruby/infinidysk/commit/b81c13f4d23c65033fdd39922aa6ff5880a94b02))
* **ui:** keep Arr Health last-import tooltip inside the dashboard ([#1283](https://github.com/samtheruby/infinidysk/issues/1283)) ([d62a8b5](https://github.com/samtheruby/infinidysk/commit/d62a8b516c584e95dec96a638aaf81968dcdfb87))
* **ui:** keep existing installs on overview ([#1333](https://github.com/samtheruby/infinidysk/issues/1333)) ([2329c0d](https://github.com/samtheruby/infinidysk/commit/2329c0d9603015fb105cda92c5d5e503ae4d3304))
* **ui:** keep overview stats and help text usable on phones ([#1259](https://github.com/samtheruby/infinidysk/issues/1259)) ([f9439ff](https://github.com/samtheruby/infinidysk/commit/f9439ffdaee011e0304ca3e25a923664087f6b7d))
* **ui:** live file reads are now full-width rows in the Overview stack ([#1162](https://github.com/samtheruby/infinidysk/issues/1162)) ([400a99f](https://github.com/samtheruby/infinidysk/commit/400a99fef921f4a5e4e25dd9cb6e3a4adaa29b62))
* **ui:** lock live read card height above the scrollport ([#1563](https://github.com/samtheruby/infinidysk/issues/1563)) ([d64e7f9](https://github.com/samtheruby/infinidysk/commit/d64e7f933a22950187a7b0766c3cf76b441602f9))
* **ui:** make health alerts and playback failures easier to inspect ([#1499](https://github.com/samtheruby/infinidysk/issues/1499)) ([0d0d7b6](https://github.com/samtheruby/infinidysk/commit/0d0d7b6e1f5e8de4ff6027ca5065d22f61428c86))
* **ui:** make overlapping and low-volume activity easier to inspect ([#1538](https://github.com/samtheruby/infinidysk/issues/1538)) ([d4a1be8](https://github.com/samtheruby/infinidysk/commit/d4a1be83a2bc1428a44ece8916501173bf0a4323))
* **ui:** mark backup providers on the Overview Providers card ([#1579](https://github.com/samtheruby/infinidysk/issues/1579)) ([abb18af](https://github.com/samtheruby/infinidysk/commit/abb18afd6b152e005274621f67af2bbc6356a2ca))
* **ui:** match app read legend to the activity chart ([#1355](https://github.com/samtheruby/infinidysk/issues/1355)) ([2240674](https://github.com/samtheruby/infinidysk/commit/22406748e80a958e4808bdcf6607bea7f1b8846d))
* **ui:** memory overview no longer counts reclaimable kernel cache as app memory ([#1813](https://github.com/samtheruby/infinidysk/issues/1813)) ([d4f5daf](https://github.com/samtheruby/infinidysk/commit/d4f5daf5991447d2726a5b22d9232c5d9c265c94))
* **ui:** move public Base URL into General settings ([#1411](https://github.com/samtheruby/infinidysk/issues/1411)) ([82d5501](https://github.com/samtheruby/infinidysk/commit/82d55019bcb29900b7924edbafd800e92cde47e8))
* **ui:** open tabs no longer flood the server with refreshes during large cleanups ([#1850](https://github.com/samtheruby/infinidysk/issues/1850)) ([ae1b19c](https://github.com/samtheruby/infinidysk/commit/ae1b19ca39a4d3abddc81484a7fadd74177393c5))
* **ui:** overview stats stay a compact bar on tablets and wrap 3-wide on phones ([#1163](https://github.com/samtheruby/infinidysk/issues/1163)) ([09130e2](https://github.com/samtheruby/infinidysk/commit/09130e2b8d37449b4e7c47118ebd4b1e6b62dd72))
* **ui:** per-provider MB/s chart stays continuous when there is no traffic ([#1228](https://github.com/samtheruby/infinidysk/issues/1228)) ([012168b](https://github.com/samtheruby/infinidysk/commit/012168bf005d4a0ee21fd8bc32409a246e117880))
* **ui:** prevent malformed websocket traffic from stopping the frontend ([#1280](https://github.com/samtheruby/infinidysk/issues/1280)) ([80d28df](https://github.com/samtheruby/infinidysk/commit/80d28df2bbdd28671a579e239550c135dd7fee73))
* **ui:** provider outages show for their full length in every window, including All time ([#1885](https://github.com/samtheruby/infinidysk/issues/1885)) ([ba9fb1a](https://github.com/samtheruby/infinidysk/commit/ba9fb1a2204c7d26c492447a41826ffa49d9540e))
* **ui:** queue remembers your per-page size after leaving and returning to the page ([#1564](https://github.com/samtheruby/infinidysk/issues/1564)) ([b7c341d](https://github.com/samtheruby/infinidysk/commit/b7c341d08beb040353188b96cfbd74b8f258d910))
* **ui:** reject a missing frontend/backend API key before the UI starts listening ([#1270](https://github.com/samtheruby/infinidysk/issues/1270)) ([f55a3fc](https://github.com/samtheruby/infinidysk/commit/f55a3fcf56fffeeca69f4cccc8815bbf89bead87))
* **ui:** remove experimental tag from container-aware gap fill ([#1307](https://github.com/samtheruby/infinidysk/issues/1307)) ([412fc69](https://github.com/samtheruby/infinidysk/commit/412fc6988cbefa622d410577d8794bd6a7deda56))
* **ui:** render app activity reads with a solid line ([#1349](https://github.com/samtheruby/infinidysk/issues/1349)) ([56f9d4e](https://github.com/samtheruby/infinidysk/commit/56f9d4e5535b8e371004ca15a2988b456e3151f3))
* **ui:** repair settings remain saved after refresh ([#1301](https://github.com/samtheruby/infinidysk/issues/1301)) ([381c512](https://github.com/samtheruby/infinidysk/commit/381c512a9bf05d8b5936f623aa5b352f1228eb0c))
* **ui:** reserve scrollbar gutter in media preview to stop resize loop ([#1672](https://github.com/samtheruby/infinidysk/issues/1672)) ([ec9f606](https://github.com/samtheruby/infinidysk/commit/ec9f606a05be873d7218539fb9b31a09b08fc971))
* **ui:** restore logout when a direct GET request is used ([#1445](https://github.com/samtheruby/infinidysk/issues/1445)) ([3ef8667](https://github.com/samtheruby/infinidysk/commit/3ef8667b9efeb83bc7b53558cd795e8f2fa2bf8f))
* **ui:** season packs no longer repeat the same Arr import message per episode ([#1811](https://github.com/samtheruby/infinidysk/issues/1811)) ([c141857](https://github.com/samtheruby/infinidysk/commit/c1418571699a19c0ac9c60c2b60ba3353aa24c25))
* **ui:** show a clear error and exit when the frontend port is already in use ([#1276](https://github.com/samtheruby/infinidysk/issues/1276)) ([60b5518](https://github.com/samtheruby/infinidysk/commit/60b5518f8adaf368004e86d6d1296bf08d047b71))
* **ui:** size error breakdown segments outside tooltip wrappers ([#1498](https://github.com/samtheruby/infinidysk/issues/1498)) ([d04075a](https://github.com/samtheruby/infinidysk/commit/d04075a6915f94c0848be0d94d1f72b73befd251))
* **ui:** size the Right now card to its live reads instead of the first snapshot ([#1558](https://github.com/samtheruby/infinidysk/issues/1558)) ([671f422](https://github.com/samtheruby/infinidysk/commit/671f42295a58cace2005ec8a44b2a60a44e1200b))
* **ui:** stabilize the overview dashboard layout ([#1257](https://github.com/samtheruby/infinidysk/issues/1257)) ([2e72fe9](https://github.com/samtheruby/infinidysk/commit/2e72fe941f414026e5ef2468f2e3c2196f78948f))
* **ui:** stalls on the overview count only pauses a viewer would notice ([#1830](https://github.com/samtheruby/infinidysk/issues/1830)) ([317497d](https://github.com/samtheruby/infinidysk/commit/317497d5cc93c013315f95b24172db5f271533e5))
* **ui:** stop Arr Health table from showing a phantom horizontal scrollbar ([#1267](https://github.com/samtheruby/infinidysk/issues/1267)) ([81008cc](https://github.com/samtheruby/infinidysk/commit/81008cce69cbcf98454e582463a60933dab6a455))
* **ui:** surface alerts across pages and simplify navigation ([#1508](https://github.com/samtheruby/infinidysk/issues/1508)) ([55f4aed](https://github.com/samtheruby/infinidysk/commit/55f4aed8a564e42181a9ed7c765cd871501efb23))
* **usenet:** allow imports when yEnc headers omit the total count ([#1460](https://github.com/samtheruby/infinidysk/issues/1460)) ([70e9d86](https://github.com/samtheruby/infinidysk/commit/70e9d8610791305fe45fd408c94fc7958c474d87))
* **usenet:** backup accounts in a storage group are no longer charged for an article already rejected from that group ([#1724](https://github.com/samtheruby/infinidysk/issues/1724)) ([a72e11d](https://github.com/samtheruby/infinidysk/commit/a72e11d7c74edef3e69e019ff3fc7f66c99f8c78))
* **usenet:** classify corrupt decoded bodies as health-neutral discards ([#1678](https://github.com/samtheruby/infinidysk/issues/1678)) ([ffca62a](https://github.com/samtheruby/infinidysk/commit/ffca62ae745762fb926ba3da350b3d154818b57b))
* **usenet:** disabled providers no longer keep connections open or send keep-alives ([#1542](https://github.com/samtheruby/infinidysk/issues/1542)) ([6c742f5](https://github.com/samtheruby/infinidysk/commit/6c742f517ecea0ba32277bec482a6a50db5a7698))
* **usenet:** distinguish connection-open failures from local admission waits ([#1619](https://github.com/samtheruby/infinidysk/issues/1619)) ([7f46bc3](https://github.com/samtheruby/infinidysk/commit/7f46bc3fc11e066676caaaa54b5e41490416b1d3))
* **usenet:** files are no longer reported missing or sent for repair while a provider is temporarily unavailable ([#1550](https://github.com/samtheruby/infinidysk/issues/1550)) ([59cc144](https://github.com/samtheruby/infinidysk/commit/59cc1441104bb29e2c9e56e1f0f02243d9944958))
* **usenet:** harden timeout connection lifecycle ([#1224](https://github.com/samtheruby/infinidysk/issues/1224)) ([72f4d79](https://github.com/samtheruby/infinidysk/commit/72f4d7912f4d19dcc6cac279dfc54aafdcb16fbd))
* **usenet:** include protocol reasons and open timings in breaker logs ([#1465](https://github.com/samtheruby/infinidysk/issues/1465)) ([de34a6c](https://github.com/samtheruby/infinidysk/commit/de34a6c3fb97acd19dcae22a310cc3059e8c538a))
* **usenet:** keep backup-only providers demand-only with no warm floor ([#1687](https://github.com/samtheruby/infinidysk/issues/1687)) ([41a1475](https://github.com/samtheruby/infinidysk/commit/41a1475f0784b138b76e508939233e552c875d7c))
* **usenet:** keep fewer idle warm connections open per provider by default ([#1561](https://github.com/samtheruby/infinidysk/issues/1561)) ([313acc3](https://github.com/samtheruby/infinidysk/commit/313acc34374e59b939753bbb00a68c9b4468ee9f))
* **usenet:** keep pooling and config updates running if a telemetry observer throws ([#1271](https://github.com/samtheruby/infinidysk/issues/1271)) ([ba5ae40](https://github.com/samtheruby/infinidysk/commit/ba5ae406cd27e9c5bef6ad2bf70e9ddd99f8c5f1))
* **usenet:** log per-provider yenc rejection diagnostics ([#1459](https://github.com/samtheruby/infinidysk/issues/1459)) ([2e0b576](https://github.com/samtheruby/infinidysk/commit/2e0b5764f91b63c3fc570f83a7dd782576a9864d))
* **usenet:** missing-article playback no longer freezes all streams and imports ([#1199](https://github.com/samtheruby/infinidysk/issues/1199)) ([497de64](https://github.com/samtheruby/infinidysk/commit/497de64282027ba854e2e1386277149f737f8015))
* **usenet:** playback no longer stalls when read-ahead fallbacks hold every failover slot ([#1657](https://github.com/samtheruby/infinidysk/issues/1657)) ([279ead3](https://github.com/samtheruby/infinidysk/commit/279ead31f991d1addc45b763cfc0d70fbb5b997c))
* **usenet:** preserve streaming priority and release every pipelined batch resource ([#1291](https://github.com/samtheruby/infinidysk/issues/1291)) ([a2c1151](https://github.com/samtheruby/infinidysk/commit/a2c11515f3cb98f0721793098d500dfdc1d7c5b2))
* **usenet:** prevent abandoned reads from disabling healthy providers ([#1521](https://github.com/samtheruby/infinidysk/issues/1521)) ([894da90](https://github.com/samtheruby/infinidysk/commit/894da90604a24505988f8a78805469961815d4e3))
* **usenet:** prevent healthy providers being skipped while connections queue ([#1495](https://github.com/samtheruby/infinidysk/issues/1495)) ([ec275c1](https://github.com/samtheruby/infinidysk/commit/ec275c1e7c89966a53f79a88ef7c506612fdd884))
* **usenet:** prevent playback and queue stalls after missing articles ([#1514](https://github.com/samtheruby/infinidysk/issues/1514)) ([aeed8ab](https://github.com/samtheruby/infinidysk/commit/aeed8abf7b6a896337ea3b0a081c8f08241a5d3d))
* **usenet:** prevent playback stalls when a provider's transfer slots are stuck ([#1489](https://github.com/samtheruby/infinidysk/issues/1489)) ([7a81faa](https://github.com/samtheruby/infinidysk/commit/7a81faa9838f01b974c13bb3aa1658105eadfb5a))
* **usenet:** prevent queued connection waits from stalling provider failover ([#1506](https://github.com/samtheruby/infinidysk/issues/1506)) ([b8fe4c4](https://github.com/samtheruby/infinidysk/commit/b8fe4c4a43b2193260efb29abc2999971adff2fd))
* **usenet:** prevent stale provider misses from blocking imports ([#1403](https://github.com/samtheruby/infinidysk/issues/1403)) ([303b7a7](https://github.com/samtheruby/infinidysk/commit/303b7a781f60f13ad3e3af89aeb9741cffdbd39e))
* **usenet:** provider data caps count all BODY traffic and survive resets, restarts and metrics cleanup ([#1454](https://github.com/samtheruby/infinidysk/issues/1454)) ([0d68d67](https://github.com/samtheruby/infinidysk/commit/0d68d67325a561636d594e4cf817cf0f9109634b))
* **usenet:** providers that time out during background connection warming are paused until they recover ([#1555](https://github.com/samtheruby/infinidysk/issues/1555)) ([aca5770](https://github.com/samtheruby/infinidysk/commit/aca5770e69a40040e56e08652a0ffb2df64873ac))
* **usenet:** recover imports with conflicting yEnc metadata using PAR2-verified reads ([#1461](https://github.com/samtheruby/infinidysk/issues/1461)) ([ef5d503](https://github.com/samtheruby/infinidysk/commit/ef5d503c60c8996310bb28e17e2e91ebcf874910))
* **usenet:** release stalled transfers when playback is cancelled ([#1472](https://github.com/samtheruby/infinidysk/issues/1472)) ([9d0793e](https://github.com/samtheruby/infinidysk/commit/9d0793e149e136a051bb875cdf845db340a676db))
* **usenet:** share DATE liveness validation for probes and keepalives ([#1665](https://github.com/samtheruby/infinidysk/issues/1665)) ([1a5276a](https://github.com/samtheruby/infinidysk/commit/1a5276aa5752980f118181919f4032f24a4543a5))
* **usenet:** show accurate provider peak and active-average speeds ([#1540](https://github.com/samtheruby/infinidysk/issues/1540)) ([b5e7d26](https://github.com/samtheruby/infinidysk/commit/b5e7d26ac6f49c20857c3a48385c3d07807ac17d))
* **usenet:** slow background warm-up connections no longer trip a healthy provider's circuit breaker ([#1560](https://github.com/samtheruby/infinidysk/issues/1560)) ([cf39766](https://github.com/samtheruby/infinidysk/commit/cf3976678030e1ac214c1cb7b4d1d21f1dac8003))
* **usenet:** slower provider handshakes no longer trip the provider circuit under default settings ([#1578](https://github.com/samtheruby/infinidysk/issues/1578)) ([58eeecc](https://github.com/samtheruby/infinidysk/commit/58eeecc41958574057bee64ed9275a721179a558))
* **usenet:** speed tests use articles available from the selected provider ([#1361](https://github.com/samtheruby/infinidysk/issues/1361)) ([699e0ca](https://github.com/samtheruby/infinidysk/commit/699e0ca95ca9c196bd81314b3a8cf3cc2a0f159a))
* **usenet:** STAT of missing articles no longer logs unclassified cache-cleanup failures ([#1159](https://github.com/samtheruby/infinidysk/issues/1159)) ([5f568d8](https://github.com/samtheruby/infinidysk/commit/5f568d85450948adeb2a2ce050542f778c95f41d))
* **usenet:** stop skipping through incomplete files after every missing article ([#1158](https://github.com/samtheruby/infinidysk/issues/1158)) ([02df429](https://github.com/samtheruby/infinidysk/commit/02df429ac15b87c85a2b98a0b39ef66aa5e7bcde))
* **usenet:** unregister completed bandwidth waiters without blocking the limiter lock ([#1711](https://github.com/samtheruby/infinidysk/issues/1711)) ([18e902c](https://github.com/samtheruby/infinidysk/commit/18e902c344a13d8d4db70c63b01f3f6edc618e78))
* **usenet:** verify conflicting yEnc metadata against persisted PAR2 proofs ([692a67f](https://github.com/samtheruby/infinidysk/commit/692a67f0f7278a6b2d684e3b53ea0bdf73d0518d))
* **usenet:** verify retrievable articles before marking releases dead ([#1404](https://github.com/samtheruby/infinidysk/issues/1404)) ([4a4fe71](https://github.com/samtheruby/infinidysk/commit/4a4fe715bbfd84301df5c110df371a47cd6085e1))
* **usenet:** warm rereads no longer re-download cached pipelined segments ([#1289](https://github.com/samtheruby/infinidysk/issues/1289)) ([368a7da](https://github.com/samtheruby/infinidysk/commit/368a7da7eba93cdf0e41a206bdd3a51f3ec0c9ef))
* **usenet:** warn with the reason when a segment fetch is classified as protocol ([#1746](https://github.com/samtheruby/infinidysk/issues/1746)) ([9a14f4d](https://github.com/samtheruby/infinidysk/commit/9a14f4dae4589e15c60d50ebb57dc4c7d66be03c))
* **webdav:** bound view response copies and handle length overruns ([#1592](https://github.com/samtheruby/infinidysk/issues/1592)) ([d79c480](https://github.com/samtheruby/infinidysk/commit/d79c480e6f165df1a81b8ae77121c59464bc1ff4))
* **webdav:** completed downloads no longer reappear right after an Arr import deletes them ([#1821](https://github.com/samtheruby/infinidysk/issues/1821)) ([41fb2f0](https://github.com/samtheruby/infinidysk/commit/41fb2f0d1878b80a2197dafe332e0d7a11a4bdf4))
* **webdav:** directory listings no longer fail with HTTP 500 when a filename contains XML-invalid characters ([#1310](https://github.com/samtheruby/infinidysk/issues/1310)) ([1dfdcaa](https://github.com/samtheruby/infinidysk/commit/1dfdcaa79d9769607e1a31ee74d40309af50b70e))
* **webdav:** log why a stream was cut short ([#1892](https://github.com/samtheruby/infinidysk/issues/1892)) ([78ed0b7](https://github.com/samtheruby/infinidysk/commit/78ed0b7c81dcdb8f42d7ba2d87648f8fa8dc3314))
* **webdav:** make /view HEAD requests metadata-only ([#1405](https://github.com/samtheruby/infinidysk/issues/1405)) ([c2be9fb](https://github.com/samtheruby/infinidysk/commit/c2be9fb5ca696a740331b163bae4338d13b90dba))
* **webdav:** open full read-ahead window after the first segment is read ([#1653](https://github.com/samtheruby/infinidysk/issues/1653)) ([f830550](https://github.com/samtheruby/infinidysk/commit/f83055055b1504ecc68ade5be0f7af1ab0da969a))
* **webdav:** play multipart RARs with unrelated trailing volumes ([#1212](https://github.com/samtheruby/infinidysk/issues/1212)) ([65bc6d7](https://github.com/samtheruby/infinidysk/commit/65bc6d7c5943b0e2e63c7ae9b6171488a260c0ae))
* **webdav:** prevent PostgreSQL listing failures without buffering directories ([#1332](https://github.com/samtheruby/infinidysk/issues/1332)) ([dd7cc42](https://github.com/samtheruby/infinidysk/commit/dd7cc4283aab69f4ea2cb6b89ed538b7cd5faaac))
* **webdav:** range requests after a flaky header probe no longer return bytes from the wrong offset ([#1455](https://github.com/samtheruby/infinidysk/issues/1455)) ([0868917](https://github.com/samtheruby/infinidysk/commit/08689171eaa270ffb20b013a2e8ef76ae883e062))
* **webdav:** re-reading a range with filled holes no longer aborts or returns 404 ([#1698](https://github.com/samtheruby/infinidysk/issues/1698)) ([fa96956](https://github.com/samtheruby/infinidysk/commit/fa969560b350dd1599737e80521aab88aa462d64))
* **webdav:** recognize strm links under the configured base url path prefix ([#1692](https://github.com/samtheruby/infinidysk/issues/1692)) ([48715c5](https://github.com/samtheruby/infinidysk/commit/48715c5157b3902db9e00aa37a4ebb8a15cc7887))
* **webdav:** reduce unnecessary range read-ahead and improve seek diagnostics ([#1487](https://github.com/samtheruby/infinidysk/issues/1487)) ([1b11254](https://github.com/samtheruby/infinidysk/commit/1b11254d3ad03ffe123527df0b38689f6aa5ccaf))
* **webdav:** seeking near the end of some files no longer fails ([#1656](https://github.com/samtheruby/infinidysk/issues/1656)) ([4cdc4a0](https://github.com/samtheruby/infinidysk/commit/4cdc4a02553a97c3771b438a7c3c8ec08f7478c0))
* **webdav:** stop counting healthy streaming playback as slow WebDAV requests ([#1204](https://github.com/samtheruby/infinidysk/issues/1204)) ([150d185](https://github.com/samtheruby/infinidysk/commit/150d185931220f0330f0edf60eee784a28602f17))
* **webdav:** stop healthy playback triggering stalled-stream warnings ([#1334](https://github.com/samtheruby/infinidysk/issues/1334)) ([b01c0bd](https://github.com/samtheruby/infinidysk/commit/b01c0bd9d6ce97b08be6377558536372a3e5a222))


### Performance Improvements

* **api:** resolve filtered tree directories with one descendant scan ([#1671](https://github.com/samtheruby/infinidysk/issues/1671)) ([9838c46](https://github.com/samtheruby/infinidysk/commit/9838c462f0ce8e895757d2d7ab49728002029c99))
* **db:** index the health summary count ([#1851](https://github.com/samtheruby/infinidysk/issues/1851)) ([ca5c4d0](https://github.com/samtheruby/infinidysk/commit/ca5c4d03437eb343890301a542ec8d17d3932675))
* **health:** background health checks scan large libraries much faster ([#1303](https://github.com/samtheruby/infinidysk/issues/1303)) ([d8dce34](https://github.com/samtheruby/infinidysk/commit/d8dce34ae1c53e1b995279a549cd2e4174e092da))
* **health:** reduce redundant PAR2 repair work ([#1385](https://github.com/samtheruby/infinidysk/issues/1385)) ([9f72826](https://github.com/samtheruby/infinidysk/commit/9f72826d782e00332a0fed06b27b0a3259f7995c))
* **queue:** fail dead NZBs after one probe instead of scanning every article ([#1148](https://github.com/samtheruby/infinidysk/issues/1148)) ([23bcf61](https://github.com/samtheruby/infinidysk/commit/23bcf61b6e3b1ff52c1db8bd4529a845cb94c355))
* **queue:** faster seeking and smoother playback in multi-volume RAR releases ([#1636](https://github.com/samtheruby/infinidysk/issues/1636)) ([40595d9](https://github.com/samtheruby/infinidysk/commit/40595d9b28162922f4e49f7f42598b5453b3ac1b))
* **queue:** imports into large categories no longer read every existing folder ([#1856](https://github.com/samtheruby/infinidysk/issues/1856)) ([3402409](https://github.com/samtheruby/infinidysk/commit/340240947b71cd7f5c99e8fb5fd66dfa8c1b4e88))
* **queue:** imports with queue pipelining enabled no longer download archive headers twice ([#1622](https://github.com/samtheruby/infinidysk/issues/1622)) ([b0df768](https://github.com/samtheruby/infinidysk/commit/b0df768bc6e173d7d8e7cd953bde59dd093eb537))
* **queue:** RAR releases stream faster after the first volume ([#1634](https://github.com/samtheruby/infinidysk/issues/1634)) ([85de0cf](https://github.com/samtheruby/infinidysk/commit/85de0cfeef600669ee7920b4b453e5289ba8bbc0))
* **usenet:** default segment buffer retention to capacity ([#1299](https://github.com/samtheruby/infinidysk/issues/1299)) ([51c0ed8](https://github.com/samtheruby/infinidysk/commit/51c0ed8fa35a678a715aa1877d2bff792aa64dee))
* **usenet:** multi-volume imports no longer stall on throttled reconnects ([#1621](https://github.com/samtheruby/infinidysk/issues/1621)) ([b010c99](https://github.com/samtheruby/infinidysk/commit/b010c990cffb47689823f8ab4f17f4648e946f4e))
* **usenet:** report payload bytes per chunk instead of per line ([#1580](https://github.com/samtheruby/infinidysk/issues/1580)) ([e6761e5](https://github.com/samtheruby/infinidysk/commit/e6761e57cc452ebf73783bb908d9f76330acc539))
* **webdav:** disable thread-pool unfair semaphore spinning to cut streaming CPU ([#1614](https://github.com/samtheruby/infinidysk/issues/1614)) ([e406258](https://github.com/samtheruby/infinidysk/commit/e40625863ba81f6324f82bc36876d78e6187279d))
* **webdav:** faster streaming when segments do not line up with response chunks ([#1893](https://github.com/samtheruby/infinidysk/issues/1893)) ([c1f2b40](https://github.com/samtheruby/infinidysk/commit/c1f2b40d2ac4e2f7f3e1f1370221428c1573aacb))
* **webdav:** fetch the rest of a seek range while the first article downloads ([#1697](https://github.com/samtheruby/infinidysk/issues/1697)) ([2f9f45a](https://github.com/samtheruby/infinidysk/commit/2f9f45a04d231f1ef931a835d6a189c4cf2b65f1)), closes [#1677](https://github.com/samtheruby/infinidysk/issues/1677)
* **webdav:** memory returns to idle after playback stops ([#1617](https://github.com/samtheruby/infinidysk/issues/1617)) ([37fba57](https://github.com/samtheruby/infinidysk/commit/37fba5713a13d890b655d91006ad1c8f70dd31a9))
* **webdav:** new streams and seeks use less memory while ramping up ([#1618](https://github.com/samtheruby/infinidysk/issues/1618)) ([f399e97](https://github.com/samtheruby/infinidysk/commit/f399e9713ba9a661b15ccc09d741e83023872185))
* **webdav:** PAR2-verified files now stream at full speed ([#1664](https://github.com/samtheruby/infinidysk/issues/1664)) ([4d5fc59](https://github.com/samtheruby/infinidysk/commit/4d5fc595b6d62c114ee03eae3f8be6523272a085))
* **webdav:** pause prefetch when shared streams have no readers ([#1675](https://github.com/samtheruby/infinidysk/issues/1675)) ([b73f56a](https://github.com/samtheruby/infinidysk/commit/b73f56a7adc4228169b8d5a4443b7baa52f29c51))
* **webdav:** playback keeps moving when one article is slow to arrive ([#1660](https://github.com/samtheruby/infinidysk/issues/1660)) ([4bbffc2](https://github.com/samtheruby/infinidysk/commit/4bbffc23817e456de24e1b52c4585bc0a3e6e875))
* **webdav:** releases with very large articles start playing faster and use less memory ([#1635](https://github.com/samtheruby/infinidysk/issues/1635)) ([c7d0da7](https://github.com/samtheruby/infinidysk/commit/c7d0da7869ef846b18e93268848e70d3c6d11816))
* **webdav:** seeks and playback starts no longer wait on one slow first article ([#1670](https://github.com/samtheruby/infinidysk/issues/1670)) ([54934ff](https://github.com/samtheruby/infinidysk/commit/54934ffb7a73e9eef4fbb59877ce4aa963202218))
* **webdav:** smoother playback across multi-volume archive boundaries ([#1659](https://github.com/samtheruby/infinidysk/issues/1659)) ([f9db281](https://github.com/samtheruby/infinidysk/commit/f9db281a4bc57f53baf1578bb0df2e12bdb0754a))
* **webdav:** smoother playback across RAR volume boundaries ([#1630](https://github.com/samtheruby/infinidysk/issues/1630)) ([13b1bee](https://github.com/samtheruby/infinidysk/commit/13b1bee823d8fd5e745dcf09903edf769cbb315e))
* **webdav:** smoother playback with far shorter stalls between Usenet articles ([#1638](https://github.com/samtheruby/infinidysk/issues/1638)) ([6260e1d](https://github.com/samtheruby/infinidysk/commit/6260e1dda5b7418fa47a5517c9824c7728cf615b))
* **webdav:** smoother playback with fewer stalls while streaming ([#1606](https://github.com/samtheruby/infinidysk/issues/1606)) ([31c837f](https://github.com/samtheruby/infinidysk/commit/31c837fa08c04495de2a2201813199b5dce0326e))
* **webdav:** start ranged playback without waiting for the full first article ([#1290](https://github.com/samtheruby/infinidysk/issues/1290)) ([d3e5815](https://github.com/samtheruby/infinidysk/commit/d3e58153f93cae9840861b04e6d3e1c55abda667))


### Reverts

* **webdav:** stream response bytes through the 256 KiB buffer again ([#1895](https://github.com/samtheruby/infinidysk/issues/1895)) ([2aef6a6](https://github.com/samtheruby/infinidysk/commit/2aef6a6bbc590963dc4ece3b45b9c5acc1fb328f))


### Build System

* publish 2.x images from infinidysk/infinidysk ([c773c9f](https://github.com/samtheruby/infinidysk/commit/c773c9fbfe3f30bc25882a093a30e0149aa6b736))
* publish Linux binary archives with each release ([#1859](https://github.com/samtheruby/infinidysk/issues/1859)) ([cdedc4b](https://github.com/samtheruby/infinidysk/commit/cdedc4b4deb7fef5abed4b15c907cddda8870759))

## [2.0.0-beta.7](https://github.com/infinidysk/infinidysk/compare/v2.0.0-beta.6...v2.0.0-beta.7) (2026-11-10)


### Features

* **queue:** import NZBs that contain another NZB ([#1875](https://github.com/infinidysk/infinidysk/issues/1875)) ([db91586](https://github.com/infinidysk/infinidysk/commit/db915861fa075483721e9cf1fd7ef6983e7016c2))
* **ui:** remind you to remove 1.x data after the upgrade, with its estimated disk usage ([#1876](https://github.com/infinidysk/infinidysk/issues/1876)) ([eebad20](https://github.com/infinidysk/infinidysk/commit/eebad20e14e0e7739a50757a22e68000db5b99da))
* **ui:** the queue no longer shows failed imports older than a day unless you filter for them ([#1865](https://github.com/infinidysk/infinidysk/issues/1865)) ([2db9609](https://github.com/infinidysk/infinidysk/commit/2db96096a071f31edf0ce38ee0be21bd3175b30c))


### Bug Fixes

* **arr:** Radarr and other Arrs save the infinidysk webhook even when they cannot reach it yet ([#1861](https://github.com/infinidysk/infinidysk/issues/1861)) ([e3e0507](https://github.com/infinidysk/infinidysk/commit/e3e0507366d9e17abda275018644d3aa92f069f2))
* **deps:** Bump fuse3 from 0.9.0 to 0.10.0 ([#1873](https://github.com/infinidysk/infinidysk/issues/1873)) ([6ef351a](https://github.com/infinidysk/infinidysk/commit/6ef351a177ab9e950ddaf4e6e8229990c56cdcf5))
* **deps:** Bump the cargo-minor-patch group with 4 updates ([#1872](https://github.com/infinidysk/infinidysk/issues/1872)) ([fc62ad5](https://github.com/infinidysk/infinidysk/commit/fc62ad52f375ac8dd5773a977a171986c66d1cf3))
* **deps:** Bump the npm-minor-patch group in /ui with 4 updates ([#1869](https://github.com/infinidysk/infinidysk/issues/1869)) ([6bb8e3a](https://github.com/infinidysk/infinidysk/commit/6bb8e3a56d213f1a6e0364241e6a7b72b45e1136))
* **health:** hold the write permit only while health work writes ([#1868](https://github.com/infinidysk/infinidysk/issues/1868)) ([07a61e5](https://github.com/infinidysk/infinidysk/commit/07a61e5c2edf9b2009357f587b46fc7c841b1ee5))
* **health:** repairs follow the Arr's own search instead of always waiting two minutes ([#1867](https://github.com/infinidysk/infinidysk/issues/1867)) ([9b6ae7a](https://github.com/infinidysk/infinidysk/commit/9b6ae7a7758499d692d1181573784a83a5c40dec))
* **import:** measure a pending volume when a known size cannot fit its articles ([#1878](https://github.com/infinidysk/infinidysk/issues/1878)) ([180f9ab](https://github.com/infinidysk/infinidysk/commit/180f9abf1eddd581a6257da7a5e8ca021a19ea92))
* **import:** the import report shows progress instead of a silent console ([#1877](https://github.com/infinidysk/infinidysk/issues/1877)) ([b29bc25](https://github.com/infinidysk/infinidysk/commit/b29bc257bd0ecf55b025fc8027f74a4e41e963ea))
* **mount:** distinguish failed tuning writes from external tuning ([#1866](https://github.com/infinidysk/infinidysk/issues/1866)) ([3bee375](https://github.com/infinidysk/infinidysk/commit/3bee3758d2602bc8a003b93298c453550c114883))
* **ui:** clearer status and failure reasons on phones, and a missing-articles rate that reflects playback ([#1874](https://github.com/infinidysk/infinidysk/issues/1874)) ([6b6dcad](https://github.com/infinidysk/infinidysk/commit/6b6dcad9092a08f0a3792e879fd27e6737fd9b7d))

## [2.0.0-beta.6](https://github.com/infinidysk/infinidysk/compare/v2.0.0-beta.5...v2.0.0-beta.6) (2026-11-06)


### Features

* **db:** choose where infinidysk keeps its database and files ([#1858](https://github.com/infinidysk/infinidysk/issues/1858)) ([c1f6f93](https://github.com/infinidysk/infinidysk/commit/c1f6f936462bd2e2a003971ff67c88dd28e331fe))
* **ui:** the Queue link shows when a download needs you in the Arr ([#1849](https://github.com/infinidysk/infinidysk/issues/1849)) ([2c1a095](https://github.com/infinidysk/infinidysk/commit/2c1a0953d2aa2a3c06f1044a8255c07dad959b22))


### Bug Fixes

* **api:** link the update notice to the release notes of the newer tag ([#1860](https://github.com/infinidysk/infinidysk/issues/1860)) ([005812a](https://github.com/infinidysk/infinidysk/commit/005812a4248f4d5685257dd76dbb429181e4aff2))
* **ui:** open tabs no longer flood the server with refreshes during large cleanups ([#1850](https://github.com/infinidysk/infinidysk/issues/1850)) ([ae1b19c](https://github.com/infinidysk/infinidysk/commit/ae1b19ca39a4d3abddc81484a7fadd74177393c5))


### Performance Improvements

* **db:** index the health summary count ([#1851](https://github.com/infinidysk/infinidysk/issues/1851)) ([ca5c4d0](https://github.com/infinidysk/infinidysk/commit/ca5c4d03437eb343890301a542ec8d17d3932675))
* **queue:** imports into large categories no longer read every existing folder ([#1856](https://github.com/infinidysk/infinidysk/issues/1856)) ([3402409](https://github.com/infinidysk/infinidysk/commit/340240947b71cd7f5c99e8fb5fd66dfa8c1b4e88))


### Build System

* publish Linux binary archives with each release ([#1859](https://github.com/infinidysk/infinidysk/issues/1859)) ([cdedc4b](https://github.com/infinidysk/infinidysk/commit/cdedc4b4deb7fef5abed4b15c907cddda8870759))

## [2.0.0-beta.5](https://github.com/infinidysk/infinidysk/compare/v2.0.0-beta.4...v2.0.0-beta.5) (2026-11-06)


### Features

* **api:** better Lidarr support: more audio formats, faster cleanup after album deletes, and a tagging warning ([#1838](https://github.com/infinidysk/infinidysk/issues/1838)) ([e138a06](https://github.com/infinidysk/infinidysk/commit/e138a062aa1df9f9a85a0aaecf532a2e060fbc98))
* **arr:** support Sonarr v5 ([#1833](https://github.com/infinidysk/infinidysk/issues/1833)) ([b743f54](https://github.com/infinidysk/infinidysk/commit/b743f544313a0ad447687c8bcd7a678abab56a63))
* **auth:** show your identity provider's name on the SSO sign-in button ([#1835](https://github.com/infinidysk/infinidysk/issues/1835)) ([1845fe8](https://github.com/infinidysk/infinidysk/commit/1845fe8182b8f084da671ca399a12bff028500d0))
* **mount:** turn off the built-in FUSE mount when you do not need it, without warnings ([#1841](https://github.com/infinidysk/infinidysk/issues/1841)) ([d721677](https://github.com/infinidysk/infinidysk/commit/d721677513bc8f0e23005450114a2a6f93ea7379))


### Bug Fixes

* **db:** cleanup runs on SQLite no longer stop when other work writes to the database ([#1840](https://github.com/infinidysk/infinidysk/issues/1840)) ([6d676ab](https://github.com/infinidysk/infinidysk/commit/6d676ab28a308139bcf8c3d12e3446c91fd11837))
* **db:** failed maintenance runs and API errors now say what the database reported ([#1839](https://github.com/infinidysk/infinidysk/issues/1839)) ([43ac7fd](https://github.com/infinidysk/infinidysk/commit/43ac7fd1f399ef79ae9032c01e4276ef487a3924))
* **deps:** Bump the npm-minor-patch group in /ui with 3 updates ([#1844](https://github.com/infinidysk/infinidysk/issues/1844)) ([ba17029](https://github.com/infinidysk/infinidysk/commit/ba17029c9e28fd63a39ec257dbbed551f71c31cb))
* **health:** broken files from an Arr that cannot repair them are kept for you instead of deleted ([#1837](https://github.com/infinidysk/infinidysk/issues/1837)) ([c3bd0ba](https://github.com/infinidysk/infinidysk/commit/c3bd0baf90b13846da6aca35e26f945b106385e4))

## [2.0.0-beta.4](https://github.com/infinidysk/infinidysk/compare/v2.0.0-beta.3...v2.0.0-beta.4) (2026-11-05)


### ⚠ BREAKING CHANGES

* **api:** infinidysk no longer starts while a Readarr Arr instance is configured. Before upgrading, remove Readarr instances or change them to Chaptarr in Settings > Arr instances. If already upgraded, start the previous version to do so, or override the list with INFINIDYSK__ARR_INSTANCES.

### Features

* **api:** support Chaptarr instead of the abandoned Readarr ([#1827](https://github.com/infinidysk/infinidysk/issues/1827)) ([24e55b5](https://github.com/infinidysk/infinidysk/commit/24e55b51b6843a7df13364c2a310d77cf36a999c))
* **nntp:** add the news-central.giganews.com server to the Giganews profile ([#1824](https://github.com/infinidysk/infinidysk/issues/1824)) ([028d6fb](https://github.com/infinidysk/infinidysk/commit/028d6fb3663d9a266396ecd39cf7cc17e94bb98d))
* **ui:** backups get their own settings page ([#1826](https://github.com/infinidysk/infinidysk/issues/1826)) ([343cd7f](https://github.com/infinidysk/infinidysk/commit/343cd7f3340c5a0b3320cdec91f65c8e6a54d058))


### Bug Fixes

* **health:** a provider outage no longer marks good files as damaged ([#1829](https://github.com/infinidysk/infinidysk/issues/1829)) ([e8963ed](https://github.com/infinidysk/infinidysk/commit/e8963edac9355be750a6073988403993cd3986a9))
* **health:** repairs no longer replace a newer file the Arr imported from another download ([#1832](https://github.com/infinidysk/infinidysk/issues/1832)) ([107cabe](https://github.com/infinidysk/infinidysk/commit/107cabe2704dcb0ad23e703c4a36fc816ed64b57))
* **mount:** keep files referenced by legacy library links ([#1828](https://github.com/infinidysk/infinidysk/issues/1828)) ([4e1c914](https://github.com/infinidysk/infinidysk/commit/4e1c914b7ad927bbf205126199ff9955981ef2bc))
* **ui:** stalls on the overview count only pauses a viewer would notice ([#1830](https://github.com/infinidysk/infinidysk/issues/1830)) ([317497d](https://github.com/infinidysk/infinidysk/commit/317497d5cc93c013315f95b24172db5f271533e5))
* **webdav:** completed downloads no longer reappear right after an Arr import deletes them ([#1821](https://github.com/infinidysk/infinidysk/issues/1821)) ([41fb2f0](https://github.com/infinidysk/infinidysk/commit/41fb2f0d1878b80a2197dafe332e0d7a11a4bdf4))

## [2.0.0-beta.3](https://github.com/infinidysk/infinidysk/compare/v2.0.0-beta.2...v2.0.0-beta.3) (2026-11-05)


### Features

* **auth:** sign in with single sign-on (OIDC), carried over from 1.x ([#1812](https://github.com/infinidysk/infinidysk/issues/1812)) ([4fc3b6a](https://github.com/infinidysk/infinidysk/commit/4fc3b6a4e834c478313466e1af95aa9bbf0b7350))
* **import:** upgrade 1.x installs that keep their data in PostgreSQL ([#1815](https://github.com/infinidysk/infinidysk/issues/1815)) ([6ee6cbf](https://github.com/infinidysk/infinidysk/commit/6ee6cbfc686a4be55d4f04afcc4ce74af634d35a))


### Bug Fixes

* **arr:** skip the automatic-search wait when no release was blocklisted ([#1817](https://github.com/infinidysk/infinidysk/issues/1817)) ([23be919](https://github.com/infinidysk/infinidysk/commit/23be9194448dbb028bee7cb4c21378f2357610c2))
* **ui:** memory overview no longer counts reclaimable kernel cache as app memory ([#1813](https://github.com/infinidysk/infinidysk/issues/1813)) ([d4f5daf](https://github.com/infinidysk/infinidysk/commit/d4f5daf5991447d2726a5b22d9232c5d9c265c94))
* **ui:** season packs no longer repeat the same Arr import message per episode ([#1811](https://github.com/infinidysk/infinidysk/issues/1811)) ([c141857](https://github.com/infinidysk/infinidysk/commit/c1418571699a19c0ac9c60c2b60ba3353aa24c25))

## [2.0.0-beta.2](https://github.com/infinidysk/infinidysk/compare/v2.0.0-beta.1...v2.0.0-beta.2) (2026-11-04)


### Features

* **db:** back up your database nightly and restore it from the Maintenance page ([#1809](https://github.com/infinidysk/infinidysk/issues/1809)) ([0c40be7](https://github.com/infinidysk/infinidysk/commit/0c40be7d06360f75e2bca544b940744212ea6357))
* **db:** move from SQLite to PostgreSQL from the settings page ([#1807](https://github.com/infinidysk/infinidysk/issues/1807)) ([20a87fb](https://github.com/infinidysk/infinidysk/commit/20a87fbbb770026a549acd335c350ce01cb353c6))
* **mount:** read history shows which app started ffmpeg or ffprobe ([#1791](https://github.com/infinidysk/infinidysk/issues/1791)) ([25e114a](https://github.com/infinidysk/infinidysk/commit/25e114ac59e4738f9594a30c4ccb30d98d945817))
* **ui:** overview activity shows download speed by workload as bars ([#1810](https://github.com/infinidysk/infinidysk/issues/1810)) ([dfa8146](https://github.com/infinidysk/infinidysk/commit/dfa81468bc7504bea4c00f7c3f4c3d83849ff93b))


### Bug Fixes

* **api:** an unresponsive STRM folder no longer freezes settings and the SAB API ([#1795](https://github.com/infinidysk/infinidysk/issues/1795)) ([a7eb784](https://github.com/infinidysk/infinidysk/commit/a7eb784e4e39b7db6850817a00bac2ef3b2b1332))
* **api:** Arrs that start after InfiniDysk now connect without a restart ([#1806](https://github.com/infinidysk/infinidysk/issues/1806)) ([ba4972f](https://github.com/infinidysk/infinidysk/commit/ba4972f6a813f765cb49847098e489644735b9d9))
* **archive:** malformed 7z headers can no longer hang or exhaust memory during import ([#1794](https://github.com/infinidysk/infinidysk/issues/1794)) ([7091745](https://github.com/infinidysk/infinidysk/commit/7091745063ffba6feb7826191f9fea16a219be54))
* **arr:** files imported by a second Arr are no longer deleted by cleanup of the first ([#1802](https://github.com/infinidysk/infinidysk/issues/1802)) ([3464a0c](https://github.com/infinidysk/infinidysk/commit/3464a0c14d3f0187e113c962b132e267c42ec5de))
* **import:** migrate large legacy metadata without size-based skips ([#1797](https://github.com/infinidysk/infinidysk/issues/1797)) ([29f8e2f](https://github.com/infinidysk/infinidysk/commit/29f8e2f4b9eb83f4cfc41fc739b1e853321a9534))
* **import:** migration no longer follows symlinks out of the old config folder ([#1796](https://github.com/infinidysk/infinidysk/issues/1796)) ([a877923](https://github.com/infinidysk/infinidysk/commit/a877923a8bb0cbaacf7f71662bd1f8bd4747c6bf))
* **import:** reject Arr paths that climb out of a library folder ([#1800](https://github.com/infinidysk/infinidysk/issues/1800)) ([fe058ed](https://github.com/infinidysk/infinidysk/commit/fe058edfa5dcd20dc2b98ce2bce766d2ba54d053))
* **import:** upgrading from 1.x shows progress while it checks your library instead of looking stuck ([#1799](https://github.com/infinidysk/infinidysk/issues/1799)) ([53bd352](https://github.com/infinidysk/infinidysk/commit/53bd3524485eed2339fe61669eb0985066f356d0))
* **nntp:** fail over on articles that end before their announced size ([#1805](https://github.com/infinidysk/infinidysk/issues/1805)) ([27ce044](https://github.com/infinidysk/infinidysk/commit/27ce0448d4b6a27f4ffe990dadf2b195c29d72e5))
* **par2:** index large PAR2 sets without quadratic lookups ([#1801](https://github.com/infinidysk/infinidysk/issues/1801)) ([8c1fdff](https://github.com/infinidysk/infinidysk/commit/8c1fdff880d8693bb1b4081580587aa209794f67))
* **queue:** bound outstanding import tasks ([#1803](https://github.com/infinidysk/infinidysk/issues/1803)) ([1155315](https://github.com/infinidysk/infinidysk/commit/11553154af8a75c533527c85a6679078115a780c))
* **queue:** limit concurrent archive key derivations ([#1804](https://github.com/infinidysk/infinidysk/issues/1804)) ([6073369](https://github.com/infinidysk/infinidysk/commit/607336974219104987752825e99fd17ba9c6ae4a))
* **queue:** STRM and library files are no longer written through symlinked subfolders ([#1798](https://github.com/infinidysk/infinidysk/issues/1798)) ([b030f90](https://github.com/infinidysk/infinidysk/commit/b030f9001a1bccd85ad223533ee7c6cd10753117))
* **queue:** STRM cleanup and writes no longer follow planted paths out of the STRM folder ([#1793](https://github.com/infinidysk/infinidysk/issues/1793)) ([ce0868e](https://github.com/infinidysk/infinidysk/commit/ce0868e4175c58dba3a9611d462847938482324d))

## [2.0.0-beta.1](https://github.com/infinidysk/infinidysk/compare/v2.0.0-alpha.17...v2.0.0-beta.1) (2026-11-03)

### Beta

* InfiniDysk 2.0 is now in beta. It is a rewrite in Rust: one native binary with the server, the web UI and a built-in FUSE mount. It speaks the same SABnzbd API and serves the same WebDAV paths as 1.x, so Arr apps and media servers see no difference ([What's new in 2.x](https://www.infinidysk.com/v2/whats-new/))
* The image is ghcr.io/infinidysk/infinidysk-next:v2.0.0-beta.1 for Linux x64 and arm64. The edge tag is always the newest 2.x release; there is no latest tag until 2.0.0 ([Run with Docker](https://www.infinidysk.com/v2/install/docker/))

### Upgrading from 1.x

* Moving from 1.x to 2.x is a breaking change with manual steps: copy your config, run the import, and replace the rclone sidecar with the built-in mount. Changing the image name alone is not an upgrade ([Before you upgrade](https://www.infinidysk.com/v2/upgrade/))
* Some 1.x features are not in 2.x yet ([Feature comparison](https://www.infinidysk.com/v2/whats-new/#feature-comparison))
* 1.x continues on the v1 branch with bug fixes only and keeps the ghcr.io/infinidysk/infinidysk image and all its tags ([Looking for 1.x?](https://github.com/infinidysk/infinidysk#looking-for-1x))

### Other changes

* **ui:** update @tanstack/react-query, fast-uri, qs and systeminformation

### Reporting problems

* Open a GitHub issue (the bug form asks which version you run) or ask on Discord ([Reporting a bug](https://www.infinidysk.com/v2/help/reporting/))

## 2.0.0-alpha.17 (2026-11-02)


### Bug Fixes

* **stream:** keep disk cache writes the startup scan used to delete
* **stream:** keep reading the disk cache after its directory link changes
* **stream:** stop a reopened disk cache deleting writes still in progress

## 2.0.0-alpha.16 (2026-11-02)


### Features

* **docker:** containers report healthy only once the mount and database are ready


### Bug Fixes

* **ui:** ignore extension scripts when checking for updates
* **ui:** keep activity visible beside large spikes
* **ui:** keep the read position bar at a fixed width
* **ui:** show playback in green and health checks in blue on the activity graph

## 2.0.0-alpha.15 (2026-11-01)


### Features

* **api:** check provider logins and report each provider's connection state
* **api:** search and filter health and import history
* **health:** repair through Lidarr and Whisparr
* **ui:** explain each health state on the Health page
* **ui:** search and filter import and health history
* **ui:** show which providers serve each read in progress
* **ui:** test provider connections and show their state


### Bug Fixes

* **deps:** bump the cargo-minor-patch group with 3 updates
* **health:** check ebooks instead of ignoring them
* **import:** check imported files with recorded misses right away
* **ui:** align overview read rows and drop the activity chart's y-axis
* **ui:** bigger tap targets for slider thumbs, Advanced settings and inline links
* **ui:** call the stats library card Library and make provider settings a button
* **ui:** clearer provider name and Arr download-client hints
* **ui:** fill the system card grid and give the mount path room on phones
* **ui:** full-width editor sheets on phones and an explicit provider pick
* **ui:** name 1.x STRM links plainly and hide the notice when unused
* **ui:** one split button to start read traces
* **ui:** readable maintenance errors, relative run times and why Run now is off
* **ui:** show a dash for empty explorer cells and explain a missing import time
* **ui:** show provider misses as warnings on stats
* **ui:** show which performance settings the environment sets
* **ui:** stop the update banner from reloading every page
* **ui:** tidy phone layouts on overview, providers and explorer
* **ui:** type delete to run unlinked-file removal by hand

## 2.0.0-alpha.14 (2026-11-01)


### Features

* **ui:** show disk cache use and health on the System page
* **ui:** show release notes from the System page


### Bug Fixes

* **api:** let empty folders of categories no longer offered be removed
* **ui:** color the wordmark on the sign-in and setup screens
* **ui:** keep unsaved settings when saved settings change underneath
* **ui:** reload open tabs onto a new version after an upgrade
* **ui:** show the release folder for obfuscated file names
* **ui:** tuck reader process ids behind an info tip

## 2.0.0-alpha.13 (2026-11-01)


### Features

* **import:** serve upgrade progress while importing C# data


### Bug Fixes

* **api:** check the public image registry for newer releases
* **import:** upgraded installs bring back files with an extra listed article
* **ui:** preserve the app when upgrade status refresh fails


### Performance Improvements

* **import:** reuse matching measured volume geometry

## 2.0.0-alpha.12 (2026-11-01)


### Bug Fixes

* **import:** upgrades carry over archive files with wrong sizes in their posts again
* **import:** upgrades no longer hide a missing article in archive volumes that match an earlier volume's size
* **stream:** hedge pending responses when the preferred provider has spare capacity

## 2.0.0-alpha.11 (2026-10-31)


### Bug Fixes

* **import:** restore more skipped upgrade files and correct log ownership

## 2.0.0-alpha.10 (2026-10-31)


### Features

* **health:** count a 100% import as the first health check
* **import:** note that WebDAV deletes stop working after upgrading from a writable C# setup
* **ui:** explain what the health sample size covers


### Bug Fixes

* **auth:** accept the admin username in any case, as 1.x did
* **queue:** posts with wrong yEnc file sizes now import, and upgrades bring back files they skipped

## 2.0.0-alpha.9 (2026-10-30)


### Features

* **api:** say which setting a validation error is about
* **ui:** add a Stats page and show what needs attention on Overview
* **ui:** color dysk in the sidebar wordmark
* **ui:** edit providers in a side sheet
* **ui:** lay settings out as grouped panels
* **ui:** manage Arr instances in a list and side sheet
* **ui:** merge Admin API and Authentication into Access
* **ui:** move Support to the System page
* **ui:** move the download speed limit to Performance
* **ui:** show connection details on WebDAV, Download client and Mount
* **ui:** split Library settings from Imports
* **ui:** switch experiments on and off in Settings
* **ui:** tidy provider row and header actions


### Bug Fixes

* **archive:** key RAR archives with the first 127 password characters
* **deps:** bump crc32fast
* **stream:** keep win-floor out of analysis reads
* **stream:** stop speculative fetches past bounded read ranges
* **ui:** fit explorer, queue and logs on phones; tidy stats and health empty states
* **ui:** fit tables on phones and follow the design system on queue, explorer, health, system and stats
* **ui:** fix settings copy and placeholders
* **ui:** format sizes the same way on Performance
* **ui:** give icon-only buttons tooltips and specific names
* **ui:** harden settings forms
* **ui:** keep text on the type scale
* **ui:** keep the live status in the sidebar footer
* **ui:** link the health-checks-off notice to health settings
* **ui:** make preset cards one radio group
* **ui:** make sign-in errors, focus and button contrast accessible
* **ui:** mobile menu scrolls and closes on every navigation
* **ui:** page titles, skip link and screen-reader labels in the shell
* **ui:** put the WebDAV password beside its label
* **ui:** readable warning and success text in light theme
* **ui:** rename Report 1970 file dates to Disable file timestamps
* **ui:** shorten settings hints
* **ui:** show maintenance run reasons
* **ui:** show recent reads ten at a time
* **ui:** show server validation errors on their field
* **ui:** show the provider speed test as a row button
* **ui:** use the Advanced settings toggle in Performance


### Performance Improvements

* **nntp:** add pipe-weight experiment that charges large articles more download slots
* **nntp:** charge large playback articles one download slot per MB
* **ui:** load app pages on demand so sign-in renders first

## 2.0.0-alpha.8 (2026-10-27)


### Features

* **mount:** optional 1970 file dates to match rclone --no-modtime mounts


### Bug Fixes

* **api:** show why an Arr rejected a request
* **mount:** answer GETATTR on an open file from its handle
* **mount:** keep the FUSE session at error when RUST_LOG is set
* **stream:** stream progress only for the two segments read next


### Performance Improvements

* **db:** skip the idle-connection ping before SQLite queries
* **mount:** read kernel requests without a blocking-pool hop when running as root
* **mount:** stop revalidating fixed directories every second
* **nntp:** share decoded bodies with the memory cache instead of copying them
* **queue:** parse PAR2 index articles once as they arrive
* reopen files without re-reading their metadata
* **stream:** skip a body copy on each disk cache write and hit

## 2.0.0-alpha.7 (2026-10-26)


### Features

* **ui:** show warm provider connections in the sidebar


### Bug Fixes

* **mount:** allow group members to unlink completed symlinks
* **mount:** stop FUSE reads stalling forever behind a busy-reader probe
* **nntp:** log what a provider replied when it sends an unexpected response
* **nntp:** retain connection headroom during background requests
* **queue:** group old-style RAR volumes past .r99 with their set
* **queue:** import files whose NZB lists a part twice
* **queue:** stop the article check at the first missing segment of a media file
* **queue:** time out STRM directory checks and writes during handoff
* **ui:** copy keys and stream links on plain-HTTP LAN addresses

## 2.0.0-alpha.6 (2026-10-25)


### Features

* **api:** warn when a read stalls and add stall details to live status
* **mount:** report the effective kernel FUSE limits and queue
* **nntp:** show what each busy provider connection is waiting for
* **stream:** show which stage each waiting read is stuck in
* **ui:** restart from settings to apply startup-only changes


### Bug Fixes

* **deps:** bump the cargo-minor-patch group with 2 updates
* **deps:** bump the npm-minor-patch group in /ui with 6 updates
* **deps:** update ctutils to 0.4.4 for RUSTSEC-2026-0385
* **import:** refuse C# installs older than v1.3.0 before reading their schema
* **stream:** never let a blocked read wait on the read-ahead budget
* **stream:** warn about misaligned segments once a minute per file
* **ui:** make settings usable on touch and guard unsaved changes


### Build System

* **deps:** bump rust-toolchain from 1.99.0 to 1.99.1

## 2.0.0-alpha.5 (2026-10-23)


### Features

* **health:** remove dead library links and have the Arr search again
* **health:** repair migrated files that have no download through the Arr that links them
* **ui:** mark service restarts in the logs
* **ui:** show queue and action-needed counts in the sidebar nav


### Bug Fixes

* **api:** record owners of earlier imports as soon as the Arr is reachable
* **health:** a renamed file no longer counts as replaced
* **health:** never delete a migrated file before its Arrs were asked
* **import:** bring back skipped migrated files the library still links to
* **import:** carry over migrated files whose C# segment list lacks an article
* **import:** find the Arr download of migrated files so broken ones get replaced
* **import:** keep broken migrated files for review instead of deleting them
* **import:** keep broken unowned files for review on installs already migrated from C#
* **import:** list every file the C# import left out
* **import:** recognise library links into the C# mount folder when the mount moved
* **mount:** keep out-of-order kernel reads from resetting the read-ahead
* **nntp:** an article the NZB never listed counts as missing
* **ui:** reword the setting for broken files not imported by an Arr
* **ui:** say nothing to reclaim when compacting a database is skipped
* **ui:** show the maintenance window in the server's time zone

## 2.0.0-alpha.4 (2026-10-23)


### Features

* **api:** remove unlinked files as a scheduled maintenance job
* **db:** compact the databases in the maintenance window
* **import:** carry over the C# unlinked-file cleanup schedule
* **import:** carry the C# download limit over
* **nntp:** cap total download speed from providers
* **ui:** download limit under Settings &gt; Network
* **ui:** explain stalls in the recent reads table
* **ui:** list Maintenance under System in settings
* **ui:** maintenance page with remove unlinked files
* **ui:** move live activity to the middle of the sidebar and shorten the version label


### Bug Fixes

* **api:** give maintenance schemas unique names and query paging params
* **db:** pause background writes while compacting the database
* **health:** catch articles that decode but belong to another part of the file
* **ui:** clearer maintenance job description and schedule toggle
* **ui:** connections in use never exceeds the connection limit


### Performance Improvements

* **db:** keep query planner statistics fresh
* **mount:** cap max playback read-ahead memory at 2000 MB
* **mount:** size preset read-ahead memory for 5, 10 and 20 streams


### Refactors

* **health:** call broken files no Arr imported "unowned"

## 2.0.0-alpha.3 (2026-10-22)


### Features

* **queue:** show import progress and time left


### Bug Fixes

* **health:** judge a segment by the message-id playback reads
* **mount:** serve modified times in whole seconds
* **queue:** blame the NZB, not the providers, when it lacks a file's first segment
* **queue:** fail NZBs that lack segments without downloading the whole file
* **queue:** import obfuscated RAR sets listed out of order
* **queue:** leave out an incomplete non-media RAR member instead of failing the job
* **queue:** wait out the retry backoff when a job's result cannot be written
* **sab:** accept the speedlimit command and ignore it
* **stream:** report a corrupt segment even after the reader streamed past it
* **ui:** keep the explorer video player inside its window


### Performance Improvements

* **queue:** parse, hash and compress NZBs off the async runtime

## 2.0.0-alpha.2 (2026-10-22)


### Bug Fixes

* **import:** read C# times in the container's time zone
* **stream:** hedge a slow last segment


### Performance Improvements

* **nntp:** send hedges only to idle connections
* **stream:** read 60 MB ahead by default

## 2.0.0-alpha.1 (2026-10-21)


### ⚠ BREAKING CHANGES

* **db:** databases created by earlier pre-releases no longer open. Back up the config directory (database, -wal and metrics files), then start with a new database.

### Features

* **api:** add DB-backed settings with an authoritative env overlay, catalog providers and arr instances
* **api:** add per-file read history, most-read files and workload split
* **api:** add provider speed test and pipeline auto-tune
* **api:** add public URL setting under network
* **api:** add read, import, health and cache trends and usage by app to the overview
* **api:** admin API with OpenAPI document and live settings
* **api:** discover which Arr download clients point at this installation
* **api:** download queued and finished NZBs and retry failed jobs from the queue page
* **api:** explorer API with signed player links
* **api:** export redacted traces for bug reports
* **api:** keep logs across restarts
* **api:** list rejected releases and report stuck counts on queued jobs
* **api:** live updates over server-sent events
* **api:** provider download quotas with monthly or block resets, and a timed speed test
* **api:** record usage metrics with live samples, overview history and Prometheus export
* **api:** report container CPU and memory in live metrics
* **api:** reveal stored API and download keys in settings
* **api:** richer overview metrics with per-provider series, records, catalogue and live minute totals
* **api:** run the server with the SAB API and WebDAV on one port, the queue worker and the FUSE mount
* **api:** toggle read tracing and download traces
* **api:** trust local network ranges as reverse proxies by default
* **api:** upload NZBs into a category through the admin API
* **archive:** add a sans-I/O RAR4/RAR5 header scanner that maps members to byte ranges
* **archive:** read 7z headers, including LZMA-encoded ones, and map stored members to byte ranges
* **arr:** clear stuck imports from Arr queues
* **arr:** reconcile owned files against each Arr's library daily
* **arr:** record owners of earlier imports from each Arr's history
* **arr:** register webhooks and delete items their Arr deleted
* **auth:** admin account with argon2id, signed session cookies and an admin API key
* **auth:** let sign-in be required always, off for local addresses, or off
* **core:** add item ids, file metadata and the versioned zstd blob format
* **db:** add SQLite and PostgreSQL storage for items, blobs and config
* **db:** add the metrics store with minute, hour and lifetime rollups
* **db:** broadcast queue, history and health changes
* **db:** health check schedule and results
* **db:** keep unreferenced NZBs for a retention window and prune old history
* **db:** list recent health check results
* **db:** paged, filtered file queries for the explorer
* **db:** query id shards, completed download dirs and remove queued jobs
* **db:** record which item each finished read was of
* **db:** squash migrations into one initial schema
* **db:** store queue and history
* **db:** store the single admin login in accounts
* **health:** analyze media with ffprobe and repair broken MP4 containers
* **health:** choose the check sample size with a slider
* **health:** find the Arr that imported a STRM handoff
* **health:** report playback damage, hide replaced files and retry with 503
* **health:** share a durable per-media search limit
* **health:** show the check schedule and link checked files to the explorer
* **health:** STAT health checks with Sonarr/Radarr repair
* **health:** two-strike checks, damage classification and Arr replacement
* **import:** accept C# admin and WebDAV passwords at the first sign-in
* **import:** carry a C# install's library, history and settings over on first boot
* **import:** carry C#'s STRM setup over and keep its STRM links playing
* **import:** convert the library when the import strategy, STRM key, public URL or mount changes
* **import:** keep Arrs waiting when the upgrade from C# fails
* **import:** map C# settings onto ours in the upgrade report
* **import:** report what importing a C# /config would carry over
* **mount:** log FUSE requests and mount lifecycle
* **mount:** mount the tree read-only over FUSE with remount backoff and kernel tuning
* **mount:** name FUSE readers by process, pid and uid/gid
* **nntp:** add community-maintained provider catalog compiled from providers/*.toml
* **nntp:** add Easyusenet and more provider servers to the catalog
* **nntp:** add implicit TLS, pipelined BODY and zero-copy streaming decode
* **nntp:** add missing provider servers to the catalog
* **nntp:** add pipelined per-provider connection pool with global download permits
* **nntp:** add pipelined STAT and a keepalive warm connection floor
* **nntp:** count breaker trips and provider rescues, trace reply latency and decode
* **nntp:** count provider requests and trace segment fetches
* **nntp:** fail over across providers with per-provider circuit breakers and connection-limit throttling
* **nntp:** fetch and decode yEnc article bodies over one connection
* **nntp:** let diagnostics take a provider exclusively and yield to playback
* **nntp:** log provider outages and connection limits once as warnings
* **nntp:** meter provider downloads and skip providers whose quota is used up
* **nntp:** open connections ahead of demand with prewarm
* **nntp:** route by provider priority levels and skip missed backbones
* **nntp:** skip providers that recently lacked an article
* **par2:** read PAR2 file descriptions and slice checksums from partial files and verify slices
* **queue:** count imports and health check results since start
* **queue:** expand stored archives nested inside archives
* **queue:** fail full disc releases in video categories
* **queue:** fail releases with missing or invalid media and enforce the owning Arr's media type
* **queue:** hand jobs off as STRM files in STRM mode
* **queue:** import and stream AES-encrypted RAR and 7z members
* **queue:** import queued NZBs into /content with PAR2 names, archive members and STAT sampling
* **queue:** import two jobs at once and drop results of jobs removed mid-import
* **queue:** name obfuscated files after their release folder
* **queue:** parse NZBs with SABnzbd's acceptance rules, including gzip and namespaced files
* **queue:** pause the queue or single jobs, configure concurrency and back off retries
* **queue:** requeue imports that stall and fail them on the third stall
* **queue:** return the queued job for a duplicate NZB and record refused NZBs as failed
* **queue:** store Windows-safe file and folder names
* **sab:** add NZBs by URL with mode=addurl
* **sab:** identify as SABnzbd when fetching NZBs
* **sab:** retry failed jobs from their stored NZB
* **sab:** serve the SABnzbd API for adding NZBs, queue and history
* **sab:** tell owning Arrs about finished jobs
* **stream:** add a shared segment cache and performance settings
* **stream:** add seekable segment reader with ordered prefetch
* **stream:** bound decoded bytes in flight with a shared in-order budget
* **stream:** fill missing MPEG-TS segments with null packets
* **stream:** stop playback past too much missing data
* **stream:** trace read-ahead window, connection queueing, hedge wins and drained replies
* **ui:** add a performance settings page
* **ui:** add Network settings with trusted proxies
* **ui:** add NZBs from the queue page with a chosen category
* **ui:** add provider and settings screens
* **ui:** add provider speed test and auto-tune pipeline actions
* **ui:** add sign-in requirement to Settings &gt; Authentication
* **ui:** add sign-in, queue, history and health screens
* **ui:** add Sportarr instances, move providers under settings as NNTP Providers and settings below system
* **ui:** add the overview dashboard, Prometheus toggle and trace export
* **ui:** chip input for download client categories
* **ui:** choose between symlinks and STRM files on the Imports page
* **ui:** collapse subtitle tracks into one media line
* **ui:** confirm the admin password during first-time setup
* **ui:** download a support pack from Settings &gt; Support
* **ui:** edit extra blocked filename patterns in import settings
* **ui:** filter the Explorer by encryption and show it in file details
* **ui:** group repeated reads of a file into one playback row
* **ui:** group settings into platform, automation and system sections and rename account to authentication
* **ui:** health monitoring settings, state filters and needs-attention list
* **ui:** hide system folders in the explorer tree behind a toggle
* **ui:** in-browser player with recovery and playback diagnostics
* **ui:** library explorer with tree, filters, details and removal preview
* **ui:** link completed queue jobs to their files in the explorer
* **ui:** list overview providers in failover order
* **ui:** mute release details after the year in item names
* **ui:** pause and resume the queue and jobs, set import concurrency
* **ui:** preview and follow library conversions from the Imports page
* **ui:** provider quota settings, usage bars, usage reset and timed test progress
* **ui:** redesign the overview dashboard with activity, provider, rescue, record and catalogue panels
* **ui:** replace the logo with a simpler vector mark
* **ui:** restyle with shadcn and the logo palette
* **ui:** rework overview layout, chart controls and stat hierarchy
* **ui:** say on the health page when routine checks are off
* **ui:** serve the embedded web UI
* **ui:** show container CPU and memory on the System page
* **ui:** show each Arr's SABnzbd clients and whether they point here
* **ui:** show history below the queue and drop the history page
* **ui:** show import errors in a details dialog and quiet queue rows
* **ui:** show media analysis and broken containers in the explorer
* **ui:** show mount status and recent logs
* **ui:** show shared backbones and failover order on the providers page
* **ui:** show streaming quality, provider tail latency, workload cost and read history
* **ui:** show the segment cache budget on the memory bar
* **ui:** show trends, usage by app, rejected releases, stall counts and import durations
* **ui:** show version and live activity in the sidebar
* **ui:** show when a newer build is available on main
* **ui:** split segment cache from app memory on the System page
* **ui:** split settings into a page per category
* **ui:** test an Arr connection from Settings &gt; Arr instances
* **ui:** trace reads and show where playback stalled
* **ui:** view the C# import report again from Settings &gt; Support
* **vfs:** list open reads and trace them on demand
* **vfs:** serve /content, /.ids, /completed-symlinks and /nzbs with multipart readers
* **webdav:** serve the tree over WebDAV and /view with ranges, Basic auth and NZB drop-in
* **webdav:** show the client address in read history
* **yenc:** add incremental decode that stops at yEnc control lines and the NNTP terminator
* **yenc:** add rapidyenc-backed yEnc decode, encode and CRC32 crate


### Bug Fixes

* **api:** check for newer releases instead of newer commits on main
* **api:** count only failures the caller sees as errors
* **api:** decimal performance presets that keep at least the previous byte budgets
* **api:** group read usage by the app's first word
* **api:** load library folders saved before they gained an Arr path
* **api:** no trailing dot on links converted from STRM files for extensionless items
* **api:** read the player filter of /reads from the query string
* **api:** say the server keeps no copy of a support pack
* **api:** start with defaults instead of failing on an out-of-range stored setting
* **api:** write the support pack generated_at as an RFC 3339 time
* **arr:** reconcile only after the first discovery found each Arr's clients
* **auth:** say the username or password is wrong when sign-in fails
* **db:** delete a job folder emptied through its subfolders
* **db:** delete job folders left empty when their last file is deleted
* **db:** keep metrics stores that fail migration and quarantine corrupt ones
* **deps:** update rustls to 0.23.46 for RUSTSEC-2026-0346..0349
* **deps:** update rustls-webpki and webpki-roots for distrusted CA advisories
* **health:** keep items when an Arr reports a file missing from disk
* **health:** keep repair owner lookup working after SAB history deletion
* **health:** never replace a file while it is being watched
* **health:** one failing file no longer stops health checks for the library
* **health:** repair migrated files whose download history is gone
* **import:** accept a library folder that holds the mount or STRM directory
* **import:** bring C# health checks scheduled years out within 90 days
* **import:** carry over C# downloads with an empty category or unknown size
* **import:** carry over C# quota usage and storage-group backbones
* **mount:** date fixed directories from server start instead of 1970
* **mount:** give fixed folders a constant date instead of server start
* **mount:** keep FUSE reads in order and survive panics and kills
* **mount:** let Arr apps import links from the FUSE mount
* **mount:** measure first byte from the first read, not from open
* **mount:** warn when FUSE readahead can't be raised in Docker
* **mount:** warn when the mount is not visible outside the container
* **nntp:** a STAT success no longer resets the breaker back-off
* **nntp:** count a dropped provider connection as one failure
* **nntp:** fail over to the next provider when a stream read times out
* **nntp:** fail over when a provider serves the wrong part of a post
* **nntp:** probe a tripped provider once its cooldown ends
* **nntp:** report unavailable rather than corrupt when a provider was skipped
* **nntp:** requests that finish after a trip no longer close the breaker
* **nntp:** stop hung new connections from stalling playback
* **nntp:** stream reads give up after 30 s without a download slot
* **queue:** cap each import at 16 provider requests across all steps
* **queue:** fail over when a provider serves the wrong article during import
* **queue:** one crashing import no longer stops the queue
* **queue:** rename every file of packs that carry one PAR2 set per file
* **sab:** create category folders up front so Arr path checks pass
* **sab:** match parameter and NZB file field names case-insensitively
* **stream:** keep disk cache recency across restarts
* **stream:** stamp body progress at arrival and allow per-reader experiment switches
* **ui:** align overview tile trends and show short read times in seconds
* **ui:** allow picking NZB files on iOS
* **ui:** clarify the read-ahead hint
* **ui:** drop decimals from overview activity totals
* **ui:** fit provider settings on mobile and name slider thumbs
* **ui:** fit the player to the window and warn about undecodable audio
* **ui:** focus the username field on the sign-in page
* **ui:** format sub-millisecond first bytes and single stalls in read history
* **ui:** give settings section headers their own tier
* **ui:** indent the orphan action under auto-repair
* **ui:** mute release details in overview file names
* **ui:** open the player on plain-HTTP LAN addresses
* **ui:** pluralize held reconciliation counts
* **ui:** put Add Arr instance at the top like Add provider
* **ui:** queue page no longer crashes when the default category is empty
* **ui:** rename the providers settings link to Providers
* **ui:** scroll a new Arr instance fully into view
* **ui:** scroll dialogs that are taller than the window
* **ui:** scroll to the file details card when it opens in Explorer
* **ui:** show an error with a reload button instead of a blank page
* **ui:** show sizes, speeds and tuning in decimal MB and GB
* **ui:** show the hostname, port, TLS and backbone a provider profile sets
* **ui:** show the orphan action only while auto-repair is on
* **ui:** stop asking to convert a library that needs no changes
* **ui:** stop library conversion buttons from saving settings
* **ui:** wrap page header actions on narrow screens


### Performance Improvements

* **db:** index job folders, NZB references and latest health checks
* **db:** keep an hourly provider-bytes summary for metrics records
* **db:** look up latest health only for the explorer page
* **db:** open the metrics store in the metrics task
* **mount:** raise FUSE background limits inside containers
* **nntp:** keep two connections warm to each primary provider
* **nntp:** serve waiting playback requests before imports and health
* **nntp:** spread requests across idle connections before pipelining
* **nntp:** stream decoded body chunks and skip requests cancelled while queued
* **nntp:** wait for a connecting slot instead of queueing behind a busy connection
* **sab:** filter and page history in SQL
* **stream:** cache bodies that arrive after their reader left
* **stream:** hedge slow head segments and warn on size mismatches
* **stream:** keep the previous segment so out-of-order reads do not reset prefetch
* **stream:** keep the read-ahead open when playback keeps pace with downloads
* **stream:** open the read-ahead window fully after the first segment
* **stream:** prewarm connections when a read window starts
* **stream:** serve the awaited segment as it arrives and open bounded ranges fully
* **stream:** stream every prefetched segment in as it arrives


### Refactors

* **health:** move the Arr client into an arr crate shared by all six profiles


### Build System

* **docker:** build the web UI into the image
* **docker:** include ffprobe in the runtime image
* **docker:** move the image and release builds to Ubuntu 26.04
* **docker:** ship the server as an ubuntu:24.04 image with FUSE support
* target glibc on Ubuntu 24.04 instead of musl
