# Installation

## Windows

1. Extract the release ZIP.
2. Open PowerShell inside the extracted `Solenne-Codex-Pet-v1.0.0` folder.
3. Run:

```powershell
$source = Join-Path (Get-Location) 'pet\solenne'
$target = Join-Path $env:USERPROFILE '.codex\pets\solenne'
New-Item -ItemType Directory -Path $target -Force | Out-Null
Copy-Item -LiteralPath (Join-Path $source 'pet.json') -Destination $target -Force
Copy-Item -LiteralPath (Join-Path $source 'spritesheet.webp') -Destination $target -Force
```

4. Restart the desktop app if Solenne is not immediately visible in the pet selector.

If an older Solenne installation exists, back up its folder before using the commands above.

## macOS or Linux

From inside the extracted release folder:

```bash
mkdir -p ~/.codex/pets/solenne
cp pet/solenne/pet.json ~/.codex/pets/solenne/
cp pet/solenne/spritesheet.webp ~/.codex/pets/solenne/
```

Restart the desktop app if the pet list does not refresh immediately.

## Manual installation

Create a folder named `solenne` under `.codex/pets/`, then place `pet.json` and `spritesheet.webp` directly inside it. The final layout must be:

```text
.codex/
└── pets/
    └── solenne/
        ├── pet.json
        └── spritesheet.webp
```

## Verification

- `pet.json` and `spritesheet.webp` must be in the same folder.
- `pet.json` must contain `"spriteVersionNumber": 2`.
- `spritesheet.webp` must be `1536 × 2288` with transparency.
- If the pet does not appear, restart the desktop app and confirm the directory name is exactly `solenne`.

