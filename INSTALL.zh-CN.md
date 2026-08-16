# 安装说明

## Windows

1. 解压发布 ZIP。
2. 在解压后的 `Solenne-Codex-Pet-v1.0.0` 文件夹中打开 PowerShell。
3. 运行：

```powershell
$source = Join-Path (Get-Location) 'pet\solenne'
$target = Join-Path $env:USERPROFILE '.codex\pets\solenne'
New-Item -ItemType Directory -Path $target -Force | Out-Null
Copy-Item -LiteralPath (Join-Path $source 'pet.json') -Destination $target -Force
Copy-Item -LiteralPath (Join-Path $source 'spritesheet.webp') -Destination $target -Force
```

4. 如果宠物选择列表没有立即出现 Solenne，请重新启动桌面应用。

如果已经安装过旧版 Solenne，建议先备份原来的文件夹，再执行以上覆盖命令。

## macOS 或 Linux

在解压后的发布文件夹中运行：

```bash
mkdir -p ~/.codex/pets/solenne
cp pet/solenne/pet.json ~/.codex/pets/solenne/
cp pet/solenne/spritesheet.webp ~/.codex/pets/solenne/
```

如果宠物列表没有立即刷新，请重新启动桌面应用。

## 手动安装

在 `.codex/pets/` 下创建名为 `solenne` 的文件夹，然后把 `pet.json` 和 `spritesheet.webp` 直接放入其中。最终结构必须是：

```text
.codex/
└── pets/
    └── solenne/
        ├── pet.json
        └── spritesheet.webp
```

## 安装检查

- `pet.json` 和 `spritesheet.webp` 必须位于同一个文件夹。
- `pet.json` 必须包含 `"spriteVersionNumber": 2`。
- `spritesheet.webp` 必须是带透明通道的 `1536 × 2288` 图像。
- 如果宠物没有出现，请重启桌面应用，并确认文件夹名称准确地写作 `solenne`。

