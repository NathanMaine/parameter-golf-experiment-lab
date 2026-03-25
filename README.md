# Parameter Golf — Experiment Lab

**Interactive dashboard visualizing 352 submissions from the [OpenAI Parameter Golf](https://github.com/openai/parameter-golf) competition.**

> **Disclaimer:** This dashboard is not affiliated with, endorsed by, or officially associated with OpenAI, RunPod, or the Parameter Golf competition organizers. It is solely an independent attempt by one participant to document, visualize, and analyze data from a public open-source competition. All data is sourced from publicly available GitHub pull requests.

## Live Dashboard

**[View the live dashboard →](https://nathanmaine.github.io/parameter-golf-experiment-lab/)**

## What's Inside

- **Community Leaderboard** — All 352 submissions ranked by BPB, searchable and filterable by status (open/closed/merged), size compliance, author, and technique
- **Score Timeline** — BPB progression chart showing legal vs illegal zones
- **Experiment Log** — 46+ personal experiments with full config, timing, and outcome data
- **Technique Matrix** — What worked, what didn't, and what got banned
- **Cost Analysis** — $256 across 5 RunPod pods, broken down by session with efficiency metrics
- **Pod Comparison** — GPU benchmarks across pods (TFLOPS, step times, locations)
- **Key Discoveries** — Timeline of insights from 6 days of competition

## Data Sources

- `submission.json` files from 485 public pull requests
- Personal experiment logs from RunPod sessions
- Organizer comments and rulings from GitHub issues

## Related

- **[RunPod GPU Benchmark](https://github.com/NathanMaine/runpod-gpu-benchmark)** — 30-second script to find the fastest GPU pod before training
- **[OpenAI Parameter Golf](https://github.com/openai/parameter-golf)** — The competition repo
- **[Discussion Post](https://github.com/openai/parameter-golf/discussions/743)** — GPU benchmark tool shared with the community

---

**Nathan Maine** — [Memoriant Inc.](https://memoriant.ai)
NVIDIA Inception Member | Building AI compliance tools for defense contractors
