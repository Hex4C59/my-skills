# last30days-skill 来源记录

- 来源类型：第三方修改版（仅添加中文收录入口与来源说明，`upstream/` 中的上游文件未改动）。
- 作者 / 组织：Matt Van Horn（mvanhorn）。
- 官方项目：https://github.com/mvanhorn/last30days-skill
- 主 Skill 固定版本：https://github.com/mvanhorn/last30days-skill/blob/267d50f7fcbab8a6457a93ad6ca15cbc199f633c/skills/last30days/SKILL.md
- 官方下载地址：https://codeload.github.com/mvanhorn/last30days-skill/tar.gz/267d50f7fcbab8a6457a93ad6ca15cbc199f633c
- 分支：`main`（下载时通过 GitHub API 解析到下面的固定提交）。
- 提交：`267d50f7fcbab8a6457a93ad6ca15cbc199f633c`。
- 版本标识：SKILL / pyproject.toml 3.27.2。
- 收录日期：2026-10-11（Asia/Shanghai）。
- 上游根许可证：MIT，原文见 [upstream/LICENSE](upstream/LICENSE)，入口目录另保留一份 [LICENSE](LICENSE)。上游子目录中的其他许可证及声明也随快照保留。
- 原始下载包 SHA-256：`c2c61a2d9c9acee62b22f0e24793a8deaeb4d820cc9b81d0f007805fb9bde9a3`。

## 本地收录方式

- `upstream/` 保存该提交的完整仓库源码快照，保留原始目录、署名、脚本、数据、参考资料和仓库内符号链接；不含 `.git` 历史或本地安装产物。
- 顶层 `SKILL.md` 是中文索引入口，名称与当前收录目录一致；实际工作流程指向原版 `skills/last30days/SKILL.md`。未翻译或改写上游指令与脚本。
- 顶层 `SOURCE.md` 记录来源和本地包装；顶层 `LICENSE` 是上游根许可证的原样副本。
- 上游仓库可能还包含其他 Skill 和宿主适配；它们作为原始源码的一部分保留，不表示已在本机安装。

## 依赖与验证边界

Python >=3.12；具体来源可能需要 API Key、认证、浏览器或其他工具，按上游运行说明配置。脚本和 references/ 已保留；原版入口名称为 last30days。

本次只下载、检查和收录源文件，没有运行安装器、安装业务依赖、配置账号、启动服务或执行完整业务流程。宿主兼容性与实际运行结果需要在后续明确使用时验证。

## 官方压缩包的排除规则

上游 `.gitattributes` 使用 `export-ignore`，官方压缩包省略了部分仓库文件。本次另外通过官方 Git 仓库检出同一个固定提交，补齐 364 个文件；`upstream/` 按 GitHub API 返回的完整 Git 树核对。上面的 SHA-256 仅对应首次下载的官方压缩包，不能单独代表补齐后的全部文件。
