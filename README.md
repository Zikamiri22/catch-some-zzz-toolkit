# Catch Some ZZZ Guild Toolkit v3.15

## Event Timer restoration patch

* Restored the missing Event Timer expansion definitions, event schedule dataset, preference helpers, favorites helpers, and next-occurrence calculation.
* Fixed the JavaScript failure that left Local Time blank, Visible Events at 0, and prevented filters and event cards from rendering.
* Preserved explicit UTC handling for irregular schedules such as Tequatl.
* Updated visible version labels and the service-worker cache to `cszzz-toolkit-v3.15`.
* Kept the Guild Wars 2 Wiki Event Timers page as the schedule reference source.

# Catch Some ZZZ Guild Toolkit v3.14

## Provisioner Token audit

Rebuilt the Provisioner Token guide from the current GW2 Wiki acquisition table. Added all fixed one-token exchange vendors shown in that table, grouped exchange choices under the correct vendor, and modeled weekly limits at the vendor/exchange source level rather than multiplying the limit by every displayed item choice. Added search, region filtering, weekly account-scoped completion, Wiki links, and copyable verified waypoints where available.

# Catch Some ZZZ Guild Toolkit v3.11

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



## v3.10 Credits and disclaimer

- Added a compact linked source credit line for GW2 Wiki, Snow Crows, Mukluk, Hardstuck, GuildJen, and GW2Efficiency.
- Added a concise unofficial fan project disclaimer in the global footer.
- Kept attribution visible without adding a large credits page or cluttering tool layouts.
- Updated service-worker cache to `cszzz-toolkit-v3.10`.

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


## v3.11 Event timer accuracy patch

- Added explicit UTC schedule support for irregular event rotations.
- Corrected Tequatl the Sunless to the verified UTC starts: 00:00, 03:00, 07:00, 11:30, 16:00, and 19:00.
- Added Splintered Coast area information and a verified schedule label for Tequatl.
- Removed unverified Visions of Eternity timer entries until authoritative schedules are available.
- Added a direct source link to the official Guild Wars 2 Wiki Event Timers page.
- Updated the service-worker cache to `cszzz-toolkit-v3.11`.


## v3.14 Raid Wing Mapping Fix

Replaced API catalog-order grouping with a fixed verified Wing 1 through Wing 8 encounter map. Removed invalid Gate and Camp entries and corrected all encounter assignments. Weekly completion still comes from `/account/raids`.
