# Git repository rules

## Table of contents

- [Repository naming](#repository-naming)
- [Git branch rule](#git-branch-rule)
- [Coding style guide](#coding-style-guide)
- [Versioning rule](#versioning-rule)
- [Git repositories management](#git-repositories-management)

## Repository naming

**Repository directory**

- Repository Directory should be divided into a release directory and a non-release directory
- The release directory is to be deployed from its release branch
- The non-release directory contains sample code

**Repository name**

- all in lowercase
- project prefix-module name
  - arc-auth

**Readme file**

- All the repositories in the release directory should contain readme files in markup language format
  - Dependencies
  - Configurations
  - How to compile and build
  - How to deploy (preferably docker)

## Git branch rule

- See [Git flow guide](git-flow-guide.md)

## Coding style guide

- [Google Style Guides](https://google.github.io/styleguide/)
- [Developer portal coding standard](https://pretia.atlassian.net/wiki/spaces/SD/pages/1962508395)

| Language | Convention |
| --- | --- |
| C++ | [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html) |
| Html / CSS | [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html) |
| C# | [Microsoft Style](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions) |
| Golang | [Golang Style](https://github.com/golang/go/wiki/CodeReviewComments) / [GoFmt](https://golang.org/cmd/gofmt/) |

## Versioning rule

> [!TIP]
> Reference: [Semantic Versioning 2.0.0](https://semver.org/)

- Version numbers for the release can be maintained as: MAJOR.MINOR.PATCH,
  - MAJOR version when you make incompatible API changes
  - MINOR version when you add functionality in a backward-compatible manner
  - PATCH version when you make backward-compatible bug fixes.

## Git repositories management

### Context

The company makes the repository rules, and we need senior developers and above to follow the rules and make sure everyone in every project is compliant with the rules.

### Responsibility

- Review the naming conventions
  - The repository naming: The repository name should be consistent across all company projects or by divisions.
  - The repository branch naming: The repository name should be consistent across all company projects, by divisions, by functional teams, or by projects.
- Branch management
  - All the active branches should be valid within 3 months, older than 3 months would be considered garbage and should be removed (merged, archived, or deleted)
  - Branch synchronization: If there is any branch out-of-sync for too long, we should have someone to put it back to in-sync or remove it.
- Commit rules compliance should be consistent across all the company projects
- The coding convention should be consistent across all the company projects
