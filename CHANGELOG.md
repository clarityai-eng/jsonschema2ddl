# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0](https://github.com/clarityai-eng/jsonschema2ddl/releases/tag/0.2.0) - 2021-03-25

### Added

- Feat: use the `format` parameter in jsonschema to determine date and datetime types.

## [0.1.2](https://github.com/clarityai-eng/jsonschema2ddl/releases/tag/0.1.2) - 2021-03-22

### Changed

- Feat: preserve order in columns definitions
- Chore: Update pipelines with dry run option

## [0.1.1](https://github.com/clarityai-eng/jsonschema2ddl/releases/tag/0.1.1) - 2021-03-17

### Changed

- Chore: Migrate from travis to github actions
- Feat: Accept null as column type with lowest priority

## [0.1.0](https://github.com/clarityai-eng/jsonschema2ddl/releases/tag/0.1.0) - 2020-10-26

This is the first release of the jsonschema2ddl repo. This project is a direct fork from the original.

In this first we don't include major changes in functionality but there is a good amount of code refactor that will make this project more maintainable.

### Added

- feat: Don't drop the schema when creating the tables by default. A new parameter is introduced to do so.
- feat: Provide options to select whether to drop the tables if exists and with cascade or not.
- feat: Provide an option to autocommit the changes in the schema creation.
- feat: Validate jsonschema before launching the migrations

### Changed

- feat: Code is organized in a more object oriented model structure for easy extensibility and mantainability.
- tests: Use testscontainers to be able to tests the postgres inserts
- chore: Use poetry for dependency and publishing
- chore: Provide Makefile for development
- chore: More elaborate travis.ci to be able to push based on tags
- chore: Change the project structure for the company python standars
- docs: Use different docs structure
