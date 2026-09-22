<h1 id="16b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take a normalized state for which the indicated variances and operator pairings exist. Set $A=\hat L_3-\langle\hat L_3\rangle$ and $B=\hat x_1-\langle\hat x_1\rangle$. For real $\lambda$, positivity of the squared [norm](../../../../../../norm.md) gives

$$
0\le\|(A+i\lambda B)\psi\|^2=(\Delta_\psi L_3)^2+\lambda^2(\Delta_\psi x_1)^2+i\lambda\langle[\hat L_3,\hat x_1]\rangle.
$$

The [canonical commutation relations](../../../../../../canonical-commutation-relation.md) yield $[\hat L_3,\hat x_1]=i\hbar\hat x_2$. Thus the quadratic polynomial in $\lambda$ is nonnegative everywhere only if its discriminant is nonpositive. This gives the [Robertson uncertainty principle](../../../../../../robertson-uncertainty-principle.md)

$$
\boxed{\Delta_\psi\hat L_3\,\Delta_\psi\hat x_1\ge\frac\hbar2|\langle\hat x_2\rangle_\psi|,\qquad M=\frac\hbar2|\langle\hat x_2\rangle_\psi|.}
$$

If either variance is zero, the same polynomial argument forces the commutator expectation to vanish, so that edge case is included. Centering the operators is essential to obtain variances rather than uncentered second moments.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16B](../../16b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
