# Parameter Golf — Experiment Lab

**Interactive dashboard visualizing 793+ scored submissions from the [OpenAI Parameter Golf](https://github.com/openai/parameter-golf) competition ($1M prize pool).**

> **Disclaimer:** This dashboard is not affiliated with, endorsed by, or officially associated with OpenAI, RunPod, or the Parameter Golf competition organizers. It is solely an independent attempt by one participant to document, visualize, and analyze data from a public open-source competition. All data is sourced from publicly available GitHub pull requests. TTT legality classifications are our best interpretation of the current rules and may not be 100% accurate.

## Live Dashboard

**[View the live dashboard →](https://nathanmaine.github.io/parameter-golf-experiment-lab/)**

## What's Inside

- **Community Leaderboard** — 793+ submissions ranked by BPB, searchable and filterable by status, size compliance, TTT legality, and record eligibility
- **TTT Legality Filtering** — Classifications based on [issue #402](https://github.com/openai/parameter-golf/issues/402) rulings: Legal, Illegal (multi-epoch TTT), Suspect (n-gram cache exploits)
- **Record Eligible Filter** — Legal + Open + Under 16MB: the realistic competition leaderboard
- **Score Timeline** — BPB progression chart across 95+ personal experiments
- **Experiment Log** — 95+ runs across 13 pods, 5 regions, with full config, timing, and outcome data
- **Technique Matrix** — What worked (SLOT, Vocab 4096, Brotli-11), what didn't, and what got banned
- **Cost Analysis** — ~$360 across 13 RunPod pods, broken down by session with efficiency metrics
- **Pod Comparison** — GPU benchmarks across pods (up to 802 TFLOPS in Reykjavik, Iceland)
- **Key Discoveries** — Timeline of insights from 15 days of competition

## Current Best Results

| PR | BPB | Technique | Status |
|---|---|---|---|
| [#1291](https://github.com/openai/parameter-golf/pull/1291) | **1.0925** (3-seed mean) | Vocab4096 + MLP4.0x + SLOT | Submitted |
| [#1287](https://github.com/openai/parameter-golf/pull/1287) | **1.1048** (3-seed mean) | Vocab4096 + MLP4.0x (no TTT/SLOT) | Submitted |

Both beat the merged SOTA of 1.1147 (PR #1019). No n-gram cache, no multi-epoch TTT.

## Data Sources

- `submission.json` files from 1,315+ public pull requests (793 with valid BPB scores)
- PR metadata (author, title, date, status) from GitHub API
- Personal experiment logs from 13 RunPod sessions across 5 regions
- Organizer comments and rulings from GitHub issues #402 and #677

## Related

- **[RunPod GPU Benchmark](https://github.com/NathanMaine/runpod-gpu-benchmark)** — 30-second script to find the fastest GPU pod before training
- **[OpenAI Parameter Golf](https://github.com/openai/parameter-golf)** — The competition repo
- **[Discussion Post](https://github.com/openai/parameter-golf/discussions/747)** — Dashboard updates shared with the community

---

**Nathan Maine** — [GitHub](https://github.com/NathanMaine) | [LinkedIn](https://linkedin.com/in/nathanmaine)
NVIDIA Inception Member | Building AI compliance tools for defense contractors
