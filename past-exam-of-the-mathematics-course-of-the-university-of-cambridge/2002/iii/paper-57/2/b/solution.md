<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) in part (a) is strictly positive and start with all four species positive. Choose weights recursively by $w_{i+1}=w_ia_i/b_i$ and define

$$
V=\sum_{i=1}^4w_i\bigl[X_i-X_{i*}-X_{i*}\log(X_i/X_{i*})\bigr].
$$

The weighted interaction [matrix](../../../../../../matrix.md) is [skew-symmetric matrix](../../../../../../skew-symmetric-matrix.md): for every adjacent pair $w_ia_i=w_{i+1}b_i$. On differentiating $V$, the [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) removes the constant growth terms, while paired products cancel. Thus $\dot V=0$. Each summand is nonnegative and diverges as its positive argument approaches zero or infinity. A fixed level of $V$ therefore bounds every abundance above and away from zero. This proves genuine persistence of all four species, although their dynamics need not converge to a fixed point.

Integrate each per-capita equation over $[0,T]$ and divide by $T$. Since $\log X_i(T)$ is bounded, the left side tends to zero. Writing $\overline X_i(T)=T^{-1}\int_0^TX_i(t)\,dt$, the limiting balances give

$$
\boxed{\lim_{T\to\infty}\overline X_i(T)=X_{i*}\quad(i=1,2,3,4),}
$$

with the explicit abundances listed in part (a). The limit exists because the invertible four-level interaction [matrix](../../../../../../matrix.md) solves the averaged linear equations, whose residuals tend to zero. Periodicity or an ergodic assumption is not needed.

The same proof works for any even nearest-neighbor chain with a feasible positive [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md). It does not make all even-chain parameters feasible. Odd chains generically lack the required positive balance, and in their exceptional balanced cases the averaged equations do not uniquely fix every abundance. Resource density dependence and more general feeding interactions alter both the conservation law and the simple parity classification. **Coexistence and the stated [mean](../../../../../../expected-value.md) abundances hold under positivity of the [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md), not as an unconditional rule for every [food chain](../../../../../../food-chain.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
