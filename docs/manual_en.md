# TradeForge — User Manual

> This online manual is maintained as the program changes. Open the guide for your installed version in the program: “Settings → General → 📖 Manual”. If your version only offers “Current league” and Standard, check for updates: the league selection interface depends on the program version.
>
> Some screenshots were taken in earlier versions and show an older interface or a test server address. Use the official address **https://tradeforge.download**. [Download the latest version](https://github.com/Svetl286/TradeForge-PoE2/releases/latest).

TradeForge is a trading assistant for Path of Exile 2: it prices any
items against the market (waystones, rings, amulets, jewels, tablets and
much more), crafts right in your stash — crafting methods for different
item kinds are set up in the Craft Constructor — lists items in your
shop tabs and watches the prices. You set it up — the program does the
clicking.

What you will need:

- Windows 10/11 and Path of Exile 2 (Steam) running in **windowed mode**
  at **1024×768** — the program is calibrated for this window size and will
  not work with any other (checked at start; with a different resolution
  the program will not launch its runs);
- a character standing next to the stash chest and the NPC Ange;
- a license key like `TF-XXXXX-XXXXX-XXXXX-XXXXX` and the price server
  address (provided by the seller);
- 15 minutes for the first-time setup.

> Every frame has a continuous "Fig. XX" caption. If a frame requires a
> running game or the installer and has not been captured yet, an explicit
> placeholder is shown instead. Tables below interface frames enumerate the
> controls with local numbers and explain what they do.

---

## 1. Quick start "in 15 minutes"

### Before you start

Prepare the game before every live run:

- hide or turn off the in-game chat blocks so they cannot cover stash cells,
  notifications or item tooltips;
- close item descriptions, menus, pop-up notifications and extra panels. The
  program can usually close or wait out harmless panels, but this costs time
  and an overlapping panel can still hide something important;
- make sure the Path of Exile 2 window is active, fully visible and not covered
  by another window.

