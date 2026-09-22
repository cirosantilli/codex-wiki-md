<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First perform [splaying](../../../../../splaying.md) on the key to be deleted, making its node the [root of a tree](../../../../../root-of-a-tree.md). Delete that root, leaving left and right [subtrees](../../../../../subtree.md) $L,R$. If either is empty, return the other. Otherwise find the maximum key $m$ of $L$ by following right-child references, and perform [splaying](../../../../../splaying.md) on $m$ within $L$. This makes $m$ the root of $L$ with an empty right [subtree](../../../../../subtree.md). Attach $R$ there. **The result is the original [splay tree](../../../../../splay-tree.md) with exactly the selected key removed.** An unsuccessful lookup leaves the represented [set](../../../../../set-split.md) unchanged.

For [algorithm correctness](../../../../../algorithm-correctness.md), all keys of $L$ are smaller than the deleted key, and all keys of $R$ are larger. [Splaying](../../../../../splaying.md) preserves the [binary search tree](../../../../../binary-search-tree.md) property by the permitted assumption. Since $m$ is the maximum of $L$, it has no larger key within $L$; since every key of $R$ exceeds $m$, attaching $R$ as its right [subtree](../../../../../subtree.md) preserves every ordering condition. All remaining keys occur once. This is the join-based deletion of a [splay tree](../../../../../splay-tree.md).[Author-hosted publication record and abstract: splay-tree search, insertion and deletion operations](../../../../../self-adjusting-binary-search-trees-by-daniel-sleator-and-robert-tarjan.md)

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
