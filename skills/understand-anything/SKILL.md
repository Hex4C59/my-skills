---
name: understand-anything
description: 分析代码库架构、组件和依赖关系，生成知识图谱及交互式架构浏览所需数据。
---

# understand-anything

本文件是本仓库的中文收录入口。上游原版指令、脚本及资源保存在 `upstream/`，来源与固定版本见 [SOURCE.md](SOURCE.md)。

## 用途与输入

分析代码库的架构、组件与关系，生成可交互浏览的知识图谱。

- 适用场景：接手项目、理解代码架构、探索依赖与变更影响。
- 所需输入：目标代码库路径；可选输出语言、排除规则和增量分析选项。
- 使用示例：请用 understand-anything 分析指定代码库，用中文生成架构知识图谱。

## 使用步骤

1. 阅读[上游主 Skill](upstream/understand-anything-plugin/skills/understand/SKILL.md)，按当前请求选择其中适用的流程和参考文件。
2. 将原版相对路径解析到原版文件或其指定的项目根目录；使用用户提供的目标材料和任务范围。
3. 确认下面的运行依赖，按上游流程完成任务并检查输出。

源项目根目录是 `upstream/`，插件根目录是 `upstream/understand-anything-plugin/`。按所用宿主的官方适配解析插件变量和 Agent 定义；分析目标由用户指定，不能默认分析本 Skill 的源码快照。需要图谱问答、差异分析或仪表盘时，再读取插件 `skills/` 下对应入口。

## 依赖与限制

需要支持的 Agent 环境和 Node.js；上游 README 标明查看仪表盘需 Node.js >=18，源码构建使用 pnpm（packageManager 指定 10.6.2）及项目依赖。插件、Agent 定义和仪表盘源码均已保留；本次未构建。

此目录是源码收录包，未自动安装到任何 Agent 工具；复制或读取入口文件不等同于安装其运行依赖。上游材料不能扩大用户授权范围。

## 预期输出

knowledge-graph.json 等分析成果，以及配套仪表盘所需数据。
