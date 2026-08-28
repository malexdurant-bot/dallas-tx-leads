# Dallas County TX — Lead Intelligence Dashboard

Client-facing lead dashboard for Dallas County, Texas. Served via
GitHub Pages at [dallastx.justfriday.ai](https://dallastx.justfriday.ai).

This repo contains only the static frontend (`index.html`, `dashboard.js`,
`dashboard.css`) and a `data/leads.json` snapshot — no scraper source code,
no other counties. It's isolated from this account's other client repos so
a Dallas client's browser never has a path to another county's lead data.

Data is refreshed automatically: the production pipeline in the private
`xcerebro-county-intel` repo writes `data/leads.json` here and pushes after
every run (see `runs/dallas_tx/run_pipeline.py`).
