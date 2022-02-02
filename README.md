# ROCC OpenAPI Specification

[![GitHub Release](https://img.shields.io/github/release/Sage-Bionetworks/rocc-schemas.svg?include_prereleases&color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/Sage-Bionetworks/rocc-schemas)
[![GitHub CI](https://img.shields.io/github/workflow/status/sage-bionetworks/rocc-schemas/ci.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/sage-bionetworks/rocc-schemas)
[![GitHub License](https://img.shields.io/github/license/sage-bionetworks/rocc-schemas.svg?color=94398d&labelColor=555555&logoColor=ffffff&style=for-the-badge&logo=github)](https://github.com/sage-bionetworks/rocc-schemas)

## Introduction

TBA

### Latest

- https://sage-bionetworks.github.io/rocc-schemas/latest/docs/
- https://sage-bionetworks.github.io/rocc-schemas/latest/openapi.yaml
- https://sage-bionetworks.github.io/rocc-schemas/latest/openapi.json

### Edge

- https://sage-bionetworks.github.io/rocc-schemas/edge/docs/
- https://sage-bionetworks.github.io/rocc-schemas/edge/openapi.yaml
- https://sage-bionetworks.github.io/rocc-schemas/edge/openapi.json

## Specification

- ROCC schemas version: 0.6.0

## Requirements

- [Node] >=14

## Implementations

### Service

GitHub repository                               | Language
------------------------------------------------|---------
[Sage-Bionetworks/rocc-service]                 | Python

### Web Client

GitHub repository                               | Language
------------------------------------------------|---------
[Sage-Bionetworks/rocc-app]                     | TypeScript-Angular

### Client Libraries

GitHub repository                               | Language
------------------------------------------------|---------
[Sage-Bionetworks/rocc-client-angular]          | TypeScript-Angular
[Sage-Bionetworks/rocc-client-python]           | Python

## Usage

### `npm start`

Starts the reference docs preview server.

### `npm run build`

Bundles the definition to the dist folder.

### `npm test`

Validates the OpenAPI specification.

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

[Node]: https://nodejs.org/en/
[Sage-Bionetworks/rocc-service]: https://github.com/Sage-Bionetworks/rocc-service
[Sage-Bionetworks/rocc-app]: https://github.com/Sage-Bionetworks/rocc-app
[Sage-Bionetworks/rocc-client-angular]: https://github.com/Sage-Bionetworks/rocc-client-angular
[Sage-Bionetworks/rocc-client-python]: https://github.com/Sage-Bionetworks/rocc-client-python
[semantic versioning]: https://semver.org/
[contribution guidelines]: .github/CONTRIBUTING.md
[Apache License 2.0]: https://github.com/Sage-Bionetworks/rocc-schemas/blob/main/LICENSE
