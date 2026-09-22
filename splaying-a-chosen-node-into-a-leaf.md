# Splaying a chosen node into a leaf

↑ **Parent:** [Splaying](splaying.md)

Every node of a [splay tree](splay-tree.md) with at least four distinct keys can become a [leaf of a rooted tree](leaf-of-a-rooted-tree.md) using only successful [splaying](splaying.md) operations. At an extreme key, access that key and then its sole adjacent stored key; the [consecutive keys in a binary search tree](consecutive-keys-in-a-binary-search-tree.md) property makes the extreme key a leaf. For an interior key $x$ with two larger stored keys, take consecutive $a<x<b<c$ and access $c,a,b$; the mirror construction handles two smaller keys.

For a quick shape proof, use $k(L,R)$ for a node and its two [subtrees](subtree.md). After accessing $c,a$, the right [subtree](subtree.md) of $a$ can only be $c(b(x,0),D)$, $c(x(0,b),D)$, $b(x,c(0,D))$, or $x(0,c(b,D))$, with outside [subtrees](subtree.md) $A$ below $a$ and $D$ above $c$. This follows by inspecting the final [zig step](zig-step.md), [zig-zig step](zig-zig-step.md) or [zig-zag step](zig-zag-step.md) that moves $a$ above the former root $c$. In each case, accessing $b$ yields $b(a(A,x),c(0,D))$, where $x$ is a leaf and $0$ denotes an empty [subtree](subtree.md). These rotations prove the bound for arbitrary outside [subtrees](subtree.md).

## ↑ Ancestors (7)

1. [Splaying](splaying.md)
2. [Splay tree](splay-tree.md)
3. [Binary search tree](binary-search-tree.md)
4. [Binary tree](binary-tree.md)
5. [Data structure](data-structure-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/1/f/solution.md)
