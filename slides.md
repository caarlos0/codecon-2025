slidenumbers: true
footer: Carlos Becker - Codecon Summit 2025
slide-transition: fade(0.5)
theme: Plain Jane
slide-dividers: #

# [fit] Building GoReleaser

## [fit] from shell script to paid product

# $ whoami

Carlos Alexandro Becker

- `@caarlos0` most places
- works `@charmbracelet`
- maintains `@goreleaser`
- [`caarlos0.dev`](https://caarlos0.dev)

![fit right](https://carlosbecker.com/carlos-and-bash.png)

# Agenda

1. What is GoReleaser
1. The Lore
1. Lessons learned
1. The Future

# GoReleaser

- Release automation tool
- Build, package, publish, announce
- Configurable in a single `.yaml` file
- Nudges you into doing the _right thing_
- Supports Go, Rust, Zig, Python, and TypeScript
- [goreleaser.com](https://goreleaser.com)

![fit right](https://raw.githubusercontent.com/goreleaser/artwork/refs/heads/master/goreleaserfundo.png)

# The Lore

# June, 2015

- I was working on one of my Go projects
- Created a [`release.sh`](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)
- Unassuming
- Similar to many others out there

![fit right](much.png)

# March, 2016

- I now have a dozen of Go projects
- All of them need releasing
- Moved that script into its [own repository](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)
- Configuration via `--flags`
- It sucked, but scratched the itch

# December, 2016

- Doing OSS during holidays
- "I need Homebrew"
- "It'll suck to do that with bash..."
- "Gonna make this into a Go project!"
- Shared it on `/r/golang` and Twitter, got some traction

# 2017

- Kept adding features to it
- Using it in all my projects
- Meetups
- > 1k stars

# 2018

- nFPM
- > 1k public repositories using it
- More meetups
- OpenCollective
- _Gophercon Brazil_
- Refactor the core to support multiple languages

# 2019

- Started talking about launching a v1.0.0
- > 5k stars
- Burnout

# 2020

![inline](./wth.gif)

# 2021

- _GoTime_ Podcast
- **GoReleaser Pro**
- Supply chain integrity (cosign, SBOMs)
- **v1.0.0!** 🎉
- Proper release announcements
- GitHub Sponsors

# 2022

- > 10k stars
- > 1k commits

# 2023

- Release calendar
- Release announcements
- > 12k stars

# 2024

- Launched **v2.0.0** 🎉
- Rust and Zig support!
- > 14k stars

# 2025

- Bun, Deno, Poetry, and UV support
- _Cup o' Go_ and _Fallthrough_ Podcasts
- Better support for desktop apps
- ~200 customers
- _Codecon Summit_ 🙃

# Lessons learned

# GoReleaser is boring software

And _boring is good_, actually.

Boring is _predictable_.

Turns out people want _predictable_ when releasing their software.

Incidentally, most people don't want to work on boring things. 💵

# Naming things is hard

- "it releases Go binaries, its GoReleaser"
- "gore leaser"
- mix up with `gorelease` (without the `r`)
- locked in to the tech

# _"die Welt ist ein Dorf"_

Because of GoReleaser, I got to meet and chat with a lot of amazing people.

Who you know matters a lot more than I thought back then.

The world is indeed a village - **be nice.**

# Enterprise plans should be expensive

- **So. Much. Paperwork.**
- They ask a lot about you, your product, and your processes
- It makes sense to charge extra, as you'll spend hours filling this stuff
- Most of it doesn't matter in our specific case, they ask anyway

# Things I would have done differently

- Launched multiple languages back in 2018
- Created the Pro version earlier, circa 2019
- Both these would have lead me to:
  - Change the license in time
  - Change the name before being so well known

# The hacker way

- Solve the problem you already have instead of
  finding a problem for the solution you want to implement
- Try to think like a product manager
- Flexibility needs to be intentional
- Simple is good, but it's not easy

^ User should be able to start without reading dozens of docs

# The Future

- Support more languages
- Support more distribution channels
- tl;dr keep working on it

# Thanks!

![inline](./thanks.gif)

# Links

- [caarlos0.dev](https://caarlos0.dev)
- [goreleaser.com](https://goreleaser.com)
- [github.com/caarlos0/codecon-2025](https://github.com/caarlos0/codecon-2025)
