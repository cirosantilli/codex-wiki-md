<h1 id="40c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $s=\gamma^{-1/2}$. Then

$$
\alpha=s^2,
\qquad
\beta=(1-s)^2,
\qquad
\sqrt\beta=1-s.
$$

For an eigenvalue $\lambda$, the corresponding $2\times2$ block has characteristic polynomial

$$
z^2-(1+\beta-\alpha\lambda)z+\beta.
$$

For $\lambda=1$,

$$
1+\beta-\alpha=2(1-s)=2\sqrt\beta,
$$

so the polynomial is

$$
(z-\sqrt\beta)^2.
$$

For $\lambda=\gamma$, it is

$$
z^2-\beta z+\beta.
$$

Its discriminant is $\beta(\beta-4)<0$, so its conjugate roots have product $\beta$ and modulus $\sqrt\beta$. Both blocks therefore have the same [spectral radius](../../../../../../spectral-radius.md), and

$$
\boxed{\rho(M)=\sqrt\beta=1-\frac1{\sqrt\gamma}.}
$$

This is the [heavy-ball rate for a two-eigenvalue diagonal quadratic](../../../../../../heavy-ball-rate-for-a-two-eigenvalue-diagonal-quadratic.md).

By contrast, the steepest-descent factor is

$$
\frac{\gamma-1}{\gamma+1}
=1-\frac{2}{\gamma}+O(\gamma^{-2}).
$$

The heavy-ball factor is $1-\gamma^{-1/2}$, which is substantially smaller for $\gamma\gg1$: it gives an iteration scale of order $\sqrt\gamma$ rather than order $\gamma$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [40C](../../40c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
