# glucose-log

Daily glucose tracking for GDM. Entries are saved by index.html via the GitHub Contents API into data/YYYY-MM.json. Each save is a commit.

## Setup on a phone

1. Open index.html (via htmlpreview or download it and open locally, see below).
2. First launch asks for a GitHub token. Create a fine-grained PAT at github.com/settings/personal-access-tokens with Repository access set to ONLY this repo and Contents read/write permission. Paste it once. It stays in that phone's localStorage.
3. Log the day: tap Now when eating starts, the page shows when to prick (1 hour later), enter the reading, tap Save to log.

## Targets

Fasting under 95, 1 hour post meal under 140 (per care team).

## Data format

data/2026-08.json is a JSON object keyed by date, then meal (Fasting, Breakfast, Lunch, Dinner), each with eatTime, reading, readTime, food.

## Opening the page

The repo is private so GitHub Pages is off. Options: open the raw index.html locally (download once to the phone, open in browser), or serve via any static host you control. The page itself contains no secrets.
