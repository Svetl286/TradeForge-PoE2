# TradeForge changelog

## 1.0.0 — 2026-08-02

- first stable TradeForge release milestone;
- Cython-hardened licensing, application gate and pricing relay modules;
- one-pass shop repricing mode that respects listing age and reports completion;
- verified HTTPS updater metadata with exact filename, size and SHA-256;
- improved release delivery reliability through the official VPS mirror;
- RU/EN interface, manuals and seller search by required item quantity.

Known limitations remain unchanged: the installer is not digitally signed;
Auto fix/relogin is disabled; production cryptocurrency payments and automatic
license fulfillment are not enabled.

### Русский

- первый стабильный релизный рубеж TradeForge;
- Cython-защита модулей лицензирования, входа в программу и ценового relay;
- одноразовая перепроверка цен с соблюдением возраста лотов и уведомлением о
  завершении;
- проверяемые HTTPS-метаданные обновления: точное имя, размер и SHA-256;
- повышена надёжность доставки релиза через официальное VPS-зеркало;
- RU/EN-интерфейс, руководства и поиск продавцов по нужному количеству.

Ограничения прежние: установщик не подписан цифровой подписью;
Auto fix/relogin выключен; production-криптооплата и автоматическая выдача
лицензий не включены.

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

### Русский

- публичные HTTPS-сервисы лицензирования, цен и обновлений;
- проверка SHA-256 установщика и безопасное атомарное обновление через `.part`;
- RU/EN-интерфейс и поддержка русского/английского клиента игры;
- мастер настройки, проверка разрешения и центрированные диалоги;
- сценарии крафта, оценки, предпродажи, распределения по лавкам и репрайса;
- настраиваемые пауза, продолжение, остановка и аварийные углы;
- публичные RU/EN-руководства и ссылки на Telegram/Discord;
- усиленный release pipeline с аудитом секретов и опциональным Cython-этапом.

Известные ограничения: установщик не подписан цифровой подписью;
Auto fix/relogin выключен; production-криптооплата и автоматическая выдача
лицензий не включены; после обновлений игры отдельные сценарии требуют живой
повторной проверки.
