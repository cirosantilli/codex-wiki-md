<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**True.** Choose a countable dense sequence $(x_j)$ in the separable [Banach space](../../../../../../banach-space-split.md) $E$. For $\phi,\psi$ in its closed dual [unit ball](../../../../../../unit-ball.md), put

$$
\rho(\phi,\psi)=\sum_{j=1}^\infty2^{-j}
\frac{|(\phi-\psi)(x_j)|}{1+|(\phi-\psi)(x_j)|}.
$$

This is a [metric](../../../../../../metric.md): positivity follows because continuous functionals agreeing on a [dense subset](../../../../../../dense-set.md) agree everywhere; symmetry is immediate; and the triangle inequality follows from subadditivity of $t/(1+t)$ for $t\geq0$. The tail of the series is uniformly small, so convergence on these coordinates implies convergence for this metric, and conversely metric convergence controls each individual coordinate.

The uniform bound $\|\phi-\psi\|\leq2$ upgrades coordinate convergence to [pointwise convergence](../../../../../../pointwise-convergence.md) on all of $E$. For any $x\in E$, choose $x_j$ close to $x$ and use

$$
|\phi(x)-\psi(x)|\leq|\phi(x_j)-\psi(x_j)|+2\|x-x_j\|.
$$

For neighbourhoods involving finitely many $x$, choose finitely many such approximations. This proves equality of the induced topologies, including for arbitrary nets. Thus the [weak-star metrizability of the dual ball](../../../../../../weak-star-metrizability-of-the-dual-ball.md) gives

$$
\boxed{B'\text{ is metrizable in its relative weak-star topology}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
