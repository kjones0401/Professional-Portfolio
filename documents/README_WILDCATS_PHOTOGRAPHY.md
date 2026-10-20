# Bath County Wildcats Photography Hub

A responsive website organizing 2026 Wildcats football photo and video albums by opponent and event, backed by a separate local gallery management workflow.

## Problem and solution

Families needed one place to locate albums scattered across shared Google Photos links. The hub presents compact game/event cards and an immediate text search while retaining the photographs in Google Photos.

## Features

- Cinematic photo-first header using `images/wildcats-hero.jpg`
- Compact, responsive gallery grid
- Search by opponent, event, category, or description
- External Google Photos album links
- Gallery metadata stored in `wildcats_galleries.json`
- Local Gallery Manager for editing and exporting metadata

## Technologies

HTML, CSS, vanilla JavaScript, JSON, and GitHub Pages.

## Data workflow

1. Upload game photos to Google Photos and create a shared album.
2. Open the **Gallery Manager locally**, import the existing JSON file, and add/edit a gallery record.
3. Export `wildcats_galleries.json` from the manager.
4. Update that JSON file in the website repository.
5. The published Photography Hub reads and displays the updated gallery records.

The Gallery Manager is designed to stay on the owner's computer, **not** in the public GitHub Pages repository. The public site has no in-browser publishing or administrator authentication.

## Files

- `highschool_photo_hub_2026_albums.html` — public page
- `wildcats_galleries.json` — public album metadata
- `images/wildcats-hero.jpg` — photographic header image

## Preview

- [View the Photography Hub](https://bathcountyfootball.github.io/bcfootball_clean/highschool_photo_hub_2026_albums.html)

## Checks to perform after updates

- Confirm search finds an opponent such as Rowan.
- Confirm gallery counts and gallery ordering.
- Verify each album opens its intended Google Photos shared link.
- Confirm the hero photograph and mobile gallery cards display correctly.
- Verify the newly exported JSON is the file deployed to the website.

## Privacy and maintenance

Album links are publicly viewable by anyone with the links, depending on Google Photos sharing settings. Avoid putting private albums or personal data in public JSON. Keep the editable administrative tool and any private credentials out of the public site.
