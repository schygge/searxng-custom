# searxng-custom

SearXNG proxy image for the myorigins genealogy engine's search-supply rail.

Built on Render from this repo (Dockerfile at the repo root). The settings
keep DuckDuckGo, add bot-tolerant engines (Bing, Wikipedia, Mojeek,
Marginalia, Brave, Startpage), disable Google CSE (rate-limited from
datacenter IPs), enable the JSON format, and raise the outgoing timeout.

The same files live under `infra/searxng/` in schygge/new-genealogy, where a
workflow also publishes the built image to ghcr.io (private). This public
mirror exists because Render's free tier cannot pull a private ghcr package.
