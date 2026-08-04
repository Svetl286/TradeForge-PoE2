# Verify a TradeForge installer

Official releases publish the exact filename, byte size and SHA-256 hash.

For TradeForge `1.0.0`:

```text
Filename: TradeForge_Setup_1.0.0.exe
Size:     70057824 bytes
SHA-256:  F53A52759B13DAAFCB2636EE22C1E5D09730E5D9C8CDE08D0B3208B06AC4C327
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
- https://t.me/TradeForgePoE2Bot
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
