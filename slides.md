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

# 2015: The beginning

- I was working on one of my Go projects
- Created a [`release.sh`](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)
- Unassuming
- Similar to many others out there

![fit right](much.png)

# 2016: Rewrite in Go

- I now have a dozen of Go projects
- Moved that script into its [own repository](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)
- Doing OSS during holidays, needed more features
- Rewrote it in Go
- Shared it on `/r/golang` and Twitter

^ All of them need releasing
Configuration via `--flags`
It sucked, but scratched the itch
"I need Homebrew"
"It'll suck to do that with bash..."
"Gonna make this into a Go project!"

# 2017: Spreading the word

- Kept adding features to it
- Wife drew the mascot/logo
- Using it in all my projects
- Meetups
- \>1k stars

# 2018: Burning out

- nFPM
- \>1k public repositories using it
- OpenCollective
- More meetups, _Gophercon Brazil_
- Refactor the core to support multiple languages
- Burnout

# 2019 & 2020: Recovering and COVID

- Recovering from burnout
- Started talking about launching a v1.0.0
- \>5k stars

---

![inline](./wth.gif)

# 2021: We are SO back!

- _GoTime_ Podcast
- **GoReleaser Pro**
- **v1.0.0!** 🎉
- Proper release announcements
- GitHub Sponsors

# 2022: Full-time open source

- Working at Charm, doing OSS all day long
- \>10k stars
- \>1k commits

# 2023: More professional

- Release calendar
- Release announcements
- \>12k stars

# 2024: At last, multiple languages

- Launched **v2.0.0** 🎉
- Rust and Zig support!
- \>14k stars

# 2025: Moving forward

- Bun, Deno, Poetry, and UV support
- _Cup o' Go_ and _Fallthrough_ Podcasts
- Better support for desktop apps
- ~200 customers and ~15k stars
- _Codecon Summit_ 🙃

# Lessons learned

# Boring software

_Boring is good_, actually.

Boring is _predictable_.

Turns out people want _predictable_ when releasing their software.

# Distribution

You can game it a little bit, but luck still plays a big role.

Good README, some art/screenshots helps.

# Naming things is hard

- "it releases Go binaries, its GoReleaser"
- "gore leaser"
- mix up with `gorelease` (without the `r`)
- locked in to the tech

# _"die Welt ist ein Dorf"_

Because of GoReleaser, I got to meet and chat with a lot of amazing people.

Who you know matters a lot more than I thought back then.

# Enterprise plans should be expensive

- **So. Much. Paperwork.**
- They ask a lot about you, your product, and your processes
- It makes sense to charge extra, as you'll spend hours filling this stuff
- Most of it doesn't matter in our specific case, they ask anyway

# Licensing

- MIT is probably too permissive
- If you plan to monetize, mind the license

# Flexibility

The more flexible, the crazier it gets.

TODO: more

# Simplicity

Scope creeps into every project that lives long enough.

TODO: more

# Building products

Solve the problem you already have instead of finding a problem for the
solution you thing would be fun to implement.

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
