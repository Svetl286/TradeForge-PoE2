# Verify your download / Проверка загрузки

Download the installer from [GitHub Releases](https://github.com/Svetl286/TradeForge-PoE2/releases/latest). The release page is the source for the exact version, filename, byte size and SHA-256. Do not compare a new installer against an older release's hash.

В [GitHub Releases](https://github.com/Svetl286/TradeForge-PoE2/releases/latest) скачайте установщик и возьмите имя, размер и SHA-256 с той же страницы. Хеш старой версии не подходит для новой.

Open PowerShell in the download folder / Откройте PowerShell в папке загрузки:

```powershell
# Replace X.Y.Z with the version you downloaded / Подставьте скачанную версию.
$installer = Get-Item -LiteralPath .\TradeForge_Setup_X.Y.Z.exe
$installer.Name
$installer.Length
Get-FileHash -LiteralPath $installer.FullName -Algorithm SHA256
```

All 64 hash characters must match (letter case does not matter). If the filename, size or hash differs, do not run the installer; download it again from the official release or contact support.

Все 64 символа хеша должны совпасть (регистр букв не важен). При несовпадении имени, размера или хеша не запускайте файл: скачайте его заново из официального релиза или обратитесь в поддержку.

The installer is not currently digitally signed, so Windows SmartScreen may show a warning. / Установщик пока не подписан цифровой подписью; Windows SmartScreen может показать предупреждение.

Support / Поддержка: [Discord](https://discord.gg/UtU9Ty2bBv), [Telegram bot](https://t.me/TradeForgePoE2Bot).
