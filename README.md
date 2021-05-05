# Standards

This is the org-wide repository that contains Syvita standards. These are standards mainly regarding code style for Guild projects. They are not enforced, only recommendended.

## Current list of (potential) standards

* Syv-01.md - Clarity coding standard
* Syv-02.md - Architecture model standard
* Syv-03.md - Unit testing standard

## Naming

### Standard naming

Standards are named in the format `Syv-XX` where `XX` is the standard identifier. This identifier changes incrementally.

## Release naming

### Tags

If the release is a pre-release (an alpha or beta), the tag will be the next available version number with the suffix of `alpha` or `beta`.

A standard is in `alpha` until it is finalised and `beta` until it's implemented in an Syvita project.

After the pre-release is implemented by a project, the pre-release becomes a recognised release without the suffix.

Example:

Previous release was `v4`...
`v5-alpha`, `v5-beta` and then `v5`.

### Name

A release's name is the abbreviation of the title, a forward-slash and the release tag.

Example:

`SyvR-v1` (Syvita standard Release v1)

## Implementing standards

When implementing deployed standards from this repo, you should state implementation in the following ways:

If you're using a *release*, where you comply with every standard in said release, you should say something like this...

> This project complies with [Syv-03/v2](https://github.com/labs3/standards/releases/tag/v2).

- Make it clear
- The release name should be the abbreviation of the title, a forward-slash and the release tag.
- Link the release name to the release link from this repo
- You can put the release title in brackets after if wanted.

If you're using *individual standards*, you should list them.

> This project complies with Syv-01, 02 & 03.
