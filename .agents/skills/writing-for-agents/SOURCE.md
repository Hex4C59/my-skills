# writing-for-agents 来源记录

创建时间：未知（历史文档未记录）

修改时间：2026-10-11

- 来源类型：第三方修改版（Agent 文档结构整理与 humanizer 表达检查）。
- 作者 / 组织：Matt Pocock（mattpocock）。
- 官方项目：https://github.com/mattpocock/skills
- 具体 Skill 目录：https://github.com/mattpocock/skills/tree/49dd158d1076134a641b33efb035946536778336/skills/productivity/writing-for-agents
- 原版主文件下载：https://raw.githubusercontent.com/mattpocock/skills/49dd158d1076134a641b33efb035946536778336/skills/productivity/writing-for-agents/SKILL.md
- 官方固定提交源码包：https://codeload.github.com/mattpocock/skills/tar.gz/49dd158d1076134a641b33efb035946536778336
- 固定提交：`49dd158d1076134a641b33efb035946536778336`；上游提交时间：2026-10-09T10:56:49Z。
- 独立版本：上游未提供，以固定提交标识版本。
- 收录与本地修改日期：2026-10-11（Asia/Shanghai）。
- 许可证：MIT，署名 Matt Pocock，原文见 [LICENSE](LICENSE)。
- 上游主文件 SHA-256：`551adca942227b44192edba88acd4e8db911f0121ce58ad16944ccf6a896a74a`，对应 [references/writing-for-agents-original.md](references/writing-for-agents-original.md)。

## 本地文件与改动

- [SKILL.md](SKILL.md)：先整理 Agent 文档的结构、规则、引用条件和完成标准，再读取同级目录的 [humanizer](../humanizer/SKILL.md)，统一检查易懂程度与 AI 套话，最后复核含义和约束。
- [references/writing-for-agents-original.md](references/writing-for-agents-original.md)：上游主文件的逐字节副本，以普通参考文件名保存，避免被重复识别为同名 Skill。
- [references/SKILL-MECHANICS.md](references/SKILL-MECHANICS.md)：上游 Skill 格式说明的参考副本，仅调整返回主参考文件的相对链接；元数据与调用说明仍需结合目标工具实际支持情况使用。
- [agents/openai.yaml](agents/openai.yaml)：从上游界面元数据原样复制。
- [LICENSE](LICENSE)：同一提交的根许可证副本。

维护源位于 my-skills 的 `skills/writing-for-agents/`。维护源内的 `upstream/` 保留原始目录及内容；安装包只包含中文执行入口、来源记录、许可证、界面元数据和普通参考文件，安装目录只保留一个 `SKILL.md`。

## 同步与依赖

2026-10-11，按用户授权同步已安装本 Skill 的 Codex 项目，并在同级目录补齐当前 humanizer 修改版。无需额外程序依赖。后续先修改维护源，再同步上述安装文件；无需复制整份上游目录。

验证范围为入口格式、本地引用、参考原文和安装文件一致性。实际写作效果仍需在后续任务中核对。
