# Depth-first search parenthesis property

↑ **Parent:** [Depth-first search](depth-first-search.md)

The discovery-to-finishing intervals of distinct [vertices](vertex-graph-theory.md) in a [depth-first search](depth-first-search.md) are either disjoint or strictly nested. A recursive call completes before its caller returns; separate completed branches have disjoint intervals. Thus the displayed nesting holds exactly when $v$ is a proper [descendant in a rooted tree](descendant-in-a-rooted-tree.md) of $u$ in the discovery [forest](forest.md). A [directed path](directed-path.md) alone does not imply this nesting, because it can leave the current branch through an already discovered ancestor.

## ↑ Ancestors (4)

1. [Depth-first search](depth-first-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
