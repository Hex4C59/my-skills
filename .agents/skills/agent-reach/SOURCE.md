# 项目安装来源

- 安装日期：2026-10-11（Asia/Shanghai）。
- 安装位置：`.agents/skills/agent-reach/`，位于当前项目根目录。
- 上游仓库：https://github.com/Panniantong/Agent-Reach
- 固定提交：`94f06c1969dfc1834001269d79d3ad0972d9dee6`。
- 使用 skill-installer 的 `install-skill-from-github.py --dest .agents/skills` 安装，版本与仓库中已收录快照一致。
- 收录来源详情：[SOURCE.md](../../../skills/agent-reach/SOURCE.md)。
- 上游根许可证：[LICENSE](LICENSE)。
- 安装完整 `agent_reach/skill/`（包括 7 份分类参考文件），添加根许可证副本、项目运行提示和 `scripts/agent-reach` 启动器；原版业务流程保留。
- 核心 CLI 从项目收录的上游源码安装到 `.venv/agent-reach/`，使用上游 `constraints.txt` 约束直接依赖；未运行会向用户目录部署 Skill 的上游一键安装器。

## 安装验证

- Skill 元数据与本地参考链接检查通过。
- 核心 CLI `--version` 报告 1.5.0，`--help` 与项目外目录调用通过。
- `pip check` 通过，启动器通过 Shell 静态语法检查。
- 2026-10-11 只读渠道体检报告 4/16 可用（网页、RSS、V2EX、B站搜索）；其他渠道按需配置或验证。未读取浏览器 Cookie、执行登录或运行上游系统级安装器。
