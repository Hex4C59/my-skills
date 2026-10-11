# career-ops 来源记录

- 来源类型：第三方修改版（仅添加中文收录入口与来源说明，`upstream/` 中的上游文件未改动）。
- 作者 / 组织：Santiago Fernández de Valderrama（santifer）/ career-ops-hq。
- 官方项目：https://github.com/career-ops-hq/career-ops
- 主 Skill 固定版本：https://github.com/career-ops-hq/career-ops/blob/7e0a3d0babbb5ed5eeb599cd7dac8708866fdd13/.agents/skills/career-ops/SKILL.md
- 官方下载地址：https://codeload.github.com/career-ops-hq/career-ops/tar.gz/7e0a3d0babbb5ed5eeb599cd7dac8708866fdd13
- 分支：`main`（下载时通过 GitHub API 解析到下面的固定提交）。
- 提交：`7e0a3d0babbb5ed5eeb599cd7dac8708866fdd13`。
- 版本标识：package.json 1.36.0。
- 收录日期：2026-10-11（Asia/Shanghai）。
- 上游根许可证：MIT，原文见 [upstream/LICENSE](upstream/LICENSE)，入口目录另保留一份 [LICENSE](LICENSE)。上游子目录中的其他许可证及声明也随快照保留。
- 原始下载包 SHA-256：`ff3725cc77dea66c9a15a8256457635b55feac662afe4430b8fa2a844cfae71d`。

## 本地收录方式

- `upstream/` 保存该提交的完整仓库源码快照，保留原始目录、署名、脚本、数据、参考资料和仓库内符号链接；不含 `.git` 历史或本地安装产物。
- 顶层 `SKILL.md` 是中文索引入口，名称与当前收录目录一致；实际工作流程指向原版 `.agents/skills/career-ops/SKILL.md`。未翻译或改写上游指令与脚本。
- 顶层 `SOURCE.md` 记录来源和本地包装；顶层 `LICENSE` 是上游根许可证的原样副本。
- 上游仓库可能还包含其他 Skill 和宿主适配；它们作为原始源码的一部分保留，不表示已在本机安装。

## 依赖与验证边界

package.json 声明 Node.js ^22.13.0 或 >=23.4.0；按功能需要浏览器、模型服务配置及 PDF/LaTeX 等工具。路由依赖 modes/、config/ 和脚本，均已保留。

本次只下载、检查和收录源文件，没有运行安装器、安装业务依赖、配置账号、启动服务或执行完整业务流程。宿主兼容性与实际运行结果需要在后续明确使用时验证。

历史仓库地址 `santifer/career-ops` 经 GitHub API 重定向至 `career-ops-hq/career-ops`；本次使用重定向后的官方地址。
