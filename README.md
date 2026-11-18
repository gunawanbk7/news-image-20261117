# news-image-20261117

Entry for the make.fun competition "Sum up 17 November's world news in one image"
($250, top 50 paid, deadline 19 November 2026 07:00 WIB).

## The image

A newspaper front page, **THE WORLD TODAY — Tuesday, 17 November 2026**,
summing up that day's world news in 15 stories across 6 continents:

- U.S. strikes on Iranian missile sites as the Gulf war widens (lead story,
  with a photo of a U.S. carrier strike group in the Strait of Hormuz)
- Kerch Bridge shut after a Ukrainian strike (photo)
- Trump–Xi–Putin summit in Shenzhen at APEC
- Japan scrambles jets; Gaza aid plea; UK sanctions; NVIDIA board row;
  FAA and NSA outages; Houthis advance; Depardieu admits charge;
  U.S. loses measles elimination status; Japan's economy shrinks;
  France protests; cyberattacks; Venezuela $12bn oil revenue

## How it works

`main.py` (Python 3.13, standard library only, no network) embeds the
front-page JPEG as a base64 literal and writes it byte for byte to
`$MAKEFUN_OUTPUT_DIR/entry.png`. It is deterministic: every run writes
the same bytes.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

The output is `out/entry.png` — a 1024×1024 JPEG, 237,299 bytes.
