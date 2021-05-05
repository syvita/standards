# Standards

This is the org-wide repository that contains Syvita standards. These are standards mainly regarding code style for Guild projects. They are not enforced, only recommendended.

## Current list of (potential) standards

* Syv-01.md - Clarity coding standard
* Syv-02.md - Architecture model standard
* Syv-03.md - Unit testing standard
* Syv-04.md - Markdown standard

## Naming

### Standard naming

Standards are named in the format `Syv-XX` where `XX` is the standard identifier. This identifier changes incrementally.

A standard is in `alpha` phase until it is finalised and `beta` phase until it's implemented in a Standard Release.

### Release naming

Standard Releases are groups of `Syv-XX` standards launched as versions.

They follow the form `SyvR-vX` where `X` is the next available integer version.

Example:

`SyvR-v4` (Standard Release v4)

### Tags

Releases are released as `vX`s where `X` is the next available integer version.

Example:

Previous release was `v4` so next will be `v5`.

## Implementing standards

When implementing deployed standards from this repo, you should state implementation in the following ways:

If you're using a *release*, where you comply with every standard in said release, you should say something like this...

> This project complies with [SyvR-v4](https://github.com/labs3/standards/releases/tag/v4).

* Make it clear
* The release name should be the abbreviation of the title, a forward-slash and the release tag.
* Link the release name to the release link from this repo

If you're using *individual standards*, you should list them.

> This project complies with Syv-01, 02 & 03.
