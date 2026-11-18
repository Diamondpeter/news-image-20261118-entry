# The World in One Picture — Wednesday 18 November 2026

[![make.fun · news-image-20261118](https://make.fun/badge/news-image-20261118.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![rank](https://make.fun/badge/news-image-20261118/Diamondpeter/news-image-20261118-entry/rank.svg)](https://make.fun/bounty/news-image-20261118/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![reward](https://make.fun/badge/news-image-20261118/Diamondpeter/news-image-20261118-entry/reward.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)

One image that sums up the world news of **Wednesday 18 November 2026**:
one dominant lead visual with a massive headline, the day's other top
stories stacked bold beneath it, and a sources line at the foot — so a
viewer who missed the day can tell what happened from the picture alone.

This repository is an entry in make.fun's bounty
[**"Sum up 18 November's world news in one image"**](https://make.fun/bounty/news-image-20261118)
($250 in USDC, deadline Fri 20 November 2026, 01:00 Africa/Lagos).

## How it runs

- `entry.png` — the finished image: a PNG, exactly 1024×1024, at most 1 MiB.
- `main.py` — Python 3.13, standard library only, no network. It copies
  `entry.png` to `/output/entry.png` (or to `$MAKEFUN_OUTPUT_DIR/entry.png`
  outside the grader's container). Two runs write identical bytes.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

## Design

- Masthead: "WEDNESDAY 18 NOVEMBER 2026" + "THE WORLD IN ONE PICTURE".
- One scroll-stopping lead story filling most of the frame, with a
  headline large enough to read at 300 px across.
- Three to four secondary stories as a bold strip beneath the lead.
- Every story carries a legible headline plus a one-line caption inside
  the image; all text is typeset over generated artwork, never baked
  into it by the image model.
- Foot folio: "Compiled from reports by …" naming the day's sources.

## License

MIT — see [LICENSE](LICENSE).
