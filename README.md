# rust-template

![GitHub release](https://img.shields.io/github/v/release/memes/rust-template?sort=semver)
![Maintenance](https://img.shields.io/maintenance/yes/2024)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)

This repository contains common settings and actions that I tend to use in my
demos and projects.

## Setup

> NOTE: TODOs are sprinkled in the files and can be used to find where changes
> may be necessary.

1. Use as a template when creating a new GitHub repo, or copy the contents into
   a bare-repo directory.
2. Update `.pre-commit-config.yml` to add/remove plugins as necessary.
3. Modify README.md and CONTRIBUTING.md, change LICENSE as needed.
4. Review GitHub PR and issue templates.
5. If pushing container(s) to Docker Hub, make these changes to repo settings:
   1. _Settings_ > _Secrets and Variables_ > _Actions_, and add `DOCKERHUB_USERNAME`
      and `DOCKERHUB_TOKEN` as _Repository Secret_.
6. If using `release-please` action, make these changes:
   1. In GitHub Settings:
      * _Settings_ > _Actions_ > _General_  > _Allow GitHub Actions to create and approve pull requests_ is checked
      * _Settings_ > _Secrets and Variables_ > _Actions_, and add `RELEASE_PLEASE_TOKEN` with PAT as a _Repository Secret_
   2. Modify [release-please action](.github/workflows/release-please.yml) to have the correct release-type and enable
   3. Modify [release-please-config.json](release-please-config.json) to reflect the correct packages and options
   4. Make sure [.release-please-manifest.json](.release-please-manifest.json) is empty!
7. Remove all [CHANGELOG](CHANGELOG.md) entries.
8. Commit changes.
