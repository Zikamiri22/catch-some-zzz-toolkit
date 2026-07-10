# Catch Some ZZZ Guild Toolkit v3.2

GitHub Pages ready web package.

## v3.2 changes

* Expanded Catch Some ZZZ guild identity throughout the application
* Larger official guild logo treatment in the sidebar
* Branded dashboard hero with the Catch Some ZZZ mascot and guild copy
* Branded API connection experience
* Subtle guild logo marks across section headers
* Guild branded footer and leadership treatment
* Universal GW2 Wiki link helper for account data
* Wallet currency names now link to the GW2 Wiki
* Favorite currency dashboard entries now link to the GW2 Wiki
* Material Storage item names now link to the GW2 Wiki
* Bank item names now link to the GW2 Wiki
* Item Finder results and dashboard finder summaries now link to the GW2 Wiki
* Legendary Armory entries now link to the GW2 Wiki
* Legendary material and currency tracker entries now link to the GW2 Wiki
* Dashboard account coin label links to the GW2 Wiki
* Preserves the customizable dashboard and grouped navigation introduced in v3.1
* Service worker cache updated to v3.2

## Wiki linking standard

Displayed GW2 items, materials, and currencies use the shared Wiki link helper and open the Guild Wars 2 Wiki in a new tab. New features should use the same helper instead of hardcoding individual Wiki URLs.

## Privacy model

Each user supplies their own GW2 API key. The app calls the official GW2 API directly from the browser. No project backend receives account data. Optional remembered keys and all dashboard settings remain in browser storage.

## Deployment

Upload the contents of this folder to the repository root and commit the changes. Do not upload the ZIP itself or nest these files under another folder.
