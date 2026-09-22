<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\mathcal F_n=\sigma(X_0,\ldots,X_n)$ and $\tau=T_0\wedge T_y$. Before $\tau$, the integer-valued increment belongs to $\{-1,0,1\}$. The [martingale](../../../../../../martingale-split.md) property gives

$$
\mathbb P(X_{n+1}-X_n=1\mid\mathcal F_n)
=\mathbb P(X_{n+1}-X_n=-1\mid\mathcal F_n).
$$

Their sum is at least $1/2$, so each conditional probability is at least $1/4$. From any state in $\{1,\ldots,y-1\}$, a run of at most $y$ upward moves reaches $y$ and has conditional probability at least $4^{-y}$. Applied in successive blocks of $y$ steps, this gives

$$
\mathbb P(\tau>ky)\leq(1-4^{-y})^k,
$$

so $\tau<\infty$ almost surely.

The stopped process $X_{n\wedge\tau}$ takes values in $[0,y]$, hence is a bounded martingale and has [uniform integrability](../../../../../../uniform-integrability.md). The [optional sampling theorem for a supermartingale](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
x=\mathbb E[X_\tau]
=y\mathbb P(T_y<T_0),
$$

because $X_\tau$ is zero or $y$. Therefore

$$
\boxed{\mathbb P(T_y<T_0)=\frac{x}{y}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
