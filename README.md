# Repete 2 — published dashboard

This repo is a **page, not a program.** It holds the rendered status dashboard
for Repete 2, an FX paper-trading agent running against an OANDA v20 **practice**
account. The bot's source is private.

**https://connorshibley.github.io/repete2-dashboard/**

`index.html` and `dashboard_data.json` are regenerated from the bot's own
records every 15 minutes and pushed here by `scripts/publish_dashboard.sh`,
behind a guard that refuses to publish an artifact disagreeing with those
records. Nothing here is hand-edited.

The page polls `dashboard_data.json` for a freshness badge — a static page
otherwise cannot say when it stopped being updated.

**Paper trading. Not investment advice.** No strategy in this project has passed
a gate, none is enabled, and no trade has ever been placed.
