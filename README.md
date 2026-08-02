

## Now building

**MOSS** — a local-first daily dashboard. Calendar, money, meals, news, email, and notes
on one screen, with no account and no server: the data sits in a SQLite database on your
own machine, encrypted on disk with SQLCipher if you set a profile password. In public
beta.

<sub>TypeScript · Electron · React · SQLite</sub>

**A macOS menu-bar app** — in development, not released.

**A production site template** — Astro, static HTML, zero client-side JavaScript, on
Cloudflare Pages. Turning it into a new client site is one config file and about thirty
minutes.

<sub>Astro · TypeScript · Cloudflare Pages</sub>

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

<sub>Pure shell · one command to mute</sub>

### [claude-statusline](https://github.com/braxhughes/claude-statusline) · MIT

The Claude Code status line plus the one number it's missing: how much of your five-hour
usage pool is gone, and whether it's time to switch accounts — before you hit the wall
mid-task, not after.

```
[acct1] Opus 5 · myapp:main · ctx 18% · 5h 24%used resets 2h29m
```

It can never break your session: unparseable input, missing fields, and absent rate
limits all print nothing and exit 0. There are tests that assert exactly that, because
the promise is the whole product.

```sh
git clone https://github.com/braxhughes/claude-statusline.git
cd claude-statusline && ./install.sh
```

<sub>Pure shell · backs up your settings before writing</sub>

### [mossprint](https://github.com/braxhughes/mossprint) · MIT · public beta

The public repository for MOSS. Every release ships installers you can download and run:
`.dmg` for Apple silicon and Intel, `.exe` for Windows, `.deb` and `.AppImage` for Linux.

[**Download the latest release →**](https://github.com/braxhughes/mossprint/releases/latest)

---

## Reach me

- **Email** — [Braxtonaodha@proton.me](mailto:Braxtonaodha@proton.me)
- **LinkedIn** — [braxton-hughes-469b64284](https://linkedin.com/in/braxton-hughes-469b64284)
