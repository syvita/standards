# Standards

This is the org-wide repository that contains the labs3 standards. These are standards mainly regarding code style for organisation projects.

## Naming

### Standard naming

Standards are named in the format `L3S-XX` where `XX` is the standard identifier. This identifier changes incrementally.

## Release naming

### Tags

If the release is a pre-release (an alpha or beta), the tag will be the next available version number with the suffix of `alpha` or `beta`.
After the pre-release is implemented by a project, the pre-release becomes a recognised release without the suffix.

Examples:

Previous release was `v4`...
`v5-alpha`, `v5-beta` and then `v5`.

### Title

The title of a release is usually 



## Implementing standards

When implementing deployed standards from this repo, you should state implementation in the following ways:

If you're using a recognised release, where you comply with every standard in said release, you should say something like this

> This project complies with [L3S v1]

- Make it clear
- Link the release name to the release link from this repo

If you're using a pre-release, where you comply with every standard in said release, you should say something like this:

> This project complies with [AYLIP/v1-beta (A Young Lady's Illustrated Primer)](https://github.com/labs3/standards/releases/tag/v1-beta)

If you're using 1-3 standards from here, you should list them as following.

> This project complies with L3S-01, 02 & 03.

