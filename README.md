<img src="https://readme-typing-svg.demolab.com/?font=Georgia&size=25&duration=3200&pause=1000&color=1E4B3A&vCenter=true&width=640&height=52&lines=Local-first+software.;No+account%2C+no+server.;Tools+that+know+when+to+be+quiet." alt="Local-first software. No account, no server. Tools that know when to be quiet." />

# Braxton Hughes

WSU Vancouver CS student learning and building at the frontier of AI and software
development.

One thread runs through all of it: software that stays on your own machine, keeps quiet
until it has something worth saying, and ships the tests that guard the promise.

[![Contribution activity](https://github-readme-activity-graph.vercel.app/graph?username=braxhughes&theme=minimal&bg_color=fbf9f6&color=17150f&line=1e4b3a&point=a8501f&area=true&hide_border=true)](https://github.com/braxhughes)

---

## Now building

**MOSS** — a local-first daily dashboard. Calendar, money, meals, news, email, and notes
on one screen, with no account and no server: the data sits in a SQLite database on your
own machine, encrypted on disk with SQLCipher if you set a profile password. In public
beta.

`TypeScript` `Electron` `React` `SQLite`

**A macOS menu-bar app** — in development, not released.

**A production site template** — Astro, static HTML, zero client-side JavaScript, on
Cloudflare Pages. Turning it into a new client site is one config file and about thirty
minutes.

`Astro` `TypeScript` `Cloudflare Pages`

---

## Shipped and public

### [agent-bell](https://github.com/braxhughes/agent-bell) · MIT

Sound alerts for Claude Code: a rising tone when an agent needs you, a settled one when
it finishes. The two events get different sounds because they mean different things — a
rising tone asks something of you, a settled one reports. After a day you stop hearing
them as sounds and start hearing them as *go* and *done*.

Ships as a Claude Code plugin, so the hooks come with it and your `settings.json` is
never touched.

```
/plugin marketplace add braxhughes/agent-bell
/plugin install agent-bell@braxhughes
```

`Shell` — one command to mute

### [claude-pool](https://github.com/braxhughes/claude-pool) · MIT

A read-only status line: it prints one line of text and advises, and it cannot switch,
authenticate, or manage anything. What it does that the other eighty or so status lines
don't is check whether switching would even help — before naming a destination it compares
the `accountUuid` of sibling `~/.claude-*` config directories against the current session,
and when they match it says *wrap up*, because two directories signed into one account are
one five-hour rate-limit pool rather than two.

```
[acct1] Opus 5 · myapp:main · ctx 18% · 5h 24%used resets 2h29m
```

It can never break your session: unparseable input, missing fields, and absent rate
limits all print nothing and exit 0. There are tests that assert exactly that, because
the promise is the whole product.

```sh
git clone https://github.com/braxhughes/claude-pool.git
cd claude-pool && ./install.sh
```

`Shell` — terminal CLI only, since the desktop app and the VS Code extension ignore
`statusLine` entirely. The usage figures need a Claude Pro or Max subscription; on an API
key you still get model, project, and context, just no percentages.

### [mossprint](https://github.com/braxhughes/mossprint) · MIT · public beta

[![release](https://img.shields.io/github/v/release/braxhughes/mossprint?include_prereleases&label=release&style=flat&labelColor=17150f&color=1e4b3a)](https://github.com/braxhughes/mossprint/releases/latest)
[![last commit](https://img.shields.io/github/last-commit/braxhughes/mossprint?label=last%20commit&style=flat&labelColor=17150f&color=1e4b3a)](https://github.com/braxhughes/mossprint/commits)
[![license](https://img.shields.io/github/license/braxhughes/mossprint?label=license&style=flat&labelColor=17150f&color=1e4b3a)](https://github.com/braxhughes/mossprint/blob/main/LICENSE)

The public repository for MOSS. Every release ships installers you can download and run:
`.dmg` for Apple silicon and Intel, `.exe` for Windows, `.deb` and `.AppImage` for Linux.

[**Download the latest release →**](https://github.com/braxhughes/mossprint/releases/latest)

---

## Reach me

- **Email** — [Braxtonaodha@proton.me](mailto:Braxtonaodha@proton.me)
- **LinkedIn** — [braxton-hughes-469b64284](https://linkedin.com/in/braxton-hughes-469b64284)
