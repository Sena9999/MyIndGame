# 初始化参考与取舍

查阅日期：2026-10-22。以下链接是资料来源，不代表已选定相应引擎。模板内容为本项目重新编写，未直接搬入外部仓库文件。

| 来源 | 采用内容 | 在本项目中的落实 |
| --- | --- | --- |
| [Godot 官方：Project organization](https://docs.godotengine.org/en/stable/tutorials/best_practices/project_organization.html) | 相关场景和资源靠近、保持命名一致、关注大小写 | `game/README.md` 提供按功能组织的建议；具体布局服从引擎 |
| [GitHub：GDDMarkdownTemplate](https://github.com/LazyHatGuy/GDDMarkdownTemplate) | 明确体验、玩法与项目范围 | 精简为一页策划；暂不展开完整剧情、AI 等尚不需要的章节 |
| [Git 官方：gitignore](https://git-scm.com/docs/gitignore) | 忽略生成文件；忽略规则不影响已跟踪文件 | 缓存和本地构建进入 `.gitignore`，源文件保留 |
| [GitHub 官方：Git LFS](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage) | 大文件以指针关联外部存储 | 先提供启用步骤，待实际素材与托管方案确定后配置 |

个人迭代、阶段门槛和完成定义是针对当前空白项目的工作建议，不是对外部经验贴成功率的承诺。等玩法、时间预算和制作工具确定后再调整。
