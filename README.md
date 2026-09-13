# wa-team

Installs Worms Armageddon team and scheme files.

## Linux (Steam Flatpak)

```bash
base="$HOME/.var/app/com.valvesoftware.Steam/data/Steam/steamapps/common/Worms Armageddon/User"; \
mkdir -p "$base/Teams" "$base/Schemes"; \
curl -L -s https://raw.githubusercontent.com/house-of-vanity/wa-team/main/WG.WGT -o "$base/Teams/WG.WGT"; \
curl -L -s https://raw.githubusercontent.com/house-of-vanity/wa-team/main/oldfag.wsc -o "$base/Schemes/oldfag.wsc"
```

## Windows

Run in PowerShell:

```powershell
$base="C:\Program Files (x86)\Steam\steamapps\common\Worms Armageddon\User"; New-Item -ItemType Directory -Force -Path "$base\Teams","$base\Schemes" | Out-Null; Invoke-WebRequest -Uri "https://raw.githubusercontent.com/house-of-vanity/wa-team/main/WG.WGT" -OutFile "$base\Teams\WG.WGT"; Invoke-WebRequest -Uri "https://raw.githubusercontent.com/house-of-vanity/wa-team/main/oldfag.wsc" -OutFile "$base\Schemes\oldfag.wsc"
```
