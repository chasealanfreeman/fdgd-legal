# Updating the app's live content

Edit `content.json` in this repo (GitHub web editor is fine) and commit —
the app picks it up within ~15 minutes, no App Store update needed.

- `fest.start` — countdown target (ISO date with timezone)
- `fest.dateLabel` — the date text on the Home screen, e.g. "April 2–4, 2027"
- `days` — day-picker labels in the Lineup tab
- `schedule` — the full lineup (id/day/t/title/venue/cat; cat one of:
  music, race, contest, plunge, family, ceremony, food)
- `notice` — Home-screen banner: `{"id": "unique-id", "text": "...", "url": "optional"}`
  (set to null to hide; change the id to re-show after users dismissed an old one)
- `grandpaFacts` — extra facts Grandpa treats as the latest official word

If the file is ever broken/unreachable, the app falls back to its built-in data.
