# writing-clearly-and-concisely 来源记录

- 来源类型：第三方修改版（中文技术表达与交付前检查）。
- Skill 项目维护者：obra（Jesse Vincent）；参考书作者：William Strunk Jr.。
- 官方项目：https://github.com/obra/the-elements-of-style
- 具体 Skill 目录：https://github.com/obra/the-elements-of-style/tree/05fc4f0d2b97b7c042dd9949ad658568e4a1324e/skills/writing-clearly-and-concisely
- 原版主文件下载：https://raw.githubusercontent.com/obra/the-elements-of-style/05fc4f0d2b97b7c042dd9949ad658568e4a1324e/skills/writing-clearly-and-concisely/SKILL.md
- 英文参考资料下载：https://raw.githubusercontent.com/obra/the-elements-of-style/05fc4f0d2b97b7c042dd9949ad658568e4a1324e/skills/writing-clearly-and-concisely/elements-of-style.md
- 官方固定提交源码包：https://codeload.github.com/obra/the-elements-of-style/tar.gz/05fc4f0d2b97b7c042dd9949ad658568e4a1324e
- 固定提交：`05fc4f0d2b97b7c042dd9949ad658568e4a1324e`；上游提交时间：2026-08-12T21:47:28Z。
- 独立版本：上游主文件未提供，以固定提交标识版本。
- 收录与修改日期：2026-10-11（Asia/Shanghai）。

## 许可说明

同一提交的上游 [README](upstream/README.md) 将 1918 年《The Elements of Style》参考文本标为 Public Domain（公有领域），[英文参考全文](upstream/elements-of-style.md)也保留该声明及作者署名。

检查固定提交的完整文件树，未发现独立的 LICENSE、COPYING 或 NOTICE 文件。Skill 指令和其他项目代码是否适用相同许可，待确认；本仓库不将参考文本的声明扩大为整个项目的许可，也不自行添加 MIT 等许可证。

## 保留文件与校验值

以下文件从官方 GitHub Contents API 按固定提交读取，原样保留：

- [upstream/SKILL.md](upstream/SKILL.md)：具体 Skill 主文件；SHA-256：`1448ea19147b339ce37ae70551b233bb329d6bdfa46f0bf627b43b6133372233`。
- [upstream/elements-of-style.md](upstream/elements-of-style.md)：具体 Skill 的英文参考全文；SHA-256：`d0edf854b5d39e22da68793603830e5bbdddb9266d272007993bcb821ba2799d`。
- [upstream/README.md](upstream/README.md)：仓库根说明，保留作者、参考文本来源和公有领域声明；SHA-256：`77806d1f39f26e18105f2eb5e6927d7628f69493f8276ab72c702b0e05bdc3da`。

仅保留具体 Skill 目录及根 README，未复制其他宿主适配或安装文档。上游 README 中的仓库相对链接仍指向原仓库结构，相关内容须到固定提交的官方项目查阅。

## 本地改动

- [SKILL.md](SKILL.md)改为中文执行入口，补充读者背景、首次术语解释、具体行为和按需举例的规则。
- 保留准确的代码标识符、技术含义、条件和限制；示例中的假设不能成为具体项目的事实。
- 增加交付前检查，检查空泛表述、解释引入的陌生术语、无依据的效果及重复内容。
- 英文参考资料按问题读取，英文语法和标点规则用于英文内容。
- 上游主 Skill 作为对照存档，当前中文入口直接执行，无其他 Skill 或子代理依赖。

## 维护与安装

维护源为 `skills/writing-clearly-and-concisely/`。2026-10-11 曾按用户授权安装到当前项目；同日按用户确认的精简方案撤下该安装，将本地中文表达规则合并到 humanizer。此目录及上游原文继续保留作参考，不再作为当前项目的独立写作入口。

日常文字与技术说明使用 humanizer；Agent 指令文档使用 writing-for-agents，由它调用 humanizer。撤下安装时保留了可恢复副本，没有删除本目录的源码或上游资料。
