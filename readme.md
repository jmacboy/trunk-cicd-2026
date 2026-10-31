# Trunk-Based Development

A small reference project explaining **Trunk-Based Development (TBD)**, a source-control branching model where developers integrate small changes into a single shared branch (`main`, the "trunk") at least once a day.

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | Visual explanation of TBD with a branch diagram |
| `readme.md` | This file |
| `.gitignore` | Files Git should not track |

## View it

Open `index.html` in any browser. No build step or dependencies required.

## Key ideas

- **One trunk**: everyone commits to `main` (directly or via short-lived branches).
- **Short-lived branches**: feature branches live hours, at most 1–2 days.
- **Small commits**: integrate often to avoid painful merges.
- **Always releasable**: CI runs on every commit; a broken trunk is fixed immediately.
- **Feature flags**: ship incomplete work hidden behind toggles instead of long branches.
- **Release from trunk**: tag `main`, or cut a release branch only for hotfixes.

## Trunk-Based vs. GitFlow

| | Trunk-Based | GitFlow |
| --- | --- | --- |
| Long-lived branches | Only `main` | `main`, `develop`, `release/*`, `hotfix/*` |
| Branch lifetime | Hours to ~2 days | Days to weeks |
| Merge conflicts | Small and rare | Large and frequent |
| CI/CD fit | Excellent | Harder |

## References

- [trunkbaseddevelopment.com](https://trunkbaseddevelopment.com/)
- [DORA: Trunk-based development](https://dora.dev/capabilities/trunk-based-development/)
