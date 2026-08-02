# Verify a TradeForge installer

Official releases publish the exact filename, byte size and SHA-256 hash.

For TradeForge `0.1.39`:

```text
Filename: TradeForge_Setup_0.1.39.exe
Size:     70518181 bytes
SHA-256:  A734574E7797E554F65E686E39334A579D6BA163329C8940DA90FE22743DCB4D
```

PowerShell:

```powershell
Get-FileHash -LiteralPath .\TradeForge_Setup_0.1.39.exe -Algorithm SHA256
```

The returned hash must match all 64 hexadecimal characters. Delete the file
and contact support if the hash, filename or size differs.

The current installer is not digitally code-signed. A SmartScreen warning is
therefore possible even for the authentic file; SHA-256 verification is
especially important.

Official sources:

- https://github.com/Svetl286/TradeForge-PoE2/releases
- https://tradeforge.freelancepulse.work/api/v1/update/download?version=0.1.39
- https://t.me/TradeForgePoE2
- https://discord.gg/UtU9Ty2bBv

## Проверка установщика на русском

Официальный релиз всегда содержит точное имя файла, размер в байтах и
SHA-256. Для TradeForge `0.1.39` ожидаются значения из блока выше.

Откройте PowerShell в папке с установщиком и выполните:

```powershell
Get-FileHash -LiteralPath .\TradeForge_Setup_0.1.39.exe -Algorithm SHA256
```

Результат должен совпасть по всем 64 шестнадцатеричным символам. Если имя,
размер или SHA-256 отличаются, удалите файл и обратитесь в поддержку.

Установщик пока не подписан цифровой подписью, поэтому SmartScreen может
показать предупреждение даже для подлинного файла. Проверка SHA-256 особенно
важна; скачивайте программу только по официальным ссылкам выше.
