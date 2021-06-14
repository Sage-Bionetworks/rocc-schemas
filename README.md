# Registry of Open Community Challenges Schemas

[![GitHub Release](https://img.shields.io/github/release/Sage-Bionetworks/rocc-schemas.svg?include_prereleases&color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/Sage-Bionetworks/rocc-schemas)
[![GitHub CI](https://img.shields.io/github/workflow/status/sage-bionetworks/rocc-schemas/ci.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/sage-bionetworks/rocc-schemas)
[![GitHub License](https://img.shields.io/github/license/sage-bionetworks/rocc-schemas.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/sage-bionetworks/rocc-schemas)

The OpenAPI specification implemented by Challenge Registries.

## Introduction

TBA

## Specification

- ROCC schemas version: 0.1.4

## Requirements

- [Node] >=14

## ROCC Services

GitHub repository                               | Language
------------------------------------------------|---------
[Sage-Bionetworks/rocc-service]                 | Python

## ROCC Clients

GitHub repository                               | Language
------------------------------------------------|---------
[Sage-Bionetworks/rocc-client-angular]          | TypeScript-Angular
[Sage-Bionetworks/rocc-client-python]           | Python

## Working on your OpenAPI Definition

### Install

1. Install [Node JS](https://nodejs.org/).
2. Clone this repo and run `npm install` in the repo root.

## Usage

### `npm start`

Starts the reference docs preview server.

### `npm run build`

Bundles the definition to the dist folder.

### `npm test`

Validates the definition.

## Versioning

### GitHub release tags

This repository uses [semantic versioning] to track the releases of the NLP
Sandbox schemas. This repository uses "non-moving" GitHub tags, that is, a tag
will always point to the same git commit once it has been created.

### Schemas / GitHub Pages tags

The artifact published by this repository are OpenAPI schemas and documentation
published to GitHub Pages. The versions of the schemas are aligned with the
GitHub tags of this repository. For example:

- https://sage-bionetworks.github.io/rocc-schemas/latest/docs/
- https://sage-bionetworks.github.io/rocc-schemas/latest/openapi.yaml
- https://sage-bionetworks.github.io/rocc-schemas/latest/openapi.json

The table below describes the schemas tags available.

| Tag name                        | Description                                            | Moving
|---------------------------------|--------------------------------------------------------|-------
| `latest`                        | Latest stable release.                                 | Yes
| `edge`                          | Lastest commit made to the default branch.             | Yes
| `edge-<sha>`                    | Same as above with the reference to the git commit.    | No
| `<major>.<minor>.<patch>`       | Latest stable patch release `<major>.<minor>.<patch>`. | No

## Contributing

Thinking about contributing to this project? Get started by reading our
[contribution guidelines].

## License

[Apache License 2.0]

<!-- Links -->

[Sage-Bionetworks/rocc-service]: https://github.com/Sage-Bionetworks/rocc-service
[Sage-Bionetworks/rocc-client-angular]: https://github.com/Sage-Bionetworks/rocc-client-angular
[Sage-Bionetworks/rocc-client-python]: https://github.com/Sage-Bionetworks/rocc-client-python
[semantic versioning]: https://semver.org/
[contribution guidelines]: .github/CONTRIBUTING.md
[Apache License 2.0]: https://github.com/Sage-Bionetworks/rocc-schemas/blob/develop/LICENSE
