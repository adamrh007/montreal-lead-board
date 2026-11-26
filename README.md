# Montreal Lead Board

A one-page tool to work through local business leads for NFC Google review cards.

Load the `leads.csv` produced by `leads.py` (Google Places API), then:

- **Filter by borough** (all 19 Montreal boroughs, detected from the search query or address), reason (few reviews / low rating) and status
- **Open in Maps** using the exact `maps_link` from the CSV
- **Copy review link** to paste into the NFC Tools app
- **Track each shop**: To visit → Visited → Interested → Sold → Not interested, with a note
- **Goal meter**: price per card × sales vs. your goal
- **Download / copy** everything back as CSV, statuses and notes included

## Use it

Open the live page (GitHub Pages) or just double-click `index.html`. No install, no server.

Your CSV is read **in your browser only**. Nothing is uploaded. Statuses and notes are saved in that browser's local storage.

## CSV columns

`name, address, rating, reviews, reason, phone, website, maps_link, review_link, search`

Optional: `borough` (overrides automatic detection).

> Real lead files (`*.csv`) are ignored by git so they never end up in this repo.
