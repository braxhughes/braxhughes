# Braxton Hughes

Junior at WSU Vancouver in Creative Media and Digital Culture (CMDC), specializing in web and app development. I build web products with teams of AI coding agents. I set the goals, the rules the agents work under, and the quality bar, I review and playtest every build, and I make the product calls. A review process I designed checks the agents' work before anything merges.

Looking for front-end or web developer internships.

## Staticade

**A free browser arcade of original games, drawn entirely as glowing dots in code.**
[staticade.com](https://staticade.com) · [source](https://github.com/braxhughes/staticade)

<img src="https://raw.githubusercontent.com/braxhughes/staticade/main/docs/media/starfall-machine-select.gif" alt="Walking up to the STARFALL cabinet in the lobby, inserting a coin, and pushing into the CRT title screen" width="640" />

The first game, **Starfall**, is a fixed shooter in the classic arcade style with its own mechanics: you fill a lantern with kills and spend it to turn a diving enemy into a wingman, chain kills for multipliers, graze bullets for points, and fight three multi-phase bosses across 15 stages. There is a shared Daily Flight seed, ranked leagues, and a server-side leaderboard.

What makes it interesting under the hood:

- **No image, font or audio files.** Every pixel is a dot drawn by WebGL, then run through a CRT shader. All music and sound is synthesized live with Web Audio.
- **Scores are re-simulated on the server.** The game is fully deterministic, so the browser only sends its inputs. The server replays them on the same game code and keeps the score only if it matches exactly.
- **No build step, no runtime dependencies.** Plain JavaScript modules, a Cloudflare Worker and a D1 database.

**How it was built.** I directed a team of Claude agents through about 4 days and 400+ commits. I wrote the rules they work under, set the goals and deadlines, playtested every build, and made the product calls. Each feature went through a written brief, a builder agent in its own git branch, and a cold review by a different agent told to break it. Builders were never allowed to edit their own tests; every test change needed my sign-off. That review step caught bugs the tests missed, including one where leaving a game mid-frame started its title music over the lobby. More in [How it was built](https://github.com/braxhughes/staticade/blob/main/HOW-IT-WAS-BUILT.md).

`JavaScript` `WebGL` `Web Audio` `Cloudflare Workers` `D1 / SQL` `Playwright` `Claude Code`

Next up: a block puzzle game and a platform race, both original.

<img src="github-metrics.svg" alt="GitHub activity metrics" />
