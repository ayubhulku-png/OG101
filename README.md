# My Life OS — empty-first iPad foundation

This build preserves the existing dependency-free PWA architecture while removing seeded/demo records and hard-coded daily/calendar state.

## Included
- iPad/desktop responsive app shell
- Life / Work / Founder modes
- Today command centre with data-driven empty states
- Explainable next-action foundation
- Tasks, Projects, Goals, People, Knowledge
- Calendar Month / Week / Day / Schedule navigation
- Real calendar date navigation across months and years
- Calendar category filters
- Finance from locally recorded transactions only
- Inbox capture and conversion to tasks
- Reviews, Analytics, Automations, Files, Settings
- Command Center (⌘K / Ctrl+K)
- Natural-language quick capture into Inbox
- Focus mode
- LocalStorage persistence
- JSON export/import
- PWA manifest, iPad metadata, icons and service-worker app-shell caching
- Reduced-motion support

## Empty-first rule
A clean installation starts with zero tasks, people, goals, projects, calendar events, transactions, activity, content, or other user records. The UI uses intentional empty states instead of fabricated data or decorative metrics.

## Run
Serve this directory from any static web server, for example:

`python3 -m http.server 8080`

Then open `http://localhost:8080`.

## Architecture
The current repository is dependency-free. The build keeps that architecture rather than introducing a framework/backend without the surrounding infrastructure. Future PostgreSQL/authentication/sync/vector-search/integration work should be added behind explicit service boundaries.
