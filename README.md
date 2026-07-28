# epicbreezy.com

Static website for the **Epic Breezy 2026** project — a multi-segment cross-country
journey in a custom open-cockpit homebuilt airplane (N149X), all four corners of the
U.S. across six flying weeks.

## Files

- `index.html` — landing page; segment status, links to YouTube playlists, KML downloads.
- `Segment1_Trip.kml` — actual GPS-recorded flight track for Segment 1 (KOKB → KBRO,
  April 14-18, 2026). 12 legs colored by day, with airport markers and altitude profile.
  Opens in Google Earth Pro.
- `Segment2_Trip.kml` — Segment 2 (KBRO → KCGC, June 5-13, 2026). 19 legs, 17 airports.
- `Segment3_Trip.kml` — Segment 3 (KCGC → KGTF, July 2-24, 2026). 47 legs, 48 airports.

All three KMLs are 1 Hz tracks recorded by the wing-mounted GoPros. Segments 2 and 3
had no filed flight plan to work from, so their legs and airport lists were derived
from the GPS telemetry itself — see `E:\epicbreezy\tools\` for the pipeline and the
per-segment `route` notes on the footage drive for what each one found.

## Deploy

The site auto-deploys to Dreamhost via a `git pull` cron job in
`~/epicbreezy.com/` on the host. Pushing to `main` makes changes live within ~5 min.

## Channel

Videos: <https://www.youtube.com/@PaulBreed>
