# Verify a TradeForge installer

Official releases publish the exact filename, byte size and SHA-256 hash.

For TradeForge `1.0.0`:

```text
Filename: TradeForge_Setup_1.0.0.exe
Size:     70008484 bytes
SHA-256:  5EA0FA9E1C15A87AF1BCB92E175189E118794B9A740F5BFD58774A42B374482B
```

PowerShell:

```powershell
Get-FileHash -LiteralPath .\TradeForge_Setup_1.0.0.exe -Algorithm SHA256
```

The returned hash must match all 64 hexadecimal characters. Delete the file
and contact support if the hash, filename or size differs.

The current installer is not digitally code-signed. A SmartScreen warning is
therefore possible even for the authentic file; SHA-256 verification is
especially important.

Official sources:

- https://github.com/Svetl286/TradeForge-PoE2/releases
- https://tradeforge.freelancepulse.work/api/v1/update/download?version=1.0.0
- https://t.me/TradeForgePoE2
- https://discord.gg/UtU9Ty2bBv

## Проверка установщика на русском

Официальный релиз всегда содержит точное имя файла, размер в байтах и
SHA-256. Для TradeForge `1.0.0` ожидаются значения из блока выше.

Откройте PowerShell в папке с установщиком и выполните:

```powershell
Get-FileHash -LiteralPath .\TradeForge_Setup_1.0.0.exe -Algorithm SHA256
```

Результат должен совпасть по всем 64 шестнадцатеричным символам. Если имя,
размер или SHA-256 отличаются, удалите файл и обратитесь в поддержку.

Установщик пока не подписан цифровой подписью, поэтому SmartScreen может
показать предупреждение даже для подлинного файла. Проверка SHA-256 особенно
важна; скачивайте программу только по официальным ссылкам выше.
