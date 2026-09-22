<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the small-slope [Monge representation](../../../../../../monge-representation.md), $s=x+O(y_x^2)$, $\mathbf t=(1,y_x)+O(y_x^2)$, and the leading transverse velocity is $y_t$. With no imposed axial prestress, the induced [filament tension](../../../../../../filament-tension.md) is second order in transverse amplitude, so its transverse contribution is higher order. The transverse component of force balance reduces to the [small-slope elastohydrodynamic filament equation](../../../../../../small-slope-elastohydrodynamic-filament-equation.md)

$$
\boxed{c_\perp y_t=-By_{xxxx}.}
$$

An externally imposed zeroth-order tension would instead add $Ty_{xx}$.

For the transverse motion, the off-diagonal part of the [resistive-force theory](../../../../../../resistive-force-theory.md) tensor gives axial propulsive force density $(c_\perp-c_\parallel)y_xy_t$ to second order. Its integral is

$$
\boxed{F=(c_\perp-c_\parallel)\int_0^L y_xy_t\,dx.}
$$

Substitute the bending equation and integrate by parts:

$$
\int_0^L y_xy_{xxxx}\,dx=\left[y_xy_{xxx}\right]_0^L-\int_0^L y_{xx}y_{xxx}\,dx=\left[y_xy_{xxx}-\frac12y_{xx}^2\right]_0^L.
$$

The [boundary expression for transverse filament thrust](../../../../../../boundary-expression-for-transverse-filament-thrust.md) is therefore

$$
\boxed{F=B\left(1-\frac{c_\parallel}{c_\perp}\right)\left[\frac12y_{xx}^2-y_xy_{xxx}\right]_0^L.}
$$

Only endpoint slope, bending moment, and shear enter this expression. Exact [inextensibility](../../../../../../inextensible-filament.md) also generates second-order longitudinal material motion; if that motion is retained in instantaneous total axial drag, it adds $-c_\parallel\int v_x\,dx$. For a periodic deformation with fixed axial base position, that additional term has zero cycle average. Thus the displayed formula is the transverse propulsive contribution and also gives the cycle-averaged propulsive force.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 334](../../../paper-334-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
