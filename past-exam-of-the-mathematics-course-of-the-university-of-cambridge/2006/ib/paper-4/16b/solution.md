<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

For a variation $y+\varepsilon\eta$ with $\eta(a)=0$ but arbitrary $\eta(b)$, differentiation and integration by parts give

$$
\delta I=\int_a^b(F_y\eta+F_{y'}\eta')\,dx
=\left[F_{y'}\eta\right]_a^b+\int_a^b\left(F_y-\frac d{dx}F_{y'}\right)\eta\,dx.
$$

First choose variations supported inside the interval. The fundamental lemma of the [calculus of variations](../../../../../calculus-of-variations-split.md) gives the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md). Then allow arbitrary endpoint variation to obtain the [natural boundary conditions for a free endpoint](../../../../../natural-boundary-conditions-for-a-free-endpoint.md):

$$
\boxed{\frac d{dx}F_{y'}-F_y=0,\qquad F_{y'}(b)=0.}
$$

Because $F$ has no explicit dependence on $x$,

$$
\frac d{dx}(F-y'F_{y'})=y'F_y+y''F_{y'}-y''F_{y'}-y'\frac d{dx}F_{y'}=0.
$$

Thus the [Beltrami identity](../../../../../beltrami-identity.md) is **$F-y'F_{y'}=k$**, constant along an extremal.

For the [brachistochrone problem](../../../../../brachistochrone-problem.md), put $u=-y>0$, so [conservation of energy](../../../../../conservation-of-energy.md) gives the bead speed $v=\sqrt{2gu}$. Its travel time is

$$
T=\frac1{\sqrt{2g}}\int_0^{x_0}\sqrt{\frac{1+u'^2}{u}}\,dx.
$$

The [Beltrami identity](../../../../../beltrami-identity.md) now gives $u(1+u'^2)=2R$ for a positive constant $R$. A descending [cycloid](../../../../../cycloid.md) parametrizes this relation:

$$
x=R(\theta-\sin\theta),\qquad u=R(1-\cos\theta),\qquad u'=\cot(\theta/2).
$$

The free endpoint has $F_{u'}=0$, hence $u'(x_0)=0$. On the first descending arc this occurs at $\theta=\pi$. Therefore

$$
\boxed{R=\frac{x_0}{\pi},\qquad y(x_0)=-\frac{2x_0}{\pi},\qquad
x=\frac{x_0}{\pi}(\theta-\sin\theta),\quad y=-\frac{x_0}{\pi}(1-\cos\theta),\quad0\leq\theta\leq\pi.}
$$

Along this arc $ds=2R\sin(\theta/2)d\theta$ and $v=2\sqrt{gR}\sin(\theta/2)$, so

$$
\boxed{T_{\min}=\pi\sqrt{R/g}=\sqrt{\pi x_0/g}.}
$$

The initial vertical tangent causes no divergent travel time: the quotient $ds/v$ has the finite constant limit $\sqrt{R/g}\,d\theta$.

To verify global minimality, take any admissible wire graph of finite travel time below the release level, and let $H>0$ be its maximum depth. For $0<u\leq H$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\frac{\sqrt{1+u'^2}}{\sqrt u}\geq\frac1{\sqrt H}+|u'|\sqrt{\frac1u-\frac1H}.
$$

Indeed the two coefficients on the right, after multiplication by $\sqrt u$, form a unit vector. Since the path starts at depth zero and reaches depth $H$, the weighted total variation is at least the integral over all depths from $0$ to $H$. Consequently

$$
T\geq\frac1{\sqrt{2g}}\left[\frac{x_0}{\sqrt H}+\int_0^H\sqrt{\frac1u-\frac1H}\,du\right]
=\frac1{\sqrt{2g}}\left[\frac{x_0}{\sqrt H}+\frac\pi2\sqrt H\right]
\geq\sqrt{\frac{\pi x_0}{g}}.
$$

The last inequality is minimized at $H=2x_0/\pi$. Our [cycloid](../../../../../cycloid.md) attains equality throughout: its depth increases to $H$ and $u'=\sqrt{H/u-1}$. Thus it achieves the genuine minimum over the wire graphs, not merely a stationary time. Reflection handles a negative horizontal endpoint coordinate by replacing $x_0$ with $|x_0|$.

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
