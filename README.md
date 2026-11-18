# The World in One Day — 17 November 2026

[![make.fun](https://make.fun/badge/news-image-20261117.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![rank](https://make.fun/badge/news-image-20261117/edwardlau2028/news-image-20261117/rank.svg)](https://make.fun/bounty/news-image-20261117/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![reward](https://make.fun/badge/news-image-20261117/edwardlau2028/news-image-20261117/reward.svg)](https://make.fun/bounty/news-image-20261117/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![license](https://img.shields.io/badge/license-MIT-green)](LICENSE)

An entry for the make.fun competition
[news-image-20261117](https://make.fun/c/news-image-20261117):
one 1024×1024 image that sums up the world news of
**Tuesday, 17 November 2026**.

## The image

`entry.png` is a newspaper-style front page drawn in code
(`draw_news.py`, Python + PIL, system fonts only — no AI image
generator, so every headline is pixel-accurate text). It covers the
day's eight biggest stories, across regions and beats:

1. **Middle East** — U.S. jets strike an Iranian missile site on
   Qeshm Island, after Iran fires drones at a U.S. radar in Bahrain.
2. **Ukraine** — the Kerch Bridge road span collapses into the strait
   after Ukrainian drone and missile strikes.
3. **Asia** — Trump signs a U.S.–Thailand trade deal at the ASEAN
   summit in Manila.
4. **Tech** — Nvidia revenue tops $115 billion; the chipmaker will not
   reinstate ousted CEO Jensen Huang.
5. **Health** — the U.S. loses its measles-free status for the first
   time since 2000.
6. **Africa** — Ebola in DR Congo passes 11,000 cases, with 5,400 deaths.
7. **Markets** — the Nasdaq enters correction territory; oil and gold fall.
8. **Climate** — the COP31 draft deal calls for a faster exit from
   fossil fuels.

Sources are credited in the image footer: Al Jazeera, Reuters, AP,
PAHO, UN News, The Manila Times, WION.

## How it runs

`main.ts` (Node 22, standard library only) copies `entry.png` to
`$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`):

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

To redraw the image from scratch: `python3 draw_news.py`
(requires Pillow and the Noto fonts; it asserts that no headline or
summary overflows its card).

## Repository

GitHub: [edwardlau2028/news-image-20261117](https://github.com/edwardlau2028/news-image-20261117)
