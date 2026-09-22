<h1 id="27c/solution">Solution</h1>

↑ **Parent:** [27C](../27c.md)

Take the logarithmic derivative of the proposed [asymptotic expansion](../../../../../asymptotic-expansion.md). Through order $z^{-1}$, $u'/u=\lambda+\mu/z+O(z^{-2})$ and $u''/u=\lambda^2+2\lambda\mu/z+O(z^{-2})$. Matching the constant and inverse-power terms gives

$$
\boxed{\lambda^2+f_0\lambda+g_0=0,\qquad\mu=-\frac{f_1\lambda+g_1}{2\lambda+f_0}.}
$$

The second formula assumes a simple root, $2\lambda+f_0\ne0$. At a repeated root the ansatz can fail: the next equation first requires $f_1\lambda+g_1=0$, and if that holds higher orders determine the remaining behaviour.

For the [Bessel differential equation](../../../../../bessel-differential-equation.md), $\lambda=\pm i$ and $\mu=-1/2$. Set $u=e^{\lambda z}z^{-1/2}v(z)$. Direct substitution leaves $v''+2\lambda v'+(1/4-\nu^2)z^{-2}v=0$. With $v=1+a/z+O(z^{-2})$, matching $z^{-2}$ gives $a=(1/4-\nu^2)/(2\lambda)$. Thus

$$
\boxed{a^{(1)}=\frac{i(4\nu^2-1)}8,\qquad a^{(2)}=-\frac{i(4\nu^2-1)}8.}
$$

Two constant multiples of the [Hankel functions](../../../../../hankel-function.md) normalize their leading coefficients to one and realize these solutions in their appropriate sectors.

For generic $\nu$, these are sectorial expansions, not unchanged expansions for a single branch over arbitrarily continued $\arg z$. The factors $z^{-1/2}$ require a branch, and crossing sector boundaries can introduce the other exponential by [Stokes phenomenon](../../../../../stokes-phenomenon.md) and analytic continuation. More precisely, the standard normalized first Hankel solution has its expansion for $-\pi+\delta\leq\arg z\leq2\pi-\delta$, and the second for $-2\pi+\delta\leq\arg z\leq\pi-\delta$, with any fixed positive $\delta$ inside these sectors. In particular both are valid in the common slit sector $-\pi<\arg z<\pi$, away from its boundaries. These sector statements are recorded in [NIST's Hankel asymptotics](https://dlmf.nist.gov/10.17). Exceptional half-integer orders have terminating elementary expressions, so a blanket assertion of nonzero Stokes mixing for every order would be too strong.

## ↑ Ancestors (10)

1. [27C](../27c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
