# Apollo memory & Command Center

Private repository powering the cross-device Command Center for Max Mazur.

## Layout

- `/data/` — durable state (goals, blockers, fitness, journal entries). Source of truth.
- `/docs/` — Command Center web app, served via GitHub Pages.

## Web app

Live URL (after Pages is enabled): https://greenerconcepts.github.io/apollo-memory/

Auth: paste your fine-grained PAT once on first visit; it's stored in browser localStorage and used for all GitHub API calls. Never sent anywhere except api.github.com.

## Backup

iCloud `~/Library/Mobile Documents/com~apple~CloudDocs/Apollo/` is the local mirror. Apollo (on the Mac) and the web app (on phone/anywhere) both write through here. Local Mac sessions read iCloud directly; web app reads/writes via GitHub API.
