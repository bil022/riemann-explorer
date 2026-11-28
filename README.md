# Riemann Hypothesis proof explorer · 黎曼猜想证明浏览器

**<https://bil022.github.io/riemann-explorer/>**

A website for going through the Lean proofs of the Riemann Hypothesis level by
level, each page showing one theorem, the parts used only by it, their sizes,
how they use each other, and their Lean code. The menu at the top left picks
the proof:

- the first proof,
  [leanprover-community/riemann-hypothesis](https://github.com/leanprover-community/riemann-hypothesis)
  (commit `6c68212`, 727,065 declarations);
- its readable rewrite, [lsernau/grh-lean](https://github.com/lsernau/grh-lean)
  folder `grh/` (commit `72fead1`, 21,597 declarations);
- its compact rewrite, folder `grh-compact/` of the same repository (12,533
  declarations).

一个可以一层层浏览黎曼猜想 Lean 证明的网站：每一页显示一个定理、只为它服务的各部分、它们的
大小、彼此的引用关系，以及 Lean 代码。左上角的菜单选择证明：最早的
leanprover-community/riemann-hypothesis（727,065 个声明），以及 lsernau/grh-lean 里的
易读版 `grh/`（21,597 个）和紧凑版 `grh-compact/`（12,533 个）。

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
