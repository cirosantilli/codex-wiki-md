# Recursively repetition-free labelled tree

↑ **Parent:** [Rooted tree](rooted-tree.md)

For a label [set](set-split.md) $D$, define $\mathcal T(D)$ inductively: choose a root label $d\in D$ and a [finite repetition-free sequence](finite-repetition-free-sequence.md) of [rooted trees](rooted-tree.md) in $\mathcal T(D\setminus\{d\})$ as its children. Each object is a finite ordered [rooted tree](rooted-tree.md). Labels are distinct along each root-to-leaf path, and child [rooted trees](rooted-tree.md) at a vertex are distinct as whole [rooted trees](rooted-tree.md). Labels may repeat across different branches; children need not have distinct root labels. For a finite pool of size $m$, the exact number $t_m$ of [rooted trees](rooted-tree.md) satisfies

$$
t_0=0,\qquad t_m=m\sum_{k=0}^{t_{m-1}}\frac{t_{m-1}!}{(t_{m-1}-k)!}.
$$

This follows by choosing the root and then an ordered repetition-free list from the finite pool of smaller [rooted trees](rooted-tree.md).

**Table of contents**

- [Recursively repetition-free labelled trees preserve Dedekind-finiteness](recursively-repetition-free-labelled-trees-preserve-dedekind-finiteness.md)

## ↑ Ancestors (6)

1. [Rooted tree](rooted-tree.md)
2. [Tree (graph theory)](tree-graph-theory.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135/1/2/solution.md)
