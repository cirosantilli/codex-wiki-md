<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [terminal object](../../../../../../terminal-object.md) and [pullbacks in a category](../../../../../../pullback-category-theory.md) give a binary product $X\times Y$ by pulling back $X\to1\leftarrow Y$. Repeating this gives every finite product, with the empty product supplied by the [terminal object](../../../../../../terminal-object.md). The preceding parts then construct [equalizers](../../../../../../equaliser.md) of arbitrary parallel arrows.

For a diagram $D:J\to\mathcal C$ with finitely many objects and arrows, form $P=\prod_{j\in\operatorname{Ob}J}D(j)$ and $Q=\prod_{a:j\to k}D(k)$. Define $r,s:P\to Q$ by $r_a=D(a)\pi_j$ and $s_a=\pi_k$. Their [equalizer](../../../../../../equaliser.md) $e:L\to P$ has projections $\pi_je$ satisfying every cone equation. Conversely a [categorical cone](../../../../../../cone-over-a-diagram.md) supplies a unique map to $P$, and its cone equations say that this map equalizes $r,s$, hence factors uniquely through $L$. Thus $L$ is the [categorical limit](../../../../../../categorical-limit.md). This proves **a [terminal object](../../../../../../terminal-object.md) and all pullbacks give all finite limits**, including the empty diagram.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
