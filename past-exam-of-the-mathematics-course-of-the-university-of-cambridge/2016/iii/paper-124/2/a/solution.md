<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The event that infinitely many $A_n$ occur is $\limsup_n A_n=\bigcap_{m\ge1}\bigcup_{n\ge m}A_n$. For every $m$, the [union bound](../../../../../../boole-s-inequality.md) and monotonicity of a [probability measure](../../../../../../probability-measure.md) give

$$
0\le\mathbb P(\limsup_n A_n)\le\mathbb P\left(\bigcup_{n\ge m}A_n\right)\le\sum_{n\ge m}\mathbb P(A_n).
$$

The right-hand side tends to zero as the tail of a convergent series. Therefore **the first Borel-Cantelli conclusion** is

$$
\boxed{\mathbb P(\limsup_n A_n)=0.}
$$

This proves the [Borel-Cantelli first lemma](../../../../../../borel-cantelli-first-lemma.md) without any [independence](../../../../../../independent-random-variables.md) assumption.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
