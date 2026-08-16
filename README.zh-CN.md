# Solenne — 档案精灵

[English](README.md)

英文名：**Solenne — Archive Familiar**

Solenne 是一只自定义 Codex 动画宠物。她是一位沉静的星辰学者、档案管理员与观察者，会在你工作时安静地阅读、分析并陪伴在旁。

![Solenne 角色总览](previews/solenne-overview.png)

## 特色

- 精致的动漫风 SD／Q 版设计，同时保持成熟学者气质
- 银白长发、圆框眼镜、蓝色眼睛、深海军蓝学者服装与星辰档案书
- 9 种 Codex 标准动画状态
- 16 个顺时针观察方向
- 透明背景、无损 WebP 精灵图集
- Codex v2 宠物格式（`spriteVersionNumber: 2`）

## 快速安装

把 `pet/solenne/` 中的两个文件复制到本地 Codex 宠物目录：

```text
pet.json
spritesheet.webp
```

目标目录：

- Windows：`%USERPROFILE%\.codex\pets\solenne\`
- macOS/Linux：`~/.codex/pets/solenne/`

如果宠物列表没有立即刷新，请重新启动桌面应用。完整步骤请阅读 [INSTALL.zh-CN.md](INSTALL.zh-CN.md)。

## 动画状态

| 状态 | 表现 |
| --- | --- |
| `idle` | 安静阅读、呼吸与眨眼 |
| `running-right` | 向屏幕右侧移动 |
| `running-left` | 向屏幕左侧移动 |
| `waving` | 克制地挥手问候 |
| `jumping` | 轻盈跳起或悬浮 |
| `failed` | 遇到错误时表现轻微担忧 |
| `waiting` | 等待批准或用户输入 |
| `running` | 主动阅读、分析与处理任务 |
| `review` | 检查已经完成的工作 |

第 9–10 行包含 16 个顺时针观察方向，从 `000`（向上）到 `337.5`（左上）。

## 发布包结构

```text
Solenne-Codex-Pet-v1.0.0/
├── pet/solenne/
│   ├── pet.json
│   └── spritesheet.webp
├── previews/
│   ├── solenne-overview.png
│   ├── contact-sheet.png
│   ├── look-directions.png
│   └── animations/*.gif
├── README.md
├── README.zh-CN.md
├── INSTALL.md
├── INSTALL.zh-CN.md
├── QA.md
├── LICENSE.md
└── SHA256SUMS.txt
```

## 技术规格

- 图集尺寸：`1536 × 2288`
- 网格：`8 × 11`
- 单帧尺寸：`192 × 208`
- 格式：无损 RGBA WebP
- 宠物 ID：`solenne`
- 精灵版本：`2`

发布图集已经通过结构验证，没有错误或警告。详情参见 [QA.md](QA.md)。

## 许可

这是一个采用自定义条款、并非开源的个人使用版本。在遵守 [LICENSE.md](LICENSE.md) 的前提下，允许个人非商业使用、截图、录制视频，以及原封不动地转载完整发布包。商业使用、销售、制作衍生宠物包，以及用于 AI／模型训练均需另行取得许可。

## 制作说明

Solenne 的角色身份以创作者提供的原创概念图为基础。Codex 宠物精灵、图集组装、验证和发布整理工作由 Codex 与图像生成工具在创作者指导下完成。
