# my-skills

个人工作与编程中使用的 AI Agent Skill 集合，集中保存原创 Skill、收集的第三方 Skill，以及个人修改版。

本 README 用于介绍每一个已收录的 Skill，帮助快速判断它能做什么、什么时候使用、需要准备什么，以及从哪里获取原始版本。

## 目录结构

```text
my-skills/
├── AGENTS.md          # 维护与协作规则
├── README.md          # Skill 总览、介绍和来源
└── skills/            # 每个 Skill 一个独立目录
    └── <skill-name>/
        └── SKILL.md   # Skill 的具体指令
```

## Skill 总览

已收录 **11 个项目入口**：图片中第 2、3、4、5、6、8、9 项，以及 `git-commit`、`writing-for-agents`、`writing-clearly-and-concisely`、`frontend-art-direction`，收录日期为 **2026-10-11**。每项保留固定提交的上游源码、中文入口及来源记录，许可证或许可说明见各项介绍。前 7 项保留完整仓库快照；frontend-art-direction 保留上游发布文件与维护说明；其余项目保留各自的具体 Skill 目录。快照中的其他 Skill、变体和宿主适配不另行计入本表。

`skills/` 用于源码维护。Humanizer、Agent-Reach、git-commit 与 writing-for-agents 已按用户授权安装到当前项目的 `.agents/skills/`；其余 7 个项目保留源码收录状态。文字和技术说明统一使用 humanizer；Agent 指令文档使用 writing-for-agents，由它调用 humanizer。writing-clearly-and-concisely 保留源码参考，已撤下项目安装。Agent-Reach 的核心 CLI 与 Python 依赖安装在项目独立环境中，详见下方“当前项目安装”。

