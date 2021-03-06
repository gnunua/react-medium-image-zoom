# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [3.0.1] - 2017-10-20

### Fixed
- Now supporting keyboard interaction for accessibility (https://github.com/rpearce/react-medium-image-zoom/issues/70). Classified this as a bug and therefore a patch version.

## [3.0.0] - 2017-10-13

### Added
- support for React v16, making use of such things as its portals concept

### Removed
- support for React < v16

## [2.0.3] - 2017-09-22

### Fixed
- `shouldRespectMaxDimension` was allowing images that were already rendered at their maximum size to be "zoomed," thus creating the issue where they don't _actually_ zoom and instead just moved to the center of the screen.

## [2.0.2] - 2017-09-21

### Fixed
- Fixed undefined method call (underscore was missing...c'mon eslint)
- Fixed original image not staying hidden until unzoom is complete

## [2.0.1] - 2017-09-21

### Added
- Dev: eslint & prettier for code formatting and double-dhecking

## [2.0.0] - 2017-09-21

### Added
- Changelog (so meta...)
- When in controlled mode (`isZoomed` is provided), the `onUnzoom` callback will fire when the component normally would have closed

### Changed
- Differentiation between controlled & uncontrolled modes (when `isZoomed` is passed vs letting component control itself)

### Removed
- Removed preload functionality

### Fixed
- Support for the component immediately zooming if `isZoomed={true}` is provided on mount
