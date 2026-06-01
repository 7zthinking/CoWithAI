# coWithAI

> 与 AI 协作的技能与工具集合

## 这是什么

存放可复用的 AI 协作规范、技能、工具。每个 skill 都是自包含的——可直接拿走使用，无需额外上下文。

## 项目结构

```
coWithAI/
├── README.md                    # 本文件
├── INDEX.md                     # 全部 skill / tool 索引
├── CHANGELOG.md                 # 项目变更记录
├── skills/                      # Skill 集合
│   └── <skill-name>/
│       ├── SKILL.md             # 核心内容
│       └── README.md            # skill 简介
├── tools/                       # 配套脚本、模板
├── docs/                        # 原理说明
└── examples/                    # 使用示例
```

## 命名规范

- skill / tool 文件夹用 kebab-case：`science-coding-protocol`
- 核心文件统一命名 `SKILL.md`
- 每个 skill 自带 `README.md`（对外介绍）+ `SKILL.md`（实际内容）
- 工具脚本放在 `tools/<skill-name>/<script>.py`

## 如何新增一个 skill

1. 在 `skills/<skill-name>/` 下创建文件夹
2. 写 `SKILL.md`（YAML frontmatter + 主体内容）
3. 写 `README.md`（skill 简介）
4. 在 `INDEX.md` 注册
5. 更新 `CHANGELOG.md`

## 如何使用一个 skill

直接读 `SKILL.md` 即可上手。每个 skill 都设计为：
- ✅ 自包含（不依赖外部上下文）
- ✅ 触发条件清晰（什么时候用）
- ✅ 行动明确（要做的事、不做的事）
- ✅ 可单独拷贝使用

## 协议

本项目采用 [MIT License](LICENSE) 开源（待补）。
