# humanizer 来源记录

- 来源类型：第三方修改版（中文技术表达、AI 套话检查与来源说明，`upstream/` 中的上游文件未改动）。
- 作者 / 组织：Siqi Chen（blader）。
- 官方项目：https://github.com/blader/humanizer
- 主 Skill 固定版本：https://github.com/blader/humanizer/blob/225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8/SKILL.md
- 官方下载地址：https://codeload.github.com/blader/humanizer/tar.gz/225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8
- 分支：`main`（下载时通过 GitHub API 解析到下面的固定提交）。
- 提交：`225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8`。
- 版本标识：SKILL 元数据 3.1.0。
- 收录日期：2026-10-11（Asia/Shanghai）。
- 上游根许可证：MIT，原文见 [upstream/LICENSE](upstream/LICENSE)，入口目录另保留一份 [LICENSE](LICENSE)。上游子目录中的其他许可证及声明也随快照保留。
- 原始下载包 SHA-256：`1375ce268d42b898a5526011218fa5bac3273db793e7245cb1ad9ca525b6ed6b`。

## 本地收录方式

- `upstream/` 保存该提交的完整仓库源码快照，保留原始目录、署名、脚本、数据、参考资料和仓库内符号链接；不含 `.git` 历史或本地安装产物。
- 顶层 `SKILL.md` 是中文执行入口，合并本次用户确认的中文技术表达规则，并读取上游规则完成 AI 套话检查。原版文件、脚本和完整源码快照未改动。
- `references/humanizer-original.md` 是上游 `SKILL.md` 的逐字节副本，供执行入口读取。使用普通参考文件名，安装目录不增加第二个 `SKILL.md`。
- `agents/openai.yaml` 提供本地修改版的界面说明。
- 顶层 `SOURCE.md` 记录来源和本地包装；顶层 `LICENSE` 是上游根许可证的原样副本。
- 上游仓库可能还包含其他 Skill 和宿主适配；它们作为原始源码的一部分保留，不表示已在本机安装。

## 依赖与验证边界

主要依赖语言模型，无专用脚本运行依赖；原版说明以英文为主。

最初收录仅下载并检查源文件。2026-10-11 的本次整理检查了入口格式、本地引用、上游原文及维护源与安装副本的一致性，未运行辅助脚本或完整业务流程；后续写作效果仍需在实际任务中验证。

## 后续项目安装记录

2026-10-11，按用户授权将此版本安装到项目级 [`.agents/skills/humanizer/`](../../.agents/skills/humanizer/SKILL.md)，安装详情见[安装来源记录](../../.agents/skills/humanizer/SOURCE.md)。源码快照保持原样。

## 中文表达规则合并

2026-10-11，按用户确认的精简方案，将此前为 writing-clearly-and-concisely 编写的本地中文表达规则并入 humanizer，包括读者背景、首次术语解释、具体行为、按需举例、技术准确性及交付前检查。该扩展来自本次对话中用户确认的修改稿，不复制另一项目的英文参考书或上游 Skill 指令，也不将其许可声明用于本 Skill。

writing-for-agents 继续调用 humanizer，负责 Agent 指令文档的结构与约束；humanizer 统一负责易懂程度和 AI 套话检查。writing-clearly-and-concisely 的源码保留作参考，当前项目安装已撤下。

维护时先修改本目录，再同步 `SKILL.md`、`references/humanizer-original.md` 和 `agents/openai.yaml` 到目标 Skill 目录，并附上许可证及安装来源记录。完整上游辅助文件保留在维护源，旧安装文件在本次同步前已备份；无需复制整份 `upstream/` 快照到安装目录。

## 跨项目同步

2026-10-11，按用户授权检查 Codex 已保存项目，将已安装的 humanizer 副本和本机用户级副本同步为当前修改版，并为使用 writing-for-agents 的项目补齐同级 humanizer。安装包包括中文执行入口、上游规则参考、许可证、界面说明和安装来源记录；上游完整源码继续保存在维护源，不作为另一个 Skill 安装。
