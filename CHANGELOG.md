# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.3] - 2025-02-24

### Added
- Add support for authn-jwt
  [cyberark/conjur-api-python#50](https://github.com/cyberark/conjur-api-python/pull/50)

## [0.1.2] - 2024-08-01

### Security
- Update python dependencies

## [0.1.1] - 2024-03-14

### Added
- Add proxy parameter for http requests to Conjur (ONYX-48020)

### Security
- Upgrade ubuntu base image in Dockerfile.test to 23.04
  [conjur-api-python#41](https://github.com/cyberark/conjur-api-python/pull/41)
- Upgrade aiohttp and cryptography (CONJSE-1841, CONJSE-1844)

## [0.1.0] - 2023-02-14

### Added
- Add support for Role Memberships endpoint
  [conjur-api-python#30](https://github.com/cyberark/conjur-api-python/pull/33)
- Add support for Check Privilege endpoint
  [conjur-api-python#34](https://github.com/cyberark/conjur-api-python/pull/34)
- Add support for Show Role endpoint
  [conjur-api-python#30](https://github.com/cyberark/conjur-api-python/pull/30)
- Add `role_exists` method
  [conjur-api-python#35](https://github.com/cyberark/conjur-api-python/pull/35)
- Add support for Show Resource endpoint
  [conjur-api-python#31](https://github.com/cyberark/conjur-api-python/pull/31)
- Add `resource_exists` method
  [conjur-api-python#32](https://github.com/cyberark/conjur-api-python/pull/32)
- Add support for LDAP authentication
  [conjur-api-python#22](https://github.com/cyberark/conjur-api-python/pull/22)
- Supplying api token manually is now supported
  [conjur-api-python#19](https://github.com/cyberark/conjur-api-python/pull/19)
- Add support for OIDC authentication
  [conjur-api-python#19](https://github.com/cyberark/conjur-api-python/pull/19)
- Add support for enabling and disabling of an authenticator
  [conjur-api-python#19](https://github.com/cyberark/conjur-api-python/pull/19)
- Add support for creating hosts using host factory with provided annotations
  [conjur-api-python#19](https://github.com/cyberark/conjur-api-python/pull/19)
- The `get_server_info` method is now available in SDK. It is only supported against Conjur enterprise server
  [conjur-api-python#19](https://github.com/cyberark/conjur-api-python/pull/19)

### Changed
- Include system truststore certs even if cert_file config is present
  [conjur-api-python#37](https://github.com/cyberark/conjur-api-python/pull/37)
- Abstract authentication flow into new `AuthenticationStrategyInterface`
  [conjur-api-python#20](https://github.com/cyberark/conjur-api-python/pull/20)
- Store API key in `CreditentialsData` object
  [conjur-api-python#23](https://github.com/cyberark/conjur-api-python/pull/23)

[Unreleased]: https://github.com/cyberark/conjur-api-python/compare/v0.1.1...HEAD
[0.1.1]: https://github.com/cyberark/conjur-api-python/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/cyberark/conjur-api-python/releases/tag/v0.1.0
