<h1 id="22f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a countable [dense subset](../../../../../../dense-set.md) $\{x_1,x_2,\ldots\}$ of the [normed vector space](../../../../../../normed-vector-space.md) $X$. For each fixed $j$, the scalar sequence $(f_n(x_j))$ is bounded because

$$
|f_n(x_j)|\leq\|f_n\|\,\|x_j\|\leq\|x_j\|.
$$

Repeated use of the [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md) followed by a [diagonal subsequence argument](../../../../../../diagonal-subsequence-argument.md) produces a subsequence $(f_n)_{n\in\Lambda}$ for which $f_n(x_j)$ converges for every $j$.

Let $D$ be the linear span of the $x_j$. On every $x\in D$, define

$$
f(x)=\lim_{\substack{n\in\Lambda\\n\to\infty}}f_n(x).
$$

Finite linear combinations show that $f:D\to\mathbb R$ is linear, and passage to the limit in $|f_n(x)|\leq\|x\|$ gives $|f(x)|\leq\|x\|$. Thus $f$ is a [bounded linear functional](../../../../../../continuous-linear-functional.md) on the dense linear subspace $D$ and extends uniquely to an element of the [dual space](../../../../../../dual-space.md) $X^*$ with $\|f\|\leq1$.

For arbitrary $x\in X$ and $y\in D$,

$$
|f_n(x)-f(x)|
\leq|f_n(x-y)|+|f_n(y)-f(y)|+|f(y-x)|
\leq2\|x-y\|+|f_n(y)-f(y)|.
$$

First choose $y$ close to $x$, then let $n\in\Lambda$ tend to infinity. This proves

$$
\boxed{f_n(x)\longrightarrow f(x)\quad\text{for every }x\in X}.
$$

This is the [Sequential Banach-Alaoglu theorem for a separable predual](../../../../../../sequential-banach-alaoglu-theorem-for-a-separable-predual.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22F](../../22f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
