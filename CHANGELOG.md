# 1.0.9 (2020-03-18)
## Edge Hub
### Bug fixes
* Use parallel processing for subscription processing ([eac1a18](https://github.com/Azure/iotedge/commit/eac1a1862bac70d09880a84df9d429eedacf58fb))
* Set timeout on edgeHub's side for device and module client's OpenAsync ([1d37dc9](https://github.com/Azure/iotedge/commit/1d37dc941a2fcd6534f331470b4ea32aeae50d07))

# 1.0.9-rc6 (2020-02-29)
## Edge Hub
### Bug Fixes
* Hotfix [Linux ARM32 and ARM64 security vulnerability](https://lists.ubuntu.com/archives/ubuntu-security-announce/2020-January/005286.html) by updating base dotnet core runtime images ([fa634ef](https://github.com/Azure/iotedge/commit/fa634efccdc9694e611d97c4dd57a44ad9b742bb))
* Use LogLevel to limit RocksDB LOG file size ([c984f63](https://github.com/Azure/iotedge/commit/c984f6330daec8800e6887f666036df5bdc7ec68))

## Edge Agent
### Bug Fixes
* Hotfix [Linux ARM32 and ARM64 security vulnerability](https://lists.ubuntu.com/archives/ubuntu-security-announce/2020-January/005286.html) by updating base dotnet core runtime images ([fa634ef](https://github.com/Azure/iotedge/commit/fa634efccdc9694e611d97c4dd57a44ad9b742bb))
* Use LogLevel to limit RocksDB LOG file size ([c984f63](https://github.com/Azure/iotedge/commit/c984f6330daec8800e6887f666036df5bdc7ec68))

# 1.0.9-rc5 (2020-02-21)
## Edge Hub
### Features
* Update Microsoft.Azure.Devices to version 1.18.4 and Microsoft.Azure.Devices.Client to version 1.22.0 ([f155469])(https://github.com/Azure/iotedge/commit/f1554690f539dc53fac0cacb4fc226a159baa45d)
* AMQP Heartbeat feature for edgeHub ([8f26e82])(https://github.com/Azure/iotedge/commit/8f26e82e74e68282cd09be7137eec37e99474ed2)

### Bug fixes
* Dispose all clients when network disconnection ([4269881])(https://github.com/Azure/iotedge/commit/42698815243b5ec4746b47d09e61b0c0a9d84bba)
* Fix Connect to cloud lock ([fbcc45a]) (https://github.com/Azure/iotedge/commit/fbcc45a1f819a85053e7a8e1a2c8114c4aa8fa2f)
* Fix offline restart for edgeHub ([faa2bfb])(https://github.com/Azure/iotedge/commit/faa2bfb35b7cdcc1d621d3ee2c86ab318f8ede33)
* Metrics fixes ([c1f5ae4])(https://github.com/Azure/iotedge/commit/c1f5ae483c6c7206043b2919b1b7267659dfa489)
* Update Windows base images for arm32 and amd64 ([dcebcd1])(https://github.com/Azure/iotedge/commit/dcebcd1a423b8963750feb7ba3f317c176bc6db9)

## Edge Agent
### Features
* Update Microsoft.Azure.Devices to version 1.18.4 and Microsoft.Azure.Devices.Client to version 1.22.0 ([f155469])(https://github.com/Azure/iotedge/commit/f1554690f539dc53fac0cacb4fc226a159baa45d)
* AMQP Heartbeat feature for edgeAgent ([daa4e54])(https://github.com/Azure/iotedge/commit/daa4e5418aa7788ebb37563bfff82a35cf397a6f)

### Bug fixes
* Metrics fixes ([c1f5ae4])(https://github.com/Azure/iotedge/commit/c1f5ae483c6c7206043b2919b1b7267659dfa489)
* Update Windows base images for arm32 and amd64 ([dcebcd1])(https://github.com/Azure/iotedge/commit/dcebcd1a423b8963750feb7ba3f317c176bc6db9)

## iotedged
### Features
* Add rust-toolchain file instead of always using stable ([2676621])(https://github.com/Azure/iotedge/commit/267662113d876dc17dd9a83cbc54007a99a9edef)
* Change DPS provisioning check error to warning ([86d44ea])(https://github.com/Azure/iotedge/commit/86d44eaedd5188a6fcd068ef256624f246a111b7)

### Bug fixes
* Fix Windows build to compile against openssl 1.1.1 ([acf6bf3])(https://github.com/Azure/iotedge/commit/acf6bf3ca051e00371493a37003701bc408415ed)
* Make auto_generated_cert_lifetime not required ([319a020])(https://github.com/Azure/iotedge/commit/319a0203a17326d8ad853b0131ae1ec8eab3e928)
* Fix verbiage for edge check certificate warning ([e468d03])(https://github.com/Azure/iotedge/commit/e468d03d79b71bb0bdcc254fe08e1e3028fbab7d)
* Changed ASN1 encoding of Basic Constrains/CA ([3fee6d2])(https://github.com/Azure/iotedge/commit/3fee6d29b1148dda0d78860f1a1e3fcc0e7db70b)

# 1.0.8.5 (2020-01-23)

## Edge Hub
### Bug Fixes
Hotfix [windows security vulnerability](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-0601) by updating base nanoserver images ([5a88e89](https://github.com/Azure/iotedge/commit/5a88e89e55f589c42c1b391794a1555d853dcef0))

## Edge Agent
### Bug Fixes
Hotfix [windows security vulnerability](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-0601) by updating base nanoserver images ([5a88e89](https://github.com/Azure/iotedge/commit/5a88e89e55f589c42c1b391794a1555d853dcef0))

# 1.0.9-rc4 (2020-01-10)

## Edge Hub
### Features
* Update Microsoft.Azure.Devices to version 1.18.2 ([ade908a](https://github.com/Azure/iotedge/commit/ade908a78a0d885cdfadf11f1b6636e6d1a8ffa6))
* Update Microsoft.Azure.Devices.Client to version 1.21.3 ([b52c719](https://github.com/Azure/iotedge/commit/b52c719f41b342876dc926c542cf660fe7e3224d))
* Install Trust Bundle in EdgeAgent and EdgeHub ([2847ffc](https://github.com/Azure/iotedge/commit/2847ffcf32f3e3467a4523c1d84c4d971ea7ceed))
* Add support for Queue length metric in EdgeHub ([4ce6aa4](https://github.com/Azure/iotedge/commit/4ce6aa43f82c9e5fdece6c6d2ceb4a2b6249af23))
* Direct method calls now support multibyte utf8 encoded characters in payload ([bfc87a8](https://github.com/Azure/iotedge/commit/bfc87a82e85687bbf368f94eefde430b453dbed9))

### Bug Fixes
* Fix flag typo ([5d8e6b0](https://github.com/Azure/iotedge/commit/5d8e6b06fe62f82353e6792fcd26d0ec22b5d141))
* Fix edgeHub crash when using experimental features ([5c7dfe9](https://github.com/Azure/iotedge/commit/5c7dfe9e63aba1d39815ff8ce72b9696f948bc28))
* Fix message loss during transient network scenarios ([ada2042](https://github.com/Azure/iotedge/commit/ada2042e0da344a586f4e5fed03c46369f9ca856))
* Fix message ordering during transient network scenarios ([25ebf58](https://github.com/Azure/iotedge/commit/25ebf58de507720b1560ee5a06b33bd0d279d66d))

## Edge Agent
### Features
* Update Microsoft.Azure.Devices to version 1.18.2 ([ade908a](https://github.com/Azure/iotedge/commit/ade908a78a0d885cdfadf11f1b6636e6d1a8ffa6))
* Update Microsoft.Azure.Devices.Client to version 1.21.3 ([b52c719](https://github.com/Azure/iotedge/commit/b52c719f41b342876dc926c542cf660fe7e3224d))
* Add prometheus metrics to Agent ([1268500](https://github.com/Azure/iotedge/commit/1268500b8f1977722987d5e87e5b23e8dde4347e))
* Add host and docker level metrics ([d5531d4](https://github.com/Azure/iotedge/commit/d5531d4bb93b4e22c8d03ba7af21b3fd4cdab4ef))
* Install Trust Bundle in EdgeAgent and EdgeHub ([2847ffc](https://github.com/Azure/iotedge/commit/2847ffcf32f3e3467a4523c1d84c4d971ea7ceed))

## iotedged
### Features
* Update rust to 1.40.0 ([f7a14fd](https://github.com/Azure/iotedge/commit/f7a14fd84270d242d13574654c56aa351816d35f))

# 1.0.9-rc3 (2019-11-21)
## Edge Hub
### Features
* Update Twin max property depth and length limits to match IoTHub ([2d69f78](https://github.com/Azure/iotedge/commit/2d69f7879ee4c90e805f6ae6b0053d5b71b2947c))
* Update .NET core version to 2.1.13 ([6b27f06](https://github.com/Azure/iotedge/commit/6b27f064fcd78374bae8a7f53162130d6eb4916c))

### Bug fixes
* Update Twin property value validation to apply 4K property value length limit ([4acce35](https://github.com/Azure/iotedge/commit/4acce3576be89cfc8c929229d6c5c7c6a6b41cc5))
* Set max rocksdb write-ahead-log size to 512MB ([1853388](https://github.com/Azure/iotedge/commit/18533882b86db081e8370d9f9be5750181d3e930))
* Fix iotedge version passed instead of client version ([4b335d2](https://github.com/Azure/iotedge/commit/4b335d2336d15f72a1be110f1168d75e69c37c00))

## Edge Agent
### Features
* Add iotedge support bundle ([1853388](https://github.com/Azure/iotedge/commit/18533882b86db081e8370d9f9be5750181d3e930))
* Update .NET core version to 2.1.13 ([6b27f06](https://github.com/Azure/iotedge/commit/6b27f064fcd78374bae8a7f53162130d6eb4916c))

### Bug fixes
* Update deployment status to "success" if there is no deployment change ([ee0ce67](https://github.com/Azure/iotedge/commit/ee0ce67eed7a7fd685f8a719054c543bbadd428d)) 
* Set max rocksdb write-ahead-log size to 512MB ([1853388](https://github.com/Azure/iotedge/commit/18533882b86db081e8370d9f9be5750181d3e930))
* Fix iotedge version passed instead of client version ([4b335d2](https://github.com/Azure/iotedge/commit/4b335d2336d15f72a1be110f1168d75e69c37c00))

## iotedged
### Features
* Allow the user to specify auto generated certificate expiry ([d0f6ed3](https://github.com/Azure/iotedge/commit/d0f6ed3a2caef77881ec536e56c83c48091c5577))

### Bug fixes
* Fix "storage directories are mounted from host" checks to account for mounts of parent directories ([666313b](https://github.com/Azure/iotedge/commit/666313b79be406f96904e0a7c724a15759cad5cc))

# 1.0.8.4 (2019-11-19)
## Edge Hub
### Bug Fixes
* Fix Twin property 4K length validation ([c4a97a4](https://github.com/Azure/iotedge/commit/c4a97a40e0b1db1ceb1483baa7dab6b17705467b))
* Updating Twin update limits to match IoTHub ([0ae34d3](https://github.com/Azure/iotedge/commit/0ae34d3a8b6750e9caae8045b71cd21d2e40e119))
* Fix iotedge version passed instead of client version ([b0e13d8](https://github.com/Azure/iotedge/commit/b0e13d85035181ec3aafa347a7fd12b086608db1))
* Update dotnetcore to 2.1.13 ([df015b4](https://github.com/Azure/iotedge/commit/df015b4ea7f0322da6386fac6c5d22ec8b2593ae))
* Changed CloudEndpoint to fail subsequent batches after a transient error ([d2115b6](https://github.com/Azure/iotedge/commit/d2115b6d017c28dec66ca3b43b2f7712f6278766))

# 1.0.8.3 (2019-10-18)
## Notes
* If using the C# SDK, please use version 1.20.3

## Edge Hub
### Bug Fixes
* Add ASC support ([466759f](https://github.com/Azure/iotedge/commit/466759fc6a24acec3b124af4f5f05dd98ab0d190))
* Fix deployment status ([f602329](https://github.com/Azure/iotedge/commit/f602329a5555b7e32dda2326cf0dd6956c20a80f))
* Fix message loss caused by connectivity exceptions ([e079073](https://github.com/Azure/iotedge/commit/e0790738e1888c1f8a53bf8ab2600edcb6eba304))

# 1.0.8.2 (2019-09-27)
## Edge Hub
### Bug Fixes
* Set RocksDB total WAL size to 512M ([07ee35d](https://github.com/Azure/iotedge/commit/07ee35d79a11eb6daab2a883e82ffbd7a1e93682))
* Fix leaking event handlers in offline scenario ([f3b8a46](https://github.com/Azure/iotedge/commit/f3b8a463372d94163c286bd4c1a81ea9eb811832))
* Fix error if client does not send product info  ([9267a05](https://github.com/Azure/iotedge/commit/9267a0545ac4394400afbcabdc123737ebcfbc17))

# 1.0.9-rc2 (2019-09-05)
## Edge Hub
### Bug fixes
* Fix delay in module 2 module messages ([6907bef](https://github.com/Azure/iotedge/commit/6907bef066479cbdda2325722e7715e02966c4d1))
* Add back V0 metrics ([0301448](https://github.com/Azure/iotedge/commit/03014487cd8b096afc81fbd63b12f0958faa9a45))
* Change tags for messages_sent metric ([6376d92](https://github.com/Azure/iotedge/commit/6376d92412a1d4b6ea97b8c43669458df95cd48e))

## iotedged
### Bug fixes
* Show certificate expiry in self-signed certs warning ([bb9b40c](https://github.com/Azure/iotedge/commit/bb9b40c5ac0311de060d9b85808651d0fb670230))

# 1.0.8.1 (2019-08-27)
## Edge Hub
### Bug Fixes
* EdgeHub: Fix delay in module 2 module messages ([06ec89f](https://github.com/Azure/iotedge/commit/06ec89f5220404fe24cea59e4c6241326f2c179a))
* Set client subscriptions when cloud connection is re-created ([a274ca0](https://github.com/Azure/iotedge/commit/a274ca02bde1bdacc48d76b5b43abaf919c9d4fc))

# 1.0.9-rc1 (2019-08-16)
* Support running the Windows installer script in 32-bit PS host on 64-bit Windows ([76eacaf](https://github.com/Azure/iotedge/commit/76eacaf988e7d421b4e45c70a45d8160f1feaaa1))
* `iotedge check` improvements ([8090d6c](https://github.com/Azure/iotedge/commit/8090d6c7fc47a377787d5d9ff15ed5fea894112c))

## Edge Agent
### Features
* Add support to get logs using direct method ([493782f](https://github.com/Azure/iotedge/commit/493782f42a5d563df5fcb40d79a07fcd30a4f01d))
* Add support for specifying a pull policy for modules ([a39543c](https://github.com/Azure/iotedge/commit/a39543ce1924e7d16b27c43d66bbbc5eb0a7ca29))
* Add support to restart module using direct method ([fbeec72](https://github.com/Azure/iotedge/commit/fbeec72cf974b0b37f45de83fb6a395ba79b6029)))

### Bug fixes
* Fix desired property updates with empty patch ([46c77a5](https://github.com/Azure/iotedge/commit/46c77a525c439089b069da62a9f6c5b9af0e87e4))
* Fix getting status of failed tasks ([bd51b6b](https://github.com/Azure/iotedge/commit/bd51b6b341c9e1c2dd18a98261382e7fa8623352))

## Edge Hub
### Features
* Metrics in EdgeHub ([f93c6f3](https://github.com/Azure/iotedge/commit/f93c6f3f217a3ee2a6bc0ba291c936db7aef7f50))
* Support for forwarding ASC property in messages ([fe1fcf6](https://github.com/Azure/iotedge/commit/fe1fcf63bc58b24ed7566bf302c47afe50f59dda))

### Bug fixes
* Fix leaking event handlers in offline scenario ([4f05275](https://github.com/Azure/iotedge/commit/4f052756228bf84ac663e4f6171a0a47aa2025ae))
* Fix handling cloud subscriptions if a feedback message is received multiple times ([f9d1e07](https://github.com/Azure/iotedge/commit/f9d1e07a57fba5e171d1956e012e901a8427b72c))
* Fix handling connections with no product information ([bb31324](https://github.com/Azure/iotedge/commit/bb31324b90caa7ac28b9526034f289dd5551d2fa))
* Initialize EdgeHub before starting protocol heads ([32888fa](https://github.com/Azure/iotedge/commit/32888fa62a72d8e15b8b412682704cde1b301fbc))

## iotedged
### Features
* Add a new external provisioning mode that uses a hosting environment endpoint for retrieving device specific information ([539efad](https://github.com/Azure/iotedge/commit/539efad6a67aabfddb76f1a320d5c16125549388))
* Support for hybrid X.509 certificate authentication for IoT Edge ([f012c28](https://github.com/Azure/iotedge/commit/f012c28cdff2b0ac743e167c543d371b5a3269d0))
* Add support for additional container network configuration to support IPv6-only devices ([9001b8e](https://github.com/Azure/iotedge/commit/9001b8e86b4e7323e970542760b13016c5ae5ace))
* Use file URIs for X.509 identity certificates ([34f833c](https://github.com/Azure/iotedge/commit/34f833c495479f1666c7fc72a7084356678bbd78))
* Remove Edge identity certificate auto generation ([81fbdf4](https://github.com/Azure/iotedge/commit/81fbdf42844bd563c95c591f9e61a8abe0206991))

### Bug fixes
* Don't restart iotedged when config.yaml isn't ready ([1570c2c](https://github.com/Azure/iotedge/commit/1570c2cb2129b609d56b24800af9f00499b388fd))
* Add timeout to workload api operations ([da97168](https://github.com/Azure/iotedge/commit/da97168ce1529105422f5673e66dc184d95c6981))
* Sort `iotedge list` output by module name ([0ea4943](https://github.com/Azure/iotedge/commit/0ea4943f390fbaadc45af993df05cafe03bf2030))
* Should not reconfigure when DPS reprovisioning from backup ([8d36200](https://github.com/Azure/iotedge/commit/8d362006f6c011e10740cc577b371f48f55a34d9))

# 1.0.8 (2019-07-22)
* Fix Win install setup for symmetric key provisioning mode ([602472f](https://github.com/Azure/iotedge/commit/602472fa2a205e08cf87b345544a364eea09a5dd))

## Edge Agent
### Bug Fixes
* Put experimental features behind experimental flags ([9e6ea0c](https://github.com/Azure/iotedge/commit/9e6ea0c7df6568554cb6508ca56a8f9ae489b07b))

## Edge Hub
### Bug Fixes
* Put experimental features behind experimental flags ([9e6ea0c](https://github.com/Azure/iotedge/commit/9e6ea0c7df6568554cb6508ca56a8f9ae489b07b))

# 1.0.8-rc3 (2019-07-02)
* Upgrade C# Client SDK to 1.20.3 and Service SDK to 1.18.1
* Various improvements to `iotedge check` troubleshooting command

## Edge Agent
### Bug Fixes
* Fix file extension for logs uploaded to blob store
* Add ability to get status of logs upload request

# 1.0.8-rc2 (2019-06-18)
* Stability improvements

## Edge Agent
### Bug Fixes
* Be more resilient on GetTwin calls ([2c4bc2a](https://github.com/Azure/iotedge/commit/2c4bc2aa54827b5e1500fb4e48c88e31d78fc833))
* Strip headers in get logs calls when sending to blob store ([95a657a](https://github.com/Azure/iotedge/commit/95a657af429ab7d444af035f01d9bbbae4d09b8d))
* Implement equality on registry credentials to prevent unnecessary backup ([c6b0ba9](https://github.com/Azure/iotedge/commit/c6b0ba9eff39a64e05fd5de41406a794b0bdfc95))
* Add timeout to workload client calls ([a1b77bf](https://github.com/Azure/iotedge/commit/a1b77bf1370fef739ce430debab297b463c7f34e))

## Edge Hub
### Bug Fixes
* Configure MQTT protocol head to use num_procs * 2 threads. Improves stability on constrained devices. ([206568c](https://github.com/Azure/iotedge/commit/206568caa575cf9f358e5ff3ab4b6e24d082b7fa))

## iotedged
### Bug Fixes
* Do not reconfigure when provisioning from the backup ([b40ab5b](https://github.com/Azure/iotedge/commit/b40ab5b7e969e553fa868604f168eb0ca37e6194))

# 1.0.8-rc1 (2019-06-03)
* Preview support for Linux arm64
* Upgrade Moby version in .cab file to 3.0.5 ([f23aca1](https://github.com/Azure/iotedge/commit/f23aca1fb532574e6ee7ebb0b70452d4c672ae1a))
* Update .NET Core version to 2.1.10 ([ad345ef](https://github.com/Azure/iotedge/commit/ad345efae692bbf3e28dc3d763f32ab25d667265))

## Edge Agent
### Features
* Support for arm64 ([6189e21](https://github.com/Azure/iotedge/commit/6189e21c47c474ce719685b504d1e2bcde1304f2))
* Initial support for remote get of module logs ([c49f957](https://github.com/Azure/iotedge/commit/c49f957c67ab8362b7e939bc348ed7e853c2c154), [6bc92d2](https://github.com/Azure/iotedge/commit/6bc92d2e235cbdbb24d81d7931253e7c3d81b8eb), [e064a59](https://github.com/Azure/iotedge/commit/e064a599a4842b58b6ff6bd4e88b5b7a1711a828), [5b310b1](https://github.com/Azure/iotedge/commit/5b310b137381d736fec3400909d3a4d36d18994c), [a8cdf8d](https://github.com/Azure/iotedge/commit/a8cdf8daf25fe6d36933494b51272eb425c9d9c6), [75d7460](https://github.com/Azure/iotedge/commit/75d74603664d1f206585ab3473294236b142a011), [951afd8](https://github.com/Azure/iotedge/commit/951afd8cad725bb5fa9b2d4b4ede3f2e047d21e3), [edaad81](https://github.com/Azure/iotedge/commit/edaad8191b854f52ad3d72ba92dc63c22fff685e), [83118b2](https://github.com/Azure/iotedge/commit/83118b2d7ecf8c65be8c07f682294d4fad01b0b3), [5ce1903](https://github.com/Azure/iotedge/commit/5ce1903c54f40d2646f236b7e3fe1e96f278100d), [372026e](https://github.com/Azure/iotedge/commit/372026eb2b9b6df5547dbadc28e182fbd29d26df))
* Additional optional settings to limit upstream bandwidth usage

### Bug Fixes
* Fix NRE in IotHubReporter.ReportShutdown ([81065db](https://github.com/Azure/iotedge/commit/81065db19033c0a4c6aac634b69f837581f8c466))
* In some cases Edge Agent won't restart a stopped module ([6261fc9](https://github.com/Azure/iotedge/commit/6261fc9dc69773332f742295f35d71ac0d4aa35c))
* Edge Agent can support local Docker registries ([2086d4b](https://github.com/Azure/iotedge/commit/2086d4bf40cdce74ffd3f5cc906ee576e7dc848f))

## Edge Hub
### Features
* Support for arm64 ([4fdfa40](https://github.com/Azure/iotedge/commit/4fdfa40686f9308f6f67d7662c50b6664c472994))
* Upstream performance improvements ([864b33d](https://github.com/Azure/iotedge/commit/864b33d6a038596aa6656a58f2f3d28ae4358cc4))
* Twin Manager v2 is now default ([96a0087](https://github.com/Azure/iotedge/commit/96a0087456bf982aad8f11020ab6d39d4b5f9e8b))
* Encrypt twins at rest ([075d5c0](https://github.com/Azure/iotedge/commit/075d5c0a39009eb9b0569e97c02ee1840dd5719f))
* Additional optional settings to limit upstream bandwidth usage

### Bug Fixes
* Fix IoT Hub name parsing in AMQP SASL Plain auth ([bb6c327](https://github.com/Azure/iotedge/commit/bb6c3271b035579ffb4e30af5fa4ab3637cf49f0))
* Set EdgeHub user id to UID 1000 explicitly ([cf40c16](https://github.com/Azure/iotedge/commit/cf40c165f4ffe777086a72bc3e278751be335cbd))
* Fix possible NRE in messages ([1c2efc6](https://github.com/Azure/iotedge/commit/1c2efc63fc4b949f3fd1dd8f06a42e453d5c1966))
* Fix edge case in checking twin version when storing ([663198c](https://github.com/Azure/iotedge/commit/663198cc30257a216f3c301ea5dfba0bf603e174))
* Forward product information for connected devices and modules ([749b9b7](https://github.com/Azure/iotedge/commit/749b9b7212b4257331db8f1641d9afd8a93bd30d))

## iotedged
### Features
* Update uTPM to support Resource Manager v2 ([a272069](https://github.com/Azure/iotedge/commit/a272069cc4f28aa1b724f50b3460f0eab13cad42))
* Return meaningful exit codes on failure ([62f3d44](https://github.com/Azure/iotedge/commit/62f3d44f9da239f5e6ef4a5637df14d93c8a5fe3))

### Bug Fixes
* Properly handle asynchronous errors when pulling images ([020ddbc](https://github.com/Azure/iotedge/commit/020ddbc7e73650956cb85dfa0dea152a89c44e60))
* Fix RPM packages for SUSE ([c16bc50](https://github.com/Azure/iotedge/commit/c16bc50731677040d2a371c1374aa6941b9a34d8))
* Don't lowercase the keys in `config.yaml` ([34df35a](https://github.com/Azure/iotedge/commit/34df35a3975767f9dcd5fc62f3f6bd80a5c63af5))
* Windows install script checks for container feature ([90f6368](https://github.com/Azure/iotedge/commit/90f63680bf19781ba09e9bbfaad26283cc7787b1))

## Simulated Temperature Sensor
### Features
* Support for arm64 ([a9474e0](https://github.com/Azure/iotedge/commit/a9474e0fdc117533886d3bc32fd97cc11105d43d))

# 1.0.7.1 (2019-05-24)
* Fix regression in DPS use on Windows
* Stability improvements

## Edge Agent
### Bug Fixes
* Workaround `ObjectDisposedException` bug in C# SDK by exiting the process ([bbc8d3c](https://github.com/Azure/iotedge/commit/bbc8d3ce1ebc2583717295dfeeb1d737642e9946))

## Edge Hub
### Bug Fixes
* Workaround `ObjectDisposedException` bug in C# SDK by recreating the client ([e458e14](https://github.com/Azure/iotedge/commit/e458e14294d8c39f9e6f72e2c42418bfd298eeb2), [7598ef0](https://github.com/Azure/iotedge/commit/7598ef045c9b104dfdc758d270722007d981d1bb), [c608f38](https://github.com/Azure/iotedge/commit/c608f38b33652f4f2b10a97790fe155e39d9280a))

## iotedged
### Bug Fixes
* Fix bug preventing `iotedged` service starting when DPS provisioning is configured ([8a0f5c0](https://github.com/Azure/iotedge/commit/8a0f5c0ebb9489c98f591851e96e9f6766e031a9), [1ac1e94](https://github.com/Azure/iotedge/commit/1ac1e94298de332f180efe7ab343257207a77ebf))

# 1.0.7 (2019-05-06)
* Upgrade C# SDK to 1.20.1

## Edge Agent
### Bugs
* Add explicit timeout to `Edge Agent` <--> `iotedged` operations and more debug logs ([f2cb600](https://github.com/Azure/iotedge/commit/f2cb6003076cded75dec2dc87a3e79c23aa98fc9))

### Features
* Upgrade to version 1.20.1 of the C# SDK ([1637ff9](https://github.com/Azure/iotedge/commit/1637ff9303a162144f16b4c514859c247cc857fc))

## Edge Hub
### Features
* Upgrade to version 1.20.1 of the C# SDK ([1637ff9](https://github.com/Azure/iotedge/commit/1637ff9303a162144f16b4c514859c247cc857fc))

## iotedged
### Bugs
* Fix `iotedge check` default image ([8c9d5f0](https://github.com/Azure/iotedge/commit/8c9d5f06db57a0388ab30a825a2b9af684c0f7db))
* Load encryption key before generating it ([9174a89](https://github.com/Azure/iotedge/commit/9174a896f7cca21c3dd4ae84c9e097d0d20305d5))

## Simulated Temperature Sensor
### Features
* Upgrade to version 1.20.1 of the C# SDK ([1637ff9](https://github.com/Azure/iotedge/commit/1637ff9303a162144f16b4c514859c247cc857fc))

## Functions Binding
### Features
* Upgrade to version 1.20.1 of the C# SDK ([1637ff9](https://github.com/Azure/iotedge/commit/1637ff9303a162144f16b4c514859c247cc857fc))

# 1.0.7-rc2 (2019-04-10)
* `iotedge check` troubleshooting command
* Upgrade C# SDK to 1.20.0

## Edge Agent
### Features
* Upgrade to version 1.20.0 of the C# SDK ([50420d2](https://github.com/Azure/iotedge/commit/50420d21a4deea6827f9650ebb92fc9eaa89ea5f))

## Edge Hub
### Features
* Upgrade to version 1.20.0 of the C# SDK ([50420d2](https://github.com/Azure/iotedge/commit/50420d21a4deea6827f9650ebb92fc9eaa89ea5f))

## iotedged
### Features
* Add `iotedge check` troubleshooting command ([1d74b97](https://github.com/Azure/iotedge/commit/1d74b97e1893134d6989366145e694dedd162f0f))
* Use CAB file for Windows installation ([ce232a8](https://github.com/Azure/iotedge/commit/ce232a8f8ef98f2b22964242ae34dc810e02672a))

## Simulated Temperature Sensor
### Features
* Upgrade to version 1.20.0 of the C# SDK ([50420d2](https://github.com/Azure/iotedge/commit/50420d21a4deea6827f9650ebb92fc9eaa89ea5f))

## Functions Binding
### Features
* Upgrade to version 1.20.0 of the C# SDK ([50420d2](https://github.com/Azure/iotedge/commit/50420d21a4deea6827f9650ebb92fc9eaa89ea5f))

# 1.0.7-rc1 (2019-02-21)

## Edge Agent
### Features
* Agent pulls images before stopping ([57c6f7d](https://github.com/Azure/iotedge/commit/57c6f7d02c99634fc59f2f9a87fddc867691acb0), [4992833](https://github.com/Azure/iotedge/commit/4992833344f5fbf167c75af4b33b181e2b214692))
* Update C# SDK version ([a3fc35c](https://github.com/Azure/iotedge/commit/a3fc35cd270c85fc25264aaf5eabb951ab59bb13))

### Bug Fixes
* Twin refresh timer logic is now a simple loop ([cb7af40](https://github.com/Azure/iotedge/commit/cb7af4090aca24d624e96ced572d6dc31b7c97c0))

## Edge Hub
### Features
* Update C# SDK version ([a3fc35c](https://github.com/Azure/iotedge/commit/a3fc35cd270c85fc25264aaf5eabb951ab59bb13))

### Bug Fixes
* Defaults to OptimizeForPerformance=false on arm32v7 ([43d47b0](https://github.com/Azure/iotedge/commit/43d47b04c4e70fd7c48a5b05f728925010f2e1ba))
* Limit MQTT thread count on arm32v7 ([2509438](https://github.com/Azure/iotedge/commit/2509438464cf9c7d99922ecd5e15caaf4e9ae242), [56a6db1](https://github.com/Azure/iotedge/commit/56a6db1f0faacf46162e2017a2f4344ac320c6e9))
* Process subscriptions from clients in batch ([20cb6c4](https://github.com/Azure/iotedge/commit/20cb6c46b9c26557a31a7c22261507ed1d3ebe78))

## iotedged
### Features
* Support for DPS symmetric key provisioning ([b7adfff](https://github.com/Azure/iotedge/commit/b7adfffefe85cef84e27302aa0c8f00a3e8a81c2))
* All modules processes are authorized to connect ([777aec1](https://github.com/Azure/iotedge/commit/777aec16a673cad2407bf75291d29b6d5e71ef25))

### Bug Fixes
* Encode deviceid/moduleid for IoT Hub operations ([bb10be0](https://github.com/Azure/iotedge/commit/bb10be01360ed7393260351af2c6e8ad7498346d))

## Simulated Temperature Sensor
### Features
* Add SendData and SendInterval twin configuration ([7dc7041](https://github.com/Azure/iotedge/commit/7dc7041f790ebe323d720913782e8085f1f65c21))
* Update C# SDK version ([a3fc35c](https://github.com/Azure/iotedge/commit/a3fc35cd270c85fc25264aaf5eabb951ab59bb13))

# 1.0.6.1 (2019-02-04)

## iotedged
### Bug Fixes
* Reverts name sanitization of the common name on generated certificates ([078bda7](https://github.com/Azure/iotedge/commit/078bda7b86b55e8017077b8e2490dede1f8703dc))

# 1.0.6 (2019-01-31)
* Stability and reliability fixes

## Edge Agent
### Features
* Update to .NET Core 2.1.6 ([d2023be](https://github.com/Azure/iotedge/commit/d2023bec1bf362cd78d2aff06178b2f18d62cb7c))

### Bug Fixes
* Fix module restart logic when Edge Agent clock is off ([72f7112](https://github.com/Azure/iotedge/commit/72f7112113320fdc8b3d546a24a880d46fb4cd74))
* Use HTTPS proxy on Linux and Windows ([fceef9f](https://github.com/Azure/iotedge/commit/fceef9f35e3c3021523201920f33e06398f26ebb))

## Edge Hub
### Features
* Update to .NET Core 2.1.6 ([d2023be](https://github.com/Azure/iotedge/commit/d2023bec1bf362cd78d2aff06178b2f18d62cb7c))
* Support X509 certificate authentication by default for downstream devices ([4a46290](https://github.com/Azure/iotedge/commit/4a46290d2c2bd309ea9bbf7c697b71851923a08e))
* New improved Twin manager - in preview and not enabled by default ([d99f8ff](https://github.com/Azure/iotedge/commit/d99f8ff085799092fb665466ae7ed7beeffceea3))

### Bug Fixes
* Use HTTPS proxy on Linux and Windows ([eb75f34](https://github.com/Azure/iotedge/commit/eb75f346e19a21953c46f6cc0c2a4c77115d13e9))
* Allow modules on Edge devices with no device scope to connect to Edge Hub ([761254f](https://github.com/Azure/iotedge/commit/761254fa948d95d6de022c6b3c3e5c8e77594679))
* Handle clients with special characters ([82ce72e](https://github.com/Azure/iotedge/commit/82ce72e49a20bdd4feec417c2f7c021af8fc55c4))
* Fix potential for dropped messages when device is rebooted ([88fd5ab](https://github.com/Azure/iotedge/commit/88fd5abc2a817d32adda1338685c0f1f9e1ff744))

## iotedged
### Bug Fixes
* Sort serialization of environment variables in config.yaml ([0e6a402](https://github.com/Azure/iotedge/commit/0e6a402fecf9f11c3f8afff7713352ddc165a234))
* Support installing iotedged on localized Windows installations ([d9b12c9](https://github.com/Azure/iotedge/commit/d9b12c96168222d23fdf1ebc122f3a7ada6fafd2))
* Reinstate "nat" as the Moby network for Windows containers ([913678a](https://github.com/Azure/iotedge/commit/913678ac7e7f65f4f954ba898a4325efdc05dc5a))

# 1.0.5 (2018-12-17)
* Support Windows 10 1809 (RS5)
* Improved error messages in `iotedge`/`iotedged`
* Stability and reliability fixes

## Edge Agent
### Features
* Parallelize stopping modules on shutdown ([271e930](https://github.com/Azure/iotedge/commit/271e930d5ad5fe5fa17d05fee25f55d4cc6ed2a3))

### Bug Fixes
* Avoid caching backup.json on every reconcile ([2cea69f](https://github.com/Azure/iotedge/commit/2cea69f97fb24ebbacdfeec73bb805bfd61f85f7))

## Edge Hub
### Features
* Drain messages from disconnected clients to IoT Hub ([d3f801b](https://github.com/Azure/iotedge/commit/d3f801ba27acea42664876d3dd70fd695f69de5e))
* Make device/module client operation timeout configurable -- helps slow connections ([6102e31](https://github.com/Azure/iotedge/commit/6102e31b660296054e117de3787c149ac1bc627e))
* Resync service identity if client request cannot be authenticated ([677e16d](https://github.com/Azure/iotedge/commit/677e16d96bde53c88459e61ec72b67cd3ef29a3a))
* Enable support for X.509 thumbprint and CA auth for downstream devices - not enabled by default ([187e3df](https://github.com/Azure/iotedge/commit/187e3dfc526a6b49da09d69e75eef7e4454f04d7))
* Add support for X.509 auth for HTTP and MQTT over Websockets - not enabled by default ([9b56f3d](https://github.com/Azure/iotedge/commit/9b56f3d49444d122e2263b494512557576b19b29))
* AMQP and AMQP+WS support for X.509 authentication - not enabled by default ([875776c](https://github.com/Azure/iotedge/commit/875776c71ea6a551caa4150f2a251086c36e2196))
* Allow multiplexing client connections over AMQP ([93be534](https://github.com/Azure/iotedge/commit/93be5343561362c6244e5e42e09b413baecd53c3))

### Bug Fixes
* Fix NRE in TwinManager ([29f5b74](https://github.com/Azure/iotedge/commit/29f5b745057663966eb9fd27d3c0f0b5c9b86c79))
* Handle NRE thrown by device SDK ([5f5fd67](https://github.com/Azure/iotedge/commit/5f5fd67631d69e95c17c6bc32e9f1926da237034))
* Fix obtaining upstream connection when offline ([75e7968](https://github.com/Azure/iotedge/commit/75e796826d7a8c8161b0189e24da2cc6f27655d8))
* Fix MessageStore initial offset after restart ([81f93dc](https://github.com/Azure/iotedge/commit/81f93dc408b24cb1f5cc7bbcbdaf9133a5e24937))
* Add timeout / cancellation support to Store apis ([0eb279b](https://github.com/Azure/iotedge/commit/0eb279beaf5175d5b4e8342f6d313411c748eae7))

## iotedged
### Features
* Add identity certificate endpoint to workload API ([40f1095](https://github.com/Azure/iotedge/commit/40f10950dc65dd955e20f51f35d69dd4882e1618))
* Add module list to workload API ([5547161](https://github.com/Azure/iotedge/commit/554716151f8802a8f1c2c38bdd5a6914fe2191a5))
* Support Unix Domain Sockets on Windows :tada: ([b1ee469](https://github.com/Azure/iotedge/commit/b1ee46916514779b5d8f001bfd2a2f4fdf2bf141))
* Move network-online.target to Wants from Requires in systemd unit ([c525acc](https://github.com/Azure/iotedge/commit/c525acc28a20c3f6c4198ea8db48a76ad61e4d2c))
* Add more informative error messages ([326ef8c](https://github.com/Azure/iotedge/commit/326ef8c0075e66834c82b36fc5551b8ef74f0098))
* Add support for x.509 v3 extensions Subject and Auth Key Identifiers ([9b98780](https://github.com/Azure/iotedge/commit/9b987801a836955ffdcf0b5b6ea9f96db79159df))
* libiothsm-std now includes an so version ([5667a9f](https://github.com/Azure/iotedge/commit/5667a9fd06b6570ab3fc4a4d6b45e1d5c3988638))
* Remove write access for BUILTIN\Users in `C:\ProgramData\iotedge` ([d6b8c3a](https://github.com/Azure/iotedge/commit/d6b8c3a89a7c9b4964651490f72007cf72183112))
* Update Windows images to RS5 ([f72a238](https://github.com/Azure/iotedge/commit/f72a238ecd65dbdd627c0dd474f7a8f7ab1876bc))
* Enable TLS 1.2 for Invoke-WebRequest ([e93e707](https://github.com/Azure/iotedge/commit/e93e70721ea2089a424ec13e5fcdc5daa7d05018))
* Start service automatically on Windows startup when using Windows containers on Moby ([f72a238](https://github.com/Azure/iotedge/commit/f72a238ecd65dbdd627c0dd474f7a8f7ab1876bc))
* Restart service on crash ([f72a238](https://github.com/Azure/iotedge/commit/f72a238ecd65dbdd627c0dd474f7a8f7ab1876bc))
* Windows installer support for offline installation (using the `-OfflineInstallationPath parameter) ([8cec3d5](https://github.com/Azure/iotedge/commit/8cec3d50f9035160e3bd3e537f84ab48a6e28f58))
* Windows installer support for reusing previous config.yaml on reinstall ([82b82cc](https://github.com/Azure/iotedge/commit/82b82ccffdaeed408b04803ea2679e9b626d15c9))
* `iothsm.dll` now configured to use physical TPM instead of emulator

### Bug Fixes
* Fix potential race in management API list modules ([645545a](https://github.com/Azure/iotedge/commit/645545af22caeb2a6a4883a5adb0881eb5a2ca0f))
* Update Windows installer to create user-defined network for modules ([6d5b95a](https://github.com/Azure/iotedge/commit/6d5b95a7be94daa0f297c4288485301cb988f9f0))

# 1.0.4 (2018-10-31)
* Stability and reliability fixes
* AMQP+WS in Edge Hub
* Functions Binding published as Nuget package

## Edge Agent
### Features
* Allow longer createOptions fields ([ecfc2a0](https://github.com/Azure/iotedge/commit/ecfc2a0d30edced286c42d5090bd9eb953251b86))

### Bug Fixes
* N/A

## Edge Hub
### Features
* Add AMQP over Websockets protocol head ([87372c8](https://github.com/Azure/iotedge/commit/87372c88d5d6ee4c58ee2c050322d67c044f52be))
* Automatic server certificate renewal ([f557fc3](https://github.com/Azure/iotedge/commit/f557fc30a6ef5536c05accaa914d037ed8da70a7))

### Bug Fixes
* Fix updating message store endpoints when routes are updated ([98a61c0](https://github.com/Azure/iotedge/commit/98a61c0b6f81c601f8fa5edcfae79dc4f4cfbc94))
* Support C SDK CBS mode on AMQP ([84be08c](https://github.com/Azure/iotedge/commit/84be08c25bff3cc67606385422fd904e237f5580))
* Improve connection recovery after offline periods ([6069f7f](https://github.com/Azure/iotedge/commit/6069f7fb7bf292f1208d99e0890e5cd6106a6666))
* Setup storage directory in all cases ([e0a1a08](https://github.com/Azure/iotedge/commit/e0a1a081ed587351b58893e42eba9787f982aa3c))
* Fix handling of re-subscriptions after an offline period ([d8b9038](https://github.com/Azure/iotedge/commit/d8b90389b66c8c19bff012635926e90f11176fd8))

## iotedged
### Features
* Improved error messages for docker image pull failures ([0d13741](https://github.com/Azure/iotedge/commit/0d13741b1c2262a783bb60bb55d192e696278b2b), [9f500e4](https://github.com/Azure/iotedge/commit/9f500e49782314261ae9fd33c64b8cc6e4ae94f8))
* Update hyper http library to 0.12 ([10d1d79](https://github.com/Azure/iotedge/commit/10d1d79ddd953f423a955052fa0666cfda2f6c40))
* Regenerate quick start mode CA certificate on startup ([d2195f8](https://github.com/Azure/iotedge/commit/d2195f8b35f0105b9692ec2e25090890f8e53bf3))
* Add aarch64 build scripts ([13ddaa6](https://github.com/Azure/iotedge/commit/13ddaa6f66b7e8a8538c5c7155411c2a5066386d))
* Support HTTP proxy authentication ([42af84d](https://github.com/Azure/iotedge/commit/42af84d760c56a6ed297b5b88f68906808b27097))

### Bug Fixes
* Do not return container sizes in list response (performance improvement) ([8ecb27b](https://github.com/Azure/iotedge/commit/8ecb27b043a0e1fbc2293aa91cb61c65ff2d3a6a))
* Add PartOf to iotedge.socket units to enable proper shutdown ([f48a966](https://github.com/Azure/iotedge/commit/f48a9666f8a837bc19d977c8248bec147ff17d61))
* Add docker.service as a dependency of iotedged.service ([281c73e](https://github.com/Azure/iotedge/commit/281c73eb0e01172bdfd1a3e904a9aab26f950297))
* Improve Windows install/uninstall experience ([a135bdf](https://github.com/Azure/iotedge/commit/a135bdfb35fc3a163ebeaf7cb211052fa0410a16))
* Fix Stop-Service error on Windows ([466fe02](https://github.com/Azure/iotedge/commit/466fe02b2fbcd4537e9f767e8b3c0d74a032c322))

## Functions Binding
### Features
* Publish Functions Binding as a nuget package ([c7ed2b5](https://github.com/Azure/iotedge/commit/c7ed2b5f6c92ad38bd154fb13c644a5d196899b7))

### Bug Fixes
* N/A

## Temperature Sensor
### Features
* Limit number of messages sent ([d0b2196](https://github.com/Azure/iotedge/commit/d0b219631117fd078a158cbce9abb6c7cf3b031f))

### Bug Fixes
* N/A

# 1.0.3 (2018-10-09)
This a security release of the IoT Edge runtime.

## Edge Agent
### Features
* Update C# SDK to 1.18.1 ([5e1a983](https://github.com/Azure/iotedge/commit/5e1a9836cd55ab3f81c6cf7c9c28018d2ca7f94b))

### Bug Fixes
* N/A

## Edge Hub
### Features
* Update C# SDK to 1.18.1 ([5e1a983](https://github.com/Azure/iotedge/commit/5e1a9836cd55ab3f81c6cf7c9c28018d2ca7f94b))
* Update Protocol Gateway to 2.0.1 ([5e1a983](https://github.com/Azure/iotedge/commit/5e1a9836cd55ab3f81c6cf7c9c28018d2ca7f94b))

### Bug Fixes
* N/A

## iotedged
### Features
* N/A

### Bug Fixes
* N/A

# 1.0.2 (2018-09-21)
* Adds HTTP Proxy support across the various components of the runtime ([956c99f](https://github.com/Azure/iotedge/commit/956c99f11eb293dc2993620aec8f106933dbe09c))

## Edge Agent
### Features
* N/A

### Bug Fixes
* Remove CamelCase property name resolver from json deserializer ([a924608](https://github.com/Azure/iotedge/commit/a924608bcf50c456e5e89108a28d8080c508b611))

## Edge Hub
### Features
* Add support for extended offline (various commits)
* Upgrade device SDK to 1.18.0 ([eeee143](https://github.com/Azure/iotedge/commit/eeee143d3250aebbbda588b631f3056bd3ab1398))
* Improve startup time ([3ac39ac](https://github.com/Azure/iotedge/commit/3ac39ac2c10b2c264c5b6c46a61263e1d0d14759))

### Bug Fixes
* Fix MQTT topic parsing for topics with a trailing slash (DeviceNotFound exception) ([2b09542](https://github.com/Azure/iotedge/commit/2b095422929ebe96885a8b0452483bf1afc0243a))
* `UpstreamProtocol` environment variable values are now case insensitive ([f48c780](https://github.com/Azure/iotedge/commit/f48c780eacfc724d5bf4752a9e6c53e9ae377c6a))
* DotNetty Timeout exceptions are mapped to general timeout exceptions ([45bac36](https://github.com/Azure/iotedge/commit/45bac36450f8821c211554b5c30e4167ec7e5e66))
* Fix potential high-bandwidth usage when SAS tokens expire ([9d2ba5e](https://github.com/Azure/iotedge/commit/9d2ba5e5d7edebf8c8e30b349754a86cb353079d))
* Fix for possible `NullReferenceException` in the `TwinManager` ([0b4ef50](https://github.com/Azure/iotedge/commit/0b4ef5073cbffd1f56d3121d8a8968bcc3517fea))
* Fix twin desired property change notification request handling ([8b1fb67](https://github.com/Azure/iotedge/commit/8b1fb6752a79591391b65c81a20e7bb65431b948))

## iotedged
### Features
* Improved error messages for missing/invalid connection strings in config.yaml ([94621d5](https://github.com/Azure/iotedge/commit/94621d524eddc162a82facaf4f5bdac01afa2bf4))

### Bug Fixes
* Fix volume creation for modules that mount volumes ([0a1a47f](https://github.com/Azure/iotedge/commit/0a1a47f3fb58a16716d58c2cd5372f0a228f7754))
* RPM changes to allow reboot ([8d29056](https://github.com/Azure/iotedge/commit/8d2905689f0d4be40006a1146ef80304efc6bb52))


## Functions Binding
### Features
* Upgrade to v2.0 of the Azure Functions runtime ([1bc69d1](https://github.com/Azure/iotedge/commit/1bc69d1e8b90406818356ab2bbb702444682b428))

### Bug Fixes
* N/A

# 1.0.1 (2018-08-21)

* Updates to license (allow redistribution) and third party notices ([azure/iotedge@9ca6055](https://github.com/azure/iotedge/commit/9ca60553735a27954b1f0345c37b39cbb18554ea))

## Edge Agent
### Features
* Update to .NET Core 2.1.2 ([azure/iotedge@542971](https://github.com/azure/iotedge/commit/54297170077285f06753dd8f590a46925e57d6de))
* Update to C# SDK 1.18.0 ([azure/iotedge@dfc72b5](https://github.com/azure/iotedge/commit/dfc72b5e41cfac066595654be59dfef301cac078))

### Bug Fixes
* Ignore version property when comparing module definitions ([azure/iotedge@2fd4bf1](https://github.com/azure/iotedge/commit/2fd4bf1d9b8e08344a9ec266cd33a9509373822c))
* Fix exception in logs when MQTT is used as upstream protocol ([azure/iotedge@2d6824b](https://github.com/azure/iotedge/commit/2d6824b90f1681801d78ba3e0b8ab47aad1dff6e))
* Reduce noise in the logs for planner failures ([azure/iotedge@29fd10e](https://github.com/azure/iotedge/commit/29fd10e61293e159bc116849e18c5a3a60c1bab9))

## Edge Hub

### Features
* Update to .NET Core 2.1.2 ([azure/iotedge@542971](https://github.com/azure/iotedge/commit/54297170077285f06753dd8f590a46925e57d6de))
* Add option to turn off protocol heads ([azure/iotedge@7a6419a](https://github.com/azure/iotedge/commit/7a6419a5474020eaa5258ac9f34930ca9930d5c6))

### Bug Fixes
* Fix backwards compatibility with iotedgectl ([azure/iotedge@cc7e142](https://github.com/azure/iotedge/commit/cc7e142ae812a4d5d2d22267052cc8602f41b5c3))
* Add `connectionDeviceId` and `connectionModuleId` properties to outgoing messages on AMQP ([azure/iotedge@e636135](https://github.com/azure/iotedge/commit/e6361358f90e344f596d2328ce0cbbae67cf7da7))
* Align direct method response with IoT Hub behavior ([azure/iotedge@539f376](https://github.com/azure/iotedge/commit/539f3760c0396f5f1d787606500cb056db1a159e))
* Prevent connecting to IoT Hub for disconnected clients. Prevents possible tight loop in token refresh ([azure/iotedge@7c77b7f](https://github.com/azure/iotedge/commit/7c77b7f2e970cd1c50ac905232f6a89fbf63317e))
* Align MQTT topic parsing with IoT Hub behavior ([azure/iotedge@b19bbb4](https://github.com/azure/iotedge/commit/b19bbb4a96c35954ebb535def8997f717b5052a4))
* Fixes receiving messages in batches over AMQP ([azure/iotedge@02f193a](https://github.com/azure/iotedge/commit/02f193a027677666c4f5c73dd515a19528554569))
* Increase twin validation limits ([azure/iotedge@2590d7e](https://github.com/azure/iotedge/commit/2590d7e87db3dd0fbd21e15cfa441dfde22f4a52))
* Align AMQP link settle modes with IoT Hub ([azure/iotedge@93f13b8](https://github.com/azure/iotedge/commit/93f13b885977c72ead1671d089e6633d4636650b))

## iotedged

### Features
* Windows installation script ([azure/iotedge@dea9cfc](https://github.com/azure/iotedge/commit/dea9cfc0c4facfdc81b6fabc49f066472817d89c))
* Support older version of systemd ([azure/iotedge@df8d10b](https://github.com/azure/iotedge/commit/df8d10b13355ae0e4f664d05723e5b10139a4ddb))
* Add RPM packages for CentOS/RHEL 7.5 ([azure/iotedge@a090acb](https://github.com/azure/iotedge/commit/a090acb8d7ba6b58e16c1ebb33c8f45698054653))

### Bug Fixes
* Fix internal server error when exec'd into a container ([azure/iotedge@31468a1](https://github.com/azure/iotedge/commit/31468a1ec03d5b2d1077064563db4b853a961eab))
* Module identity delete should return 204, not 200 ([azure/iotedge@2163103](https://github.com/azure/iotedge/commit/21631034f8baac242e321a8314d7a81e4e1ef2aa))
* Ensure modules get new server certificates when requested ([azure/iotedge@5bba698](https://github.com/azure/iotedge/commit/5bba6988569903f453159f528bc7751fdb57aa6a))

## Functions Binding

### Features
* Update to .NET Core 2.1.2 ([azure/iotedge@542971](https://github.com/azure/iotedge/commit/54297170077285f06753dd8f590a46925e57d6de))
* Update to latest Azure Functions runtime on armhf ([azure/iotedge@31ad5be](https://github.com/azure/iotedge/commit/31ad5be5eddff8917c0866509bc72d8e1c07c1f1))
* Update to C# SDK 1.18.0 ([azure/iotedge@dfc72b5](https://github.com/azure/iotedge/commit/dfc72b5e41cfac066595654be59dfef301cac078))
* Binding uses MQTT protocol by default ([azure/iotedge@f0ce4a5](https://github.com/azure/iotedge/commit/f0ce4a52139e583711fd72505327b593af605490))

## Temperature Sensor

## Features
* Update to .NET Core 2.1.2 ([azure/iotedge@542971](https://github.com/azure/iotedge/commit/54297170077285f06753dd8f590a46925e57d6de))
* Update to C# SDK 1.18.0 ([azure/iotedge@dfc72b5](https://github.com/azure/iotedge/commit/dfc72b5e41cfac066595654be59dfef301cac078))

### Bug Fixes
* Allow reset command to be an array of messages ([azure/iotedge@bf5f374](https://github.com/azure/iotedge/commit/bf5f374130931be4a0a164325147de9c171a85ca))

## iotedgectl
* Add deprecation notice

# 1.0.0 (2018-06-27)
Initial release
