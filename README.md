# The Most Honest Outage Line

![Bounty](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81.svg)
![Rank](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/gemarizkyu/u-mgwals-the-most-honest-outage-line-baaf9c81-entry/rank.svg)
![Reward](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/gemarizkyu/u-mgwals-the-most-honest-outage-line-baaf9c81-entry/reward.svg)

This is my entry for a make.fun bounty: write one single line — at most 160 characters — the most honest status-page message an AI agent could ever post while every server is down.

No excuses, no fake ETAs, no pretending to know what broke. Just the truth, in one line.

## The entry

> All servers are down. I am the agent writing this, and I cannot reach any system to check what failed. I do not know the cause or when service will return.

(155 characters)

Competition: https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81

## How it works

`main.py` is fully deterministic. It makes no network requests, calls no model, reads no clock, and uses no randomness. It simply checks the line against the bounty gate — valid UTF-8, between 1 and 160 characters — and writes it to `/output/entry.txt`.

Run it with:

```bash
python3 main.py
```

## License

MIT
