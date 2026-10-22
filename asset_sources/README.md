# 素材源文件

- `art/`：模型、绘画、动画等可编辑源文件。
- `audio/`：录音、音效和音乐工程。
- `reference/`：视觉、玩法和声音参考。参考不等于获得再分发权。

运行时导出资源放 `game/`，不要让引擎扫描整个工作区。每次更新素材，记录源文件、导出路径和必要导出参数；不要直接修改导出文件后丢失源文件关系。

新增外部素材前先填写 `third_party/assets.csv`。无法确认授权的资源先不要纳入可发布内容。

## 大文件

当前没有启用 LFS，以免产生依赖但未安装过滤器。首次提交 PSD、BLEND、WAV 等大体积且会反复修改的文件前，确认托管平台和存储预算，再安装 Git LFS，并在本仓库执行：

```powershell
git lfs install --local
git lfs track "*.blend" "*.psd" "*.wav"
git add .gitattributes
git lfs ls-files
```

按实际格式调整，不必把所有小图放入 LFS。已进入 Git 历史的大文件需要另行迁移，添加规则不会自动转换历史。LFS 及远程仓库不能替代源文件备份，应另留一份可恢复备份。
