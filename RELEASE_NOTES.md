## Ocean and marine API endpoints, snapshot 15 Nov 2026

- 84,082 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 1,947 services · 123 country codes · 66,267 keyless JSON rows

### Download

- `Ocean_Marine_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 84,082 rows, 2.9 MB gzipped (26.3 MB as CSV), SHA-256 `c396955ecd1943817fec420584dec6c22dbc24f8dbe382a0555a709e7fe9bbca`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Ocean_Marine_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Ocean_Marine_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 1,334 · Wrap one station URL as a get_sea_level or get_sea_temperature tool: pass the station code, return the latest value, its unit and time, with a timeout. Dataset records and map layers in this list need a query of their own.
- 📱 App features: 6,863 · Draw protected areas, sea level rise zones or reef layers on a coastal map: each layer query returns features with names and classes you can show on a card.
- 🧠 Grounding and data pipelines: 65,097 · Read each ERDDAP description for its variables and time range, then load the series from tabledap or griddap on a schedule into your own store, so answers about sea conditions cite a dated source.
- 🧪 Evals and testing: 84,082 · Run your ocean tool against a fixed set of URLs across formats; check that time, value, unit and position parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release: 86,107 endpoints from 2,241 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 84,082 endpoints from 1,947 services, 2,025 fewer endpoints than first published under this snapshot (86,107 from 2,241 services), tested 10–15 Nov 2026 (IST).
- Left out: 130 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 2 ArcGIS proxy layers (utility.arcgis.com/usrsvcs and portal /sharing/servers/ addresses) that can call a service with a stored login.
- Left out: 415 class-exercise copies of the same few ArcGIS Online layers (Miami Beach sea level rise, high-risk areas without shelter, flooded areas, sea level rise and storm surge maps) across many organisations, many with a person's name in the title.
- Left out: 3 layers marked editable in the title (they can hold entries that people added).
- Left out: 14 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 116 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 10 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 22 rows of server information from Mastodon, PeerTube, Lemmy, Nostr and other social network servers (instance documents name the server's contact person).
- Left out: 21 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 531 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 67 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 1,344 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 42 rows that repeat an address already in the pack.
- Overlap: 5,650 of these URLs are also in 170k-weather-apis-for-agents.
- Overlap: 1,381 of these URLs are also in 240k-transit-apis-for-agents.
- Overlap: 84,067 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 801 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 1,115 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 1,174 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 82 of these URLs are also in 270k-statistics-apis-for-agents.
- Overlap: 2,461 of these URLs are also in 22k-maritime-apis-for-agents.
- Overlap: 4,185 of these URLs are also in 160k-environment-apis-for-agents.
- Overlap: 24 of these URLs are also in 19k-air-quality-apis-for-agents.
- Overlap: 1,762 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 66,254 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 9 of these URLs are also in 84k-health-apis-for-agents.
- Overlap: 3,814 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 507 of these URLs are also in 40k-hazards-apis-for-agents.
- Overlap: 5 of these URLs are also in 4.9k-wildfire-apis-for-agents.
- Overlap: 64 of these URLs are also in 67k-energy-apis-for-agents.
- Overlap: 22 of these URLs are also in 23k-aviation-apis-for-agents.
- Overlap: 968 of these URLs are also in 22k-traffic-apis-for-agents.
- Overlap: 3 of these URLs are also in 10k-parking-apis-for-agents.
- Overlap: 86 of these URLs are also in 7.8k-earthquake-apis-for-agents.
- Overlap: 61 of these URLs are also in 4.2k-volcano-tsunami-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Ocean and marine API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
