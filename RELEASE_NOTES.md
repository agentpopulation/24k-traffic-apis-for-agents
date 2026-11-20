## Traffic and roadworks API endpoints, snapshot 15 Nov 2026

- 24,641 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 2,782 services · 220 country codes · 14,404 keyless JSON rows

### Download

- `Traffic_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 24,641 rows, 1.2 MB gzipped (7.7 MB as CSV), SHA-256 `285bd7288d892cfbaedde500b347b879215177ffd8e9c315a41fb0d25b27404d`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Traffic_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Traffic_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 9,352 · Wrap one URL pattern as a get_traffic tool: pass a station id or a road area, return vehicle counts, average speed or road-surface readings with the measurement time and a timeout.
- 📱 App features: 1,080 · Show roadworks and closures near a route on a map card with the start and end dates each layer gives, and past crashes as a road-safety layer.
- 🧠 Grounding and data pipelines: 9,092 · Load counting-station files, crash tables and road-death rates on a schedule into your own store, so answers about traffic volumes and road safety cite a dated source.
- 🧪 Evals and testing: 24,641 · Run your traffic tool against a fixed set of URLs across formats; check that station, count, speed, location and time parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 1 row with an email-like address.
- Left out: 338 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 layer marked editable in the title (it can hold entries that people added).
- Left out: 65 police traffic-stop layers (they can hold details of people stopped).
- Left out: 23 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 948 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 19 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 10 rows of server information from Mastodon, PeerTube, Lemmy, Nostr and other social network servers (instance documents name the server's contact person).
- Left out: 946 development-plan map services (GetCapabilities) of Villingen-Schwenningen, Germany, tagged by the German word Verkehr: not traffic data.
- Left out: 1,215 land-use tables ("settlement and traffic areas") of German municipalities: not traffic measurements.
- Left out: 643 Destatis economy, trade and enterprise tables tagged by the word Verkehr: not road traffic.
- Overlap: 284 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 24,641 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 1,129 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 125 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 59 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 199 of these URLs are also in 1.3m-government-open-data-apis.
- Overlap: 17 of these URLs are also in 290k-statistics-apis-for-agents.
- Overlap: 970 of these URLs are also in 86k-oceans-apis-for-agents.
- Overlap: 1,307 of these URLs are also in 24k-maritime-apis-for-agents.
- Overlap: 11 of these URLs are also in 170k-environment-apis-for-agents.
- Overlap: 30 of these URLs are also in 20k-air-quality-apis-for-agents.
- Overlap: 1,833 of these URLs are also in 380k-maps-gis-apis-for-agents.
- Overlap: 14,404 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 132 of these URLs are also in 96k-health-apis-for-agents.
- Overlap: 61 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 83 of these URLs are also in 53k-hazards-apis-for-agents.
- Overlap: 15 of these URLs are also in 72k-energy-apis-for-agents.
- Overlap: 1,026 of these URLs are also in 25k-aviation-apis-for-agents.
- Overlap: 120 of these URLs are also in 12k-parking-apis-for-agents.
- Overlap: 1 of these URLs is also in 10k-earthquake-apis-for-agents.
- Overlap: 13 of these URLs are also in 17k-bike-share-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Traffic and roadworks API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
