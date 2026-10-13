# my-skills

个人在工作与编程中使用的 AI Agent Skill 源文件库，集中保存原创 Skill、收集的第三方 Skill，以及个人修改版。

Skill 是提供给 AI Agent 的任务说明，可以配套脚本、参考资料和资源文件。本仓库用于整理这些文件，保留使用说明、来源、版本和许可信息，方便查找、维护与复用。

## 查找和使用 Skill

[Skill 目录与使用说明](docs/skills.md)汇总了全部已收录 Skill 的用途、适用场景、使用示例、依赖与限制，并保留上游项目、下载地址、许可证和安装记录。

使用时先从目录中选择合适的 Skill，阅读对应的 `SKILL.md`，再按目标工具的要求安装或加载。存入本仓库的源文件不会自动安装到 Codex 或其他工具。

## 目录结构

```text
my-skills/
├── README.md               # 仓库介绍与文档入口
├── AGENTS.md               # 维护与协作规则
├── COMMIT_CONVENTION.md    # Git 提交信息规范草案
├── docs/
│   └── skills.md           # Skill 目录、详细介绍与使用说明
└── skills/
    └── <skill-name>/
        ├── SKILL.md        # Skill 入口
        ├── SOURCE.md       # 来源、版本及本地改动记录（按需）
        ├── scripts/        # 脚本（按需）
        ├── references/     # 参考资料（按需）
        └── assets/         # 资源文件（按需）
```

已安装到当前项目的 Skill 位于 `.agents/skills/`，具体版本与安装状态见[当前项目安装](docs/skills.md#当前项目安装)。

## 维护

新增或更新 Skill 时，遵循 [AGENTS.md](AGENTS.md)，同步更新 [Skill 目录](docs/skills.md)中的介绍与来源信息，并保留第三方署名和许可声明。

Git 提交信息规范见 [COMMIT_CONVENTION.md（草案，待审查）](COMMIT_CONVENTION.md)。
