<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Let $U=\{x\geq0:\|x\|_2=1\}$. This set is nonempty and [compact](../../../../../../compact-space.md) for $n\geq1$, and the [quadratic form](../../../../../../quadratic-form.md) is continuous. Its minimum $\alpha$ is therefore attained.

For every nonzero $y$ in the [nonnegative orthant](../../../../../../nonnegative-orthant.md), normalizing $y$ gives

$$
y^T(Q-\lambda I)y
=\|y\|_2^2\left[\left(\frac y{\|y\|_2}\right)^T
Q\left(\frac y{\|y\|_2}\right)-\lambda\right].
$$

The zero [vector](../../../../../../vector.md) imposes no further condition. It follows that $Q-\lambda I$ is a [copositive matrix](../../../../../../copositive-matrix.md) exactly when $\lambda\leq\alpha$. Thus the feasible [scalar](../../../../../../scalar.md) set is $(-\infty,\alpha]$, and

$$
\boxed{\alpha=\max\{\lambda:Q-\lambda I\in K\}}.
$$

Both optima are attained. This [copositive reformulation of an orthant Rayleigh minimum](../../../../../../copositive-reformulation-of-an-orthant-rayleigh-minimum.md) follows directly from homogeneity; it does not require invoking a duality theorem for the original nonconvex constraint.

The restriction to $x\geq0$ matters. For the [matrix](../../../../../../matrix.md) in part (a), this minimum is $1$ whereas the unrestricted smallest [eigenvalue](../../../../../../eigenvalue.md) is $-1$.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
