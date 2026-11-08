# 观点手册

每周收集的有趣观点和内容，整理成手册的手机网页 App，可以添加到主屏幕、离线打开。

- `data/catalog.json`：目录（每篇的标题、分类、标签、摘要和数据文件路径）
- `data/entries/<id>.json`：每篇的完整内容——`handbook`（手册）、`viewpoints`（观点）、`thinking`（思考）、`derived`（衍生）、`expression`（表达方式）、`concepts`（概念卡）
- 概念库、表达库由所有篇目自动汇总；已读和「想练」标记保存在手机本地

新内容由 Claude 整理后提交到 `data/`：新增一个 `entries/<id>.json`，并在 `catalog.json` 里加一行。手机联网打开时会自动拿到最新内容。
改了 `index.html` 之后，把 `sw.js` 里的 `VERSION` 加一，手机才会更新界面。
