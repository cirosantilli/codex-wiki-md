<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Wirtinger derivative](../../../../../wirtinger-derivatives.md) $u_z=(u_x-iu_y)/2$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md), since $\partial_{\bar z}u_z=\Delta u/4=0$ by the [Laplace equation](../../../../../laplace-equation.md). The [conformal map](../../../../../conformal-map.md) $w=z^2$ takes the quadrant to the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Integrating the prescribed [tangential boundary derivatives](../../../../../tangential-boundary-derivative.md), choose a common corner value $c$ and define the real boundary function

$$
f(s)=\begin{cases}
c+\displaystyle\int_0^{\sqrt s}g_2(r)\,dr,&s>0,\\
c+\displaystyle\int_0^{\sqrt{-s}}g_1(r)\,dr,&s<0.
\end{cases}
$$

The decaying data are bounded under the usual regularity at the corner, so $f(s)=O(1+\sqrt{|s|})$. Thus its [Poisson integral](../../../../../poisson-integral.md) converges. A [holomorphic](../../../../../complex-differentiability-at-a-point.md) function whose [real part](../../../../../real-part.md) is that [Poisson integral](../../../../../poisson-integral.md) is supplied by the regularized [Schwarz integral formula](../../../../../schwarz-integral-formula.md):

$$
W(w)=\frac1{\pi i}\int_{-\infty}^{\infty}f(s)\left(\frac1{s-w}-\frac{s}{1+s^2}\right)ds.
$$

For $u_*(z)=\operatorname{Re}W(z^2)$, the [chain rule](../../../../../chain-rule.md) gives $(u_*)_z=zW'(z^2)$. Apply [integration by parts](../../../../../integration-by-parts.md) to obtain

$$
W'(w)=\frac1{\pi i}\int_{\mathbb R}\frac{f'(s)}{s-w}\,ds,
\qquad
f'(s)=\begin{cases}
g_2(\sqrt s)/(2\sqrt s),&s>0,\\
-g_1(\sqrt{-s})/(2\sqrt{-s}),&s<0.
\end{cases}
$$

Substituting $s=r^2$ and $s=-r^2$ gives the requested particular [integral representation](../../../../../integral-representation.md):

$$
\boxed{(u_*)_z(z)=\frac{z}{\pi i}\left[\int_0^\infty\frac{g_2(r)}{r^2-z^2}\,dr+\int_0^\infty\frac{g_1(r)}{r^2+z^2}\,dr\right].}
$$

Both integrals converge absolutely for an interior point of the quadrant. The [Sokhotski–Plemelj formula](../../../../../sokhotski-plemelj-theorem.md) gives $\operatorname{Re}(u_*)_z(x)=g_2(x)/2$ on the horizontal edge and $\operatorname{Im}(u_*)_z(iy)=-g_1(y)/2$ on the vertical edge, verifying the prescribed derivatives.

The printed conditions alone do not determine $u_z$ uniquely. The general answer adds a [holomorphic](../../../../../complex-differentiability-at-a-point.md) function $H$ satisfying

$$
\operatorname{Re}H(x)=0,\qquad \operatorname{Im}H(iy)=0,
\qquad x,y>0.
$$

Equivalently, write $H(z)=ih(z^2)/z$, where $h$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) in the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) with real boundary values on the nonzero real axis. An [antiderivative](../../../../../antiderivative.md) of $2H$ has a [harmonic](../../../../../harmonic-function.md) [real part](../../../../../real-part.md) with zero [tangential boundary derivatives](../../../../../tangential-boundary-derivative.md). For example, $u=xy$ contributes $H=-iz/2$ without changing either datum. If the two edge constants differ by $c_2-c_1$, the angular [harmonic function](../../../../../harmonic-function.md) contributes $i(c_2-c_1)/(\pi z)$. The boxed expression selects the [Poisson integral](../../../../../poisson-integral.md) representative with equal edge constants; regularity and suitable growth conditions can be used to select that representative.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 328](../../paper-328-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
