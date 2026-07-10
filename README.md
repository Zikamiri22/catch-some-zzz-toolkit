# Catch Some ZZZ Guild Toolkit v3.9

## Release focus

This release corrects Fractal daily completion tracking and continues the responsive layout cleanup.

### Fractals

* Loads the current Daily Fractal achievement set from the GW2 API.
* Shows only today's Daily Tier 4 and Daily Recommended fractals.
* Compares those achievement IDs against the connected account's achievement progress.
* Separates Tier 4 and Recommended progress into clear 0/3 style summaries.
* Removes unrelated historic Fractal achievements from the daily completion screen.
* Keeps long term Fractal goals as account scoped personal checklists.
* Keeps Wiki links on all displayed fractal achievement names.

### Layout

* Reworked the Fractal page into two focused responsive completion cards.
* Improved compact status pills, spacing, and mobile readability.
* Updated dashboard Fractal widget to show Tier 4 and Recommended completion separately.

### Privacy

All API calls remain client side. Saved API keys and local tracking remain in the user's browser only.


## v3.9 Fractal Daily Source Fix

- Replaced the disabled `/v2/achievements/daily` request with `/v2/achievements/categories/88?v=latest`.
- Today's Tier 4 and Recommended Fractals now come from the live Daily Fractals achievement category.
- Account completion still syncs separately through `/v2/account/achievements` when the key has Progression permission.
- The rotation can display even when completion sync is unavailable.
- Updated service-worker cache to `cszzz-toolkit-v3.9`.

## v3.8 Fractal sync reliability fix

- Loads the public daily Fractal rotation independently of account permissions.
- Separates rotation availability from account completion availability.
- Shows active T4 and Recommended fractals even when the connected API key lacks Progression permission.
- Prevents unavailable account progress from being displayed as false 0/3 completion.
- Adds clearer permission and sync status messaging.


## v3.8 Dashboard Navigation Update
Dashboard widgets now act as direct navigation cards. Clicking or keyboard activating a widget opens its matching app section. Interactive controls inside widgets keep their existing behavior and do not trigger card navigation. Quick Tools remains a multi-action widget.
