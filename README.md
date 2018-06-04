# About
This solution is for blocking unwanted content on [twitch.tv](http://www.twitch.tv/), such as streams, games, videos etc. Currently, the following platforms are supported:
- Userscript, to be used with userscript managers such as [Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo?hl=en) or [Greasemonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/). Can be installed from [here](https://github.com/r3t3ch/hide-unwanted-streams-on-twitch/raw/master/dist/userscript/husot.user.js).

# How to use
See [User Guide](https://github.com/LinogeFly/hide-unwanted-streams-on-twitch/tree/master/docs/user-guide.md) document.

# How to run tests
Currently, tests are semi-automatic. To run tests open browser's console, select "Hide unwanted streams on Twitch" scope and run the following command:
```
husot.tests.runAll()
```
Failing tests will throw errors into console.

# Version history
- 1.3.28 Fixed an issue when channels blocking stopped working.
- 1.3.27 Fixed CSS selectors after Twitch update.
- 1.3.26 Added Firefox Quantum support for Userscript platform.
- 1.3.25 Added new Twitch UI support.
- 1.3.24 Fixed a bug when ad element was messing up channel thumbs finding logic.
- 1.3.23 Fixed a bug when blocking was not working on language specific pages.
- 1.3.22 Optimized CSS selectors for finding stream/video/game thumbs.
- 1.3.21 Fixed an issue when video blocking got broken after recent Twitch update.
- 1.3.20 Hot fix for blocking games/streams. Blocking for videos still doesn't work. Will be fixed soon.
- 1.3.19 Hot fix due to recent Twitch updates.
- 1.3.18 Fixed an issue when blocking stopped working on League of Legends page.
- 1.3.17 Added support for Communities pages.
- 1.3.16 Fixed a bug when "Infinite scroll" stopped triggering on Games page.
- 1.3.15 Fixed a bug when blocking for streams wasn't working in language specific sections.
- 1.3.14 Hot fix due to recent Twitch updates.
- 1.3.13 Reverted back Following pages support.
- 1.3.12 Added support for Following pages.
- 1.3.11 Optimized space usage for block lists.
- 1.3.10 Fixed small UI issues that appeared after Twitch Whispers update.
- 1.3.9 Optimized "Infinite scroll" triggering logic so it doesn't call internal functions on Twitch anymore.
- 1.3.8 Fixed a bug when "Infinite scroll" stopped triggering after Ember framework update on Twitch.
- 1.3.7 Fixed a bug when "Infinite scroll" didn't get triggered sometimes on language specific Channels page.
- 1.3.6 Fixed a bug when block list was getting reset if hitting total storage limit for a Chrome extension.
- 1.3.5 Fixed a bug when solution was not working if Twitch was accessed with language specific URL.
- 1.3.4 Fixed a bug when it was not possible to save long block lists due to quotation limit for settings (in Chrome only).
- 1.3.3 Fixed a bug when "Infinite scroll" didn't get triggered sometimes on Games page (in Chrome only).
- 1.3.2 Fixed a bug when streams were not hiding on CS:GO pages.
- 1.3.1 Fixed performance issue that occurred when a lot of channels and games were blocked. Blocked items are now sorted alphabetically in Settings window.
- 1.3.0 Added support for blocking games.
- 1.2.0 Added Google Chrome Extension platform.
- 1.1.0 Added support for hiding videos in addition to live streams.
- 1.0.0 First release. Only Userscript platform is supported.

# Known issues
- You can click through blocking overlay menu.
- "infinite scroll" can break, requiring a refresh
