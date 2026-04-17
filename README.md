# Supermetrics Homebrew Tap

## What is Homebrew?

Package manager for macOS (or Linux), see more at https://brew.sh

## What is a Tap?

A third-party (in relation to Homebrew) repository providing installable
packages (formulae) on macOS and Linux.

See more at https://docs.brew.sh/Taps

## How do I install packages from here?

```sh
brew install supermetrics-public/tap/name
```

You can also only add the tap which makes formulae within it
available in search results (`brew search` output):

```sh
brew tap supermetrics-public/tap
```

Note: to clone the tap via SSH you will need to use:

```sh
brew tap supermetrics-public/tap https://github.com/supermetrics-public/homebrew-tap
```

While you may search across taps, it is necessary to always use
fully qualified name (incl. the `supermetrics-public/tap/` prefix)
when refering to formulae in external taps such as this one
outside of search.

## What packages are available?

With the following commands, you can install the latest generally available (GA) version of each product:
```sh
# Formulae
brew install supermetrics-public/tap/supermetrics
```

Prereleases (including as alpha's, beta's, and release candidates) could be available in this tap.

## Why should I install packages from this tap?

Formulae for the same Supermetrics software may exist in other taps
or the [community-maintained main tap](https://github.com/Homebrew/homebrew-core).
This may raise a question of why would someone prefer one tap over the other.

The _community-maintained tap_ compiles Supermetrics software on Homebrew's own infrastructure, and builds it according to the local formulae definition.

Formulae _in this tap_ are maintained by Supermetrics, which means that it distributes
the exact binaries Supermetrics releases.

 - Updating of formulae is automated, which means that updates become available as they're released.

### Why doesn't Supermetrics maintain formulae in the `homebrew-core` (main tap)?

Homebrew's core team prefers to keep `homebrew-core` as community maintained and built from source to maintain consistency across vendors in terms of expectations around contents and updates. See [relevant discussion](https://discourse.brew.sh/t/maintenance-of-formulas-by-vendor/7649) for more information.

## Contributing

Check out our [contribution guidelines for this project](./CONTRIBUTING.md)
