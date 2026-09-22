<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Write $\mathbf g=-g\mathbf e_z$. The vertical component of the balance gives [hydrostatic pressure](../../../../../hydrostatic-pressure.md),

$$
p(x,y,z)=p_0+\rho g[h(x,y)-z].
$$

Its horizontal [gradient](../../../../../gradient.md) is $\nabla_h p=\rho g\nabla_hh$. The horizontal balance is consequently

$$
f\mathbf e_z\mathbin\times\mathbf u=-g\nabla_hh,
\qquad
\mathbf u=\frac gf\mathbf e_z\mathbin\times\nabla_hh.
$$

Thus $\mathbf u\mathbin\cdot\nabla_hh=0$: the velocity is tangent to every [level set](../../../../../level-set.md) of $h$, so those contours are [streamlines](../../../../../streamline.md) of the [geostrophic flow](../../../../../geostrophic-flow.md).

Across a vertical section joining the contours $h_0$ and $h_0+\Delta h$, an element of horizontal distance normal to the contours is $dn=dh/|\nabla_hh|$, while $|\mathbf u|=(g/f)|\nabla_hh|$. The [volumetric flow rate](../../../../../volumetric-flow-rate.md) is therefore

$$
Q=\int_{h_0}^{h_0+\Delta h}h\frac gf|\nabla_hh|\frac{dh}{|\nabla_hh|}
=\frac g{2f}[(h_0+\Delta h)^2-h_0^2]
\sim\boxed{\frac{gh_0\Delta h}{f}}.
$$

For [dimensional analysis](../../../../../dimensional-analysis.md), $[g]=LT^{-2}$, $[f]=T^{-1}$ and $[h_0]=[\Delta h]=L$, so the result has dimension $L^3T^{-1}$, exactly that of a volume flux.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
