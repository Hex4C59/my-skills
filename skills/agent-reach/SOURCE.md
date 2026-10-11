# agent-reach 来源记录

- 来源类型：第三方修改版（仅添加中文收录入口与来源说明，`upstream/` 中的上游文件未改动）。
- 作者 / 组织：Panniantong / Neo Reid（pyproject.toml；许可证署名 Agent Eyes）。
- 官方项目：https://github.com/Panniantong/Agent-Reach
- 主 Skill 固定版本：https://github.com/Panniantong/Agent-Reach/blob/94f06c1969dfc1834001269d79d3ad0972d9dee6/agent_reach/skill/SKILL.md
- 官方下载地址：https://codeload.github.com/Panniantong/Agent-Reach/tar.gz/94f06c1969dfc1834001269d79d3ad0972d9dee6
- 分支：`main`（下载时通过 GitHub API 解析到下面的固定提交）。
- 提交：`94f06c1969dfc1834001269d79d3ad0972d9dee6`。
- 版本标识：pyproject.toml 1.5.0。
- 收录日期：2026-10-11（Asia/Shanghai）。
- 上游根许可证：MIT，原文见 [upstream/LICENSE](upstream/LICENSE)，入口目录另保留一份 [LICENSE](LICENSE)。上游子目录中的其他许可证及声明也随快照保留。
- 原始下载包 SHA-256：`d608cc619e460ca982dc11ab72897677837c8d73ea23851026c6374cff864f93`。

## 本地收录方式

- `upstream/` 保存该提交的完整仓库源码快照，保留原始目录、署名、脚本、数据、参考资料和仓库内符号链接；不含 `.git` 历史或本地安装产物。
- 顶层 `SKILL.md` 是中文索引入口，名称与当前收录目录一致；实际工作流程指向原版 `agent_reach/skill/SKILL.md`。未翻译或改写上游指令与脚本。
- 顶层 `SOURCE.md` 记录来源和本地包装；顶层 `LICENSE` 是上游根许可证的原样副本。
- 上游仓库可能还包含其他 Skill 和宿主适配；它们作为原始源码的一部分保留，不表示已在本机安装。

## 依赖与验证边界

Agent Reach CLI 需要 Python >=3.10 及项目依赖；各渠道可能需要额外 CLI、MCP、网络权限或用户提供的认证配置。源码下载不代表任何渠道已可用。

本次只下载、检查和收录源文件，没有运行安装器、安装业务依赖、配置账号、启动服务或执行完整业务流程。宿主兼容性与实际运行结果需要在后续明确使用时验证。

## 后续项目安装记录

2026-10-11，按用户授权将此版本安装到项目级 [`.agents/skills/agent-reach/`](../../.agents/skills/agent-reach/SKILL.md)，安装详情见[安装来源记录](../../.agents/skills/agent-reach/SOURCE.md)。源码快照保持原样。
