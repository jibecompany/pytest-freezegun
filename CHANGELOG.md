# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.4.3] - 2022-06-29
### Fixed
- Fixed warning due to usage of distutils.
### Added
- Add support for Python 3.9.

## [0.4.2] - 2020-07-19
### Fixed
- Work with pre-release pytest versions, by [chandlernine](https://github.com/chandlernine), with a different implementation proposed by [Aly Sivji](https://github.com/alysivji).
- Marking a test with `freeze_time` should freeze time in fixtures, even if the `freezer` fixture is also used explicitly late in the fixture list. Thanks to [Christian Grossmüller](https://github.com/chgad) for pointing out the problem.

## [0.4.1] - 2020-02-02
### Added
- Support for class-based tests, by [Richard Terry](https://github.com/radiac).
- Registering the `freeze_time` mark, thanks to [Dima Tisnek](https://github.com/dimaqq), [Craig Anderson](https://github.com/craiga) and [Richard Terry](https://github.com/radiac). This was in really high demand. 
- Tests for Python 3.7 and 3.8.
- Tests for pytest 5.
- And a PyPI badge, thanks to [Andreu Vallbona Plazas](https://github.com/avallbona).

### Removed
- Support for Python before 3.5 (including 2.7), implemented by [Nicolas Delaby](https://github.com/ticosax).
  Those versions are getting hard to test on CI.

## [0.3.0.post1] - 2018-11-22
### Changed
- Build universal wheels, to support Python 2 and 3. Thanks to [Oliver Bristow](https://github.com/Code0x58) for pointing out I've forgot about Python 2.

## [0.3.0] - 2018-11-15
### Added
- Support for pytest 3.6+, including 4.0. Thanks to [Oliver Sauder](https://github.com/sliverc) and [Nate Parsons](https://github.com/nsp).

### Removed
- Support for freezegun 0.3.0 (it might still work, but is not tested anymore)
- Support for Python 3.3 (it might still work, but is not tested anymore)
