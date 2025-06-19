slidenumbers: true
footer: Carlos Becker - Codecon Experience 2025
slide-transition: fade(0.5)
theme: Plain Jane
slide-dividers: #

# [fit] Building GoReleaser

## [fit] from a shell script to a paying product

# $ whoami

Carlos Alexandro Becker

- `@caarlos0` most places
- works `@charmbracelet`
- maintains `@goreleaser`
- [`caarlos0.dev`](https://caarlos0.dev)

![fit right](https://carlosbecker.com/carlos-and-bash.png)

# Agenda

1. The lore behind it
1. What I learned
1. Future

# The Lore

# June, 2015

- I was working on another project I had
- Created a [`release.sh`](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)
- Few days later: [added more stuff to it](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)

# March, 2016

- Moved that script into its [own repository](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)
- I needed to use it in more repositories

# December, 2016

- "I need Homebrew"
- "It'll suck to do that with bash..."
- "Gonna make this a Go project!"
- And so [I did](https://github.com/goreleaser/goreleaser/commit/8b63e6555be45234c4c2a69576ca2ddab705302c)!
- Posted it on `/r/golang` and Twitter

# 2017

- Kept adding features to it
- Using it in all my projects
- Meetups
- > 1k stars

# 2018

- > 1k public repositories using it
- More meetups
- OpenCollective
- Talk about it at _Gophercon Brazil_
- Refactor the core to allow to add more languages

# 2019

- > 5k stars
- Talks about a v1
- Burnout

# 2020

## whatever the f✱ck happened here

# 2021

- Talk about it at the _GoTime_ Podcast
- Launched **GoReleaser Pro**
- Works on supply chain integrity (cosign, SBOMs, etc)
- Launched **v1.0.0!** 🎉
- Proper release announcements

# 2022

- GitHub Sponsors
- > 10k stars
- > 1k commits

# 2023

- Release cadence slowed down
- Pro gets old version support
- > 12k stars

# 2024

- Launched **v2.0.0** 🎉
- Rust and Zig support!
- > 14k stars

# 2025

- Bun, Deno, Poetry, and UV support
- Talk about it at _Cup o' Go_ and _Fallthrough_ Podcasts
- More support for desktop apps
- ~200 customers
- Talk about it at _Codecon Experience_ 🙃

# What I learned

# GoReleaser is boring software

And boring is _good_, actually.

Boring is _predictable_.

Turns out people want _predictable_ when releasing their software.

And most people don't want to work on boring things.

Which is why _GoReleaser Pro_ sells.

# Naming things is hard

I didn't think about it _at all_ 🫣

- "it releases Go binaries, its GoReleaser"
- "gore leaser"
- mix up with `gorelease` (without the `r`)
- doesn't sound like it supports more languages

# _die Welt ist ein Dorf_

Because of GoReleaser, I got to meet a lot of amazing people, got invited into events, got job opportunities...

People will also try to take advantage of you and your product platform.

The world is indeed a village.

**Be nice.**

# Luck

People like to brag it's all them - and they have their credit, for sure, but luck also plays in subtle but important ways.

# Original marketing x OSS

- Anything goes
- It's all _vibes_
- See HTMX on X for example

# Enterprise plans should be expensive

- **So. Much. Paperwork.**
- They ask a lot about you, your product, and your processes
- It makes sense to charge extra, as you'll spend hours filling this stuff

# Timing

- Should probably have made the Pro version earlier
- Should probably have added more languages earlier
- Should probably have changed the license early, now I probably never gonna

# Future

- Support more languages and distribution channels
-
