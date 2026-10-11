# frontend-art-direction 来源记录

- 来源类型：第三方修改版（仅添加中文收录入口与来源说明，上游文件原样保留）。
- 作者 / 组织：davaded（GitHub 仓库所有者；未确认其他作者信息）。
- 官方项目：https://github.com/davaded/frontend-art-direction
- 主 Skill 固定版本：https://github.com/davaded/frontend-art-direction/blob/9696da4c573bada9deea5564af7cfeb159f6fdda/SKILL.md
- 官方主文件下载：https://raw.githubusercontent.com/davaded/frontend-art-direction/9696da4c573bada9deea5564af7cfeb159f6fdda/SKILL.md
- 官方固定提交源码包：https://codeload.github.com/davaded/frontend-art-direction/tar.gz/9696da4c573bada9deea5564af7cfeb159f6fdda
- 分支：`main`（通过 GitHub API 解析到下面的固定提交）。
- 提交：`9696da4c573bada9deea5564af7cfeb159f6fdda`。
- Git tree：`43647ecdcea1a7b76fd135282d168ffd4cd67ba9`。
- 版本：`package.json` 与原版 `SKILL.md` 元数据均为 `1.0.0`。
- 提交时间：2026-10-11 06:26:52（Asia/Shanghai；原始时间 2026-10-10T22:26:52Z）。
- 收录日期：2026-10-11（Asia/Shanghai）。
- Skill 整体许可证：待确认。该提交根目录未见 `LICENSE`、`COPYING` 或 `NOTICE`；`package.json` 未声明 `license`，GitHub 仓库 API 的 `license` 为 `null`。未创建或推定许可证。

## 收录范围与下载核对

`upstream/` 保存上游 `package.json` 的 `files` 字段指定的全部 Skill 发布文件：`SKILL.md`、`README.md`、`agents/`、`bin/`、`scripts/`、`data/`、`references/`、`templates/` 和 `docs/`。另保留 `package.json`、`CHANGELOG.md` 和 `CONTRIBUTING.md`。

本次共保存 77 个上游文件、914,398 字节。未收录 `benchmarks/`、`.github/`、Git 历史或安装产物；此目录是 Skill 运行文件快照，不是完整仓库快照。

官方源码包传输及完整仓库 API 下载在大体积测试图片上超时。本次改为通过 GitHub API 获取固定提交的发布文件，并逐文件核对字节数和 Git blob SHA-1；已通过核对。上方源码包链接保留为官方获取入口，本次没有生成完整压缩包的 SHA-256。

上游测试素材目录另有 [lucide-LICENSE.txt](https://github.com/davaded/frontend-art-direction/blob/9696da4c573bada9deea5564af7cfeb159f6fdda/benchmarks/visual/shared/assets/lucide-LICENSE.txt)，该目录不在发布文件范围内，未一并收录。这份素材许可不能视为整个 Skill 的许可。

## 本地修改

- 顶层 `SKILL.md` 是中文索引入口，名称与收录目录一致，实际设计流程指向 `upstream/SKILL.md`。
- 顶层 `SOURCE.md` 记录来源、固定版本、收录范围和许可情况。
- 上游文件未翻译或改写。20 个流程检查点、迭代记录等要求原样保留，未为 pipi 或其他项目定制流程。

## 依赖与验证边界

辅助脚本要求 Node.js >=18；实际前端实现、构建和截图依赖目标项目环境。截图工具需要目标项目已有 Playwright 或 Puppeteer；动效桥在需要时会获取固定版本的外部参考。

本次仅下载和收录源码，并进行格式、引用、脚本语法和 CLI 帮助入口检查。没有运行安装器、安装业务依赖、启动前端服务、执行完整设计流程或视觉测试，也没有安装到 Codex、pipi 或其他项目。实际设计效果和宿主兼容性需在后续明确使用时验证。
