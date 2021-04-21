# standard
# Contributing

Merging a PR in this repository (or pushing a commit to `master`) will automatically build and publish a new version

## Versions

This project uses semver-style version naming. By default the deploy process will [increment](https://github.com/marketplace/actions/automated-version-bump) the "patch" version number. You can change which version gets incremented using the following keywords (case sensitive)

- Major version: `[MAJOR]` (or `[Major]` or `[major]`)
- Minor version: `[MINOR]` (or `[Minor]` or `[minor]`)
- Patch version (default): `[PATCH]` (or `[Patch]` or `[patch]`)
- Release version: `[RELEASE]` (or `[Release]` or `[release]`)
- Release version: `[CANDIDATE]` (or `[Candidate]` or `[candidate]`)

Most changes should bump the patch version, or last decimal place (i.e. 1.1.9 -> 1.1.10). If you're adding a new service, that should most likely be the minor version, or middle decimal (i.e. 1.1.1 -> 1.2.1). Restructuring how the directory/schema works or removing a type should be a major version change, increasing the first number (i.e. 1.1.1 -> 2.1.1).
