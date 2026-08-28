# MINDR4CER RADIO

A six-channel web radio programmed from a personal vinyl collection.

Each channel is a curated run of records, streamed via the YouTube IFrame Player API.
No build step, no dependencies — one static HTML file.

## Stations

| CH | Station | Programming |
|----|---------|-------------|
| 01 | Kosmos | Baltic cosmic synth, Estonian library & folk-electronics |
| 02 | Deep House Church | DJ Sprinkles ↔ Detroit — Sound Signature, KDJ, Comatonse |
| 03 | Dub Techno Chamber | Deepchord, Gas, Basic Channel lineage |
| 04 | Kankyō | Japanese environmental music & the Music From Memory orbit |
| 05 | Spiritual Jazz & Library | Modal & spiritual jazz, Brazilian instrumental |
| 06 | Deep Dubstep | Deep Medi / Hyperdub / Skull Disco |

## Features

- Play/pause, skip, shuffle, volume
- Video-hide toggle for background listening
- Clickable queue per station
- Remembers your last station via `localStorage`
- Auto-skips region-blocked or removed videos

## Running it

Needs to be served over http(s) — the YouTube player rejects a `file://` origin.

```bash
python3 -m http.server 8777
```

Then open http://localhost:8777

## Note

This page hosts no audio. It embeds publicly available YouTube uploads through the
official IFrame Player API. Support the artists and labels — buy the records.
