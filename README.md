# TradeForge for Path of Exile 2

[English](README.md) · [Русский](README_RU.md) ·
[Quick start](docs/QUICK_START_EN.md) ·
[Telegram Bot](https://t.me/TradeForgePoE2Bot) ·
[Discord](https://discord.gg/UtU9Ty2bBv) ·
[Releases](https://github.com/Svetl286/TradeForge-PoE2/releases)

![TradeForge](assets/tradeforge-avatar.png)

TradeForge is a helper tool for Path of Exile 2: item preparation and crafting,
market pricing, shop routing, listing and price updates.

> This is a public showcase, documentation and binary release repository.
> The application source code is not published here and this repository is
> not an open-source distribution.

## Current release

- Version: **1.0.0**
- Published: **2026-08-02**
- Installer: `TradeForge_Setup_1.0.0.exe`
- Size: **70,008,484 bytes**
- SHA-256: `5EA0FA9E1C15A87AF1BCB92E175189E118794B9A740F5BFD58774A42B374482B`
- [Official VPS download](https://tradeforge.freelancepulse.work/api/v1/update/download?version=1.0.0)
- [GitHub Releases mirror](https://github.com/Svetl286/TradeForge-PoE2/releases/latest)

The VPS download is the canonical source used by the built-in updater. GitHub
Releases are a public mirror for release notes, hashes and manual downloads.

## What it does

| Workflow | TradeForge capability |
|---|---|
| Crafting | Configurable stage constructor, currency and omen workflows |
| Pricing | Market search, cascading queries, listing comparison and saved variants |
| Selling | Pre-sale staging, shop routing, listing and low-value handling |
| Repricing | Rule-based and smart price updates and shop relocation workflows |
| Seller search | Convenient seller search by the required purchase quantity |
| Control | Start, pause, resume, stop, progress, logs and preflight dialogs |
| Support | RU/EN interface, manuals, Telegram bot, Discord and explicit log submission |

![Management](assets/screenshots/en/tab_management.annotated.png)

![Prices](assets/screenshots/en/tab_prices.annotated.png)

### Seller search by item quantity

Set the minimum available item count to find sellers suitable for the required
purchase quantity.

![Seller search by item quantity](assets/screenshots/en/tab_search.annotated.png)

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
  private keys, operator databases or private source tree.
- The installer is currently **not digitally code-signed**. Windows
  SmartScreen may therefore display a warning. Verify SHA-256 before running
  it and download only from the official links above.
- As part of its advertised functions, TradeForge can control mouse and
  keyboard input, read item text from the clipboard, capture configured screen
  regions and communicate with the official HTTPS licensing/pricing service.
- Full support logs are submitted only through the explicit in-app support
  action. Never publish full logs, license keys or account cookies in Issues.

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

- Telegram license/payment/support bot: https://t.me/TradeForgePoE2Bot
- Discord: https://discord.gg/UtU9Ty2bBv
- Bugs and feature requests: [GitHub Issues](https://github.com/Svetl286/TradeForge-PoE2/issues)

Do not post license keys, payment data, tokens, POESESSID or full logs in a
public Issue. Use the in-app support upload for logs.

## Third-party acknowledgements

TradeForge uses language/stat data derived from
[Exiled Exchange 2](https://github.com/Kvan7/Exiled-Exchange-2) under the MIT
License. This does not imply endorsement or partnership. See
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
