# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.2] - 2020-08-28

### Fixed
- Fixed an issue where inline code blocks were not detected if placed after a
  fenced code block.

## [1.0.1] - 2019-07-25

### Changed
- Change ProcessWire version requirement in composer.json to 3.0.0 or later.

## [1.0.0] - 2019-07-07

### Added
- Added the composer.json file.

### Changed
- Added support for literal three backticks by replacing groups of six backticks
  with HTML entities.

## [0.1.0] - 2018-11-08

### Changed
- Better handling for <br> tags at the start of a fenced code block; avoid
  extraneous line breaks at the beginning of the resulting code block.
- Avoid accidentally creating nested code blocks when a single backtick is
  placed within an existing code block (including fenced code blocks).
- README.txt renamed as README.md.
