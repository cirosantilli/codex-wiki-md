<h1 id="22f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $z_0\in S^1$, and let $\delta_{z_0}\in C(S^1)^*$ be the [point evaluation functional](../../../../../../point-evaluation-functional.md) $\delta_{z_0}(f)=f(z_0)$. Define orbit averages in the dual space by

$$
\mu_n=\frac1n\sum_{j=0}^{n-1}(T^*)^j\delta_{z_0}.
$$

Each $\mu_n$ has norm at most one and satisfies $\mu_n(1_{S^1})=1$. The space $C(S^1)$ is separable, so part (a) gives a subsequence converging pointwise to some $\mu\in C(S^1)^*$. In particular,

$$
\mu(1_{S^1})=1.
$$

For every $f\in C(S^1)$, the [Cesaro average](../../../../../../cesaro-mean.md) telescopes at the endpoints:

$$
\mu_n(Tf)-\mu_n(f)
=\frac{\delta_{z_0}(T^nf)-\delta_{z_0}(f)}n,
$$

whose absolute value is at most $2\|f\|_\infty/n$. Passing to the convergent subsequence proves

$$
\boxed{\mu(Tf)=\mu(f)\quad\text{for every }f\in C(S^1)}.
$$

Thus $\mu$ is an [invariant functional of a composition operator](../../../../../../invariant-functional-of-a-composition-operator.md).

It need not be unique when $T$ is not the [identity operator](../../../../../../identity-operator.md). For the nonidentity [homeomorphism](../../../../../../homeomorphism.md) $\tau(z)=\overline z$, both $1$ and $-1$ are fixed. Hence the two distinct point evaluations

$$
\delta_1(f)=f(1),
\qquad
\delta_{-1}(f)=f(-1)
$$

have value one on $1_{S^1}$ and are invariant under $T$. Therefore **nonidentity does not imply uniqueness**.

## ↑ Ancestors (11)

1. [C](../c.md)
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
