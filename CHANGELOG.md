# Changelog
All notable changes to `laravel-dag-manager` will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Changed
- ...

## [v1.0.0] - 2021-01-02
### Added
- Make table name configurable
- Add property/argument/return types
- Supports PHP 8
- Tests via Github Actions

### Removed
- Redundant doc-blocks

### Changed
- Make code more strict
- Migrate phpunit configuration
- Make service provider deferrable

## [v0.10.0] - 2020-09-09
### Added
- Laravel 8.0 support

## [v0.9.1] - 2020-08-08
###Fixed
- Corrected error reading from configuration.

## [v0.9.0] - 2020-08-08
###Added
- Introduced a way to configure the database connection for the dag_edges table.

## [v0.8.0] - 2020-07-31
###Added
- Introduced a dagRelationsOf scope to get all relations, eg both ancestors and descendants

## [v0.7.0] - 2020-03-04
### Added
- Laravel 7.0 support

### Removed
- support for anything less/older than Laravel 6.0

## [v0.6.0] - 2020-02-06
### Changed
- `IsDagManaged` scopes now accept an array of model IDs

## [v0.5.0] - 2020-02-04
### Added
- scopes enforce minimum `$maxHops` value

## [v0.4.0] - 2020-01-28
### Added
- added helpful messages to the two exception classes

## [v0.3.0] - 2020-01-07
### Added
- added `$maxHops` optional parameter to `IsDagManaged` trait's `descendantsOf` and `ancestorsOf` scopes

## [v0.2.0] - 2019-10-28
### Added
- `IsDagManaged` trait now has `ancestorsOf` scope

### Removed
- order and distinct on `IsDagManaged` trait's `descendantsOf` scope

## [v0.1.1] - 2019-09-17
### Changed
- Now supporting Laravel 6.0.
- Updated phpunit version.

## [0.1.0] - 2019-03-15
### Added
- Updated the requirements section in [README](README.md) to include minimum PHP version.

### Changed
- Minor documentation update/clean-up.
- Now supporting Laravel 5.7 and 5.8.
- Updated phpunit version.
- Now using unsigned big integer fields in `dag_edges` table.

## [0.0.7] - 2018-05-18
### Added
- Introduced an Eloquent model trait, `Telkins\Dag\Models\Traits\IsDagManaged` to assist in some basic, helpful functionality for "DAG managed" models.

## [0.0.6] - 2018-05-09
### Fixed
- Corrected migration filename error.  Third time's the charm...?!

## [0.0.5] - 2018-05-09
### Fixed
- Corrected copy/paste filename error related to migration filename and publishing.

## [0.0.4] - 2018-05-09
### Added
- Introduced the ability to publish the migration and updated [README](README.md) accordingly.

### Changed
- Updated the credits section in [README](README.md).

## [0.0.3] - 2018-05-04
### Added
- Introduced some new tests for adding/deleting using different sources.
- Added implicit requirements for Illuminate DB and Support dependencies.
- Update minimum PHP and Laravel requirements to 7.1.3 and 5.6, respectively.

### Changed
- Indexed `dag_edges.source`.

### Fixed
- Fixed a minor section title error in [README](README.md).

## [0.0.2] - 2018-05-03
### Added
- Basic usage section in [README](README.md).
- Installation section content in [README](README.md).
- Warning section in [README](README.md).

## 0.0.1 - 2018-05-03
### Added
- Basic add/remove functionality.
- A set of tests.
- Minimal documentation.

[Unreleased]: https://github.com/telkins/laravel-dag-manager/compare/v0.10.0...HEAD
[1.0.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.10.0...v1.0.0
[0.10.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.9.1...v0.10.0
[0.9.1]: https://github.com/telkins/laravel-dag-manager/compare/v0.9.0...v0.9.1
[0.9.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.8.0...v0.9.0
[0.8.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.7.0...v0.8.0
[0.7.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.6.0...v0.7.0
[0.6.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.5.0...v0.6.0
[0.5.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.4.0...v0.5.0
[0.4.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.3.0...v0.4.0
[0.3.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.1.1...v0.2.0
[0.1.1]: https://github.com/telkins/laravel-dag-manager/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/telkins/laravel-dag-manager/compare/v0.0.7...v0.1.0
[0.0.7]: https://github.com/telkins/laravel-dag-manager/compare/v0.0.6...v0.0.7
[0.0.6]: https://github.com/telkins/laravel-dag-manager/compare/v0.0.5...v0.0.6
[0.0.5]: https://github.com/telkins/laravel-dag-manager/compare/v0.0.4...v0.0.5
[0.0.4]: https://github.com/telkins/laravel-dag-manager/compare/v0.0.3...v0.0.4
[0.0.3]: https://github.com/telkins/laravel-dag-manager/compare/v0.0.2...v0.0.3
[0.0.2]: https://github.com/telkins/laravel-dag-manager/compare/v0.0.1...v0.0.2
