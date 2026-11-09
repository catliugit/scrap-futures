> **This project is now Thread Futures.** Active code and website: [github.com/catliugit/ThreadFutures](https://github.com/catliugit/ThreadFutures) · [threadfutures.com](https://threadfutures.com). This repository is archived and kept for history.

# Scrap Futures

**No unsold clothes wasted.** Scrap Futures helps fashion brands route unsold stock to its best legal home (off-price, resale, donation or reprocessing), keep the evidence the EU's ban on destroying unsold clothes requires, and buy less next season.

Live site: **[scrapfutures.netlify.app](https://scrapfutures.netlify.app/)** · Investor page: [investors.html](https://scrapfutures.netlify.app/investors.html)

> Independent project, pre-revenue. Product screens are illustrative prototypes; forecasting results come from simulated data.

## What's in this repo

| Folder / file | What it is |
|---|---|
| `index.html`, `investors.html` | The website (static HTML, no build step). Netlify deploys it from `main`; GitHub Pages mirrors it. |
| `forecast.js`, `model.js` | The in-browser forecast demo: a gradient-boosted quantile model exported to JSON, evaluated in plain JavaScript. |
| [`forecasting/`](forecasting/) | The forecasting engine: production simulator, data pipeline, quantile ML (8.8% mean error vs 20.3% for the industry rule of thumb, on simulated runs), grading, matching, a Claude tool-use agent and 12 unit tests. See its [README](forecasting/README.md). |

## Run the forecasting engine

```bash
cd forecasting
pip install -r requirements.txt
make data && make train && make test
```

## Contact

Cathy Liu · [linkedin.com/in/cathyqliu](https://www.linkedin.com/in/cathyqliu/) · cathyqliu1@gmail.com
