<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [dominant balance for algebraic roots](../../../../../../dominant-balance-for-algebraic-roots.md) separates one small [root of a polynomial](../../../../../../root-of-a-polynomial.md) from three large ones. For the small [root of a polynomial](../../../../../../root-of-a-polynomial.md), write $z=\varepsilon+a\varepsilon^3+O(\varepsilon^5)$ in $z=\varepsilon(1+z^2)^2$. Comparing coefficients gives $a=2$, so

$$
\boxed{z_{\mathrm{small}}=\varepsilon+2\varepsilon^3+O(\varepsilon^5).}
$$

This is a real [analytic function](../../../../../../space-of-holomorphic-functions.md) of real $\varepsilon$ near zero, since the derivative with respect to $z$ of $z-\varepsilon(1+z^2)^2$ is one at $(0,0)$.

For the large [roots of a polynomial](../../../../../../root-of-a-polynomial.md), use the real cube root $s=\operatorname{sgn}(\varepsilon)|\varepsilon|^{1/3}$ and set $z=w/s$. The transformed equation is

$$
w=(w^2+s^2)^2.
$$

Its three nonzero leading [roots of a polynomial](../../../../../../root-of-a-polynomial.md) are $w=\omega$, with $\omega^3=1$. Writing $w=\omega+as^2+O(s^4)$ gives $a=4a+2\omega^2$, hence $a=-2\omega^2/3$. Therefore

$$
\boxed{z_\omega=\frac{\omega}{s}-\frac23\omega^2s+O(s^3),\qquad \omega=1,e^{2\pi i/3},e^{-2\pi i/3}.}
$$

The choice $\omega=1$ is the second real [root of a polynomial](../../../../../../root-of-a-polynomial.md); the other two form a [complex conjugate](../../../../../../complex-conjugate.md) pair for either sign of $\varepsilon$. The nonzero transformed [roots of a polynomial](../../../../../../root-of-a-polynomial.md) are simple, so their [Taylor series](../../../../../../taylor-series.md) in $s^2$ exist locally and exhaust the three large [roots of a polynomial](../../../../../../root-of-a-polynomial.md). Together with the small one these give all four [roots of a polynomial](../../../../../../root-of-a-polynomial.md) for sufficiently small nonzero $\varepsilon$. At $\varepsilon=0$ itself the rational equation has only the finite root zero; the other three escape to infinity. Multiplying by $(1+z^2)^2$ has not introduced roots at $z=\pm i$, since those points do not solve the multiplied equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
