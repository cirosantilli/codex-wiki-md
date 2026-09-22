<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

Fix a [Hankel contour](../../../../../hankel-contour.md) with a positive-radius circle around zero and a branch $-\pi<\arg t<\pi$, traversing the lower bank inwards and the upper bank outwards. Write its numerator as $I(z)=\int_Ht^{z-1}e^t\,dt$. For fixed circle radius, $I$ is an [entire function](../../../../../entire-function.md) of $z$: the finite contour pieces avoid zero, and the tails converge uniformly on compact $z$ sets by exponential decay, also after differentiation with respect to $z$.

At $z=-n$, the two straight-bank contributions cancel because $t^{-n-1}e^t$ is single-valued. The remaining circle is positively oriented, so the [residue theorem](../../../../../residue-theorem.md) and the [exponential series](../../../../../exponential-series.md) give

$$
I(-n)=2\pi i\operatorname{Res}_{t=0}(t^{-n-1}e^t)=\frac{2\pi i}{n!}.
$$

Since $\sin(\pi z)=(-1)^n\pi(z+n)+O((z+n)^3)$, the quotient has the [simple pole](../../../../../simple-pole.md)

$$
\boxed{\operatorname{Res}_{z=-n}\Gamma(z)=\frac{(-1)^n}{n!},\qquad n\geq0.}
$$

For [cancellation of positive-integer gamma singularities on a Hankel contour](../../../../../cancellation-of-positive-integer-gamma-singularities-on-a-hankel-contour.md), at a positive [integer](../../../../../integer.md) $n$, the integrand $t^{n-1}e^t$ is entire and its bank contributions again cancel; its circular integral is zero. Hence $I(n)=0$. The numerator is analytic near $n$, while the denominator has a simple zero with nonzero derivative. Factoring $I(z)=(z-n)J(z)$ therefore cancels that zero, proving **there is no [pole](../../../../../pole.md) at a positive [integer](../../../../../integer.md)** using only this representation. Cancellation of the numerator, not merely the zero of the sine, decides the issue. One can also shrink the contour for $\Re z>0$, obtaining $I(z)=2i\sin(\pi z)\int_0^\infty u^{z-1}e^{-u}\,du$ and hence the finite value $(n-1)!$.

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
