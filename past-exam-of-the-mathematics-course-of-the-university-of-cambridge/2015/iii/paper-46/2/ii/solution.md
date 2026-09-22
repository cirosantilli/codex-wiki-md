<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply a [Feynman parameter](../../../../../../feynman-parameter.md) and shift the loop momentum to $\ell=p+xk$. The common denominator becomes $[\ell^2+M_x^2]^2$, where

$$
M_x^2=m^2+x(1-x)k^2.
$$

For positive $M_x^2$, the Gamma-integral representation $a^{-2}=\int_0^\infty ds\,s e^{-sa}$ and a [Gaussian integral](../../../../../../gaussian-integral.md) give

$$
\int\frac{d^d\ell}{(2\pi)^d}\frac1{(\ell^2+M_x^2)^2}
=\frac1{(4\pi)^{d/2}}\int_0^\infty ds\,s^{1-d/2}e^{-sM_x^2}
=\frac{\Gamma(2-d/2)}{(4\pi)^{d/2}}(M_x^2)^{d/2-2}.
$$

This formula initially converges for $\operatorname{Re}d<4$ and defines the [Euclidean massive loop integral](../../../../../../euclidean-massive-loop-integral.md) at other dimensions by [analytic continuation](../../../../../../analytic-continuation.md). Consequently,

$$
I(k)=\frac{g^2\mu^{6-d}}{2(4\pi)^{d/2}}\Gamma(2-d/2)\int_0^1dx\,[m^2+x(1-x)k^2]^{d/2-2}.
$$

With $d=6-\epsilon$, the [Gamma function](../../../../../../gamma-function.md) factor is $\Gamma(-1+\epsilon/2)=-2/\epsilon+O(1)$. Only its pole matters: the other factors can be evaluated at $\epsilon=0$ when extracting that pole. Since $\int_0^1x(1-x)dx=1/6$,

$$
\boxed{I_{\mathrm{div}}(k)=-\frac{g^2}{(4\pi)^3\epsilon}\left(m^2+\frac{k^2}{6}\right).}
$$

This is the [one-loop two-point divergence in six-dimensional cubic scalar theory](../../../../../../one-loop-two-point-divergence-in-six-dimensional-cubic-scalar-theory.md). Its polynomial momentum dependence is precisely what permits subtraction by local [counterterms](../../../../../../counterterm.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
