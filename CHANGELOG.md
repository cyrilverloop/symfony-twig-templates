# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased
### Added
- `base` : a `preloads` block.

## [2.0.1] - 2023-12-10
### Fixed
- "twig/twig" missing dependency.

## [2.0.0] - 2023-12-05
### Added
- "composer.lock".

### Fixed
- "symfony/asset" missing dependency.

### Removed
- Compatibility with Symfony <7.0.

## [1.1.2] - 2022-08-05
### Fixed
- `base` : locales like `en_GB` are automaticaly converted into `en-GB` in order to keep W3C validation.

## [1.1.1] - 2021-03-02
### Fixed
- `base` : the meta description placeholder could not be defined through the `metaDescription` variable.

## [1.1.0] - 2021-03-01
### Added
- A `layout` template.
- The documentation.

## [1.0.0] - 2021-02-25
### Added
- A `base` template.
