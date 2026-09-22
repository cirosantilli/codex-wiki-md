<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Y(t)$ be the [porous thermal front](../../../../../../thermal-front-in-a-porous-medium.md) and $X(t)$ the polymer front. With the literal stated convention for [Darcy velocity](../../../../../../darcy-velocity.md),

$$
Y'=\Gamma U,\qquad X'=U/\phi,\qquad Y(0)=X(0)=0.
$$

Therefore $Y=\beta X$ with $\beta=\Gamma\phi$. This is [thermal-front retardation in Darcy flow](../../../../../../thermal-front-retardation-in-darcy-flow.md). The region $0<x<Y$ is cold injected fluid of [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\mu$; $Y<x<X$ is heated injected fluid of [dynamic viscosity](../../../../../../dynamic-viscosity.md) $b\mu$; $X<x<L$ is oil of [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\mu_h$. The [pressure](../../../../../../pressure.md) drop is consequently

$$
\Delta P=\frac{U}{k}\left[\mu Y+b\mu(X-Y)+\mu_h(L-X)\right]=\frac{U}{k}\left[\mu_hL+(\mu_{\rm eff}-\mu_h)X\right],
$$

where $\mu_{\rm eff}=\mu[\beta+b(1-\beta)]$. Apply the preceding [fixed-pressure planar Darcy displacement](../../../../../../fixed-pressure-planar-darcy-displacement.md) calculation with $\mu$ replaced by this effective [dynamic viscosity](../../../../../../dynamic-viscosity.md). The **polymer-front speed** is

$$
\boxed{\dot X=\frac{k\Delta P}{\phi\sqrt{(\mu_hL)^2+2(\mu_{\rm eff}-\mu_h)k\Delta P\,t/\phi}},\qquad\mu_{\rm eff}=\mu[b-(b-1)\Gamma\phi].}
$$

Its position solves $\mu_hLX+(\mu_{\rm eff}-\mu_h)X^2/2=k\Delta P\,t/\phi$, and $Y=\Gamma\phi X$. These expressions hold while both interfaces remain in the field, the [porous thermal front](../../../../../../thermal-front-in-a-porous-medium.md) is sharp and stable, and $0\leq\Gamma\phi\leq1$. For $b=1$ the original constant-viscosity answer is recovered.

Sometimes a thermal retardation factor is defined relative to the [pore velocity](../../../../../../pore-velocity.md) instead. Under that alternative definition one substitutes $\beta=\Gamma$ throughout. The factor of $\phi$ in the boxed answer follows specifically from the PDF's phrase “fraction of the Darcy speed.”

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
