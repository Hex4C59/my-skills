# understand-anything 来源记录

- 来源类型：第三方修改版（仅添加中文收录入口与来源说明，`upstream/` 中的上游文件未改动）。
- 作者 / 组织：Yuxiang Lin / Infinite Universe, Inc. / Egonex-AI。
- 官方项目：https://github.com/Egonex-AI/Understand-Anything
- 主 Skill 固定版本：https://github.com/Egonex-AI/Understand-Anything/blob/000fbf3f36b5e534a0a8d3461cf24f5dc9ae43fe/understand-anything-plugin/skills/understand/SKILL.md
- 官方下载地址：https://codeload.github.com/Egonex-AI/Understand-Anything/tar.gz/000fbf3f36b5e534a0a8d3461cf24f5dc9ae43fe
- 分支：`main`（下载时通过 GitHub API 解析到下面的固定提交）。
- 提交：`000fbf3f36b5e534a0a8d3461cf24f5dc9ae43fe`。
- 版本标识：插件 plugin.json 2.9.7。
- 收录日期：2026-10-11（Asia/Shanghai）。
- 上游根许可证：MIT，原文见 [upstream/LICENSE](upstream/LICENSE)，入口目录另保留一份 [LICENSE](LICENSE)。上游子目录中的其他许可证及声明也随快照保留。
- 原始下载包 SHA-256：`c48f6c16adb5b57cc9d0a03ca7ca755fc4c9113418a493af24f6488cf3753c50`。

## 本地收录方式

- `upstream/` 保存该提交的完整仓库源码快照，保留原始目录、署名、脚本、数据、参考资料和仓库内符号链接；不含 `.git` 历史或本地安装产物。
- 顶层 `SKILL.md` 是中文索引入口，名称与当前收录目录一致；实际工作流程指向原版 `understand-anything-plugin/skills/understand/SKILL.md`。未翻译或改写上游指令与脚本。
- 顶层 `SOURCE.md` 记录来源和本地包装；顶层 `LICENSE` 是上游根许可证的原样副本。
- 上游仓库可能还包含其他 Skill 和宿主适配；它们作为原始源码的一部分保留，不表示已在本机安装。

## 依赖与验证边界

需要支持的 Agent 环境和 Node.js；上游 README 标明查看仪表盘需 Node.js >=18，源码构建使用 pnpm（packageManager 指定 10.6.2）及项目依赖。插件、Agent 定义和仪表盘源码均已保留；本次未构建。

本次只下载、检查和收录源文件，没有运行安装器、安装业务依赖、配置账号、启动服务或执行完整业务流程。宿主兼容性与实际运行结果需要在后续明确使用时验证。

历史仓库地址 `Lum1104/Understand-Anything` 经 GitHub API 重定向至 `Egonex-AI/Understand-Anything`；本次使用重定向后的官方地址。
