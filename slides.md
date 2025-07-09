slidenumbers: true
footer: Carlos Becker - Codecon Summit 2025
slide-transition: fade(0.5)
theme: Plain Jane

# [fit] Building GoReleaser

## [fit] from shell script to paid product

![](./presentation2.png)

---

# $ whoami

Carlos Alexandro Becker

- `@caarlos0` most places
- works `@charmbracelet`
- maintains `@goreleaser`
- [`caarlos0.dev`](https://caarlos0.dev)

![fit right](./carlos-and-bash.png)

---

# Agenda

1. What is GoReleaser
1. The Lore
1. Lessons learned
1. The Future

---

# GoReleaser

- Release automation tool
- Build, package, publish, announce
- Configurable in a single `.yaml` file
- Nudges you into doing the _right thing_
- Supports Go, Rust, Zig, Python, and TypeScript
- [goreleaser.com](https://goreleaser.com)

![fit right](./goreleaserfundo.png)

---

# The Lore

![](./presentation2.png)

---

## 2015: The beginning

- I was working on one of my Go projects
- Created a [`release.sh`](https://github.com/getantibody/antibody/commit/5d06dae0c78d1655fc243183f96d8a0a7a3cc197)
- Unassuming
- Similar to many others out there

![fit right](much.png)

---

## 2016: Rewrite in Go

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

---

## 2017: Spreading the word

- Kept adding features to it
- Wife drew the mascot/logo
- Using it in all my projects
- Meetups
- \>1k stars

![fit right](./goreleaserfundo.png)

---

## 2018: Burning out

- nFPM
- \>1k public repositories using it
- OpenCollective
- More meetups, _Gophercon Brazil_
- Core now supports multiple languages, but didn't add any 🤦‍♂️
- Burnout

^ if you constantly ask yourself whether you are burn out or not, it might be worth checking it. Also, if your partner says you work too much, they probably right

---

## 2019 & 2020: Recovering and COVID

- Recovering from burnout
- Started talking about launching a v1.0.0
- \>5k stars

^ exercise, cut alcohol, eat clean, lower social media usage

---

![](./wth.gif)

---

## 2021: We are SO back!

- _GoTime_ Podcast
- **GoReleaser Pro**
- **v1.0.0!** 🎉
- Proper release announcements
- GitHub Sponsors

---

## 2022: Full-time open source

- Working at Charm, doing OSS all day long
- Split & Merge, `--nightly`, AUR
- \>10k stars

---

## 2023: More professional

- Release calendar
- Ko, health check, upx, nix, Winget
- \>12k stars

---

## 2024: At last, multiple languages

- Launched **v2.0.0** 🎉
- Rust and Zig support!
- DMG, MSI, macOS notary, App Bundles,
- \>14k stars

![right](./mascots.png)

---

## 2025: Moving forward

- Bun, Deno, Poetry, and UV support
- AI changelog, MCP server, NPM, Casks
- _Cup o' Go_ and _Fallthrough_ Podcasts
- Better support for desktop apps
- ~200 customers and ~15k stars
- _Codecon Summit_ 🙃

---

# Lessons learned

![](./presentation2.png)

---

## Boring software

_Boring is good_, actually.

Boring is _predictable_.

Turns out people want _predictability_ instead of _novelty_ when releasing their software.

---

## Distribution

Really hard, unless you are a _tech influencer_.

Making good stuff, having a good READMEs, with some cool artwork, helps.

---

## Naming things is hard

- "it releases Go binaries, its GoReleaser"
- "gore leaser"
- mix up with `gorelease` (without the `r`)
- the **Go** prefix

---

## Pricing

- Harder than pricing physical products
- Guess based on what you know
- Enterprises usually expect overcharging
- Legalese, forms, etc

---

## Licensing

- MIT is probably too permissive
- Changing later might feel like bait-and-switch
- Consider changing it earlier rather than later

---

## Flexibility, Simplicity, and finding balance

- I love flexible software
- It leads to madness
- I hate flexible software
- Scope creep, accidental complexity
- "it depends"

![right 140%](./seen-things.gif)

---

## Building products

- Starting from an existing problem will give you better chances of succeeding
- Side projects for fun and studying are still good though!

---

# The Future

![](./presentation2.png)

---

## The future

- Support more languages and distribution channels
- Improve docs, error messages, etc
- tl;dr keep working on it

---

![](./thanks.gif)

---

# Links

- [caarlos0.dev](https://caarlos0.dev)
- [goreleaser.com](https://goreleaser.com)
- [github.com/caarlos0/codecon-2025](https://github.com/caarlos0/codecon-2025)
