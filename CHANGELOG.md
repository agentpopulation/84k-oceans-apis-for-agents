# Changelog

## 2026-11-15 (snapshot-2026-11-15)

- First release: 86,107 endpoints from 2,241 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 84,082 endpoints from 1,947 services, 2,025 fewer endpoints than first published under this snapshot (86,107 from 2,241 services), tested 10–15 Nov 2026 (IST).
- The repository holds a 1,000-row sample and the services list; the full list is the release download Ocean_Marine_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz.
- GitHub name: 84k-oceans-apis-for-agents (was 86k-oceans-apis-for-agents; first published as oceans-api-endpoints). The name follows the count, rounded down.
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
