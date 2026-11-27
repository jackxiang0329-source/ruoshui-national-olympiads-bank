# Pythagoras – World Mathematical Olympiads Bank

Olympiad problem statements in English with LaTeX: national finals and IMO team selection tests, regional and international olympiads, Kangaroo, USA AMC and undergraduate competitions.

Website: https://eisatopon.github.io/national-olympiads-bank/

This repository contains only the files the website loads. **All rights reserved** — see `LICENSE`. Personal study and classroom use of the website are welcome; copying or redistributing the data or the application requires written permission. Problem statements belong to their competition organisers.

© Sokratis Romanidis · eisatopon.gr

**Repository navigation** · [Website files](index.html) · [Undergraduate competitions](undergraduate/) · [Upstream rights and license](LICENSE)


## 仓库目录 / Repository layout

- [bank/](bank/): 282 original competition JSON files; filenames use lowercase snake_case. File contents and problem identifiers are unchanged.
- [undergraduate/](undergraduate/): existing undergraduate collections; compatibility paths are retained.
- [metadata/](metadata/), [sources/](sources/), [pdfs/](pdfs/): existing metadata, provenance and PDF resources.

The website's upstream collection keys and data URLs are unchanged; for this repository's local copies, map the original root JSON filename to `bank/` plus its lowercase name with hyphens replaced by underscores. Existing external raw links to the old root paths must be updated. Original rights and license remain unchanged.


### 2026-11-27 本地题库路径一致性

网页题库读取统一指向本仓库的 `bank/`（282 个已规范化文件）和 `undergraduate/`（14 个现有集合）。保留原集合名作为 `metadata/runtime/` 的索引键，避免破坏题号、审查元数据与历史链接；不再从上游滚动 main 下载可能与本地元数据版本不一致的题目。已核对网页声明的全部296个集合路径存在；浏览器端完整交互与逐题数学审核尚未完成。需要通过 HTTP 服务打开网页，而非直接使用 file://。