| Skill | 用途 | 来源类型 | 原项目 / 下载地址 |
| --- | --- | --- | --- |
| [humanizer](skills/humanizer/SKILL.md) | 用易懂语言编写或润色文字，解释陌生术语，去掉 AI 套话并保留事实。 | 第三方修改版（中文表达与润色） | [官方项目](https://github.com/blader/humanizer) / [固定提交下载](https://codeload.github.com/blader/humanizer/tar.gz/225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8) |
| [ui-ux-pro-max-skill](skills/ui-ux-pro-max-skill/SKILL.md) | 通过本地设计数据与搜索脚本辅助界面设计、实现和 UX 检查。 | 第三方修改版（仅入口包装） | [官方项目](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) / [固定提交下载](https://codeload.github.com/nextlevelbuilder/ui-ux-pro-max-skill/tar.gz/67803eac81607188194aea9842a723b89326d90d) |
| [taste-skill](skills/taste-skill/SKILL.md) | 根据需求选择前端视觉方向，改善落地页、作品集及改版页面的模板感。 | 第三方修改版（仅入口包装） | [官方项目](https://github.com/Leonxlnx/taste-skill) / [固定提交下载](https://codeload.github.com/Leonxlnx/taste-skill/tar.gz/717446e07a78d4e6d7918b1fde1a263378eebac9) |
| [agent-reach](skills/agent-reach/SKILL.md) | 为 Agent 提供跨平台搜索、页面读取和信息获取的工具路由。 | 第三方修改版（仅入口包装） | [官方项目](https://github.com/Panniantong/Agent-Reach) / [固定提交下载](https://codeload.github.com/Panniantong/Agent-Reach/tar.gz/94f06c1969dfc1834001269d79d3ad0972d9dee6) |
| [career-ops](skills/career-ops/SKILL.md) | 组织求职工作流，支持岗位检索、职位评估、简历定制和申请进度管理。 | 第三方修改版（仅入口包装） | [官方项目](https://github.com/career-ops-hq/career-ops) / [固定提交下载](https://codeload.github.com/career-ops-hq/career-ops/tar.gz/7e0a3d0babbb5ed5eeb599cd7dac8708866fdd13) |
| [last30days-skill](skills/last30days-skill/SKILL.md) | 围绕主题调研最近 30 天的讨论、事件和趋势。 | 第三方修改版（仅入口包装） | [官方项目](https://github.com/mvanhorn/last30days-skill) / [固定提交下载](https://codeload.github.com/mvanhorn/last30days-skill/tar.gz/267d50f7fcbab8a6457a93ad6ca15cbc199f633c) |
| [understand-anything](skills/understand-anything/SKILL.md) | 分析代码库的架构、组件与关系，生成可交互浏览的知识图谱。 | 第三方修改版（仅入口包装） | [官方项目](https://github.com/Egonex-AI/Understand-Anything) / [固定提交下载](https://codeload.github.com/Egonex-AI/Understand-Anything/tar.gz/000fbf3f36b5e534a0a8d3461cf24f5dc9ae43fe) |
| [git-commit](skills/git-commit/SKILL.md) | 分析 Git diff、生成提交信息并按用户要求执行提交。 | 第三方修改版（仅入口包装） | [官方 Skill](https://github.com/github/awesome-copilot/tree/82701c24b99488536ca399ff4789a458b7a05db7/skills/git-commit) / [主文件下载](https://raw.githubusercontent.com/github/awesome-copilot/82701c24b99488536ca399ff4789a458b7a05db7/skills/git-commit/SKILL.md) |
| [writing-for-agents](skills/writing-for-agents/SKILL.md) | 整理 Agent 文档结构后调用 humanizer 润色，保留规则并改善阅读体验。 | 第三方修改版（结构与润色联动） | [官方 Skill](https://github.com/mattpocock/skills/tree/49dd158d1076134a641b33efb035946536778336/skills/productivity/writing-for-agents) / [主文件下载](https://raw.githubusercontent.com/mattpocock/skills/49dd158d1076134a641b33efb035946536778336/skills/productivity/writing-for-agents/SKILL.md) |
| [writing-clearly-and-concisely](skills/writing-clearly-and-concisely/SKILL.md) | 保留源码参考；中文表达规则已并入 humanizer，当前项目不单独安装。 | 第三方修改版（中文技术表达） | [官方 Skill](https://github.com/obra/the-elements-of-style/tree/05fc4f0d2b97b7c042dd9949ad658568e4a1324e/skills/writing-clearly-and-concisely) / [主文件下载](https://raw.githubusercontent.com/obra/the-elements-of-style/05fc4f0d2b97b7c042dd9949ad658568e4a1324e/skills/writing-clearly-and-concisely/SKILL.md) |
| [frontend-art-direction](skills/frontend-art-direction/SKILL.md) | 选择前端设计方向，结合现有组件实现界面，并通过截图与交互检查验证效果。 | 第三方修改版（仅入口包装） | [官方项目](https://github.com/davaded/frontend-art-direction) / [固定提交下载](https://codeload.github.com/davaded/frontend-art-direction/tar.gz/9696da4c573bada9deea5564af7cfeb159f6fdda) |

目录结构示例：

```text
skills/<skill-name>/
├── SKILL.md     # 本仓库的中文入口，执行规则或指向上游主 Skill
├── SOURCE.md    # 官方地址、提交、收录日期及本地包装说明
├── LICENSE      # 上游提供时保留的许可证副本；其他许可说明见 SOURCE.md
└── upstream/    # 原样保留的上游仓库或具体 Skill 目录快照
```

使用某项时先读其入口，再按原版说明配置所需工具。上游命令的相对路径应根据入口中的路径提示解析。

## Skill 详细介绍

### humanizer

- **指令文件**：[中文执行入口](skills/humanizer/SKILL.md)；[项目安装入口](.agents/skills/humanizer/SKILL.md)；[上游规则参考](skills/humanizer/references/humanizer-original.md)。
- **用途**：统一处理易懂表达与 AI 套话，解释陌生术语，保留原意、事实和技术限制。
- **适用场景**：文章润色，以及代码说明、注释、README 和技术文档的编写或修改。
- **使用示例**：`$humanizer 修改这份实现说明，解释陌生术语，去掉套话，保留代码实际支持的条件和限制。`
- **所需输入**：写作任务或待修改的文字、文件；解释实现时提供相关代码或资料。可选写作样本、读者和语气要求。
- **预期输出**：润色后的文本；根据调用方式附修改说明或残留问题检查。
- **依赖与限制**：主要依赖语言模型，无专用脚本运行依赖；原版说明以英文为主。
- **来源类型**：第三方修改版（中文技术表达与 AI 套话检查）。
- **作者 / 组织**：Siqi Chen（blader）。
- **原项目地址**：[官方仓库](https://github.com/blader/humanizer)；[该提交的主 Skill](https://github.com/blader/humanizer/blob/225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8/SKILL.md)。
- **下载地址**：[官方固定提交源码包](https://codeload.github.com/blader/humanizer/tar.gz/225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8)。
- **版本 / 提交**：SKILL 元数据 3.1.0；`225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8`。
- **许可证**：上游根许可证为 [MIT](skills/humanizer/LICENSE)；其他随附许可证和声明保留于 `upstream/`。
- **收录日期**：2026-10-11。
- **个人修改**：中文入口合并首次术语解释、具体行为、按需举例和交付前检查；由 writing-for-agents 调用时统一检查表达。项目安装同步此修改版，上游原文保持不变。详见[来源记录](skills/humanizer/SOURCE.md)。

### ui-ux-pro-max-skill

- **指令文件**：[本地入口](skills/ui-ux-pro-max-skill/SKILL.md)；[上游主 Skill](skills/ui-ux-pro-max-skill/upstream/.claude/skills/ui-ux-pro-max/SKILL.md)。
- **用途**：通过本地设计数据与搜索脚本辅助界面设计、实现和 UX 检查。
- **适用场景**：网页、移动端、桌面端界面，配色、字体、布局及设计系统。
- **使用示例**：请用 ui-ux-pro-max-skill 为一个健康管理应用设计首页与配色方案。
- **所需输入**：产品类型、用户、功能需求、技术栈；可选页面源码、截图和品牌约束。
- **预期输出**：设计建议、设计系统、界面实现或 UX 改进意见。
- **依赖与限制**：搜索脚本需要 Python 3.x，使用标准库；本地脚本、数据与参考文件已保留。官方安装 CLI 是另一项工具，本次未安装。
- **来源类型**：第三方修改版（仅增加收录入口与来源说明）。
- **作者 / 组织**：Next Level Builder（nextlevelbuilder）。
- **原项目地址**：[官方仓库](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)；[该提交的主 Skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill/blob/67803eac81607188194aea9842a723b89326d90d/.claude/skills/ui-ux-pro-max/SKILL.md)。
- **下载地址**：[官方固定提交源码包](https://codeload.github.com/nextlevelbuilder/ui-ux-pro-max-skill/tar.gz/67803eac81607188194aea9842a723b89326d90d)。
- **版本 / 提交**：CLI package.json 2.5.0（CLI 版本，不等同于 Skill 独立版本）；`67803eac81607188194aea9842a723b89326d90d`。
- **许可证**：上游根许可证为 [MIT](skills/ui-ux-pro-max-skill/LICENSE)；其他随附许可证和声明保留于 `upstream/`。
- **收录日期**：2026-10-11。
- **个人修改**：添加中文 `SKILL.md` 入口、`SOURCE.md` 和根许可证副本；`upstream/` 内原版文件未改动。详见 [来源记录](skills/ui-ux-pro-max-skill/SOURCE.md)。

### taste-skill

- **指令文件**：[本地入口](skills/taste-skill/SKILL.md)；[上游主 Skill](skills/taste-skill/upstream/skills/taste-skill/SKILL.md)。
- **用途**：根据需求选择前端视觉方向，改善落地页、作品集及改版页面的模板感。
- **适用场景**：落地页、作品集、已有页面的视觉改版。原版主 Skill 明确不面向仪表盘、数据表格和多步骤产品界面。
- **使用示例**：请用 taste-skill 改善这个作品集首页的视觉设计，保留内容与功能。
- **所需输入**：页面需求或现有源码；可选参考图、品牌和技术栈约束。
- **预期输出**：视觉方案、前端实现或对已有页面的改版。
- **依赖与限制**：主 Skill 为指令文件；实际实现依赖目标前端项目的框架与工具链。原版名称为 design-taste-frontend；上游的其他变体保留在快照中。
- **来源类型**：第三方修改版（仅增加收录入口与来源说明）。
- **作者 / 组织**：Leonxlnx。
- **原项目地址**：[官方仓库](https://github.com/Leonxlnx/taste-skill)；[该提交的主 Skill](https://github.com/Leonxlnx/taste-skill/blob/717446e07a78d4e6d7918b1fde1a263378eebac9/skills/taste-skill/SKILL.md)。
- **下载地址**：[官方固定提交源码包](https://codeload.github.com/Leonxlnx/taste-skill/tar.gz/717446e07a78d4e6d7918b1fde1a263378eebac9)。
- **版本 / 提交**：未见该主 Skill 的独立版本字段；以提交固定版本；`717446e07a78d4e6d7918b1fde1a263378eebac9`。
- **许可证**：上游根许可证为 [MIT](skills/taste-skill/LICENSE)；其他随附许可证和声明保留于 `upstream/`。
- **收录日期**：2026-10-11。
- **个人修改**：添加中文 `SKILL.md` 入口、`SOURCE.md` 和根许可证副本；`upstream/` 内原版文件未改动。详见 [来源记录](skills/taste-skill/SOURCE.md)。

### agent-reach

- **指令文件**：[本地入口](skills/agent-reach/SKILL.md)；[上游主 Skill](skills/agent-reach/upstream/agent_reach/skill/SKILL.md)。
- **用途**：为 Agent 提供跨平台搜索、页面读取和信息获取的工具路由。
- **适用场景**：网页、社交平台、视频平台、RSS 等来源的资料检索。
- **使用示例**：请用 agent-reach 搜索这个主题的公开资料，并整理来源链接。
- **所需输入**：主题、搜索词或链接，以及目标平台和检索范围。
- **预期输出**：搜索结果、页面内容、视频转写或带来源的资料。
- **依赖与限制**：Agent Reach CLI 需要 Python >=3.10 及项目依赖；各渠道可能需要额外 CLI、MCP、网络权限或用户提供的认证配置。源码下载不代表任何渠道已可用。
- **来源类型**：第三方修改版（仅增加收录入口与来源说明）。
- **作者 / 组织**：Panniantong / Neo Reid（pyproject.toml；许可证署名 Agent Eyes）。
- **原项目地址**：[官方仓库](https://github.com/Panniantong/Agent-Reach)；[该提交的主 Skill](https://github.com/Panniantong/Agent-Reach/blob/94f06c1969dfc1834001269d79d3ad0972d9dee6/agent_reach/skill/SKILL.md)。
- **下载地址**：[官方固定提交源码包](https://codeload.github.com/Panniantong/Agent-Reach/tar.gz/94f06c1969dfc1834001269d79d3ad0972d9dee6)。
- **版本 / 提交**：pyproject.toml 1.5.0；`94f06c1969dfc1834001269d79d3ad0972d9dee6`。
- **许可证**：上游根许可证为 [MIT](skills/agent-reach/LICENSE)；其他随附许可证和声明保留于 `upstream/`。
- **收录日期**：2026-10-11。
- **个人修改**：添加中文 `SKILL.md` 入口、`SOURCE.md` 和根许可证副本；`upstream/` 内原版文件未改动。详见 [来源记录](skills/agent-reach/SOURCE.md)。

### career-ops

- **指令文件**：[本地入口](skills/career-ops/SKILL.md)；[上游主 Skill](skills/career-ops/upstream/.agents/skills/career-ops/SKILL.md)。
- **用途**：组织求职工作流，支持岗位检索、职位评估、简历定制和申请进度管理。
- **适用场景**：准备简历、评估职位匹配度、跟踪申请和准备面试。
- **使用示例**：请用 career-ops 对照我的简历评估这份职位描述，列出匹配点和差距。
- **所需输入**：简历、职业资料、目标岗位或职位描述；实际使用时再配置个人档案。
- **预期输出**：岗位评估、定制简历、求职材料、申请记录或面试准备内容。
- **依赖与限制**：package.json 声明 Node.js ^22.13.0 或 >=23.4.0；按功能需要浏览器、模型服务配置及 PDF/LaTeX 等工具。路由依赖 modes/、config/ 和脚本，均已保留。
- **来源类型**：第三方修改版（仅增加收录入口与来源说明）。
- **作者 / 组织**：Santiago Fernández de Valderrama（santifer）/ career-ops-hq。
- **原项目地址**：[官方仓库](https://github.com/career-ops-hq/career-ops)；[该提交的主 Skill](https://github.com/career-ops-hq/career-ops/blob/7e0a3d0babbb5ed5eeb599cd7dac8708866fdd13/.agents/skills/career-ops/SKILL.md)。
- **下载地址**：[官方固定提交源码包](https://codeload.github.com/career-ops-hq/career-ops/tar.gz/7e0a3d0babbb5ed5eeb599cd7dac8708866fdd13)。
- **版本 / 提交**：package.json 1.36.0；`7e0a3d0babbb5ed5eeb599cd7dac8708866fdd13`。
- **许可证**：上游根许可证为 [MIT](skills/career-ops/LICENSE)；其他随附许可证和声明保留于 `upstream/`。
- **收录日期**：2026-10-11。
- **个人修改**：添加中文 `SKILL.md` 入口、`SOURCE.md` 和根许可证副本；`upstream/` 内原版文件未改动。详见 [来源记录](skills/career-ops/SOURCE.md)。

### last30days-skill

- **指令文件**：[本地入口](skills/last30days-skill/SKILL.md)；[上游主 Skill](skills/last30days-skill/upstream/skills/last30days/SKILL.md)。
- **用途**：围绕主题调研最近 30 天的讨论、事件和趋势。
- **适用场景**：近期热点、产品反馈、社区观点和技术趋势调研。
- **使用示例**：请用 last30days-skill 调研最近 30 天开发者对某项技术的反馈，并给出来源。
- **所需输入**：调研主题、问题、时间范围及重点来源。
- **预期输出**：近期讨论与趋势的研究摘要、证据和来源链接。
- **依赖与限制**：Python >=3.12；具体来源可能需要 API Key、认证、浏览器或其他工具，按上游运行说明配置。脚本和 references/ 已保留；原版入口名称为 last30days。
- **来源类型**：第三方修改版（仅增加收录入口与来源说明）。
- **作者 / 组织**：Matt Van Horn（mvanhorn）。
- **原项目地址**：[官方仓库](https://github.com/mvanhorn/last30days-skill)；[该提交的主 Skill](https://github.com/mvanhorn/last30days-skill/blob/267d50f7fcbab8a6457a93ad6ca15cbc199f633c/skills/last30days/SKILL.md)。
- **下载地址**：[官方固定提交源码包](https://codeload.github.com/mvanhorn/last30days-skill/tar.gz/267d50f7fcbab8a6457a93ad6ca15cbc199f633c)。
- **版本 / 提交**：SKILL / pyproject.toml 3.27.2；`267d50f7fcbab8a6457a93ad6ca15cbc199f633c`。
- **许可证**：上游根许可证为 [MIT](skills/last30days-skill/LICENSE)；其他随附许可证和声明保留于 `upstream/`。
- **收录日期**：2026-10-11。
- **个人修改**：添加中文 `SKILL.md` 入口、`SOURCE.md` 和根许可证副本；`upstream/` 内原版文件未改动。详见 [来源记录](skills/last30days-skill/SOURCE.md)。

### understand-anything

- **指令文件**：[本地入口](skills/understand-anything/SKILL.md)；[上游主 Skill](skills/understand-anything/upstream/understand-anything-plugin/skills/understand/SKILL.md)。
- **用途**：分析代码库的架构、组件与关系，生成可交互浏览的知识图谱。
- **适用场景**：接手项目、理解代码架构、探索依赖与变更影响。
- **使用示例**：请用 understand-anything 分析指定代码库，用中文生成架构知识图谱。
- **所需输入**：目标代码库路径；可选输出语言、排除规则和增量分析选项。
- **预期输出**：knowledge-graph.json 等分析成果，以及配套仪表盘所需数据。
- **依赖与限制**：需要支持的 Agent 环境和 Node.js；上游 README 标明查看仪表盘需 Node.js >=18，源码构建使用 pnpm（packageManager 指定 10.6.2）及项目依赖。插件、Agent 定义和仪表盘源码均已保留；本次未构建。
- **来源类型**：第三方修改版（仅增加收录入口与来源说明）。
- **作者 / 组织**：Yuxiang Lin / Infinite Universe, Inc. / Egonex-AI。
- **原项目地址**：[官方仓库](https://github.com/Egonex-AI/Understand-Anything)；[该提交的主 Skill](https://github.com/Egonex-AI/Understand-Anything/blob/000fbf3f36b5e534a0a8d3461cf24f5dc9ae43fe/understand-anything-plugin/skills/understand/SKILL.md)。
- **下载地址**：[官方固定提交源码包](https://codeload.github.com/Egonex-AI/Understand-Anything/tar.gz/000fbf3f36b5e534a0a8d3461cf24f5dc9ae43fe)。
- **版本 / 提交**：插件 plugin.json 2.9.7；`000fbf3f36b5e534a0a8d3461cf24f5dc9ae43fe`。
- **许可证**：上游根许可证为 [MIT](skills/understand-anything/LICENSE)；其他随附许可证和声明保留于 `upstream/`。
- **收录日期**：2026-10-11。
- **个人修改**：添加中文 `SKILL.md` 入口、`SOURCE.md` 和根许可证副本；`upstream/` 内原版文件未改动。详见 [来源记录](skills/understand-anything/SOURCE.md)。

### git-commit

- **指令文件**：[中文收录入口](skills/git-commit/SKILL.md)；[上游原版](skills/git-commit/upstream/SKILL.md)；[项目安装入口](.agents/skills/git-commit/SKILL.md)。
- **用途**：分析 Git diff，判断提交类型与范围，生成 Conventional Commits 提交信息；按用户请求组织暂存和执行提交。
- **适用场景**：生成 Git commit message、整理逻辑一致的提交、实际执行 Git 提交。
- **使用示例**：`$git-commit 分析当前改动，先生成中文提交信息供我审查。`
- **所需输入**：目标 Git 仓库、工作区或暂存区改动、提交范围、输出语言及格式要求。
- **预期输出**：提交标题、可选正文及页脚；任务包含实际提交时，另报告提交哈希和范围。
- **依赖与限制**：需要 Git CLI 与已初始化的目标仓库，无额外业务依赖。原版包含实际提交步骤；用户只要求生成信息时，按该范围执行。当前目录尚未初始化 Git；提交规范文档仍为待审查草案。
- **来源类型**：第三方修改版（仅收录入口包装）；项目安装版主指令保持原样。
- **作者 / 组织**：GitHub / awesome-copilot 项目贡献者。
- **原项目地址**：[官方 Skill 目录](https://github.com/github/awesome-copilot/tree/82701c24b99488536ca399ff4789a458b7a05db7/skills/git-commit)。
- **下载地址**：[原版 SKILL.md](https://raw.githubusercontent.com/github/awesome-copilot/82701c24b99488536ca399ff4789a458b7a05db7/skills/git-commit/SKILL.md)；[官方固定提交源码包](https://codeload.github.com/github/awesome-copilot/tar.gz/82701c24b99488536ca399ff4789a458b7a05db7)。
- **版本 / 提交**：无独立版本字段；`82701c24b99488536ca399ff4789a458b7a05db7`。
- **许可证**：[MIT](skills/git-commit/LICENSE)。
- **收录及安装日期**：2026-10-11。
- **个人修改**：收录目录添加中文入口和来源记录；安装目录只补充许可证及来源记录，原版 `SKILL.md` 未改动。详见[来源记录](skills/git-commit/SOURCE.md)。

### writing-for-agents

- **指令文件**：[中文收录入口](skills/writing-for-agents/SKILL.md)；[上游规则参考](skills/writing-for-agents/references/writing-for-agents-original.md)；[项目安装入口](.agents/skills/writing-for-agents/SKILL.md)。
- **用途**：编写或审查 Agent 指令文档，先整理规则、引用条件和信息层级，再调用 humanizer 润色，最后复核原意与约束。
- **适用场景**：编写或整理 `AGENTS.md`、`CLAUDE.md`、`SKILL.md` 及配套参考文档，检查重复、过时或含糊的规则。
- **使用示例**：`$writing-for-agents 审查当前 AGENTS.md 的表达和结构，先列出修改建议供我审查。`
- **所需输入**：目标文档或仓库、期望改善的问题、必须保留的约束；按需提供相关参考文件。
- **预期输出**：文档审查意见、修改建议，或按用户要求完成的指令文档和关联文件。
- **依赖与限制**：需要同级目录的 humanizer 修改版，无额外程序运行依赖。中文入口负责执行流程；上游主参考保持原样，格式说明仅调整内部链接。humanizer 缺失时明确报告表达检查未完成，不自动安装。Skill 元数据和调用说明按目标工具实际支持情况使用。
- **来源类型**：第三方修改版。中文入口增加 humanizer 联动，安装版同步运行所需文件；维护源的上游快照保持原样。
- **作者 / 组织**：Matt Pocock（mattpocock）。
- **原项目地址**：[官方 Skill 目录](https://github.com/mattpocock/skills/tree/49dd158d1076134a641b33efb035946536778336/skills/productivity/writing-for-agents)。
- **下载地址**：[原版 SKILL.md](https://raw.githubusercontent.com/mattpocock/skills/49dd158d1076134a641b33efb035946536778336/skills/productivity/writing-for-agents/SKILL.md)；[官方固定提交源码包](https://codeload.github.com/mattpocock/skills/tar.gz/49dd158d1076134a641b33efb035946536778336)。
- **版本 / 提交**：无独立版本字段；`49dd158d1076134a641b33efb035946536778336`。
- **许可证**：[MIT](skills/writing-for-agents/LICENSE)。
- **收录及安装日期**：2026-10-11。
- **个人修改**：中文入口增加“结构整理 → humanizer 表达检查 → 含义与阅读复核”，保留必要解释和例子。维护源保留上游快照；安装时仅复制执行入口和普通参考文件，避免重复识别同名 Skill。维护时先改模板，再同步安装副本。详见[来源记录](skills/writing-for-agents/SOURCE.md)。

### writing-clearly-and-concisely

- **指令文件**：[中文执行入口](skills/writing-clearly-and-concisely/SKILL.md)；[上游原版](skills/writing-clearly-and-concisely/upstream/SKILL.md)；[英文参考全文](skills/writing-clearly-and-concisely/upstream/elements-of-style.md)。
- **用途**：用具体、易懂的中文解释代码和编写文档，说明陌生术语，保留准确的技术含义。
- **适用场景**：编写或修改 README、技术文档、代码注释、实现说明、提交说明和报错文案。
- **使用示例**：需要研究英文写作原则时阅读随附参考全文；日常编写和修改技术说明使用 `$humanizer`。
- **所需输入**：写作任务或待修改的文本、文件；解释实现时提供相关代码或资料。可选读者背景、输出语言和写作样本。
- **预期输出**：符合任务格式的文字或获准修改的文件；通俗化后保留条件、限制和失败情况，明确待确认的实现依据。
- **依赖与限制**：依赖语言模型及随附参考资料，无额外程序依赖。英文参考约 12,000 tokens，按问题读取。当前仅保留源码参考，已撤下项目安装；中文表达规则已并入 humanizer。
- **来源类型**：第三方修改版（中文技术表达与交付前检查）。
- **作者 / 组织**：obra（Jesse Vincent）维护 Skill 项目；William Strunk Jr. 著参考书。
- **原项目地址**：[固定提交的官方 Skill 目录](https://github.com/obra/the-elements-of-style/tree/05fc4f0d2b97b7c042dd9949ad658568e4a1324e/skills/writing-clearly-and-concisely)。
- **下载地址**：[原版 SKILL.md](https://raw.githubusercontent.com/obra/the-elements-of-style/05fc4f0d2b97b7c042dd9949ad658568e4a1324e/skills/writing-clearly-and-concisely/SKILL.md)；[官方固定提交源码包](https://codeload.github.com/obra/the-elements-of-style/tar.gz/05fc4f0d2b97b7c042dd9949ad658568e4a1324e)。
- **版本 / 提交**：无独立版本字段；`05fc4f0d2b97b7c042dd9949ad658568e4a1324e`。
- **许可证**：上游将 1918 年参考文本标为 Public Domain（公有领域）；未发现独立许可证文件，Skill 指令许可待确认。原始声明见[上游 README](skills/writing-clearly-and-concisely/upstream/README.md)。
- **收录日期**：2026-10-11。
- **个人修改**：加入中文表达、首次术语解释、按需举例和交付前检查；英文语法与标点规则限用于英文内容。上游文件原样保留，详见[来源记录](skills/writing-clearly-and-concisely/SOURCE.md)。

### frontend-art-direction

- **指令文件**：[中文收录入口](skills/frontend-art-direction/SKILL.md)；[上游原版](skills/frontend-art-direction/upstream/SKILL.md)。
- **用途**：先了解产品与现有界面，再确定布局、字体、组件和动效，并通过实际页面验证改动。
- **适用场景**：应用、仪表盘、编辑器、设置页、产品官网，以及参考网站驱动的界面改版和视觉审查。
- **使用示例**：`请用 frontend-art-direction 审查这个应用的设置页，保留已确认的设计与功能，先报告排版和状态展示问题。`
- **所需输入**：目标项目或页面、用户任务、希望改善的问题、功能与设计约束；可选参考网站、截图和素材。
- **预期输出**：设计方向、前端实现或界面审查结果，以及与任务相符的截图、交互和运行证据。
- **依赖与限制**：辅助脚本要求 Node.js >=18；实际实现依赖目标项目工具链。截图工具需要目标项目已有 Playwright 或 Puppeteer；动效桥在需要时获取固定版本的外部参考。较大任务要求 20 个流程检查点和迭代记录。当前仅收录源码，未安装，也未为 pipi 等项目调整流程。
- **来源类型**：第三方修改版（仅添加中文入口与来源记录）。
- **作者 / 组织**：davaded（GitHub 仓库所有者；其他作者信息待确认）。
- **原项目地址**：[官方仓库](https://github.com/davaded/frontend-art-direction)；[固定提交的主 Skill](https://github.com/davaded/frontend-art-direction/blob/9696da4c573bada9deea5564af7cfeb159f6fdda/SKILL.md)。
- **下载地址**：[原版 SKILL.md](https://raw.githubusercontent.com/davaded/frontend-art-direction/9696da4c573bada9deea5564af7cfeb159f6fdda/SKILL.md)；[官方固定提交源码包](https://codeload.github.com/davaded/frontend-art-direction/tar.gz/9696da4c573bada9deea5564af7cfeb159f6fdda)。本次通过 GitHub API 获取发布文件；源码包传输超时，未下载完整压缩包。
- **版本 / 提交**：`1.0.0`；`9696da4c573bada9deea5564af7cfeb159f6fdda`。
- **许可证**：待确认。上游根目录未见整体许可证，`package.json` 未声明许可；测试素材的局部许可不代表整个 Skill 的许可。
- **收录日期**：2026-10-11。
- **个人修改**：增加中文索引入口和来源记录；按上游发布清单保留 77 个原版文件及维护说明，未改写上游指令或脚本。未收录视觉测试样例和 GitHub CI 配置。详见[来源记录](skills/frontend-art-direction/SOURCE.md)。

## 新增 Skill

1. 在 `skills/` 下新建以小写英文和连字符命名的目录。
2. 放入 `SKILL.md`，并按需添加脚本、参考材料和资源。
3. 在上方总览表添加条目，并按下方模板填写详细介绍。
4. 如果来自第三方，保留署名和许可证，填写原项目、下载地址及版本信息；有本地改动时一并说明。
5. 检查本地文件链接和外部来源地址，确认说明与实际内容一致。

### 介绍模板

复制下方模板到“Skill 详细介绍”，替换占位内容，删除不适用的字段。

```markdown
### <Skill 名称>

- **指令文件**：[SKILL.md](skills/<skill-name>/SKILL.md)
- **用途**：这个 Skill 解决什么问题。
- **适用场景**：什么时候应该使用它。
- **使用示例**：一条有代表性的请求或调用方式。
- **所需输入**：文件、链接、需求描述或其他材料。
- **预期输出**：代码、文档、报告或其他成果。
- **依赖与限制**：需要的工具、权限、平台或使用边界；无特殊依赖时注明。
- **来源类型**：原创 / 第三方 / 第三方修改版。
- **作者 / 组织**：个人或原作者名称。
- **原项目地址**：[项目或具体 Skill 目录](<原项目 URL>)。
- **下载地址**：[下载页面或文件](<官方下载 URL>)。
- **版本 / 提交**：版本号或 commit；无法确认时写“待确认”。
- **许可证**：许可证名称及文件链接；无法确认时写“待确认”。
- **收录日期**：YYYY-MM-DD。
- **个人修改**：仅第三方修改版填写，简述相对原版的变化。
```

原创 Skill 可省略外部项目、下载地址和上游版本字段；如已对外发布，也可以补充这些信息。第三方 Skill 的下载地址应能帮助获取原始文件，可使用原仓库的具体目录页面、官方发行页面或下载包链接。

## 使用说明

先阅读对应 Skill 的介绍和 `SKILL.md`，确认适用场景与依赖，再按所用 AI 工具的要求安装或加载。本文件夹用于维护源文件，不会自动安装到 Codex 或其他工具。

### 当前项目安装

安装日期：2026-10-11。使用项目级 `.agents/skills/` 目录，版本与上方收录的固定提交一致。

| Skill | 项目安装入口 | 运行依赖 |
| --- | --- | --- |
| humanizer | [已安装 SKILL.md](.agents/skills/humanizer/SKILL.md) | 无额外程序依赖 |
| agent-reach | [已安装 SKILL.md](.agents/skills/agent-reach/SKILL.md) | 核心 CLI 1.5.0 和 Python 依赖位于 `.venv/agent-reach/` |
| git-commit | [已安装 SKILL.md](.agents/skills/git-commit/SKILL.md) | Git CLI 和已初始化的目标 Git 仓库 |
| writing-for-agents | [已安装 SKILL.md](.agents/skills/writing-for-agents/SKILL.md) | humanizer Skill；无额外程序依赖 |

下一轮对话可显式使用 `$humanizer`、`$agent-reach`、`$git-commit` 或 `$writing-for-agents`。例如：

- `$humanizer 修改这份实现说明，解释陌生术语，去掉套话，保留代码实际支持的条件和限制。`
- `$agent-reach 请搜索这个主题的公开资料，并整理来源。`
- `$git-commit 分析当前改动，先生成中文提交信息供我审查。`
- `$writing-for-agents 审查当前 AGENTS.md 的表达和结构，先列出修改建议供我审查。`

从项目根目录检查 Agent-Reach：

```sh
./.agents/skills/agent-reach/scripts/agent-reach --version
./.agents/skills/agent-reach/scripts/agent-reach doctor --json
```

Agent-Reach 的本地启动器只为当前命令加载项目环境。不同平台的额外 CLI、MCP 和认证按实际需要另行配置；本次未运行上游系统级一键安装器。体检中的“可用”是工具配置状态，不等同于每个平台都已通过实际访问测试。

`.venv/` 已加入 `.gitignore`。换机器时，使用 Python >=3.10 在项目根目录重建核心运行环境（以下 `python3.11` 可替换为满足版本要求的解释器）：

```sh
python3.11 -m venv .venv/agent-reach
.venv/agent-reach/bin/python -m pip install --constraint skills/agent-reach/upstream/constraints.txt ./skills/agent-reach/upstream
```

安装检查：两个 Skill 的入口格式及参考文件检查通过；Agent-Reach 1.5.0 的 CLI 启动、项目外目录调用及 `pip check` 通过。2026-10-11 的只读渠道体检报告 4/16 可用：网页读取、RSS、V2EX、B站搜索。其余渠道需要额外工具、配置或进一步验证；这份报告不能替代逐平台的实际访问测试。

git-commit 的安装结构、元数据、许可证和原版内容检查通过；当前目录尚无 `.git`，实际提交功能需要先在目标目录初始化 Git。

writing-for-agents 继续读取同级 humanizer，统一检查易懂程度与 AI 套话。安装包以普通文档保存上游参考，只保留一个可调用的 `SKILL.md`。入口格式、本地引用及同步文件一致性检查通过。

humanizer 已合并中文表达规则，上游主文件保留为普通参考文件。writing-clearly-and-concisely 已撤下项目安装，源码仍保留作参考。

2026-10-11 已将当前版本同步至使用这两个 Skill 的本机项目：my-skills、remote-desktop、Hex4C59、pipi、微信读书、Cpp八股文面试、Cpp_learning_game，并更新本机用户级 humanizer。使用 writing-for-agents 的项目已补齐同级 humanizer。另检查了 Windows 项目 deepseek-harness，未发现安装这两个 Skill，因此未新增。

安装追溯：[Humanizer](.agents/skills/humanizer/SOURCE.md)、[Agent-Reach](.agents/skills/agent-reach/SOURCE.md)、[git-commit](.agents/skills/git-commit/SOURCE.md)、[writing-for-agents](.agents/skills/writing-for-agents/SOURCE.md)。

维护本集合时遵循 [AGENTS.md](AGENTS.md)。

Git 提交信息规范见 [COMMIT_CONVENTION.md（草案，待审查）](COMMIT_CONVENTION.md)。
