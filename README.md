# TradeForge for Path of Exile 2

[Русский](docs/QUICK_START_RU.md) · [English](docs/QUICK_START_EN.md) ·
[Telegram](https://t.me/TradeForgePoE2) ·
[Discord](https://discord.gg/UtU9Ty2bBv) ·
[Releases](https://github.com/Svetl286/TradeForge-PoE2/releases)

![TradeForge](assets/tradeforge-avatar.png)

TradeForge is a helper tool for Path of Exile 2: item preparation and crafting,
market pricing, shop routing, listing and price updates.

TradeForge — инструмент-помощник для Path of Exile 2: подготовки и крафта
предметов, оценки рынка, распределения по лавкам, выставления и обновления цен.

> This is a public showcase, documentation and binary release repository.
> The application source code is not published here and this repository is
> not an open-source distribution.

## Current release / Текущая версия

- Version: **0.1.39**
- Published: **2026-08-01**
- Installer: `TradeForge_Setup_0.1.39.exe`
- Size: **70,518,181 bytes**
- SHA-256: `A734574E7797E554F65E686E39334A579D6BA163329C8940DA90FE22743DCB4D`
- [Official VPS download](https://tradeforge.freelancepulse.work/api/v1/update/download?version=0.1.39)
- [GitHub Releases mirror](https://github.com/Svetl286/TradeForge-PoE2/releases/latest)

The VPS download is the canonical source used by the built-in updater. GitHub
Releases are a public mirror for release notes, hashes and manual downloads.

## What it does / Возможности

| Workflow | TradeForge capability |
|---|---|
| Crafting | Configurable stage constructor, currency and omen workflows |
| Pricing | Market search, cascading queries, listing comparison and saved variants |
| Selling | Pre-sale staging, shop routing, listing and low-value handling |
| Repricing | Rule-based and smart price updates, shop relocation workflows |
| Search / Поиск | Seller search by the required purchase quantity / Удобный поиск продавцов по нужному количеству закупаемого предмета |
| Control | Start, pause, resume, stop, progress, logs and preflight dialogs |
| Support | RU/EN interface, manuals, Telegram, Discord and explicit log submission |

![Management](assets/screenshots/en/tab_management.annotated.png)

![Prices](assets/screenshots/en/tab_prices.annotated.png)

### Seller search / Поиск предметов у продавцов

Set the minimum available item count to find sellers suitable for the required
purchase quantity.

Укажите минимальное количество предметов и найдите продавцов, у которых есть
нужный объём для закупки.

![Seller search by item quantity](assets/screenshots/ru/tab_search.annotated.png)

More screenshots: [feature gallery](docs/FEATURES.md).

## Requirements

- Windows 10/11, 64-bit;
- Path of Exile 2 game client;
- game client area exactly `1024×768`;
- Russian or English game client;
- internet access to the official TradeForge HTTPS service;
- a valid TradeForge license key.

## Safety and transparency

- Every release publishes an exact version, file size and SHA-256 hash.
- The public repository contains no account sessions, wallets, proxies,
  private keys, operator databases or source tree.
- The application installer is currently **not digitally code-signed**.
  Windows SmartScreen may therefore show a warning. Verify the SHA-256 before
  running it and download only from the official links above.
- TradeForge controls mouse and keyboard input, reads item text from the
  clipboard, captures configured screen regions and communicates with its
  HTTPS licensing/pricing service as part of its advertised functions.
- Full support logs are submitted only through the explicit in-app support
  action; never publish full logs, license keys or account cookies in Issues.

Read [Security](SECURITY.md), [Privacy](PRIVACY.md) and
[Verify a download](docs/VERIFY_DOWNLOAD.md) before installation.

## Important risk notice

TradeForge is an independent third-party automation tool and is not affiliated
with, endorsed by or supported by Grinding Gear Games. Automation may conflict
with the game's Terms of Use and can expose an account to restrictions or a
ban. TradeForge does not promise profit, undetectability, uninterrupted
operation or freedom from account action. Use it only after understanding and
accepting that account risk.

## Support and community

- News and manuals: https://t.me/TradeForgePoE2
- Support forum: https://t.me/TradeForgePoE2Support
- License/support bot: https://t.me/TradeForgePoE2Bot
- Discord: https://discord.gg/UtU9Ty2bBv
- Bugs and feature requests: [GitHub Issues](https://github.com/Svetl286/TradeForge-PoE2/issues)

Do not post license keys, payment data, tokens, POESESSID or full logs in a
public issue. Use the in-app support upload for logs.

## Third-party acknowledgements

TradeForge uses language/stat data derived from
[Exiled Exchange 2](https://github.com/Kvan7/Exiled-Exchange-2) under the MIT
License. This does not imply endorsement or partnership. See
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
