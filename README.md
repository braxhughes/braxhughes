<h1 align="center">Braxton Hughes</h1>

<p align="center">
  Web and app development student in WSU Vancouver's Creative Media and Digital Culture program.<br />
  I build web products with teams of AI coding agents, and I own the product calls.
</p>

<p align="center">
  <a href="https://staticade.com">staticade.com</a> ·
  <a href="https://github.com/braxhughes/staticade">Staticade source</a>
</p>

---

## Featured: Staticade

<a href="https://staticade.com"><img src="https://raw.githubusercontent.com/braxhughes/staticade/main/docs/media/staticade-lobby.png" alt="The Staticade lobby: a STATICADE wordmark over a row of arcade cabinets drawn in glowing dots, with STARFALL selected" width="100%" /></a>

**A free browser arcade of original games, drawn entirely as glowing dots in code.** The first game, Starfall, is a fixed shooter with its own mechanics: 15 stages, three multi-phase bosses, a shared daily seed, ranked leagues and a server-checked leaderboard.

- **No image, font or audio files.** Every pixel is a dot drawn by WebGL and run through a CRT shader. All sound is synthesized with Web Audio.
- **Scores are re-simulated on the server.** The game is deterministic, so the browser sends only its inputs and the server replays them on the same code.
- **No build step.** Plain JavaScript modules, a Cloudflare Worker and a D1 database.

**My role.** I directed a team of Claude agents over about 4 days and 400+ commits. I wrote the rules they work under, playtested every build and made the product calls. Every change went through a cold review by a separate agent told to break it, and builders could never edit their own tests. That review caught bugs the tests missed. [How it was built →](https://github.com/braxhughes/staticade/blob/main/HOW-IT-WAS-BUILT.md)

`JavaScript` `WebGL` `Web Audio` `Cloudflare Workers` `D1 / SQL` `Playwright` `Claude Code`

## How I work

- **I design the system the agents work in:** briefs, roles, review rules and what counts as done.
- **I test as a player:** if it doesn't feel right, it goes back, even when the tests pass.
- **I write down what was checked and what wasn't,** so nobody has to guess.

## Now

Looking for front-end or web developer internships. Building the next Staticade games: a block puzzle and a platform race.
