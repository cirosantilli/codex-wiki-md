<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because $T$ itself is a tree, every finite induced connected exhaustion has the unique spanning tree consisting of all its edges. Thus its free spanning forest is deterministically $T$.

By the stated transience criterion, choose an edge $e=uv$ whose two complementary subtrees are transient. Run [Wilson algorithm rooted at infinity](../../../../../../wilson-algorithm-rooted-at-infinity.md) first from $u$. With positive probability its loop-erased walk remains forever in the $u$-side. Starting next from $v$, there is likewise positive conditional probability that its walk remains forever in the $v$-side. On this event the two rays never use $e$, so $e$ is absent from the [wired uniform spanning forest](../../../../../../wired-uniform-spanning-forest.md). The wired law is therefore not the deterministic free law.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
