# Binary Search Tree Visualizer

An interactive, browser-based tool for building and exploring Binary Search Trees in real time. Built with vanilla JavaScript and the Canvas API — no dependencies, no build step, just open and use.

![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![HTML5 Canvas](https://img.shields.io/badge/HTML5-Canvas-orange)
![No Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen)

## What it does

Insert values one by one or hit **Random Insert** to watch the tree build itself. The canvas redraws on every operation, showing the live structure of the tree as nodes are added or removed.

Every change updates three things instantly:

- **Tree visualization** — nodes drawn on canvas with connecting edges
- **Traversal outputs** — inorder, preorder, and postorder sequences recalculated live
- **Tree stats** — total node count, height, and root value

## Operations

| Action | What happens |
|---|---|
| Insert Node | Adds value to correct BST position |
| Delete Node | Removes node, restructures tree correctly |
| Random Insert | Inserts a random value between 1–100 |
| Clear Tree | Resets everything |
| Enter key | Shortcut for Insert |

## How to run

No install, no server, no build.

```
git clone https://github.com/suyashkumar102/Binary-Search-Tree-Visualizer
cd Binary-Search-Tree-Visualizer
open index.html
```

Or just double-click `index.html`.

## Implementation notes

- Tree rendering uses the HTML5 Canvas API directly
- Node positions calculated recursively — horizontal spacing halves at each level
- Deletion handles all three cases: leaf node, one child, two children (inorder successor swap)
- Traversals implemented recursively, output as arrow-separated sequences

## BST properties visualized

Left subtree values are always less than the parent. Right subtree values are always greater. Inorder traversal of a valid BST always produces a sorted sequence — you can verify this live by inserting any values and watching the inorder output.
