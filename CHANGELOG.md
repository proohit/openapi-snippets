# Change Log

All notable changes to the "openapi-snippets" extension will be documented in this file.

## [Unreleased]

- Initial release

## [0.0.1] - 2020-04-17

- initial

## [0.0.2] - 2020-04-17

### Added

- Validation of Schema and Path Item Objects. See [OpenApi Specification v3](https://raw.githubusercontent.com/OAI/OpenAPI-Specification/master/schemas/v3.0/schema.json) for the referenced schema.
- pathput snippet

## [0.0.3] - 2020-04-21

### Added

- schemaObjects and propertyObjects can now be created from selected text
- There is a guide on how to configure keybindings. Checkout [the Readme](./README.md#keybindings)
- Added pathdelete snippet
- added pathgetparam to insert a GET path with parameters

## [0.0.4] - 2020-04-21

### Added

- added pathdeleteparam to insert a DELETE path with parameters
- added pathputparam to insert a PUT path with parameters

## [0.0.5] - 2020-05-03

### Modified

- modified Readme

## [0.0.6] - 2020-05

### Modified

- fixed pathputparam schema tabstop (were doubled)

### Added

- description to responses
- Added ContentType snippet and integration into schemas

### Removed

- default property in schemaObject

## [0.0.7] - 2020-05-20

### Added

- support for yaml files
- yaml validation

### Removed

- operationId properties from path schemas

## [0.0.8] - 2020-07-15

### Modified

- path validation now ignores trailing slash for PathItems
- added yaml extension dependency

## [0.0.9] - 2020-10-30

### Modified

- fixed json paths contentType snippet
- updated descriptions for snippets

### Added

- validation for files inside specific folders without -schema or -path filename
