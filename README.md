# Riemann Hypothesis proof explorer · 黎曼猜想证明浏览器

**<https://bil022.github.io/riemann-explorer/>**

A website for going through the Lean proof of the Riemann Hypothesis,
[leanprover-community/riemann-hypothesis](https://github.com/leanprover-community/riemann-hypothesis)
(commit `6c68212`), level by level: 727,065 declarations, each page showing one
theorem, the parts used only by it, their sizes, how they use each other, and
their Lean code.

一个可以一层层浏览黎曼猜想 Lean 证明的网站：727,065 个声明，每一页显示一个定理、只为它服务的
各部分、它们的大小、彼此的引用关系，以及 Lean 代码。

This repository holds only the built site. The scripts that build it, and how
to read it, are in
[bil022/ten-proofs/scripts/rh](https://github.com/bil022/ten-proofs/tree/main/scripts/rh)
([中文说明](https://github.com/bil022/ten-proofs/blob/main/scripts/rh/README.zh.md)).

本仓库只存放生成好的网站。生成它的脚本和使用说明在
[bil022/ten-proofs/scripts/rh](https://github.com/bil022/ten-proofs/tree/main/scripts/rh)。

To run it locally · 在本地运行：

```bash
python3 -m http.server 8000    # then open http://localhost:8000
```

The page uses [Cytoscape.js](https://js.cytoscape.org/) and cytoscape-dagre
(MIT licences in `vendor/`).
