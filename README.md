# Standards

This is the org-wide repository that contains the labs3 standards. These are standards mainly regarding code style for organisation projects.

## Naming

### Standard naming

Standards are named in the format `L3S-XX` where `XX` is the standard identifier. This identifier changes incrementally.

## Release naming

### Tags

If the release is a pre-release (an alpha or beta), the tag will be the next available version number with the suffix of `alpha` or `beta`.
After the pre-release is implemented by a project, the pre-release becomes a recognised release without the suffix.

Example:

Previous release was `v4`...
`v5-alpha`, `v5-beta` and then `v5`.

### Title

The title of a release is usually a reference from one of Neal Stephenson's writings. This could be a city, a book title, a character etc. It's free for the author to choose. Just don't be rude, or it won't be implemented.

Example:

`A Young Lady's Illustrated Primer`

### Name

A release's name is the abbreviation of the title, a forward-slash and the release tag.

Example:

`AYLIP/v1-beta`

## Implementing standards

When implementing deployed standards from this repo, you should state implementation in the following ways:

If you're using a *release*, where you comply with every standard in said release, you should say something like this...

> This project complies with [AYLIP/v1]().

- Make it clear
- The release name should be the abbreviation of the title, a forward-slash and the release tag.
- Link the release name to the release link from this repo
- You can put the release title in brackets after if wanted.

If you're using *individual standards*, you should list them.

> This project complies with L3S-01, 02 & 03.
