<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The outward [mass loss rate](../../../../../../mass-loss-rate.md) is $\dot M=4\pi r^2\rho u>0$. Put $\beta=4/(\gamma+1)$, $\alpha=4(\gamma-1)/(\gamma+1)$ and $y=\rho r^\beta$. Both terms in the [Bernoulli equation](../../../../../../bernoulli-equation.md) then have the same radial scaling: $\beta(\gamma-1)=4-2\beta=\alpha$. Eliminate $u$ and multiply by $r^\alpha$ to obtain

$$
F(r)=Cr^\alpha+GMr^{\alpha-1}=\frac{\gamma K}{\gamma-1}y^{\gamma-1}+\frac{\dot M^2}{32\pi^2y^2}=G(y).
$$

For positive terminal speed, $C>0$. Differentiation gives $F'=r^{\alpha-2}[\alpha Cr-(1-\alpha)GM]$. It has an interior minimum precisely when $0<\alpha<1$, or $1<\gamma<5/3$, at

$$
\boxed{r_c=\frac{GM}{C}\frac{5-3\gamma}{4(\gamma-1)}.}
$$

At a [sonic point](../../../../../../sonic-point.md), the [Bernoulli equation](../../../../../../bernoulli-equation.md) and $GM/r_c=2c_{s,c}^2$ give $C=c_{s,c}^2(5-3\gamma)/[2(\gamma-1)]$, recovering this radius. The limiting $C=0$, $\gamma=5/3$ case has no isolated interior minimum selected by these formulas.

The function $G$ diverges at both ends of $y>0$ and has a unique minimum where

$$
G'(y_c)=0\quad\Longleftrightarrow\quad \gamma Ky_c^{\gamma+1}=\frac{\dot M^2}{16\pi^2}.
$$

This condition is $u_c^2=c_{s,c}^2$. Thus a smooth crossing requires [minimum matching at a polytropic sonic point](../../../../../../minimum-matching-at-a-polytropic-sonic-point.md): $F(r_c)=G(y_c)$. If the minimum of $F$ is lower, an interval has no real positive solution; if it is higher, the two $y$ branches stay separate and cannot cross the sonic value. When the minima agree, their positive second derivatives give $G''(y_c)(y-y_c)^2\sim F''(r_c)(r-r_c)^2$, allowing a finite-slope branch to pass between them. The wind with finite positive terminal speed takes the lower-$y$ branch outside $r_c$, because $\rho\sim\dot M/(4\pi\sqrt{2C}\,r^2)$ and $\beta<2$ make $y\to0$.

At the matching point,

$$
c_{s,c}^2=\frac{2C(\gamma-1)}{5-3\gamma},\qquad \rho_c=\left(\frac{c_{s,c}^2}{\gamma K}\right)^{1/(\gamma-1)}.
$$

Insert these into $\dot M=4\pi r_c^2\rho_c c_{s,c}$:

$$
\boxed{\dot M=4\pi r_c^2(\gamma K)^{-1/(\gamma-1)}\left[\frac{2C(\gamma-1)}{5-3\gamma}\right]^{(\gamma+1)/[2(\gamma-1)]}.}
$$

The positive-$C$, $1<\gamma<5/3$ range is part of this finite-radius transonic wind result, rather than an unrestricted formula for every $\gamma>1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
