# SkillsBridge EU

SkillsBridge is an enterprise workforce-mobility platform that maps emerging European capabilities to verified learning pathways, personal development plans and team cohorts.

[Watch the verified product demo](docs/demo.webm)

## Business problem and users

Regulated employers need a practical way to respond to AI, cybersecurity, sustainability and data-skills gaps. Employees explore role-aligned learning; talent leaders convert gaps into accountable cohort plans; programme owners monitor readiness.

## Key workflows

- Search and filter role-aligned learning pathways.
- Compare match scores, level, provider and duration.
- Save a personal pathway and review capability readiness.
- Create and validate a team learning cohort.
- Track workforce plans from draft to enrolment.

## Vue technical highlights

- Vue 3 Composition API, typed setup scripts and computed derivations.
- Pinia setup store for catalogues, saved pathways and cohorts.
- Vue Router multi-page product navigation.
- TransitionGroup feedback, reusable card composition and controlled forms.
- Vitest store tests for high-value actions.

## Architecture and state flow

The Pinia store is the single typed domain source. Route views own transient search and form state, computed selectors derive personalised collections, and reusable pathway cards emit focused actions through the store.

## Accessibility and responsive behaviour

Search and filters are labelled, interactive controls expose descriptive names, and status feedback is announced. Grids and planning panels adapt from wide enterprise screens to compact mobile layouts.

## Run and verify

```bash
npm ci
npm test
npm run build
npm run dev
```

## Structure

- `src/views` — opportunity, pathway and planner routes
- `src/components/MediaCard.vue` — reusable pathway card
- `src/store.ts` — Pinia domain state and actions
- `src/router.ts` — route map

## Tradeoffs and roadmap

Programme and match data are illustrative. A production roadmap includes skills-taxonomy APIs, European credential wallets, HRIS integration, manager approvals, multilingual content, learning-provider evidence and privacy-preserving workforce analytics.
