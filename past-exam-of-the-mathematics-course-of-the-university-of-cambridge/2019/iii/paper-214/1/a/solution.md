<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put

$$
\alpha=\inf_{k\geq1}\frac{x_k}{k}.
$$

Fix $k\geq1$ and write $n=qk+r$ with $0\leq r<k$. Repeated [subadditivity](../../../../../../subadditive-sequence.md) gives

$$
x_n\leq qx_k+x_r,
$$

so

$$
\frac{x_n}{n}\leq\frac{qk}{n}\frac{x_k}{k}+\frac{x_r}{n}.
$$

The finitely many values $x_0,\ldots,x_{k-1}$ are bounded, hence

$$
\limsup_{n\to\infty}\frac{x_n}{n}\leq\frac{x_k}{k}.
$$

Taking the infimum over $k$ gives $\limsup x_n/n\leq\alpha$, while the definition of $\alpha$ gives $x_n/n\geq\alpha$ for every $n$. Therefore

$$
\boxed{\lim_{n\to\infty}\frac{x_n}{n}=\inf_{k\geq1}\frac{x_k}{k}.}
$$

This is [Fekete lemma](../../../../../../fekete-s-lemma.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
