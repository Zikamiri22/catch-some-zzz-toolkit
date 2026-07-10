# Catch Some ZZZ Guild Toolkit v3.5

GitHub Pages ready web package.

## v3.5 changes

* Adds multi account GW2 API key profiles.
* Members can save multiple accounts in this browser and switch between them from a dropdown in Account Status.
* Add Account opens the existing guild branded API key form with saving enabled by default.
* Remove Saved Account removes the selected local profile.
* Switching accounts clears loaded account data before the new account refreshes, preventing mixed wallet, bank, inventory, legendary, and completion data.
* Raid and strike manual weekly fallback state is now account scoped using a v2 storage key.
* Fractal daily and long term manual fallback state is now account scoped using v2 storage keys.
* Existing dashboard customization, Event Timer, Wiki linking, and API completion sync remain intact.
* Service worker cache updated to v3.5.

## Multi account storage

Saved profiles use `cszzz-api-accounts-v1`. The selected profile name uses `cszzz-active-api-account-v1`. API keys remain local to the member's browser and are sent only from that browser to the official Guild Wars 2 API.

## Deployment

Upload the contents of this folder to the repository root and commit the changes. Do not upload the ZIP itself or nest these files under another folder.
