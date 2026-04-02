# Copilot Budget Tracker

A lightweight, single-file web app that helps you stay on top of your [GitHub Copilot premium request](https://docs.github.com/en/copilot/concepts/billing/copilot-requests) allowance throughout the month.

![Status](https://img.shields.io/badge/status-active-639922?style=flat-square) ![No dependencies](https://img.shields.io/badge/dependencies-none-5aa3f0?style=flat-square) ![GitHub Pages](https://img.shields.io/badge/hosted%20on-GitHub%20Pages-1c1c1a?style=flat-square)

## What it does

Enter your monthly quota and the percentage shown on your GitHub billing page — the tracker calculates:

- **Daily budget** — how many requests you can safely spend per remaining day
- **Estimated today usage** — how much of today's daily allowance is already consumed
- **Pace status** — whether you're ahead of, on, or behind the ideal burn rate
- Color-coded bars and status banner (green / yellow / red) so you know at a glance where you stand

## Usage

1. Open your [GitHub Copilot billing page](https://github.com/settings/copilot) and note your usage percentage
2. Enter your monthly quota (300 for Pro, 1500 for Pro+) and the percentage into the tracker
3. Check back whenever you want to see your remaining daily budget

> **Tip:** GitHub doesn't expose individual premium request counts via API, so the percentage shown on their billing page is the easiest number to copy across.

## Getting started locally

No build step, no dependencies — just open the file:

```bash
git clone https://github.com/yourusername/copilot-budget
cd copilot-budget
open index.html
```

## Deploying to GitHub Pages

1. Fork or clone this repo and push to your GitHub account
2. Go to **Settings → Pages → Source** and select the `main` branch
3. Your tracker will be live at `https://yourusername.github.io/copilot-budget`

## Copilot plan quotas

| Plan | Monthly premium requests |
|---|---|
| Copilot Free | 50 |
| Copilot Pro | 300 |
| Copilot Pro+ | 1,500 |
| Copilot Business | 300 per seat |
| Copilot Enterprise | 1,000 per seat |

Allowances reset on the **1st of each month at 00:00 UTC**.

## License

MIT
