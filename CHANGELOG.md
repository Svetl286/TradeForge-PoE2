# TradeForge changelog

## 0.1.39 — 2026-08-01

- public HTTPS licensing, pricing relay and updater endpoint;
- SHA-256 verified installer download and atomic `.part` update flow;
- RU/EN user interface and game-client support;
- setup wizard, resolution preflight and centered dialogs;
- craft, pricing, pre-sale, shop routing and repricing workflows;
- configurable pause/resume/stop controls and stop corners;
- public RU/EN manuals and Telegram/Discord support links;
- hardened release pipeline with bundle secret audit and optional Cython stage.

Known limitations:

- the installer is not digitally code-signed;
- Auto fix/relogin remains disabled in the user edition;
- production cryptocurrency payment and automatic license fulfillment are not
  enabled;
- some game-dependent scenarios still require operator live validation after
  game updates.
