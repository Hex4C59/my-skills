# git-commit 来源记录

- 来源类型：第三方修改版（添加中文收录入口和来源说明，上游主 Skill 未改动）。
- 作者 / 组织：GitHub / awesome-copilot 项目贡献者；根许可证署名 GitHub, Inc.。
- 原项目：https://github.com/github/awesome-copilot
- 原始 Skill 目录：https://github.com/github/awesome-copilot/tree/82701c24b99488536ca399ff4789a458b7a05db7/skills/git-commit
- 主文件下载：https://raw.githubusercontent.com/github/awesome-copilot/82701c24b99488536ca399ff4789a458b7a05db7/skills/git-commit/SKILL.md
- 官方仓库源码包：https://codeload.github.com/github/awesome-copilot/tar.gz/82701c24b99488536ca399ff4789a458b7a05db7
- 分支：`main`；固定提交：`82701c24b99488536ca399ff4789a458b7a05db7`。
- 上游提交时间：2026-10-09T05:48:57Z。
- 独立版本：上游主文件未提供，以固定提交标识版本。
- 收录及项目安装日期：2026-10-11（Asia/Shanghai）。
- 许可证：MIT，原文见 [LICENSE](LICENSE)。许可证从相同提交的上游仓库根目录原样保留。
- 原始 `SKILL.md` SHA-256：`554d1a3c6d95f15bc1170160659ecdc9a9958b64f377f3988941b672c249b13f`。

## 收录内容与本地改动

`upstream/SKILL.md` 是固定提交下完整的 `skills/git-commit/` 目录内容；该目录只有一个文件，没有附属脚本或资源。`upstream/LICENSE` 是从上游仓库根目录另外保留的许可证。本项收录具体 Skill 目录，不复制 awesome-copilot 仓库的其他 Skill。

顶层增加中文 `SKILL.md` 入口、`SOURCE.md` 和许可证副本；原版指令未翻译或改写。

## 项目安装

通过 skill-installer 的 `install-skill-from-github.py` 安装相同固定提交，目标为当前项目 [`.agents/skills/git-commit/`](../../.agents/skills/git-commit/SKILL.md)。安装版保留原版 `SKILL.md`，另外补充许可证和来源记录，详见[安装来源记录](../../.agents/skills/git-commit/SOURCE.md)。

依赖 Git CLI 与已初始化的目标 Git 仓库，不需要额外业务依赖。当前项目目录尚无 `.git`；本次检查安装结构和内容，不执行暂存、提交或 Git 初始化。提交规范草案仍待用户审查。
