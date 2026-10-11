# writing-for-agents 来源记录

- 来源类型：第三方修改版（仅添加中文收录入口、来源说明及根许可证副本；上游文件保持原样）。
- 作者 / 组织：Matt Pocock（mattpocock）。
- 官方项目：https://github.com/mattpocock/skills
- 具体 Skill 目录：https://github.com/mattpocock/skills/tree/49dd158d1076134a641b33efb035946536778336/skills/productivity/writing-for-agents
- 原版主文件下载：https://raw.githubusercontent.com/mattpocock/skills/49dd158d1076134a641b33efb035946536778336/skills/productivity/writing-for-agents/SKILL.md
- 官方固定提交源码包：https://codeload.github.com/mattpocock/skills/tar.gz/49dd158d1076134a641b33efb035946536778336
- 分支：`main`；固定提交：`49dd158d1076134a641b33efb035946536778336`。
- 上游提交时间：2026-10-09T10:56:49Z。
- 独立版本：上游主文件未提供，以固定提交标识版本。
- 收录及项目安装日期：2026-10-11（Asia/Shanghai）。
- 许可证：MIT，原文见 [LICENSE](LICENSE)。许可证来自同一提交的仓库根目录，署名 Matt Pocock。
- 原版主文件 SHA-256：`551adca942227b44192edba88acd4e8db911f0121ce58ad16944ccf6a896a74a`。

## 收录内容

`upstream/` 保留固定提交中完整的 `skills/productivity/writing-for-agents/` 目录，包含：

- [SKILL.md](upstream/SKILL.md)：主指令。
- [SKILL-MECHANICS.md](upstream/SKILL-MECHANICS.md)：Skill 元数据、调用和路由组织的参考。
- [agents/openai.yaml](upstream/agents/openai.yaml)：上游界面元数据。

另外从仓库根目录保留 [upstream/LICENSE](upstream/LICENSE)。仅收录这一项 Skill，不复制上游仓库的其他 Skill。顶层添加中文入口和来源记录，未翻译或改写上游文件。

## 项目安装

使用 skill-installer 的 `install-skill-from-github.py`，从相同固定提交安装到项目级 [`.agents/skills/writing-for-agents/`](../../.agents/skills/writing-for-agents/SKILL.md)。安装版原样保留上游 3 个文件，额外添加根许可证副本及来源记录，详见[安装来源记录](../../.agents/skills/writing-for-agents/SOURCE.md)。

本 Skill 无额外程序运行依赖。本次执行下载、安装及结构和内容检查；实际文档改写流程留待用户提出相应任务时使用。上游调用机制说明应结合目标宿主支持情况理解。
