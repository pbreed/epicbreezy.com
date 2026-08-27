# epicbreezy.com

Static website for the **Epic Breezy 2026** project — a multi-segment cross-country
journey in a custom open-cockpit homebuilt airplane (N149X), all four corners of the
U.S. Originally planned as six segments; Segment 3 absorbed what was to be two of
them, so the trip finishes at Segment 5.

## Files

- `index.html` — landing page; segment status, links to YouTube playlists, KML downloads.
- `Segment1_Trip.kml` — actual GPS-recorded flight track for Segment 1 (KOKB → KBRO,
  April 14-18, 2026). 12 legs colored by day, with airport markers and altitude profile.
  Opens in Google Earth Pro.
- `Segment2_Trip.kml` — Segment 2 (KBRO → KCGC, June 5-13, 2026). 19 legs, 17 airports.
- `Segment3_Trip.kml` — Segment 3 (KCGC → KGTF, July 2-24, 2026). 47 legs, 48 airports.
- `Segment4_Trip.kml` — Segment 4 (KGTF → KYKM, August 20-24, 2026). 9 legs, 9 airports.

All four KMLs are 1 Hz tracks recorded by the wing-mounted GoPros. Segments 2, 3 and 4
had no filed flight plan to work from, so their legs and airport lists were derived
from the GPS telemetry itself — see `E:\epicbreezy\tools\` for the pipeline and the
per-segment `route` notes on the footage drive for what each one found.

Segment 4 is the first since Segment 2 with ground truth to check against: the pilot
stated the stop list before the derivation ran, and the blind derivation recovered all
9 legs and all 9 airports in order, 0 unresolved endpoints, every endpoint within
0.78 nm. `--route` is a post-hoc diff only — `Derive-FlightLegs.py` reads it after the
legs are built, so passing it does not compromise the independence of the derivation.

## Deploy

The site auto-deploys to Dreamhost via a `git pull` cron job in
`~/epicbreezy.com/` on the host. Pushing to `main` makes changes live within ~5 min.

## Channel

Videos: <https://www.youtube.com/@PaulBreed>
