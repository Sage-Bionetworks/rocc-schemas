# Contribution Guide

A big welcome and thank you for considering contributing to this project.

This project is a community effort and lives off your contributions, be it in
the form of bug reports, feature requests, discussions, or fixes and other code
changes.

Reading and following these guidelines will help us make the contribution
process easy and effective for everyone involved. It also communicates that you
agree to respect the time of the developers managing and developing these open
source projects. In return, we will reciprocate that respect by addressing your
issue, assessing changes, and helping you finalize your pull requests.

## Quicklinks

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
    - [Issues](#issues)
    - [Pull Requests](#pull-requests)
    - [Setup Development Environment](#setup-development-environment)
    - [HTML Preview](#html-preview)
    - [Testing](#testing)
- [Release Procedure](#release-procedure)
- [Getting Help](#getting-help)

## Code of Conduct

We take our open source community seriously and hold ourselves and other
contributors to high standards of communication. By participating and
contributing to this project, you agree to uphold our [Code of Conduct].

## Getting Started

Contributions are made to this repo via Issues and Pull Requests (PRs). A few
general guidelines that cover both:

- Search for existing Issues and PRs before creating your own.
- We work hard to makes sure issues are handled in a timely manner but,
  depending on the impact, it could take a while to investigate the root cause.
  A friendly ping in the comment thread to the submitter or a contributor can
  help draw attention if your issue is blocking.

### Issues

Issues should be used to report problems with this project, request a new
feature, or to discuss potential changes before a PR is created. When you create
a new Issue, a template will be loaded that will guide you through collecting
and providing the information we need to investigate.

If you find an Issue that addresses the problem you're having, please add your
own reproduction information to the existing issue rather than creating a new
one. Adding a [reaction] can also help be indicating to our maintainers that a
particular problem is affecting more than just the reporter.

### Pull Requests

PRs to our repositories are always welcome and can be a quick way to get your
fix or improvement slated for the next release. In general, PRs should:

- Only fix/add the functionality in question **OR** address wide-spread
  whitespace/style issues, not both.
- Add unit or integration tests for fixed or changed functionality (if a test
  suite already exists).
- Address a single concern in the least number of changed lines as possible.
- Include documentation in the repo or on our [docs site].
- Be accompanied by a complete Pull Request template (loaded automatically when
  a PR is created).

For changes that address core functionality or would require breaking changes
(e.g. a major release), it's best to open an Issue to discuss your proposal
first. This is not required but can save time creating and reviewing changes.

In general, we follow the [Forking Workflow]:

1. Fork the repository to your own Github account
2. Clone the project to your machine
3. Create a branch locally with a succinct but descriptive name
4. Commit changes to the branch
5. Following any formatting and testing guidelines specific to this repo
6. Push changes to your fork
7. Open a PR in our repository and follow the PR template so that we can
   efficiently review the changes.

We recommend that you add this repository as an [upstream remote] to your local
git repository so that you can fetch the latest updates.

On your local machine make sure you have the latest version of the `main` branch
from this upstream repository:

    git checkout main
    git pull upstream main

### Setup Development Environment

This project relies on Node tools and project-specific commands defined in
[package.json] to streamline the development and testing. The command below will
install the required development tools.

    npm ci

### HTML Preview

The command below builds and serves a preview of the HTML documentation of one
of the APIs defined in this repository:

    npm run start

where `<name>` is the name of one of the API folders included in [openapi/] for
which you want to see the HTML documentation. The HTML page will be available at
http://localhost:8080.

### Testing

Before submitting a PR, please check that the content of the branch that you
plan to submit passes with the tests defined for this project:

    npm run lint
    npm run validate

where `<name>` is the name of the API folder in [openapi/] that you want to
test.

## Release Procedure

Maintainers are required to follow the procedure below when creating a new
release. Releases are created with the npm package [release-it].

1. [Identify whether the release is a major, minor or patch release.]
2. Bump the project version in the files listed below but not in `package.json`
   (updated automatically by `release-it`).
   - `README.md`
   - `openapi/openapi.yaml`
3. Obtain a [personal access token] (release-it only needs "repo" access; no
   "admin" or other scopes).
4. Make sure the token is [available as an environment variable].
5. Preview the release information using one of the commands listed below. These
   commands will not modify any local or remote files.
    - `npm run release -- major --ci --no-npm --dry-run`
    - `npm run release -- minor --ci --no-npm --dry-run`
    - `npm run release -- patch --ci --no-npm --dry-run`
6. Create the release using one of the commands listed below.
    - `npm run release -- major --no-npm --ci`
    - `npm run release -- minor --no-npm --ci`
    - `npm run release -- patch --no-npm --ci`
7. Check that the release has been successfully created on GitHub along with any
   release artifacts that may have been created (GitHub Pages, Docker image
   pushed to Docker registry, Python package published to PyPi, etc.).

## Conventions

### Schemas

- The properties listed below `required:` must be in the same order as below `properties:`.

### Abbreviations

The name of properties must not include abbreviation in general in order to be
fully descriptive. The abbreviations listed below are accepted as exceptions to
this rule.

Short name | Full name | Motivation
-----------|-----------|-----------
Org | Organization | Increase readability of the OpenAPI document.

## Getting Help

Join us on the XXX and post your question to the channel that best matches the
topic of your request.

<!-- Links -->

[Code of Conduct]: CODE-OF-CONDUCT.md
[upstream remote]: https://help.github.com/en/articles/configuring-a-remote-for-a-fork
[reaction]: https://github.blog/2016-03-10-add-reactions-to-pull-requests-issues-and-comments/
[Forking Workflow]: https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow
[package.json]: ../package.json
[openapi/]: ../openapi/
[release-it]: https://github.com/release-it/release-it
[Identify whether the release is a major, minor or patch release.]: https://semver.org/#summary
[personal access token]: https://github.com/settings/tokens/new?scopes=repo&description=release-it
[available as an environment variable]: https://github.com/release-it/release-it/blob/master/docs/environment-variables.md