> ⚠ **The program controls the mouse and keyboard, so this PC is occupied
> while a run is in progress.** Do not use the mouse over the game or type into
> it. If you need to work in parallel, run the game and the program on a
> separate physical PC. A virtual machine is not a safe mode for PoE 2 and
> does not protect a game account from GGG account action.
> Learn [F8 pause, F9 stop and the
> emergency stop corner](#safety) before the first live run.

### 1.1 Installation

1. Run the installer `TradeForge_Setup_<version>.exe`.
2. Go through the setup wizard — administrator rights are not needed; the
   program installs into your user profile.
3. Optionally check the desktop shortcut and finish the installation.

![TradeForge installer](img_en/setup_installer.png)

All your data (license, settings, calibration, listings database) is kept
in `%APPDATA%\TradeForge`. Updating the program does not touch it: a new
version can be installed on top of the old one.

### 1.2 First launch: the license window

On startup the program checks the license first.

![License window](img_en/license_gate.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | Status | The current license state and server connection. | Read it if the program does not let you go further. |
| 2 | Server | The license and pricing server address. You normally do not need to change it. | Only when support provides another address. |
| 3 | 💾 Save and check | Saves the address and immediately checks the license and connection again. | After changing the address or when the server is back online. |
| 4 | "Key" field | Enter the `TF-…` license key. Right-click → Paste, or Ctrl+V — works on any keyboard layout. | On first launch and when entering a new key. |
| 5 | Activate | Sends the key to the server and activates the license. The validity period starts counting from this moment. | Once, after entering the key. |
| 6 | ⟳ Retry check | Checks the key and the current server connection again. | After your internet or the server is back online. |
| 7 | 💬 Discord | Opens the primary TradeForge community and support server. | Questions, support and news. |
| 8 | ✈ Telegram | Opens the license, payment and fallback-request bot. | Buy/renew a key or contact the team when Discord is unavailable. |
| 9 | 🌐 GitHub | Opens the official repository with releases, quick starts and the changelog. | Download an official build or review changes. |
| 10 | Exit | Closes the program. | If you want to come back later. |

Important: **one key = one running copy**. If the key is already in use on
another computer, the second copy will not start until the first one
closes.

### 1.3 Setup wizard

After activation the first-run setup wizard opens automatically
(7 steps). Any step can be skipped with "Next →" and finished later: the
wizard is always available in "Settings → General → 🧙 Setup wizard…".

**Step 1. Welcome** — what the wizard will set up and what you will need.

![Wizard: Welcome step](img_en/wizard_welcome.png)

**Step 2. Language** — the program language (applies after a restart) and
the game language (the language your PoE 2 client runs in — affects item
reading).

![Wizard: Language step](img_en/wizard_lang.png)

**Step 3. Key & server** — if the key is already activated, the step shows
"key active". Enter the price server address (provided by the seller
together with the key) and press "Test connection" — a checkmark and the
league name should appear. Your own proxies are NOT needed: all price
requests go through the server.

![Wizard: Key & server step](img_en/wizard_key_server.png)

**Step 4. Game window** — start Path of Exile 2 in **windowed mode at
1024×768** (game settings → Graphics → Window mode: "Windowed") and
press "🔍 Find game window". "✓ window found" and the window size should
appear; a wrong size shows "✗ …" with a hint on what to change. The program
does not work at any other resolution: all snapshots and click points
are captured at 1024×768, and starting evaluation/selling/crafting is
blocked with a warning.

![Wizard: Game window step](img_en/wizard_game.png)

**Step 5. Stash & Ange** — the program finds the stash chest and the NPC Ange
by the labels above them. Stand your character next to them, close the
game panels and press "◎ Test" for each one. If the circle is not on the
object or the test fails — "📍 Recapture…": aim the frame at the "Stash"
label (or the "Ange" name) in the window with the game screenshot that
opens.

![Wizard: Stash & Ange step](img_en/wizard_world.png)

> 💡 **Place the stash and Ange close together in your hideout.** The
> character must be able to activate both the stash and Ange while
> standing in one spot — the program does not walk around the hideout, it
> clicks the labels from where the character stands. You can rearrange
> the objects with the in-game hideout editor. A small bonus of this
> placement: when the character stands right next to them, the labels
> above the objects get slightly highlighted — snapshots with a good
> threshold recognise the label in both states, so the proximity adds an
> extra margin of reliability.

![Recommended placement: stash and Ange side by side](img_en/hideout_placement.png)

**Step 6. Stash: source & shop** — the minimum to start: one item source
tab and one shop.

![Wizard: Stash step](img_en/wizard_stash.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | ➕ Source tab… | Adds a stash tab the program takes items from (waystones, rings, tablets and so on). Any name works (the program finds tabs by snapshots, not by name); naming it as in the game is just easier to follow. | First-time setup. |
| 2 | ➕ Shop… | Adds a shop tab where the program lists items. | First-time setup. |
| 3 | Tab table | All tabs: role, coordinates ("✓"/"no"), snapshots ("✓✓"), on/off. | Check that every tab has coordinates and snapshots. |
| 4 | ✏ Set coordinates (3s) | Select the row, press the button, hover the mouse over the tab in the game and hold — the position is recorded after 3 seconds. If a point is already saved, the program asks for confirmation before overwriting. | For every added tab. |
| 5 | 📸 Photograph the tab… | Snapshots of the tab "selected" and "not selected" — the program uses them to tell which tab is open. The same window can save the click point ("① by frame"). | For every added tab. |
| 6 | 🔍 Diagnostics | Checks the saved snapshots against the live game. | If you doubt the calibration. |
| 7 | 🔮 Omens / 💰 Currency | Capture of omen and currency icons for crafting. | Needed before autonomous crafting; can be skipped for the first pricing run. |

> ⚠ **Many tabs — calibrate by the right-side menu.** If there is a
> navigation list to the right of the tab row in-game (it appears when
> the tabs no longer fit in the row), photograph the tabs and the click
> point by the rows of that list, not by the top row: tabs in the row
> shift when clicked, the saved points stop landing and the program will
> miss. The list rows always stay in place. The list must also be open
> while the program works — pin it with the padlock. If the list appeared
> later (you got more tabs) — recalibrate the already configured tabs
> by it.

**Step 7. Check** — the final checklist: license, price server, currency
rates, game window, stash and Ange, stash layout. When everything is
green — "✓ Finish".

![Wizard: Check step](img_en/wizard_check.png)

### 1.4 First cycle: price → list → watch the prices

Open the stash tab with your items (for example waystones) in the game
and keep the game window visible.

**Step 1 — price the stash.** The [Management](#management) tab → expand the
"Evaluate & list for sale" block → press "💰 Price the stash". The program
hovers the cursor over every item in the open tab, reads it and finds a
market price. Nothing gets listed: the result appears in
"[Prices → Pre-sale](#prices)". Do not touch the mouse while the program works.

![First cycle: Price the stash](img_en/first_eval_stash.png)

Before scanning, the program asks what is currently open in the game: a
regular top-level tab or a tab inside a folder with a visible row of child
tabs. This choice is required to select the correct cell grid and hover the
items accurately.

![First cycle: choose the type of the open stash section](img_en/first_eval_stash_section_type.png)

- choose **"Yes — the tab is inside a folder"** when a row of child tabs is
  visible above the item grid;
- choose **"No — a regular tab without a folder"** for a standalone
  top-level tab.

**Step 2 — list the pre-sale.** Make sure the items sit in the same cells
where they were scanned, and press "📤 List items" in the same block. The
program moves the items to the shops and lists them at the selected prices.
The result is in the Shop tab.

![First cycle: List the pre-sale](img_en/first_presale_list.png)

**Step 3 — price re-check.** Expand the "Price re-check & repricing"
block → "▶ Start". The tool watches your listed items and reprices aged
ones by your rules ("⚖ Price rules…", "⏱ Listing age…") until you stop
it.

![First cycle: Price re-check](img_en/first_reprice.png)

Done — the basic trading cycle is running. Next you can enable
[autonomous craft & sell](#management).

---

## 2. The program tab by tab

Program tabs: **Management · Prices · Shop · Log · Search · Settings**.
Settings consists of the pages "General", "License & server",
"Stash & Shops", "Captures & templates" and "Pricing rules".

### 2.1 Management

The main working tab: three accordion tools (clicking a header expands
the block) and the log at the bottom.

![Management tab](img_en/tab_management.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | League: | The league the program trades and prices in. To switch — "Settings → General" (applies after a restart). | Check it before the season starts. |
| 2 | Currency rates + ⟳ | The current rate (for example divine → chaos); "⟳" refreshes the league and the rate from the network. Every price conversion uses this rate. | If the rate is stale. |
| 3 | ▶ Autonomous craft & sell | Header of the full auto-cycle block (see 2.1.1). | The main working mode. |
| 4 | ▶ Evaluate & list for sale | Header of the pricing-and-selling block without crafting (see 2.1.2). | Sell what already sits in the stash. |
| 5 | ▶ Price re-check & repricing | Header of the price watching block (see 2.1.3). | When listings are already up. |
| 6 | ▶ Log | Collapsible log of this tab's tools; when collapsed, the last line is visible on the right (click it to expand). An activity bar appears next to it while the program runs a background operation. | Follow the progress; the full technical log is in the Log tab. |

#### 2.1.1 The "Autonomous craft & sell" block

The full cycle: stock check (suitable items, currency and omens) → crafting
by the [Craft Constructor](#craft-constructor) plan right in the source tabs
→ market pricing → listing across the shops. It runs while the selected
sources contain suitable items and there is enough currency/omens.

![Autonomous craft & sell block](img_en/mgmt_auto_block.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | Sections: Item sources | Checklist of source tabs: the program crafts and sells ONLY their contents. | Choose which tabs go into the auto-cycle. |
| 2 | Move valuable items to | Destination tabs for valuable craft results, plus a minimum value and currency selector. Works only with "Craft only". | Keep successful crafts while rerolling the rest. |
| 3 | Where to list | Checklist of shops — shared with the "Targets" of the "Evaluate & list for sale" block. Items are spread across the shops automatically: categories and price ranges come from the shop settings. | Limit which shops to list into. |
| 4 | ⚙ Stash & Shops… | Opens "[Settings → Stash & Shops](#stash-shops)" (tabs and calibration). | Add/fix tabs. |
| 5 | [🔮 Omen setup](#omen-setup) | Capture of omen icons, names, grids — used in the [Craft Constructor](#craft-constructor). | Before the first craft with omens. |
| 6 | [💰 Currency setup](#currency-setup) | Capture of currency orb icons — used in the [Craft Constructor](#craft-constructor). | Before the first craft. |
| 7 | 🛠 Craft Constructor | The sequence of crafting stages: order, on/off, orbs and omens ([details](#craft-constructor)). | Configure what to craft with and how. |
| 8 | ⚖ Price rules… | Goes to "Settings → Pricing rules": the "cheaper than N chaos → vendor" thresholds, age discounts and so on. | Configure the pricing policy. |
| 9 | ⛔ Craft only (no selling) | With no relocation destination, the program simply stops after crafting. With a destination, it prices results and continues the keep-or-reroll cycle. | Craft without listing for sale. |
| 10 | 📐 all 1×1 | All items in the sources take one cell — the program skips the size checks (faster). An item larger than 1×1 will break the layout. | Only if there are no large items in the sources. |
| 11 | Speed: | Cursor speed: 1x–3x. | Start at 1x, speed up once everything is stable. |
| 12 | 🛒 Vendor the junk | Sell cheap stuff (below the Pricing rules threshold) to the NPC vendor near Ange. Off — cheap items return to the stash. | To avoid hoarding illiquid items. |
| 13 | ⇢ After stopping → Price re-check | When the cycle finishes on its own, "Price re-check & repricing" starts automatically. | You leave the program working for a long time. |
| 14 | ▶ Start | Starts the autonomous cycle. | When everything is set up and the game is open. |
| 15 | ⏸ Pause | Pause: the current safe step finishes, then the program waits. | You need to step in briefly. |
| 16 | ■ Stop | Requests a stop; the current atomic operation finishes safely. | Finish the work. |

**How "Move valuable items to" works.** Enable "Craft only", open the
checklist and select at least one destination tab. At the bottom of the window,
set the "Move items worth at least" threshold and choose its currency. After
every craft pass, the program prices the items directly in the craft tab,
converts each result to its chaos equivalent using the current exchange rate,
and moves results worth at least the threshold. For example, a `50 chaos`
threshold also accepts an item priced at `5 divine` when its equivalent is
above 50 chaos. The remaining items stay in the source for another pass.

A source and destination cannot be the same physical tab. When selling is
enabled, the relocation route is ignored. The cycle stops safely when the
source/currency runs out, the destination fills up, or an item cannot be priced
or moved reliably.

#### 2.1.2 The "Evaluate & list for sale" block

Prices items from the source tabs against the market and lists them across
the shops: reading the sources → moving to the inventory → pricing →
distribution across the shops.

![Evaluate & list for sale block](img_en/mgmt_eval_sell.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | 🗂 Categories | Which categories to price/sell: Maps, Rings, Amulets, Belts, Jewels, Tablets. | Limit a run to one category. |
| 2 | Sections: Sources | Which stash tabs to take items from. | Choose the tabs to sell from. |
| 3 | Targets | Which shops to list into. A marked-up shop accepts only its own categories. | Limit the shops. |
| 4 | ⚖ Price rules… | Goes to "Settings → Pricing rules". | Configure thresholds and discounts. |
| 5 | 🛒 Vendor the junk | Sell cheap items to the NPC after listing. Off — they return to the stash. | To avoid hoarding illiquid items. |
| 6 | 📐 all 1×1 | Do not check item sizes before moving (faster). | Only if everything in the sources is 1×1. |
| 7 | 📦 No price → | Where to put items without a price: "(auto)" — the first enabled "no price" tab; if there is none, the items return to the source. | Usually leave "(auto)". |
| 8 | ⇢ After selling → Price re-check | Start the price watching automatically after selling. | You leave the program for a long time. |
| 9 | 🚀 Start pricing/selling | The full cycle: reading → pricing → listing. With "👁 pricing only" checked, the button turns into "🔍 Start pricing (preview)". | The block's main button. |
| 10 | 👁 pricing only | Only scanning and prices, without moving or listing; the plan appears in "Shop → Price preview". | See the prices before selling. |
| 11 | ■ Stop | Stops the run. | Interrupt the work. |
| 12 | 📊 Preview | Opens "Shop → Price preview". | View the pricing plan. |
| 13 | 📤 List by plan | Happy with the preview? Starts a normal live run: the items are rescanned and the prices recalculated at listing time. | After reviewing the preview. |
| 14 | 💰 Price the stash | Prices ALL items in the currently open stash tab. Nothing gets listed — the result goes to "Prices → Pre-sale". Open the tab you need in the game before starting. | Spot-pricing of a single tab. |
| 15 | speed: | Item reading speed (1x–3x) for "Price the stash", "🎒 Price the inventory", and verification before listing. | Speed up once everything is stable. |
| 16 | 🎒 Price the inventory | Prices all items in the character's inventory (open the inventory with the I key). The result goes to Pre-sale. | Price the loot in your bag. |
| 17 | 🔬 Check under cursor | Waits 3 seconds, reads the one item under the mouse and finds a price. The result goes to Pre-sale. | Quickly ask the price of one item. |
| 18 | 📤 List items | Lists the accumulated Pre-sale. The items must sit in the same cells where they were scanned — the program verifies each one before listing. | After "Price the stash/inventory". |

#### 2.1.3 The "Price re-check & repricing" block

Watches your listed items: reconciles the shops with the database,
re-checks the prices by the Pricing rules and reprices aged listings;
junk can go to the vendor. Runs continuously until you stop it.

![Price re-check & repricing block](img_en/mgmt_reprice.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | 🏷 Item types… | Which types to reprice (maps, rings, amulets, belts, jewels, tablets). Empty = all. | Limit the repricing. |
| 2 | ☑ Tabs… | Which shops to re-check in. Empty = all enabled. | Limit the shops. |
| 3 | ⏱ Listing age… | The age thresholds window: from what listing age to start the discounts and in what steps. | Configure "when to lower". |
| 4 | ⚖ Price rules… | Goes to "Settings → Pricing rules". | Configure "how much to lower". |
| 5 | 🗺 Maps: price by properties | Reprices the listed maps by their general properties (tier, rarity…), ignoring the mods — usually gives a lower price. The price only goes down. | Maps sit unsold for a long time — enable it and the listings will sell. |
| 6 | 🔎 verify prices | Reads the real in-game tooltip prices and updates the database before building a plan. This respects manual price changes. Off — the plan starts immediately from saved data. | Keep it on for reliability; turn it off for the fastest start only when prices were not changed manually. |
| 7 | 🛒 Vendor the junk | Sends listings classified as junk by the price rules to the NPC instead of returning them to a shop. | Free shop space from cheap items. |
| 8 | 👁 preview only | Builds the repricing plan and shows it in "Shop → Price preview" — the prices are not changed. | Review the plan before applying. |
| 9 | speed: | Shop reading and verification speed (1x–3x). | Speed up a stable verification. |
| 10 | ✓ Verify listings | Explicitly reconciles shops with the database: finds sold/missing listings and synchronizes actual prices. It does not move prices. | Tidy the database and capture manual price changes. |
| 11 | 📊 Preview | Opens "Shop → Price preview". | View the plan (filled by "👁 preview only"). |
| 12 | ✅ Reprice by plan | Apply the plan from the preview: the program opens the shops and moves the prices. | After reviewing the preview. |
| 13 | ▶ Start | The continuous loop: reprices only listings that are old enough. | The main mode. |
| 14 | ① one pass | Finish after one pass instead of waiting for the next interval. | A single automatic check. |
| 15 | ↻ Reprice now | One pass right away over all selected shops, without waiting for the age. | Refresh all prices once. |
| 16 | ⏸ Pause / ■ Stop | Pause/stop the loop. | Control the run. |

### 2.2 Prices

Item pricing and work with the database of priced items. On the left —
"Items", on the right — the market search results.

![Prices tab](img_en/tab_prices.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | ⟳ League/Rates | Refresh the league name and the currency rates (also refreshes on its own at startup). | If the rate is stale. |
| 2 | ⚖ Price rules | Goes to "Settings → Pricing rules" (smart-search settings, repricing, listing age). | Configure the pricing. |
| 3 | "On sale" tab | Listings currently listed in the shops (per the program's database). | See what is on sale. |
| 4 | "Pre-sale" tab | Priced items waiting to be listed: the results of "Price the stash/tab/inventory" land here. | Check the prices before "📤 List items". |
| 5 | ⟳ Refresh | Re-read the list from the database (does not touch the game); the list also refreshes on its own. | Manual re-check. |
| 6 | 🗑 Delete | Delete the selected records from the program's database (listings in the game are not touched). The Delete key does the same. | Clean up the list. |
| 7 | 🔎 Find in inventory | Scans the in-game inventory once, matches items to already saved Pre-sale or active-shop records and refreshes their coordinates. It does not price, list or move items. | When an item was moved into the inventory and must be linked to its saved record again. |
| 8 | Highlight | Highlight the selected items with a frame right in the game — using the saved coordinates. | Quickly find a listing in a shop/stash. |
| 9 | 💰 Price: from … to … + × | Filter the list by price in the selected currency; "×" — reset. | See only the expensive/cheap items. |
| 10 | 💰 Price (smart search) | Automatic pricing of the selected item: the program builds the market queries itself — from exact (all mods) to simplified, until enough similar listings are found. | The main pricing button. |
| 11 | ⚙ Filters ▸ | Show/hide the "Search filters" column (manual search, query fine-tuning). Not needed for regular pricing. | Advanced manual search. |
| 12 | "Found on market" tab | Items found on the market during the last price check. Matched mods are highlighted green; the pricing result is at the bottom. "Expand all" / "Collapse all" — expand/collapse the mod rows. | Check what the price was compared against. |
| 13 | "Pricing variants" tab | How "💰 Price" arrived at the price: query variants from exact to simplified; ★ — the variant the price was taken from. Click — details, double-click — show what it found. | Understand the price; pick another variant. |
| 14 | 🌐 Open on trade site | Open this same search in the browser on the official PoE2 trade site. | Double-check the market with your own eyes. |

For jewels, the manual **Search filters** column has a separate
**"Crafted mods:"** block. Crafted effects in the details of a found market
listing are shown with the **"Craft:"** prefix, so they are not confused with
the item's regular explicit mods. The **Pricing rules → Smart search** card
also contains the jewel option that keeps a crafted prefix/suffix-effect mod
as an anchor while trying nearby search variants.

![Prices: Pricing variants](img_en/prices_variants.png)

![Prices: Found on market](img_en/prices_market.png)

### 2.3 Shop

All the listings of your shop and the plan previews. Subtabs: "Listings"
and "Price preview".

![Shop tab — Listings](img_en/tab_shop_lots.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | ⟳ Refresh | Re-read the listing list from the database (does not touch the game). | Manual re-check. |
| 2 | Show sold | Also show the sold and unlisted listings (history). | View the sales statistics. |
| 3 | shop: | Filter by a single shop; the number in parentheses is how many listings are currently listed. | Work with a specific shop. |
| 4 | 💰 Price: from … to … + × | Filter by listing price; "×" — reset. | Find expensive/cheap listings. |
| 5 | ⏱ Listing age… | The age thresholds window for "Price re-check". | Configure when to lower the prices. |
| 6 | "total / selected / total" counters | The count and the total price of the listings (select with Ctrl/Shift+click, Ctrl+A). | Estimate the shop's value. |
| 7 | ⓘ hints | A cheat sheet: right-click a row — menu (edit price, price lock, unlist…); double-click the Price cell — edit the price; click a header — sort. | Quick operations on listings. |
| 8 | Listings table | All listings with prices and age. The 🔒 lock (right-click → price lock) protects a listing's price from the re-check. | The main list. |
| 9 | ⚙ Shop maintenance | A collapsed section: "✏ Edit the selected listing's price", "🧹 Unlist selected", "🧹 Unlist all active (in DB)", "delete automatically at startup", "older than (days):", "🧹 Delete old sold…". Only the database records change — items in the game are not touched. | Manual cleanup after you cleared the shop yourself. |
| 10 | ▶ Log | The tab's operation log. | Follow the operations. |

![Shop tab — Price preview](img_en/shop_preview.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | shop: | Preview filter by shop; "(вкладка)" — the results of "Price the stash". | View the plan piece by piece. |
| 2 | ⟳ Refresh | Re-read the preview from the cache. | After a new run with "👁 … only". |
| 3 | Preview table | The plan: what the tools would reprice/list and at what prices. Prices are not changed from here. Columns — below. | Check the plan before applying. |
| 4 | ✅ Reprice by plan | Apply the preview to the already listed items (the program opens the shops and moves the prices). | After "👁 preview only". |
| 5 | 📤 List by plan | List what the preview shows: starts a live "Evaluate & list for sale" run. | After "👁 pricing only". |
| 6 | ▶ Log | The page log (collapsed by default). | Follow the application progress. |

Preview table columns (click a header to sort):

| Column | Meaning |
|---|---|
| Act | The action: `reprice` (blue) — move the price; `vendor` (orange) — unlist and sell to the NPC; `skip` (grey) — leave alone (too young, price-locked 🔒 etc.). |
| Shop / Cell | The item's shop and cell (column,row). |
| Name | The item; "(вкладка)" in the shop filter — the results of "Price the stash" for the open tab. |
| Tier | Waystone tier (empty for other items). |
| Old / New | The listing's current price → the planned price. |
| Reason | Why exactly: an age rule, a discount, "below floor → vendor", "just applied", a manual price and so on. |

### 2.4 Log

The program's full technical journal.

![Log tab](img_en/tab_log.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | Log field | All program messages; pricing results and applied reprices are highlighted in color. Right-click — copy. | Figure out what the program was doing. |
| 2 | Clear | Clears the log field (the file is not touched). | Start watching from a clean slate. |
| 3 | Copy all | Copies the whole log to the clipboard. | Send a piece of the log to support. |
| 4 | 💾 save the log | Write the log to a file (needed for "📤 Export log" / "📨 Send log to server"). | Keep it enabled. |
| 5 | 🐞 DEBUG logs | The verbose journal level. | When [support](#support) asks for it. |

### 2.5 Search

Search for market sellers who have LOTS of the items you need — for bulk
buyouts (waystones, jewels, tablets).

![Search tab](img_en/tab_search.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | Templates: + 💾 Save as / ✏ Overwrite / 🗑 Delete / ↺ Reset | Filter sets: save the current filters as a new template, overwrite, delete, restore the defaults. | Switch between typical searches quickly. |
| 2 | Mode: | What to look for: "tablets", "maps" or "jewels". The filters change with the mode and are remembered separately. | Pick the mode first. |
| 3 | Filters (Tier / Rarity / Corrupted / Tablet types / Jewel bases) | Which items count as matching. The checklists show selected/total. | Narrow the search. |
| 4 | Trade type / Price: … to / Min. items | The currency and price range of the listings; how many matching items a seller must have to make the list. | Set the "big seller" threshold. |
| 5 | 🔍 Find sellers | Starts the search: first distinct sellers are collected, then each seller's matching items are counted. | The tab's main button. |
| 6 | "Sellers" table | The sellers found: how many matching items, type, minimum price. | Choose whom to buy from. |
| 7 | "Selected seller's items" table | The selected seller's items with prices. | Assess the assortment. |
| 8 | 🌐 Seller on site | Open ALL the seller's listings in the browser on the trade site (double-clicking the row does the same). Traveling to a seller requires the POESESSID cookie (Settings → General). | Buy in bulk on the site. |

After a bulk-buying session that took the character through other players'
hideouts, restart the game before crafting. Hideout transitions can leave the
game in a state where crafting clicks are accepted inconsistently; a clean
start reduces that risk.

### 2.6 Settings

#### 2.6.1 General

![Settings — General](img_en/settings_general.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | Program language: + ✔ Apply and restart | Russian or English interface; applies after a restart. | Change the interface language. |
| 2 | Game language: | The language your PoE 2 client runs in (affects item reading). After switching, recapture the stash/Ange labels and the tab snapshots. | If you play on the English client. |
| 3 | League + ✔ Apply and restart | Choose a league from the loaded list (including concurrent active leagues and Standard); Refresh list reloads available leagues. Listings, tabs and the rate are reloaded for the selected league after a restart. | Start of a new season. |
| 3a | Price server: Address | Official address: https://tradeforge.download. | Check the address after a server migration. |
| 4 | POESESSID: | The pathofexile.com session cookie. Needed ONLY for traveling to sellers from Search; prices work without it. | Optional. |
| 5 | Version + ⬇ Check for updates | Asks the server whether a new version is out; if so, "🚀 Download & install" appears (settings and license are kept). | From time to time. |
| 6 | 🧙 Setup wizard… | Opens the [step-by-step wizard](#quick-start). | Reconfigure from scratch. |
| 6a | 📖 Manual | Opens this manual in the browser — in the program's language. | Quickly check the instructions. |
| 7 | 📤 Export log | Save the latest log file to disk. | Attach the log manually. |
| 8 | 📨 Send log to server | Send the log to the developer via the server: pick the latest file (several with Ctrl+click) and describe the problem in your own words. | When contacting support. |
| 9 | 💬 Discord | Opens the primary community and support server. | Questions, support and news. |
| 10 | ✈ Telegram | Opens the license, payment and fallback-request bot. | Buy or renew a key. |
| 11 | 🌐 GitHub | Opens the official repository with releases and the changelog. | Download a build or review changes. |
| 12 | 🐞 Debug mode | The verbose journal to a file. Enable it, reproduce the problem, send the log. | When support asks for it. |
| 13 | 💡 Tooltips | Hover tooltips — across the whole program. | Turn off once you know everything. |
| 14 | ☑ Launch preflight checks | Shows a final confirmation summary before live program actions and seller search: selected tabs, mode, important parameters and warnings. | Keep enabled until the workflow is familiar. |
| 15 | ↺ Reset hidden windows | Clears remembered "do not show again" choices and restores previously hidden warnings and helper dialogs. It does not change settings, tabs or listings. | When an expected confirmation or warning no longer appears. |

The **Controls** panel on this page shows the global Pause/Resume and Stop
keys, lets you rebind them, and enables the cursor stop corner (top-right by
default). It also reports whether the global hotkey listener is working. The
**Launch preflight checks** switch controls the confirmation summaries shown
before live tools and seller search; keep them enabled until the workflow is
familiar. See [Safety](#safety).

#### 2.6.2 License & server

![Settings — License & server](img_en/settings_license_server.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | License status / Valid until | The key's state and validity period. | Check how much time is left. |
| 2 | Key + Activate | Enter and activate a new `TF-…` key (right-click → Paste or Ctrl+V). | License renewal. |
| 3 | Address: | The price server address, for example `http://192.168.1.10:8777` (provided by the seller). | Set/change the server. |
| 4 | Price source: | "server" — all price requests go through the server (recommended, no proxies needed); "own proxies" — direct requests through your pool. | Usually "server". |
| 5 | fall back to own proxies | If the server is unreachable, temporarily switch to your proxy pool. | Only if you have your own proxies. |
| 6 | Own proxies: use the pool + counter | Your personal proxy pool (the program does not provide proxies). | Optional, for advanced users. |
| 7 | Add field + ➕ Add | Add proxies one per line: `host:port`, `host:port:user:pass` or `http://user:pass@host:port`. | Filling the pool. |
| 8 | Pool test | A window that tests YOUR proxies: health, speed, external IP; "⏹ Stop" aborts the test. | After adding proxies. |
| 9 | ⟳ / Delete selected | Refresh the pool table; delete the selected rows. | Pool maintenance. |

#### 2.6.3 Stash & Shops

The full setup of stash tabs and shops: roles, rules, calibration. The
wizard (section 1.3) is the quick minimum; here you get full control.

![Settings — Stash & Shops](img_en/settings_sections.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | 📍 Stash / 📍 Ange | Point out the stash chest and the NPC Ange by the label above them (frame the "Stash" label / the "Ange" name; character nearby, panels closed). Keep the stash and Ange close together in the hideout — the character must reach both without moving (see the tip in 1.3, step 5). | First-time setup; after changing the game language. |
| 2 | In-game tab view | A preview of the tab strip as in the game; right-click a tab — menu (for example "📂 Folder"). | Quick layout editing. |
| 3 | Tab list | All records: role, tab, on ("✓"/"—"). Double-click — on/off. | Overview of the layout. |
| 4 | Tab in game: | Any tab name works (the program finds tabs by snapshots); matching the in-game name is just more convenient. Renaming carries the calibration over. | When adding/renaming. |
| 5 | Folder: | Which folder-tab the tab lives in (the program opens the folder first). "(none)" — top level. | If your tabs are grouped into folders. |
| 6 | Note: / Category: / 🗂 Categories | A free-form note and the tab's category markup (which categories live in this tab / the shop accepts). | Layouts like "rings → their own shop" and so on. |
| 7 | ▶ Shop settings (prices, currencies, overflow) | THIS shop's rules: "Base lot currency", "🪙 Listing currencies" (allowed listing currencies), "Currency switch threshold", "Priority:", "Price from:"/"to:" (only listings within this range get into the shop), "fill first (target shop)", "overflow shop (for leftovers)", "pre-vendor — cheap stuff at a fixed price" + "fixed price:" and "to NPC after (h):". | Precise routing of listings across shops and currencies. |
| 8 | ✚ Add / 💾 Save / ✕ Delete | Create a record from the form; save the edits; delete the selected one. Everything is saved immediately. | Record management. |
| 9 | ⏻ Toggle tab on/off | Whether the program uses the selected tab. | Temporarily exclude a tab. |
| 10 | ↑ / ↓ | The row order = the program's traversal priority. | The shop fill order. |
| 11 | 📸 Photograph the tab… | The "selected"/"not selected" snapshots + the click point ("① by frame"). | Calibration of every tab. |
| 12 | ✏ Set coordinates (3s) | Remember where to click the tab: press and, within 3 seconds, hover the mouse over the tab in the game. If a point is already saved you get a confirmation prompt (to just check the point — "Check: ◎ Coordinates"). | An alternative to "① by frame". |
| 13 | Check: ◎ Coordinates / 🔍 "Selected" view / 🔍 "Not selected" view | Check the calibration against the live game: a circle at the click point; snapshot match with the game (score and verdict). | After the calibration and on failures. |

The tab type (role) is not chosen anywhere in the form — it is set by
which "+" button you added the tab with: "+ tab" in the stash strip adds
a source tab, "+ no price" adds a "no price" tab, and "+ tab" in the
Ange (shop) strip adds a shop. The "+" button opens a popup: enter the
tab name (any works; matching the game is just easier) and, optionally,
a note; "✚ Add and 📸
photograph…" creates the record and immediately opens the snapshot and
click-point capture (the game must be visible on screen), while "✚ Add"
only creates the record — you can photograph later.

**How to add a new folder or tab.** In the in-game tab preview, right-click
the required place. You can add a top-level tab or folder, or add a tab to an
existing folder. In the add dialog:

1. Enter the same name as in the game. Matching is not required for
   recognition, but makes the setup much easier to verify.
2. Add a clear note if needed.
3. Press **"✚ Add and 📸 photograph…"** to save the record and immediately
   open the capture window. **"✚ Add"** creates the record without snapshots.

![Adding a new stash folder or tab](img_en/settings_sections_add_tab.png)

**How to capture the tab and save its coordinates.** The numbers in the next
figure show the order:

1. Open the required tab in the game.
2. In the capture window press **"Refresh screenshot"**.
3. Click the required tab in the screenshot to place the frame.
4. Press **"Move to frame"** and fit the frame tightly around the tab.
5. While that tab is open in the game, press **"Save: tab selected"**.
6. Open a neighbouring tab in the game, repeat steps 2–4, then press
   **"Save: tab not selected"**. The frame must remain on the tab being
   configured while another tab is selected in the game.
7. Check the frame and press **"Coordinates (from frame)"**. The program will
   click the centre of the saved area.

When a frame already exists, **"Refresh screenshot"** preserves the zoom,
viewport position and frame. For the second state, simply switch tabs in the
game and refresh the image; the **"zoom"** button still explicitly returns to
the full screenshot.

![Tab capture workflow](img_en/settings_sections_capture_steps.annotated.png)

In the enlarged view, the frame tightly covers the tab label. Avoid extra
background and neighbouring tabs: a precise frame makes state detection more
reliable.

![Frame around the tab being configured](img_en/settings_sections_capture_frame.png)

For the "tab not selected" snapshot, switch to a neighbouring tab in the
game, refresh the screenshot and leave the frame on the tab being configured.
Then save the **"tab not selected"** state.

![Tab in the not-selected state](img_en/settings_sections_capture_inactive.png)

When there are many tabs and the navigation list appears on the right, put
the frame and click point on the tab's row in that list. Pin the list with the
padlock and keep it open while the program works.

![Calibrating a tab by the right-side navigation list](img_en/settings_sections_capture_menu.png)

> ✅ After capturing, always run all three checks at the bottom of the page:
> **"◎ Coordinates"**, **"🔍 Selected view"** and
> **"🔍 Not selected view"**. The coordinate must land inside the tab, and
> both snapshots must report **"Snapshot is suitable"**. If a check fails,
> recapture that state and run the check again.

**Listing currencies** are configured separately for each shop. In
"🪙 Listing currencies", tick only the currencies the program is allowed to use for
that shop: for example, if Exalted is unchecked and Chaos + Divine stay enabled,
the price is converted to one of the allowed currencies before listing, and the
program will not select exalted in the in-game dropdown. "Base lot currency" is the
normal/default choice for regular prices; when the price reaches the "Currency
switch threshold", the program switches to a more expensive allowed currency if
one exists. "Price from/to" remains the routing filter: it decides whether the
listing goes into this shop, while listing currencies decide which currency is
entered for that listing.

> ⚠ **Many tabs — calibrate by the right-side menu.** If there is a
> navigation list to the right of the tab row in-game (it appears when
> the tabs no longer fit in the row), do "📸 Photograph the tab…" and
> "① Coordinates" by the rows of that list, not by the top row: tabs in
> the row shift when clicked and the program will start missing. The list
> rows always stay in place. The list must also be open while the program
> works — pin it with the padlock. If the list appeared later (you got
> more tabs) — recalibrate the already configured tabs by it.

#### 2.6.4 Captures & templates

All the image capture tools in one place. The program finds objects and tabs
by the saved snapshots — if something "is not found", come here.

![Settings — Captures & templates](img_en/settings_capture.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | 📍 Stash + ◎ Test | Recapture the "Stash" label above the chest; the test shows with a circle where the program will click. | "Stash not found". |
| 2 | 📍 Ange + ◎ Test | Recapture the "Ange" name above the NPC; the test shows the click point. | "Ange not found". |
| 3 | [🔮 Omen setup](#omen-setup) | Capture of omen icons from the game (names, grids) — for the [Craft Constructor](#craft-constructor). | Add a new omen. |
| 4 | [💰 Currency setup](#currency-setup) | Capture of currency orb icons (alchemy, chaos, exalt, jewel oils and so on). | Add a new currency. |
| 5 | 📸 Tab snapshots → "Stash & Shops" | Tab snapshots are tied to a specific tab — the button leads to "[Stash & Shops](#stash-shops)". | Recapture a tab's view. |

#### 2.6.5 Pricing rules

Everything that pricing, selling and the price re-check follow.

![Settings — Pricing rules](img_en/settings_price_rules.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | Rate: 1 div = + ⟳ Refresh rate | The current divine → chaos conversion rate. | Rate check. |
| 2 | 🗺 Maps + ⚙ Configure… | The map rules editor: the "cheaper than N chaos → vendor" thresholds, the junk tier, age discounts, div steps for expensive maps, safety price caps. | Map trading setup. |
| 3 | 💍 Items (general) + ⚙ Configure… | The general item rules: "Step %" "every … hours", the lower price bound (floor), "Below floor →", "Min listings", "Strategy", "expensive" in div — the base for the groups. | Item trading setup. |
| 4 | 🗂 Item groups + ⚙ Configure… | Separate numbers per group (rings, belts…); empty fields inherit from the general rules. "Reset to inherited" restores the inheritance. | Fine-tuning by type. |
| 5 | ⏱ Listing age + ⚙ Configure… | When to reprice: the minimum listing age, discounts/steps per hours. The same fields as in the "Maps"/"Items"/"Groups" editors — they change in sync. | Price re-check setup. |
| 6 | 🔍 Smart search + ⚙ Configure… | Smart-search options for waystones ("By mods and stats" or "By stats only") and jewels (keep the crafted prefix/suffix-effect mod as a search anchor). | Tune the accuracy/speed trade-off and crafted-jewel matching. |

### 2.7 Separate windows

#### 2.7.1 Craft Constructor

Opens from [Management](#management) ("🛠 Craft Constructor"). A craft plan is a list of
stages; each stage is currency passes (top to bottom) plus omens.

For ordinary, inexpensive orbs, set at least **×2**: a repeated click makes
the pass more tolerant of server lag or a click the game did not accept.
**Chaos and Divine are exceptions** — do not duplicate those clicks: an extra
Chaos can overwrite the result you wanted, and an extra Divine is costly and
can change the roll again. If crafting becomes unreliable after a bulk-buying
session in other players' hideouts, restart the game before crafting; a clean
game start plus ×2 for inexpensive orbs is usually more stable.

![Craft Constructor](img_en/win_craft_constructor.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | Stage list | The stages run in order. The checkbox — the stage takes part in crafting. | The window's main area. |
| 2 | ↑ / ↓ / delete (on a stage) | Move the stage earlier/later; delete the stage. | Order editing. |
| 3 | ≡ (on a currency) | Drag the currency row up/down — the pass order. | Pass order editing. |
| 4 | Currency row + "×N" | Which orb to click with and how many clicks per item (the row shows the currency's own name). The icon comes from [Currency setup](#currency-setup). | Use ×2 or more for ordinary inexpensive orbs; keep Chaos and Divine at the intended exact count. |
| 5 | ▲ / ▼ / ✖ (on a currency) | Move the currency earlier/later in the pass order; remove the currency from the stage. | Stage editing. |
| 6 | ➕ currency | Add a currency to the stage. | Extend the stage. |
| 7 | 🔮 Omens: … ("all active") | The omens come from [Omen setup](#omen-setup) (the active ones with assigned grids). | Check the lineup before crafting. |
| 8 | ➕ Stage | A new stage at the end of the list. | Add a crafting step. |
| 9 | ↺ Reset | Restore the standard cycle: whetstone → chaos + omens → vaal. | Start from a clean slate. |

#### 2.7.2 Omen setup

Opens from [Management](#management) or
[Captures & templates](#captures).

![Omen setup](img_en/win_omens.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | ⟳ Refresh snapshot / Screen capture | A fresh screenshot of the game window (or of the whole screen if the window is not found). | Before recapturing an icon. |
| 2 | ➕ Add omen / ▦ Save as omen | Save the framed area as the icon of a new omen. | Add an omen to the program. |
| 3 | Omen gallery, "active" checkbox | An active omen takes part in auto-crafting and is laid out on its own grid (one grid = one omen type). | Choose the omens for crafting. |
| 4 | ▭ frame / 📷 recap. | Place a frame of the omen's size and overwrite the icon. | The icon stopped being found. |
| 5 | 🔍 test / 🔦 highlight | Check whether the program finds the icon on the screen/in the inventory; show the search zones. | Diagnostics. |
| 6 | ▲ / ▼ / 🗑 | The order of moving to the inventory when crafting; delete the icon. | Fine-tuning. |

> ⚠ **When photographing currency and omens, frame only the item icon.**
> The frame must not include the stack count or any other numeric values:
> those numbers change, and the program may stop recognising the saved icon.

##### Currency setup

The "💰 Currency setup" window works the same way (without grids):
"➕ Add currency", "▦ Save as currency", "🔍 test", "🔦 highlight",
"📷 recap.", "🗑".

Treat **jewel oils as currency**: add and photograph them in Currency setup,
just like an orb. Conversely, anything that is activated before applying a
currency item and produces an omen/effect belongs in **Omen setup**; give it
an icon and, when required, its own grid there.

![Currency setup](img_en/win_currency.png)

#### 2.7.3 Categories

The "Categories for pricing/selling" window (the "🗂 Categories" button
in the "Evaluate & list for sale" block) — a checklist: Maps, Rings,
Amulets, Belts, Jewels, Tablets. The selection gates both the selling and
the price holding; where things get listed is decided by the
"🗂 Categories" markup on the shops in "Stash & Shops" ("Select all" /
"Clear all" / "Done").

![Categories window](img_en/win_categories.png)

#### 2.7.4 Sources and Targets

The "Sources (stash)" and "Targets (shops)" buttons open tab checklists.
Sources — where to take items from; targets — which shops to list into
(shared with the auto-cycle's "Where to list"). The shop fill order is
set not here but by the row order in "Stash & Shops" (↑/↓).

![Sources/Targets window](img_en/win_pools.png)

#### 2.7.5 Listing age

The "⏱ Listing age…" window (opened from the Shop tab, the "Price
re-check & repricing" block and the card in "Pricing rules") gathers ALL
the age thresholds in one place. These are the same fields as in the
"Maps"/"Items"/"Groups" editors — they change in sync and save
immediately.

![Listing age window](img_en/win_age_rules.annotated.png)

| # | Element | What it does | When to use |
|---|---------|------------|--------------------|
| 1 | All listings: "Min. listing age … hours" | Younger listings are not touched at all — the price gets time to "sit". A common gate for maps and items. | The main "when to start" threshold. |
| 2 | Maps: "Age discount: from … to … %" | An aged map is repriced by a random discount from the "from..to" % range of its current price. Expensive maps follow the div thresholds from the "Maps" editor. | How much to lower maps. |
| 3 | Items: "lower by … % every … hours" | An item gets X% cheaper for every N-hour age step. The same rule covers "unknown" types that fall into no group. | The item price decay speed. |
| 4 | Item groups + "🗂 Open groups…" | A group (rings/amulets/belts/jewels/tablets) may have its own "% every N hours" step; empty — it inherits the items rule above. The button opens the groups editor. | Fine-tuning per type. |

#### 2.7.6 Proxy pool test

The "Pool test" window ("Settings → License & server"): each of your
proxies makes a light test request; "alive" — the external IP and the
response time are shown. Up to 20 proxies at once; "⏹ Stop" aborts the
test. The trade site is not touched by this test.

![Pool test window](img_en/win_proxy_test.png)

---

## 3. Recommendations for getting started

### Limits and speed

- The market request rate is controlled by the **price server**: it gives
  the program its allowed number of parallel requests and the per-minute
  quota. If pricing runs slower than usual, it is usually server load,
  not a breakage; just wait.
- Start the **click** speed ("Speed:" and "speed:" in the Management
  blocks) at 1x. Move to 2x–3x only when runs pass consistently without
  misses: at high speeds the program may skip an item or a cell.
- Do not run two tools at once — work in turns: crafting → selling →
  price re-check.

### Trading scheme

A proven sequence:

1. **List by mods at a higher price.** Regular pricing ("by mods and
   stats") gives a higher price — try to sell expensive first.
2. **Stuck?** Listings sit without sales — enable the
   "🗺 Maps: price by properties" box in "Price re-check & repricing" and
   run a pass.
3. **Repricing by properties — it sells.** The maps get repriced against
   the broad market (usually cheaper, the price only goes down) — and the
   listings start selling.

Don't cling to the cheap stuff: "🛒 Vendor the junk" + the thresholds in
the Pricing rules free up space and time.

### Safety

#### Game-account ban risk

TradeForge is an independent third-party automation tool. It is not affiliated
with, endorsed by or supported by Grinding Gear Games. Section 7 of the Path
of Exile and Path of Exile 2 Terms of Use prohibits automated software or bots
without GGG's prior written approval. Using TradeForge can therefore result in
a temporary or permanent game-account ban. There is no safe mode or guaranteed
allowed runtime.

- Do not run the program around the clock. Our conservative recommendation for
  users who knowingly accept the risk is no more than **8–12 total operating
  hours per day**, with breaks and supervision. This is not a GGG rule, a
  "safe limit," or protection from a ban.
- Do not treat a virtual machine as protection. A VM does not make automation
  permitted or undetectable. Use a separate physical PC only when you need to
  keep your main desktop available.
- A dedicated IP, VPN or proxy may provide technical network separation, but
  it does not make automation permitted or guarantee account safety. Proxies
  configured inside TradeForge are for price queries and **do not change the
  PoE 2 game client's IP address**.
- Do not experiment with automation on a valuable main account. A separate
  account can limit the value exposed, but it does not prevent sanctions and
  must not be used to evade an existing ban.
- 24/7 operation is not recommended. Rotating two or three PoE 2 accounts does
  not make it safe or GGG-approved and may increase the overall risk.
- TradeForge can work with any PoE 2 account and its license key is not bound
  to a game account. One TradeForge key is sufficient for sequential use on
  one licensed installation; parallel runs are still subject to the license
  and active-session limits.

Only GGG determines its current rules. Read the official
[PoE/PoE 2 Terms of Use](https://www.pathofexile.com/legal/terms-of-use-and-privacy-policy)
before using the program.

#### Operational safety

- **Do not touch the mouse and keyboard** while the program works: it controls
  both. The PC is occupied until the run is paused or stopped.
- **F8** pauses the program; press **F8** again to continue. After a pause,
  bring the game window back to the foreground before continuing.
- **F9** stops the active run. Wait for the short
  **"The program has stopped."** message before taking over the mouse.
- **Emergency stop** — move the pointer into the **top-right corner** of the
  screen by default. The stop corner and the F8/F9 bindings are configurable
  in **Settings → General → Controls**.
- **Do not cover the game window** with other windows and do not minimize
  it: the program "sees" the screen and must see the game.
- Close the chat and extra panels in the game: a covered inventory or
  cell is a typical cause of misses.
- Keep the stash and Ange close together in the hideout: the character
  must be able to activate both without moving — the program clicks the
  labels from where the character stands.
- Play in windowed mode at 1024×768 — the program cannot work in fullscreen
  or with any other window size (the start is blocked with a warning).
- During item placement, moving to the inventory or selling junk to a vendor,
  server lag can leave an item **stuck to the pointer**. The program has
  protective checks and tries to put the item down safely. Do not panic or
  jerk the mouse away; wait for the program to pause or stop, then inspect the
  inventory and stash.
- If you are not prepared to accept the account-ban risk, do not run the
  automation.

---

## 4. Troubleshooting / FAQ

**"Game window not found" or the size is not 1024×768.**

- **What it means:** the program cannot see the Path of Exile 2 window, or
  its size does not match the only supported calibration size. A live run is
  blocked instead of clicking at unsafe coordinates.
- **What to check:** the game is running, visible and set to **Windowed,
  1024×768**. Borderless/fullscreen and every other size are unsupported.
- **Where to go / action:** open the [setup wizard](#quick-start) → "Game
  window" → "🔍 Find game window". Correct the game display settings and run
  the check again.

**The stash or Ange is not found.**

- **What it means:** the saved label image no longer matches what is visible
  in the game.
- **What to check:** the character is standing close enough, panels and chat
  do not cover the label, and the game language has not changed.
- **Where to go / action:** [Settings → Captures & templates](#captures)
  → "📍 Stash" or "📍 Ange" → recapture the label → "◎ Test". Recapture both
  labels after changing the game language.

**A stash/shop tab is not selected, does not open, or its snapshot does not
match.**

- **What it means:** the program cannot confirm the tab's selected/not-selected
  state or its click point no longer lands on the tab.
- **What to check:** the correct folder is saved, both snapshots belong to
  this tab, and the click point is current. With many tabs, the right-side
  navigation list must stay pinned open.
- **Where to go / action:** [Settings → Stash & Shops](#stash-shops) → select
  the tab → "📸 Photograph the tab…" and "① Coordinates" → test "◎
  Coordinates" and both "🔍 … view" snapshots. Calibrate by the pinned
  right-side list rows when the top row shifts.

**The source is empty, disabled or not selected.**

- **What it means:** the run found no suitable items in its selected source
  tabs. For a waystone-only craft plan, this may still appear as "No maps to
  craft".
- **What to check:** the source contains items for the chosen category/plan,
  is enabled, has valid calibration, and is ticked in the run's "Sources"
  list.
- **Where to go / action:** configure the tab in [Stash & Shops](#stash-shops),
  then open [Management](#management) and select it under "Sources". Put the
  expected items into the tab before retrying.

**No target/receiver shop is selected.**

- **What it means:** the program has nowhere allowed to list the current item
  category. A waystone-specific run may say "No shop for maps".
- **What to check:** at least one enabled shop is ticked under "Targets" and
  its "🗂 Categories" accepts the item category; also check that the shop is
  not full.
- **Where to go / action:** [Stash & Shops](#stash-shops) → select the shop →
  "🗂 Categories", then [Management](#management) → "Targets" / "Where to
  list" and tick that shop.

**"Not enough currency or omens".**

- **What it means:** the stock pre-check cannot supply the complete craft plan.
- **What to check:** required stacks and active omen grids exist, Currency
  setup/Omen setup recognise their icons, and the plan does not ask for more
  clicks than intended.
- **Where to go / action:** restock or recapture the items in
  [Currency setup](#currency-setup) and [Omen setup](#omen-setup), or reduce
  the [Craft Constructor](#craft-constructor) plan.

**An item "has no price" or no similar market listings were found.**

- **What it means:** none of the safe search variants produced enough useful
  comparisons; it does not mean the item is worthless.
- **What to check:** item reading is correct, the league/rate and server are
  available, and the "Pricing variants" / "Found on market" details do not
  show an overly narrow filter.
- **Where to go / action:** inspect the item in [Prices](#prices), try the
  smart price again or open the query on the trade site. Keep a calibrated
  "no price" tab available; if it is full, clear it before retrying.

**Items were left in the inventory after a run.**

- **What it means:** the program stopped rather than guessing where unresolved
  items belong. Lag, a full target, a failed tab check or an item stuck to the
  pointer can cause this.
- **What to check:** the pointer is empty, the stash and targets have room,
  and the last messages in the [Management log](#management) identify the
  failed item or tab.
- **Where to go / action:** after the run has fully stopped, put the items away
  manually and start with an empty inventory. Fix the named tab/target before
  retrying.

**"Auto-cycle stopped: no progress" or "repeated errors".**

- **What it means:** an iteration changed nothing, or several guarded steps
  failed in a row, so continuing would be unsafe.
- **What to check:** sources are not empty, targets are not full, tabs open
  reliably, and enough currency/omens remain.
- **Where to go / action:** read the expandable log in
  [Management](#management). Correct the first reported cause; if it repeats,
  enable Debug mode and follow the [diagnostic log instructions](#faq).

**The currency rate or price server is unavailable.**

- **What it means:** market pricing and price conversion cannot continue with
  a trustworthy rate. A server update or network interruption may be temporary.
- **What to check:** internet access, the server address, license state and
  league. If you selected own proxies, test that pool too.
- **Where to go / action:** Settings → License & server → "Test connection",
  then [Management](#management) → "⟳" by Currency rates. Wait and retry if
  the server is under maintenance.

**Seller search takes several minutes.**

- **What it means:** this is often normal. The program walks the full requested
  price range to get beyond the market's 100-result limit, then verifies each
  seller with separate requests.
- **What to check:** progress above the seller table is still changing and the
  price server remains reachable. Seller search does not click in the game.
- **Where to go / action:** review the launch preflight before pressing
  "Continue"; it shows the range, seller checks and expected behavior. Narrow
  the price range or raise "Min. items" in [Search](#search) if the request is
  unnecessarily broad.

**The program stopped after F9, the STOP file or the stop corner.**

- **What it means:** a safety stop was requested. The current guarded action
  exits as soon as it is safe to do so.
- **What to check:** whether F9 was pressed, the pointer entered the configured
  stop corner, or another stop control created the STOP file.
- **Where to go / action:** wait for **"The program has stopped."**, inspect
  the inventory/pointer, then restart the tool. Change the keys or corner in
  Settings → General → Controls; see [Safety](#safety).

**After F8 pause, the game lost focus.**

- **What it means:** the program is waiting, but another window became active;
  continuing while that window is in front could send input to the wrong place.
- **What to check:** the game is visible, unblocked and still 1024×768; the
  pointer is not holding an item.
- **Where to go / action:** activate the game window, then press **F8** again.
  If the state is unclear, use **F9**, wait for the stop message and restart
  the run from [Management](#management).

**"The key is already in use by another copy" or the license is inactive.**

- **What it means:** one key is already attached to another running copy, has
  expired, or has not been activated.
- **What to check:** TradeForge is closed on the other PC and the entered key
  is current. A closed copy may take a few minutes to release the key.
- **Where to go / action:** license window → "⟳ Retry check", or Settings →
  License & server → enter the new key → "Activate".

**How to enable Debug mode and send the right log to support.**

- **What it means:** support needs a short verbose recording of the failing
  run, not only a screenshot or an old log.
- **What to check:** "💾 save the log" is enabled in the [Log](#log) tab and
  the reproduced run is short enough to identify the problem clearly.
- **Where to go / action:** Settings → General → enable "🐞 Debug mode" →
  reproduce the problem once → "📨 Send log to server" → select the latest
  file and describe the action and expected result. Alternatively, "📤 Export
  log" saves it for a message through the [support contacts](#support).

---

## 5. Contacts

- Discord: https://discord.gg/UtU9Ty2bBv
- Telegram license and payment bot: https://t.me/TradeForgePoE2Bot
- Website and price server: https://tradeforge.download
- GitHub — releases, quick starts and changelog: https://github.com/Svetl286/TradeForge-PoE2

Primary support is provided in Discord. If Discord is unavailable, the
Telegram bot can accept a fallback request and forward it to the team, but
automated replies inside Telegram are not available yet.

The Discord, Telegram and GitHub buttons are also in the program itself: in
the license window at startup and under "Settings → General → Support".

When contacting support, state the program version
("Settings → General → Support") and attach the log (see "How to send
the log to support").
