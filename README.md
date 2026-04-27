# epicbreezy.com

Static website for the **Epic Breezy 2026** project — a multi-segment cross-country
journey in a custom open-cockpit homebuilt airplane (N149X), all four corners of the
U.S. across six flying weeks.

## Files

- `index.html` — landing page; segment status, links to YouTube playlists, KML download.
- `Segment1_Trip.kml` — actual GPS-recorded flight track for Segment 1 (KOKB → KBRO,
  April 14-18, 2026). 12 legs colored by day, with airport markers and altitude profile.
  Opens in Google Earth Pro.

## Deploy

The site auto-deploys to Dreamhost via a `git pull` cron job in
`~/epicbreezy.com/` on the host. Pushing to `main` makes changes live within ~5 min.

## Channel

Videos: <https://www.youtube.com/@PaulBreed>
