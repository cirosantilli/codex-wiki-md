<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $A,b$ be the coefficients of the $\nu$-stage [Runge-Kutta method](../../../../../runge-kutta-method.md). On the [Dahlquist test equation](../../../../../dahlquist-test-equation.md) $y'=\lambda y$, its [stability function](../../../../../stability-function.md) is

$$
R(z)=1+zb^T(I-zA)^{-1}\mathbf1
=\frac{\det(I-zA+z\mathbf1b^T)}{\det(I-zA)},\qquad z=h\lambda.
$$

Both polynomials have degree at most $\nu$, with denominator normalized to one at zero. Order $2\nu$ implies $R(z)-e^z=O(z^{2\nu+1})$. A rational function with these degree bounds and this accuracy is uniquely the diagonal [Padé approximant](../../../../../pade-approximant.md) $[\nu/\nu]_{e^z}$. To see uniqueness directly, if $P/Q$ and $\widetilde P/\widetilde Q$ have the required accuracy, then $P\widetilde Q-\widetilde P Q$ is a polynomial of degree at most $2\nu$ vanishing to order at least $2\nu+1$ at zero, hence identically zero.

The diagonal exponential [Padé approximant](../../../../../pade-approximant.md) can be written

$$
R(z)=\frac{P_\nu(z)}{P_\nu(-z)},\qquad
P_\nu(z)=\sum_{k=0}^{\nu}\frac{(2\nu-k)!\,\nu!}{(2\nu)!\,k!\,(\nu-k)!}z^k.
$$

Use the permitted Padé property that the zeros of $P_\nu(-z)$ lie strictly in the right half-plane and numerator and denominator are coprime. Thus $R$ has no poles in the closed left half-plane. Its real coefficients give $P_\nu(-iy)=\overline{P_\nu(iy)}$, so $|R(iy)|=1$. Also $R(z)\to(-1)^\nu$ at infinity. Applying the [maximum modulus principle](../../../../../maximum-modulus-principle.md) on left half-disks and letting their radii increase proves $|R(z)|\le1$ for $\operatorname{Re}z\le0$. There are no hidden stage poles there either: the irreducible Padé denominator has degree $\nu$, exhausting the possible degree of $\det(I-zA)$, so the latter cannot contain an additional canceled factor. **Every such maximal-order Runge-Kutta method is A-stable.** This is [maximal-order Runge-Kutta methods are A-stable](../../../../../maximal-order-runge-kutta-methods-are-a-stable.md); it does not assert [L-stability](../../../../../l-stability.md), since the stability function does not tend to zero at infinity.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
