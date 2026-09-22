<h1 id="13a/solution">Solution</h1>

↑ **Parent:** [13A](../13a.md)

The [residue theorem](../../../../../residue-theorem.md) states that a [meromorphic function](../../../../../meromorphic-function.md) with finitely many poles inside a positively oriented simple closed contour and none on it satisfies $\oint_C F(z)\,dz=2\pi i\sum\operatorname{Res}(F;a)$. The function must be holomorphic on a neighbourhood of the contour and its interior away from those poles.

Write $J=\int_0^\infty x^{1/2}\log x/(1+x^2)\,dx$ and $I=\int_0^\infty x^{1/2}/(1+x^2)\,dx$. Both integrals converge absolutely. Use the [principal complex logarithm](../../../../../principal-complex-logarithm.md) in the upper half-plane, with $z^{1/2}=e^{\log z/2}$, and an upper semicircle of radius $R>1$ indented above zero by a clockwise semicircle of radius $\epsilon<1$. The branch values on the negative real side are upper limits; equivalently use contours arbitrarily slightly above that side before taking a limit.

For $F(z)=z^{1/2}\log z/(1+z^2)$, the large arc is $O(R^{-1/2}\log R)$ and the small arc is $O(\epsilon^{3/2}|\log\epsilon|)$, so both vanish. On $z=-x$ approached from above, $z^{1/2}=i\sqrt x$ and $\log z=\log x+i\pi$. The oriented negative segment therefore contributes $iJ-\pi I$, and the positive segment contributes $J$. The only enclosed pole is $i$, with [residue](../../../../../residue.md)

$$
\operatorname{Res}(F;i)=\frac{e^{i\pi/4}(i\pi/2)}{2i}=\frac\pi4e^{i\pi/4}.
$$

Consequently

$$
(1+i)J-\pi I=2\pi i\operatorname{Res}(F;i)
=\frac{\pi^2}{2\sqrt2}(-1+i).
$$

Comparing imaginary and real parts yields the [upper-half-plane contour for square-root logarithmic integrals](../../../../../upper-half-plane-contour-for-square-root-logarithmic-integrals.md) evaluation:

$$
\boxed{\int_0^\infty\frac{x^{1/2}\log x}{1+x^2}\,dx=\frac{\pi^2}{2\sqrt2},\qquad
\int_0^\infty\frac{x^{1/2}}{1+x^2}\,dx=\frac\pi{\sqrt2}.}
$$

## ↑ Ancestors (10)

1. [13A](../13a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
