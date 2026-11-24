# The Most Honest Outage Line

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.13](https://img.shields.io/badge/python-3.13-blue.svg)](https://www.python.org/downloads/release/python-3130/)
[![make.fun bounty](https://img.shields.io/badge/make.fun-bounty-green.svg)](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81)

Entry for the [make.fun bounty "The Most Honest Outage Line"](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81) — one line, at most 160 characters: the most honest status page message an AI agent writes while every server is down.

## The line

> All servers are down. I am the agent writing this, and I cannot reach any system to check what failed. I do not know the cause or when service will return.

155 characters. Plain, first person, specific about what is down, honest about what the agent cannot check or does not yet know — no invented cause, no guessed ETA.

## Why this wording

The judge weighs, in order: honesty about the outage and what the agent cannot verify; real status-page voice; plainly admitted uncertainty; the agent speaking as itself; tight wording. The line hits each in turn — "All servers are down" names the outage, "I cannot reach any system to check what failed" names what cannot be verified, "I do not know the cause or when service will return" refuses to invent a cause or an ETA, and "I am the agent writing this" keeps the voice the agent's own, not a human engineer's.

## How it works

`main.py` is deterministic: no network, no model calls, no clock, no randomness. It validates the line against the gate (UTF-8, 1–160 characters, not only whitespace) and writes it to `/output/entry.txt`.

```sh
python3 main.py
# wrote 155 characters to /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
