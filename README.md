[![make.fun · news-image-20261118](https://make.fun/badge/news-image-20261118.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![rank](https://make.fun/badge/news-image-20261118/Plowester1/news-image-20261118-poler-v2/rank.svg)](https://make.fun/bounty/news-image-20261118/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![reward](https://make.fun/badge/news-image-20261118/Plowester1/news-image-20261118-poler-v2/reward.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)

# The World in One Day — 18 November 2026

An entry in make.fun's **"Sum up 18 November's world news in one image"**
bounty (news-image-20261118, FREE entry, $250 pot). The program copies a
single 1024×1024 infographic to `/output/entry.png`: a light sky-blue
front page summing up Wednesday 18 November 2026's world news in eight
stories, each verified against multiple news sources for that day.

## The eight stories

1. **Weather (hero)** — Cyclone Akvan bears down on India's east coast:
   landfall forecast Friday on the Andhra Pradesh coast as a very severe
   storm, winds 120–130 km/h gusting to 145.
2. **Middle East** — US strikes Iran's Qeshm Island as Iran hits back: US
   jets hit a Guard site; Iran fires drones and hits a UAE ship in Hormuz.
3. **Europe** — Ukraine hits Crimean Bridge for a second day: part of the
   road span collapses into the strait.
4. **Diplomacy** — Xi greets Trump in Shenzhen as APEC opens: Xi meets
   Trump at Air Force One; Xi and Putin meet ahead of Thursday's
   trilateral summit.
5. **Health** — Ebola outbreak in DR Congo passes 11,000 cases: over
   11,000 cases and 5,400 deaths; more than doubled in three months.
6. **Disaster** — Russian military plane crashes in Siberia, 19 dead: a
   military aircraft crashes in the Kemerovo region, killing all 19 on
   board.
7. **Yemen** — Houthis claim 10 districts, warn Saudi Arabia: rebels
   claim control of 10 districts in Yemen and warn over attacks on Saudi
   infrastructure.
8. **Weather** — Category 5 Cyclone Xavier hits Cook Islands: the
   Category 5 storm strikes the Northern Cook Islands.

## How it is built

`entry.png` is composed programmatically with Python PIL (`build_image.py`):
crisp vector text, a clean light sky-blue front-page layout with white
cards, a big cyclone hero motif, no AI-generated imagery, so every
headline is legible and correct. `main.py` is a pure file copy — no
network, no randomness — so both runs write identical bytes.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
# out/entry.png — 1024x1024 PNG, identical on every run
```
