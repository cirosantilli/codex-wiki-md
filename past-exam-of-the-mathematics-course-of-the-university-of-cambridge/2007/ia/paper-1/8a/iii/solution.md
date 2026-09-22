<h1 id="8a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For real $x$ at which the denominator is nonzero, mapping to the [unit circle](../../../../../../complex-unit-circle.md) gives $|ax+b|^2=|cx+d|^2$. There are infinitely many such real $x$, so the resulting quadratic [polynomial](../../../../../../polynomial-split.md) identity has all coefficients zero:

$$
|a|^2=|c|^2,\qquad
\operatorname{Re}(a\overline b)=\operatorname{Re}(c\overline d),\qquad
|b|^2=|d|^2.
$$

If $c=0$, the first equality gives $a=0$, contradicting the nonzero [determinant](../../../../../../determinant.md) $ad-bc$. Thus $a,c\ne0$. Put $\lambda=a/c$, $k=b/a$ and $\ell=d/c$. The equalities become

$$
|\lambda|=1,\qquad\operatorname{Re}k=\operatorname{Re}\ell,\qquad |k|=|\ell|.
$$

Two [complex numbers](../../../../../../complex-number.md) with equal real parts and equal moduli have imaginary parts equal in magnitude. Consequently $\ell=k$ or $\ell=\overline k$. The first option would give $ad-bc=ac(\ell-k)=0$, so it is excluded. The second gives

$$
\boxed{w=\lambda\frac{z+k}{z+\overline k},\qquad |\lambda|=1.}
$$

Moreover $k$ must be nonreal, since otherwise the two options coincide and the map would be constant. This proves the [Möbius transformations from the real axis to the unit circle](../../../../../../mobius-transformations-from-the-real-axis-to-the-unit-circle.md) representation directly from coefficients.

Conversely, for real $x$, the numbers $x+k$ and $x+\overline k$ are [complex conjugates](../../../../../../complex-conjugate.md), and their moduli agree. Nonreal $k$ ensures the denominator is nonzero on the [real line](../../../../../../real-line.md); multiplication by $\lambda$ preserves modulus. At the point at infinity on the [Riemann sphere](../../../../../../riemann-sphere.md), the map takes the value $\lambda$. Thus the representation also respects the extended real axis.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [8A](../../8a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
