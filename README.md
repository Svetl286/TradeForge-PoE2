<div align="center">

<img src="assets/tradeforge-banner.png" alt="TradeForge for Path of Exile 2" width="100%">

# ⚒️ TradeForge for Path of Exile 2

### Trading, Crafting & Shop Management Assistant

### 🔨 CRAFT • 🔍 FIND • 💎 PRICE • 🏷️ LIST • 📉 REPRICE

<br>

## 💎 Built for high-volume trading with minimal manual involvement

**Configure the strategy. Review the results. Let TradeForge handle the repetitive work.**

<br>

[English](README.md) ·
[Русский](README_RU.md) ·
[Quick Start](docs/QUICK_START_EN.md) ·
[Releases](https://github.com/Svetl286/TradeForge-PoE2/releases) ·
[Telegram](https://t.me/TradeForgePoE2Bot) ·
[Discord](https://discord.gg/UtU9Ty2bBv)

</div>

> **💎 100+ Divine Orbs/day potential\***<br>
> TradeForge is designed to support high-volume crafting and trading strategies with minimal repetitive manual work.
>
> **\* This is potential, not guaranteed profit.** Actual results depend on market conditions, strategy, available capital, items and configuration.

> **⚠️ Independent third-party software.**<br>
> TradeForge is not affiliated with, endorsed by or supported by Grinding Gear Games. Automation can conflict with the game's Terms of Use and creates account risk, including possible restrictions. Read the [Important Risk Notice](#important-risk-notice) before use.

---

## ⚡ One Tool. One Trading Workflow.

<div align="center">

### 🔨 CRAFT → 🔍 FIND → 💎 PRICE → 👁️ REVIEW → 🏷️ LIST → 📉 REPRICE

**Less repetitive work. More time for strategy.**

</div>

TradeForge brings the repetitive parts of a Path of Exile 2 trading workflow into one interface.

Create your rules and reusable configurations, review the important decisions, and let TradeForge carry out the configured routine in the game window.

The individual tools can be used separately or connected into a longer workflow.

This repository is a public product showcase, documentation hub and binary-release channel. The private application source code is not published here, and this is not an open-source distribution.

---

## ✨ Why TradeForge?

| Without TradeForge | With TradeForge |
|---|---|
| 🔨 Repeat the same crafting sequence | 💾 Run a saved Craft Constructor plan |
| 🔍 Browse many separate market offers | 👥 Group matching offers by seller |
| 📦 Search manually for bulk stock | 🔎 Find sellers by available quantity |
| 💰 Compare market listings manually | 💎 Run an automatic market estimate |
| 📦 Move items between tabs manually | 🏪 Route items using configured shop rules |
| 🏷️ Prepare repetitive listing actions | ⚡ Apply listing rules in batches |
| 📉 Check old listings one by one | 🔄 Recheck and reprice using your rules |
| 🔁 Repeat the entire routine | ⚙️ Connect the stages into one workflow |

---

# 🔨 Configurable Crafting

## Build your own repeatable crafting plan

With **Craft Constructor**, you decide exactly how the crafting sequence should work.

You can configure:

- stage order;
- enable or disable individual stages;
- currency used at each stage;
- number of applications;
- omens assigned to specific stages;
- additional crafting stages;
- separate templates for different strategies.

<div align="center">

### CONFIGURE → SAVE → RUN

</div>

<div align="center">

![TradeForge Craft Constructor](assets/tradeforge_craft_clean_highlights.gif)

</div>

The saved plan is executed through the configured stash tabs.

This is especially useful when the same crafting process needs to be repeated across a batch of items.

**Build the process once. Save it. Reuse it when you need it.**

More UI examples: [English Feature Gallery](docs/FEATURES.md).

---

# 🔍 Seller Search by Item Quantity

## Don't search for one item. Find the sellers with the largest available stock.

For bulk purchasing, the cheapest individual listing is not always the most useful result.

Often the important question is:

<div align="center">

### 📦 Which sellers have the most matching items available?

</div>

TradeForge lets you configure:

- the item and search filters;
- currency;
- price or price range;
- desired number of sellers;
- minimum number of matching items per seller.

TradeForge collects matching offers, groups them by seller and shows how much suitable stock each seller has.

<div align="center">

### 🔍 FIND OFFERS
### ↓
### 👥 GROUP BY SELLER
### ↓
### 📦 COUNT MATCHING ITEMS
### ↓
### 🏆 FIND THE LARGEST STOCK

</div>

![Seller search by item quantity](assets/screenshots/en/tab_search.annotated.png)

### 🛒 Built for bulk purchasing

Instead of manually opening many unrelated listings, you can quickly identify one or several sellers with the largest available stock.

The **Open seller on website** action opens the selected seller's offers on the trading website so you can continue the purchase normally.

> **TradeForge does not purchase items on your behalf.**<br>
> It helps find, group and open suitable seller offers. The purchase itself remains under your control.

---

# 💎 Automatic Market Estimate

## Compare an item with the market before listing it

TradeForge reads supported items from a selected stash tab or inventory and searches for comparable market offers.

The search begins with closer matches and can gradually broaden when there is not enough useful comparison data.

<div align="center">

### 📦 ITEM
### ↓
### 🔍 MARKET COMPARISON
### ↓
### 💎 ESTIMATED PRICE
### ↓
### 👁️ REVIEW

</div>

![Market pricing](assets/screenshots/en/tab_prices.annotated.png)

## 🧠 Smart Search

TradeForge attempts to find useful comparable offers instead of relying on a single listing.

When the initial search is too narrow, the query can be expanded to obtain additional market comparisons.

The result gives you a reference price before deciding what to do with the item.

### 👁️ Price Only / Pre-sale

Want to check the result first?

Use **Price Only / Pre-sale** mode.

TradeForge can:

1. read the item;
2. search for comparable market offers;
3. calculate an estimated market price;
4. place the result into the pre-sale table for review;
5. leave the item unlisted until you decide to continue.

**Evaluate first. Decide second. List only when you're ready.**

> Market estimates are indicative rather than guaranteed. Accuracy depends on the quantity and quality of available comparable offers.

---

# 🏷️ Listing & Shop Routing

## From reviewed price to prepared listing

Once you've reviewed the result, TradeForge can continue using your configured listing rules.

It can:

- read items from configured sources;
- move items through the configured workflow;
- apply category rules;
- apply price-range rules;
- route items to the appropriate configured shop tabs;
- prepare and place listings;
- record the result in program tables and logs.

<div align="center">

### 💎 EVALUATE → 👁️ REVIEW → 🏷️ LIST

</div>

![Shop and listing management](assets/screenshots/en/tab_management.annotated.png)

Different categories and price ranges can use different destinations and rules.

You keep the important approval point while TradeForge handles the repetitive listing routine according to your configuration.

---

# 📉 Rechecking & Repricing

## Listed doesn't mean forgotten

Market conditions change.

A listing that was competitive earlier may no longer match the current market.

TradeForge provides a separate workflow for checking existing listings and applying your repricing strategy.

You can configure:

- listing-age rules;
- repricing conditions;
- preview of proposed changes;
- category-specific rules;
- different rules for different shops;
- planned price changes for existing listings.

<div align="center">

### 🔎 CHECK → 💎 COMPARE → 👁️ PREVIEW → 📉 REPRICE

</div>

![Price rules](assets/screenshots/en/settings_sections.annotated.png)

This helps keep a larger inventory manageable without manually checking every old listing one by one.

---

# 🔄 One Connected Workflow

## Use each tool separately — or connect them

TradeForge's main systems can work independently.

They can also be combined into a longer scenario.

<div align="center">

### 🔨 CRAFT
### ↓
### 💎 PRICE
### ↓
### 👁️ REVIEW
### ↓
### 🏪 ROUTE
### ↓
### 🏷️ LIST
### ↓
### 📉 REPRICE

<br>

## You define the rules.

### TradeForge handles the repetitive work.

</div>

A connected workflow can:

1. check configured items and available resources;
2. run a saved Craft Constructor plan;
3. estimate the crafted results against the market;
4. place results into the pre-sale workflow for review;
5. route approved items to configured shops;
6. prepare and place listings;
7. later recheck existing listings and apply repricing rules.

You decide which stages are enabled and how they should behave.

---

<details>
<summary><b>⚙️ More TradeForge Features</b></summary>

<br>

### 💾 Reusable Templates

Save configurations for different workflows and reuse them when needed.

### 🎯 Categories & Price Ranges

Use different rules depending on item category, source, destination or price range.

### 🛡️ Preflight Checks

Review important settings before starting a live operation.

### 👁️ Preview Before Listing

Inspect calculated prices and prepared changes before allowing the workflow to continue.

### ⏸️ Pause & Resume

Pause an active workflow and continue when you're ready.

### ⛔ Normal Stop

Safely stop the current process.

### 🚨 Emergency Stop

Immediately interrupt active operations when necessary.

### 📊 Progress, Tables & Logs

Follow the current workflow through progress indicators, result tables and logs.

### 🌐 English & Russian

TradeForge includes English and Russian interfaces and documentation.

</details>

---

# 📦 What's Included

TradeForge includes:

- 🔨 Craft Constructor;
- 💾 reusable crafting templates;
- ✨ currency and omen configuration;
- 🔍 seller search;
- 📦 minimum seller-stock filtering;
- 👥 grouping offers by seller;
- 💎 automatic market estimation;
- 👁️ Price Only / Pre-sale review;
- 🏷️ listing workflow;
- 🏪 shop routing rules;
- 📉 rechecking and repricing;
- 🛡️ preflight checks;
- 🧭 initial setup and calibration;
- 📖 user documentation.

---

# 🔑 License Information

For current license options and availability, contact us through:

- [Discord](https://discord.gg/UtU9Ty2bBv)
- [Telegram](https://t.me/TradeForgePoE2Bot)

---

# 🚀 Download TradeForge

## Current Release: `1.0.0`

- **Installer:** `TradeForge_Setup_1.0.0.exe`
- **Published:** `2026-08-02`
- **Size:** `70,057,824 bytes`
- **SHA-256:** `F53A52759B13DAAFCB2636EE22C1E5D09730E5D9C8CDE08D0B3208B06AC4C327`

### Download

- [Official VPS Download](https://tradeforge.freelancepulse.work/api/v1/update/download?version=1.0.0)
- [GitHub Releases Mirror](https://github.com/Svetl286/TradeForge-PoE2/releases/latest)

The built-in updater tries the official VPS first.

If that route repeatedly fails, TradeForge uses the latest verified GitHub Release asset as an automatic fallback. Manual GitHub download remains available as a final option.

---

<details>
<summary><b>🛠️ System Requirements & Setup</b></summary>

<br>

TradeForge requires:

- Windows 10/11, 64-bit;
- Path of Exile 2;
- game client area exactly **1024×768**;
- Russian or English game client;
- internet access;
- a valid TradeForge license key;
- one-time setup and calibration before the first live run.

During live operations, TradeForge uses mouse and keyboard input and configured screen regions.

Keep the game window available and avoid conflicting mouse or keyboard input while an active workflow is running.

</details>

---

<details>
<summary><b>🔐 Safety & Transparency</b></summary>

<br>

For every release, TradeForge publishes:

- exact version;
- installer size;
- SHA-256 checksum;
- release information.

This public repository contains documentation, sanitized screenshots and release assets.

It does **not** contain:

- account sessions;
- wallets;
- private keys;
- proxy lists;
- operator databases;
- the private application source tree.

The installer is currently not digitally code-signed, so Windows SmartScreen may display a warning.

Verify the SHA-256 checksum and download TradeForge only from the official links provided in this repository.

Full support logs are submitted only through an explicit in-app action.

**Never post the following publicly in GitHub Issues:**

- license keys;
- account cookies;
- POESESSID;
- payment data;
- tokens;
- full support logs.

For additional information:

- [Security](SECURITY.md)
- [Privacy](PRIVACY.md)
- [Verify a Download](docs/VERIFY_DOWNLOAD.md)

</details>

---

# ⚠️ Important Risk Notice

TradeForge is an independent third-party automation tool.

It is **not affiliated with, endorsed by or supported by Grinding Gear Games**.

Automation may conflict with the game's Terms of Use and can expose an account to restrictions or a ban.

TradeForge does not promise:

- guaranteed profit;
- undetectability;
- uninterrupted operation;
- freedom from account action.

Use TradeForge only after understanding and accepting this risk.

---

# 💬 Support & Community

- **Discord — community and support:**<br>
  [Join Discord](https://discord.gg/UtU9Ty2bBv)

- **Telegram — licenses, payment and support:**<br>
  [Open Telegram](https://t.me/TradeForgePoE2Bot)

- **Bugs and feature requests:**<br>
  [GitHub Issues](https://github.com/Svetl286/TradeForge-PoE2/issues)

> Do not post license keys, payment data, tokens, POESESSID or full logs in a public Issue.

---

# 📚 Documentation

- [Quick Start](docs/QUICK_START_EN.md)
- [Feature Gallery](docs/FEATURES.md)
- [Known Issues](KNOWN_ISSUES.md)
- [Security](SECURITY.md)
- [Privacy](PRIVACY.md)
- [Third-Party Notices](THIRD_PARTY_NOTICES.md)
- [Changelog](CHANGELOG.md)

---

<details>
<summary><b>Search keywords</b></summary>

Path of Exile 2 tool, PoE2 trading, PoE2 crafting, market pricing, item valuation, seller quantity search, bulk purchase helper, shop listing, listing management, repricing, stash workflow, trade assistant.

</details>

## Third-Party Acknowledgements

TradeForge uses language and stat data derived from [Exiled Exchange 2](https://github.com/Kvan7/Exiled-Exchange-2) under the MIT License.

This does not imply endorsement or partnership.

See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

---

<div align="center">

# ⚒️ TradeForge

### 🔨 CRAFT • 🔍 FIND • 💎 PRICE • 🏷️ LIST • 📉 REPRICE

### Configure the strategy. Let TradeForge handle the repetitive work.

<br>

### 🚀 Ready to try TradeForge?

[**Download Latest Release**](https://github.com/Svetl286/TradeForge-PoE2/releases/latest)

<br>

[Quick Start](docs/QUICK_START_EN.md) ·
[Discord](https://discord.gg/UtU9Ty2bBv) ·
[Telegram](https://t.me/TradeForgePoE2Bot)

</div>
