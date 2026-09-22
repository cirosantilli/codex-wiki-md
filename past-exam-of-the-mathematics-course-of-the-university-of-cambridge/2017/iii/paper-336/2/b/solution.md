<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First make explicit the usual [method of steepest descent](../../../../../../method-of-steepest-descent.md) hypotheses: the [saddle point](../../../../../../saddle-point.md) is simple, $G'(z_0)=0$ and $g_2=G''(z_0)\ne0$; a [contour deformation](../../../../../../contour-deformation.md) leads to the two descent arms with one clockwise half-indentation around the [pole](../../../../../../pole.md); and endpoints or other contour portions contribute smaller terms. The sign of the exponential matters: $|e^{-i\lambda G}|=e^{\lambda\operatorname{Im}G}$, so decay is toward valleys of $\operatorname{Im}G$.

Use a local [analytic function](../../../../../../space-of-holomorphic-functions.md) $w(z)$ as coordinate. Nondegeneracy allows an analytic square root after factoring the double zero of $G-G(z_0)$, so the coordinate can be chosen with

$$
G(z)-G(z_0)=-\frac i2w^2,\qquad z-z_0=cw+dw^2+O(w^3),\qquad c^2=-\frac i{g_2}.
$$

The sign of $c$ is selected by the orientation of the [contour integral](../../../../../../contour-integral.md), with $w$ running from negative to positive real values. Matching cubic coefficients gives $d/c=-cG'''(z_0)/(6g_2)$. The transformed amplitude therefore has the [Laurent series](../../../../../../laurent-series.md)

$$
\frac{F(z)}{z-z_0}\frac{dz}{dw}=\frac{F(z_0)}w+B+O(w),\qquad
B=c\left[F'(z_0)-\frac{F(z_0)G'''(z_0)}{6G''(z_0)}\right].
$$

The [Cauchy principal value](../../../../../../cauchy-principal-value.md) contribution of the [pole](../../../../../../pole.md) on the two real arms is zero by oddness. Its clockwise semicircular indentation contributes $-i\pi F(z_0)$, since $\int dw/w=-i\pi$ there. The regular term contributes the [Gaussian integral](../../../../../../gaussian-integral.md) $B\sqrt{2\pi/\lambda}$. Consequently the [simple saddle coinciding with a simple pole](../../../../../../simple-saddle-coinciding-with-a-simple-pole.md) has the additive expansion

$$
\boxed{J(\lambda)=e^{-i\lambda G(z_0)}\left[-i\pi F(z_0)+B\sqrt{\frac{2\pi}{\lambda}}+O(\lambda^{-3/2})\right].}
$$

The remainder written here assumes the other contour contributions are negligible to that order. Otherwise the local result has to be supplemented by them. The next local correction is generically $O(\lambda^{-1/2})$ times the displayed exponential. If $B=0$, it can vanish; odd Taylor terms integrate to zero between the symmetric arms. When $F(z_0)\ne0$, the leading term gives the printed asymptotic equivalence. When $F(z_0)=0$, asymptotic equivalence to zero is not meaningful: the additive formula is still valid and a regular [saddle-point approximation](../../../../../../saddle-point-approximation.md) may lead instead.

Nondegeneracy is necessary and is not explicitly printed. For a counterexample to the unrestricted reading, take $F=1$, $z_0=0$ and $G(z)=-iz^4$. There is one critical point, but it is degenerate. Choose the contour from $+i\infty$ to $+\infty$, with a clockwise quarter-circle avoiding zero. Both rays are decaying valleys for $e^{-\lambda z^4}$. Their straight-ray contributions cancel, and the indentation gives $J=-i\pi/2$, not $-i\pi$. Thus the requested coefficient requires the simple [saddle point](../../../../../../saddle-point.md) and [contour deformation](../../../../../../contour-deformation.md) assumptions above; the mere existence of one critical point is insufficient.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
