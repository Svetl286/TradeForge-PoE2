# TradeForge quick start

Use https://tradeforge.download as the price server in Settings. Refresh the league list, select the active league you play in or Standard, then choose Apply and restart. When two leagues run concurrently, select your character’s league.

## 1. Download the installer from the [latest GitHub Release](https://github.com/Svetl286/TradeForge-PoE2/releases/latest).
2. Compare its filename, size and SHA-256 with that release page using the [download verification guide](VERIFY_DOWNLOAD.md).
3. Install the program and complete its setup wizard.

Full instructions: [user manual with screenshots](manual_en.md). The program's **Guide** button opens the manual for the installed version.

> The interface depends on the installed version. If you only see Current league and Standard instead of a league list, check for an available update. The in-app guide matches the installed version.

## 2. Before the first run

- start Path of Exile 2;
- set the game client area to exactly `1024×768`;
- select Russian or English as the game language;
- have a valid TradeForge license key;
- place the stash and Ange close enough to interact with both from the same
  character position.

## 3. Setup wizard

The wizard covers the app/game language, license and server, game window,
stash/Ange captures and the minimum source-tab/shop configuration. Skipped
steps can be completed later in Settings.

The license window provides official Discord, Telegram and GitHub buttons,
plus server-address editing, saving and connection re-checking.

## 4. First controlled workflow

1. Configure one source tab and one shop.
2. Start with price-only mode.
3. Review results in Prices → Pre-sale and Shop → Price Preview.
4. Start listing only after the routing and pricing rules look correct.
5. Use the configured pause/resume hotkey and the dedicated stop hotkey or
   stop corner.

## 5. New crafting and repricing controls

- **Move valuable items to** works together with **Craft only**. Select a
  separate destination tab and set a value threshold and currency. The program
  prices results directly in the craft tab, converts values at the current
  exchange rate, moves items worth at least the threshold, and keeps crafting
  the rest. A source and destination cannot be the same tab.
- **verify prices** in the repricing block reads the actual in-game prices
  before building a plan. Keep it enabled when prices may have been changed
  manually. Turning it off skips the full preliminary verification and builds
  the plan faster from saved data.

## 6. Support

- Discord — primary support: https://discord.gg/UtU9Ty2bBv
- Telegram license/payment bot and fallback request form: https://t.me/TradeForgePoE2Bot
- GitHub Issues: https://github.com/Svetl286/TradeForge-PoE2/issues

Submit full logs only through the explicit in-app support action. Never post a
license key, POESESSID, payment data or a full log in a public Issue.
