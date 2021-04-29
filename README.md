# Standards

This is the org-wide repository that contains the labs3 standards. These are standards mainly regarding code style for organisation projects. They are not enforced, only recommendended.

## Current list of (potential) standards

* L3S-01.md - Clarity coding standard
* L3S-02.md - Architecture model standard
* L3S-03.md - Unit testing standard

## Naming

### Standard naming

Standards are named in the format `L3S-XX` where `XX` is the standard identifier. This identifier changes incrementally.

## Release naming

### Tags

If the release is a pre-release (an alpha or beta), the tag will be the next available version number with the suffix of `alpha` or `beta`.

A standard is in `alpha` until it is finalised and `beta` until it's implemented in an L3 project.

After the pre-release is implemented by a project, the pre-release becomes a recognised release without the suffix.

Example:

Previous release was `v4`...
`v5-alpha`, `v5-beta` and then `v5`.

### Title

The title of a release is usually a reference from one of Neal Stephenson's writings. This could be a city, a book title, a character etc. It's free for the author to choose. Just don't be rude, or it won't be implemented. They should be unique org-wide.

Example:

`A Young Lady's Illustrated Primer`

### Name

A release's name is the abbreviation of the title, a forward-slash and the release tag.

Example:

`EOC/v1`

## Implementing standards

When implementing deployed standards from this repo, you should state implementation in the following ways:

If you're using a *release*, where you comply with every standard in said release, you should say something like this...

> This project complies with [AYLIP/v2](https://github.com/labs3/standards/releases/tag/v2).

- Make it clear
- The release name should be the abbreviation of the title, a forward-slash and the release tag.
- Link the release name to the release link from this repo
- You can put the release title in brackets after if wanted.

If you're using *individual standards*, you should list them.

> This project complies with L3S-01, 02 & 03.
