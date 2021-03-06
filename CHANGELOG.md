# Unitwise Changelog

All notable changes to Unitwise will be documented in this file, starting at
version 1.0.0.

Unitwise uses semantic versioning.

## 1.0.4 - 2015-01-10

- Added Ruby 2.2 support.
- Empty strings are no longer valid units.

## 1.0.3 - 2014-10-05

### Added
- Unitwise.valid? for checking validity of expressions

## 1.0.2 - 2014-09-14

### Fixed
- Decomposer caching is now a little smarter. This resulted in a mild
  performance increase.

## 1.0.1 - 2014-08-30

### Fixed
- Move conditional dependencies to Gemfile in order to allow proper
  installation issues on rbx and jruby.

## 1.0.0 - 2014-08-25

### Added
- Uniwise() now accepts a Unitwise::Measurement as the first argument.
- Unitwise::Measurement now supports #round.

### Fixed
- Respect Rationals when inspecting/printing a Unitwise::Measurement.
- Dynamically created methods from unitwise/ext now work with #respond_to?
  and #methods appropriately.

### Deprecated
- Unitwise() and Unitwise::Measurement.new() now requires two non-optional
  arguments (value and unit).
- Unitwise::Measurement no longer has an implicit Integer conversion.
