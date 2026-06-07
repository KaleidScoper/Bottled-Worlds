# Bottled Worlds

多世界叙事工作区 —— 每个独立世界观在 `worlds/` 下自成体系，互不干扰。

## 使用方式

1. 终端进入某个世界目录，在该目录下启动 Claude Code：
   ```
   cd worlds/<世界名>
   claude
   ```
2. Claude Code 会自动加载该世界根目录的 `CLAUDE.md`，进入该世界的叙事上下文。
3. 用 `//续写`、`//新场景` 等快捷指令驱动写作（快捷键见各世界的 CLAUDE.md）。

## 世界索引

| 目录名 | 世界名称 | 基调 | 创建日期 | 备注 |
|--------|----------|------|----------|------|
| `example-world` | 示例世界 | 待定 | 2026-06-07 | 模板参考 |

## 新建世界

1. 复制模板目录到目标位置：
   ```
   cp -r _templates/ worlds/<新世界名>/
   ```
2. 填写新世界的 `CLAUDE.md`（写作规范部分）和 `world/overview.md`（核心设定）。
3. 更新本文件中的世界索引表。

## 目录结构

```
<世界名>/
├── CLAUDE.md              # 世界的 AI 协作配置（身份、规范、指令）
├── world/                 # 核心设定
│   ├── overview.md        # 世界概览
│   ├── rules.md           # 世界规则（硬规则 / 软规则）
│   └── timeline.md        # 时间线
├── characters/            # 角色档案
│   └── _index.md          # 角色索引
├── factions/              # 势力档案
│   └── _index.md          # 势力索引
├── locations/             # 地点档案
│   └── _index.md          # 地点索引
├── sessions/              # 写作会话记录
│   └── session_001.md
└── scratchpad.md          # 自由记录（非确认设定）
```
