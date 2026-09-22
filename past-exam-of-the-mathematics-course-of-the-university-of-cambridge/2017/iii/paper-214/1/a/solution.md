<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\alpha=\inf_{k\geq1}x_k/k$. The relevant version of the [Fekete lemma](../../../../../../fekete-s-lemma.md) is the [extended-real Fekete lemma](../../../../../../fekete-s-lemma.md): $\alpha$ may be $-\infty$, but cannot be $+\infty$ because $x_1$ is real. We show that this is exactly the [limit of a sequence](../../../../../../limit-of-a-sequence.md).

Fix $k\geq1$ and, for $n\geq k$, write $n=qk+r$, where $q\geq1$ and $0\leq r<k$. Iterating the defining inequality gives $x_{qk}\leq qx_k$. If $r>0$, it also gives $x_n\leq qx_k+x_r$; if $r=0$, there is no remainder term. Thus, with $C_k=\max(0,x_1,\ldots,x_{k-1})$ and $C_1=0$,

$$
\frac{x_n}{n}\leq\frac qn x_k+\frac{C_k}n.
$$

As $n\to\infty$, $q/n\to1/k$, so $\limsup_n x_n/n\leq x_k/k$. This holds for every positive $k$. On the other hand every $x_n/n\geq\alpha$. If $\alpha$ is finite, these two bounds give the desired equality. If $\alpha=-\infty$, for every real $M$ choose $k$ with $x_k/k<M-1$; the same upper bound makes $x_n/n<M$ for all sufficiently large $n$. Therefore

$$
\boxed{\lim_{n\to\infty}\frac{x_n}{n}=\inf_{k\geq1}\frac{x_k}{k}\in[-\infty,\infty).}
$$

The index $k=0$ is excluded because its ratio is undefined, and $x_0$ is irrelevant since the defining inequality was required only at positive indices. If the printed word “[limit of a sequence](../../../../../../limit-of-a-sequence.md)” is interpreted as a finite real [limit of a sequence](../../../../../../limit-of-a-sequence.md), an additional lower bound is necessary: $x_n=-n^2$ defines a [subadditive sequence](../../../../../../subadditive-sequence.md) but $x_n/n=-n\to-\infty$. The extended-real statement is the correct unrestricted conclusion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
