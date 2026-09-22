<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $h=f^{-1}$, $w_0=f(z_0)$ and $z=h(w)$. [Continuity](../../../../continuous-function.md) of $h$ gives $z\to z_0$ as $w\to w_0$, and injectivity gives $z\ne z_0$ when $w\ne w_0$. Therefore

$$
\frac{h(w)-h(w_0)}{w-w_0}=\left(\frac{f(z)-f(z_0)}{z-z_0}\right)^{-1}\longrightarrow\frac1{f'(z_0)}.
$$

The assumed nonvanishing [derivative](../../../../derivative.md) makes this limit well defined. It exists at every $w_0\in V$, so $h$ is [holomorphic](../../../../holomorphic-function-split.md), with $\boxed{h'(w)=1/f'(h(w))}$.

Squaring maps the first [quadrant](../../../../quadrant-plane-geometry.md) bijectively onto the [upper half-plane](../../../../upper-half-plane-complex-analysis.md). For $\zeta$ in that half-plane, $|\zeta-i|<|\zeta+i|$, and the [Cayley transform](../../../../cayley-transform-complex-analysis.md) $(\zeta-i)/(\zeta+i)$ maps it bijectively onto the [unit disc](../../../../unit-disc.md). Their composition is

$$
\boxed{F(z)=\frac{z^2-i}{z^2+i}.}
$$

The inverse is the unique first-[quadrant](../../../../quadrant-plane-geometry.md) [square root](../../../../square-root.md) of $i(1+w)/(1-w)$, and is [holomorphic](../../../../holomorphic-function-split.md) by the first argument. Hence $H(w)=g(F^{-1}(w))$ is [holomorphic](../../../../holomorphic-function-split.md) throughout the disc. Its [Taylor series](../../../../taylor-series.md) at zero converges for $|w|<1$, locally uniformly there. Substituting $w=F(z)$ gives the stated expansion, with $c_n=H^{(n)}(0)/n!$, convergent at every point of the [quadrant](../../../../quadrant-plane-geometry.md) and locally uniformly on it.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
