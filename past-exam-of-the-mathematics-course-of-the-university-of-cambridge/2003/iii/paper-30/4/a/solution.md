<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $L=\inf_{k\ge1}x_k/k$. It may be $-\infty$, but cannot be $+\infty$ because $x_1$ is finite. Fix $k$ and write $n=qk+r$, $0\le r<k$. Repeated use of the [subadditive sequence](../../../../../../subadditive-sequence.md) inequality gives

$$
x_n\le qx_k+C_k,\qquad C_k=\max(0,x_1,\ldots,x_{k-1}),
$$

where $C_1=0$. Dividing by $n$ and letting $n\to\infty$ gives $\limsup x_n/n\le x_k/k$. Since this holds for every $k$, the upper [limit of a sequence](../../../../../../limit-of-a-sequence.md) is at most $L$, while every ratio is at least $L$. If $L$ is finite these bounds agree. If $L=-\infty$, choose $k$ with $x_k/k$ below any prescribed real number; the same upper-limit bound proves convergence to $-\infty$. This establishes the [extended-real Fekete lemma](../../../../../../fekete-s-lemma.md):

$$
\boxed{\lim_{n\to\infty}\frac{x_n}{n}=\inf_{k\ge1}\frac{x_k}{k}\in[-\infty,\infty).}
$$

A finite real [limit of a sequence](../../../../../../limit-of-a-sequence.md) requires a lower linear bound. For example $x_n=-n^2$ satisfies the premise but has normalized [limit of a sequence](../../../../../../limit-of-a-sequence.md) $-\infty$, so that qualification cannot be dropped.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
