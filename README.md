# MyIndGame

独立游戏工作区。当前阶段：构思与原型；游戏名称、类型、引擎和平台尚未确定。

## 从这里开始

1. 填写 [一页策划](docs/design/one_page.md)，先确定玩家做什么、为什么有趣。
2. 在 [技术决策](docs/production/decisions.md) 中记录引擎、精确版本、语言及目标平台。
3. 在 `game/` 内创建引擎工程，并按 [接入说明](game/README.md) 补齐对应配置。
4. 从 [任务板](docs/production/backlog.md) 选一个任务，完成最小核心循环。
5. 参考 [开发流程](docs/production/workflow.md) 试玩、记录、提交，再决定下一步。

## 目录

```text
MyIndGame/
├── game/                 引擎工程、运行时代码及实际导入资源
├── asset_sources/        Blender、绘画、音频等可编辑源文件
│   ├── art/
│   ├── audio/
│   └── reference/        参考资料，需记录来源及使用范围
├── docs/
│   ├── design/           一页策划与玩法说明
│   ├── production/       任务、里程碑、决策与工作流
│   ├── playtests/        试玩记录模板
│   └── research/         已阅读资料与采用理由
├── third_party/          第三方授权记录、许可证
├── tools/                项目辅助脚本
├── builds/               本地导出产物，Git 忽略
└── .github/              GitHub Issue 与 PR 模板
```

目录按需要扩展；引擎内部优先按功能组织，避免提前建立大量空系统。美术源文件放 `asset_sources/`，导出的 PNG、GLB、OGG 等放入 `game/` 的对应功能目录，记录导出关系。

## 版本管理

已提供忽略规则、换行规则与编辑器配置。生成缓存、构建包和本地密钥不提交；代码、引擎设置、导入设置、素材与授权记录应提交。首次加入大体积二进制文件前，阅读 [素材说明](asset_sources/README.md)。

建议提交粒度：一个可以解释清楚、可以验证的变化。可用 `feat:`、`fix:`、`docs:`、`chore:` 前缀。个人开发可直接使用 `main`，较大试验使用短期分支。远程仓库尚未配置；首次提交前先检查 `git status` 与 `git diff`。

参考来源和采用取舍见 [资料记录](docs/research/references.md)。当前只完成工作区初始化，还没有可运行游戏或自动构建流程。
