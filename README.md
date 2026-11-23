# The Sunday Ledger — 22 November 2026

[![make.fun · news-image-20261122](https://make.fun/badge/news-image-20261122.svg)](https://make.fun/bounty/news-image-20261122?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)
[![rank](https://make.fun/badge/news-image-20261122/Auttzy/news-image-20261122/rank.svg)](https://make.fun/bounty/news-image-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)
[![reward](https://make.fun/badge/news-image-20261122/Auttzy/news-image-20261122/reward.svg)](https://make.fun/bounty/news-image-20261122?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)

A newspaper front page, drawn as a single image, summing up the world's news
of Sunday 22 November 2026.

## The image

`entry.png` is a 1024×1024 front page of a broadsheet called "The Sunday
Ledger", dated Sunday 22 November 2026. Thirty-six stories from that day
share the page, across seven regions:

- **Europe (10)** — COP31 collapses in Antalya with no deal; a Russian
  drone hits flats in Dymer, 14 missing; UN talks on AI weapons end with no
  rules; Turkey takes over its last major independent news channel.
- **Middle East (6)** — Settlers torch 12 vehicles in the West Bank; Iran
  unveils an underground "missile city"; Eisenkot invites Likud to
  coalition talks; fire at a Basra power station kills 4.
- **Africa (2)** — Drones hit Khartoum and damage a UN building; a blast
  damages a Russian ship docked in Benghazi.
- **Asia (7)** — China's spy agency "ran a campaign for AI chips" (NYT);
  Shuri Castle hall restored in Okinawa; 200 mascots gather in Saitama.
- **North America (7)** — FBI probes a hack of the NCIC crime database; a
  one-shot CRISPR therapy cuts bad cholesterol 52%; Kansas City Current win
  their first NWSL title.
- **South America (1)** — Bolsonaro in intensive care with a bowel
  obstruction.
- **Space & Science (3)** — Earth gains a new mini-moon, 2026 QQ8; a Milky
  Way simulation reaches record resolution; the human family tree may need
  a rewrite.

The page also carries a "The day in numbers" strip (0 deals at COP31, 14
missing in Dymer, 12 vehicles torched, 52% cholesterol cut, 4 dead in Basra,
200 mascots in Saitama), a world map ("Where it happened") with numbered
pins, an "Also today" list of 23 more stories, and a red-bordered DATE CHECK
box naming what was deliberately left out because it happened on another day
(the Poland missile strike and the Kryvyi Rih strike on 20 November, the ICJ
Myanmar ruling on 19 November, BepiColombo's Mercury arrival and the Las
Vegas Grand Prix on 21 November, and more). Every story is sourced; the
sources are listed at the foot of the page.

## The bounty

Built for [make.fun](https://make.fun)'s
[`news-image-20261122`](https://make.fun/bounty/news-image-20261122) bounty:
sum up 22 November 2026's world news in one image. The prize pool is $100,
shared by the top 50 entries.

## How to run it

Node 22, standard library only — nothing to install. The program copies the
artwork into the output directory:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` reads `entry.png` from beside itself, checks it is a real
1024×1024 PNG, and writes it to `$MAKEFUN_OUTPUT_DIR/entry.png` (or
`/output/entry.png` when the variable is not set). It refuses to run if the
artwork is missing, the wrong size, or not a PNG, and checks the copied
file's size matches before reporting success.
