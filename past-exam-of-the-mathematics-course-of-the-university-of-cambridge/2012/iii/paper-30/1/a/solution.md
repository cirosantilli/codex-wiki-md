<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

This is the [Fekete lemma](../../../../../../fekete-s-lemma.md), with its possible extended-real limit made explicit. Put $L=\inf_{m\ge1}x_m/m$. Since $x_n\le nx_1$, $L$ cannot be $+\infty$; it may be $-\infty$.

Fix $m\ge1$ and write $n=qm+r$, with $0\le r<m$. Repeated [subadditivity](../../../../../../subadditive-sequence.md) gives

$$
x_n\le qx_m+x_r,
$$

where for this calculation set $x_0=0$. The finitely many possible remainder terms are bounded. Since $q/n\to1/m$,

$$
\limsup_{n\to\infty}\frac{x_n}{n}\le\frac{x_m}{m}.
$$

This holds for every $m$, whereas $x_n/n\ge L$ by the definition of an [infimum](../../../../../../infimum.md). If $L$ is finite, the upper and lower bounds agree. If $L=-\infty$, choosing $m$ with arbitrarily negative $x_m/m$ shows that $x_n/n\to-\infty$. Thus

$$
\boxed{\lim_{n\to\infty}\frac{x_n}{n}=\inf_{m\ge1}\frac{x_m}{m}\in[-\infty,\infty).}
$$

A finite real limit is not guaranteed: $x_n=-n^2$ is a [subadditive sequence](../../../../../../subadditive-sequence.md) and has $x_n/n=-n\to-\infty$. If the limit is intended to be real rather than extended real, one must add a linear lower bound.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
