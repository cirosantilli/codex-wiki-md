<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use cylindrical coordinates and tracer density $\nu(R,z)$. A steady axisymmetric [Jeans equation](../../../../../../jeans-equation.md), with no mean radial or vertical flow, is

$$
\frac{\partial(\nu\overline{v_R^2})}{\partial R}+\frac{\partial(\nu\overline{v_Rv_z})}{\partial z}+\frac{\nu}{R}(\overline{v_R^2}-\overline{v_\phi^2})=-\nu\frac{\partial\Phi}{\partial R}.
$$

Write $\overline{v_R^2}=\sigma_R^2$, $\overline{v_\phi^2}=\bar v_\phi^2+\sigma_\phi^2$, and $V_c^2=R\partial_R\Phi$. Rearrangement gives the [stellar asymmetric drift](../../../../../../stellar-asymmetric-drift.md) equation

$$
V_c^2-\bar v_\phi^2=\sigma_\phi^2-\sigma_R^2-\frac{R}{\nu}\frac{\partial(\nu\sigma_R^2)}{\partial R}-\frac{R}{\nu}\frac{\partial(\nu\overline{v_Rv_z})}{\partial z}.
$$

For an isotropic [velocity ellipsoid](../../../../../../velocity-ellipsoid.md), all three dispersions equal $\sigma$ and the cross stress vanishes. Therefore the required general result is

$$
\boxed{\bar v_\phi=\sqrt{V_c^2-A\sigma^2},\qquad A=-\frac{d\ln(\nu\sigma^2)}{d\ln R}.}
$$

The positive root is for a prograde [galactic disk](../../../../../../galactic-disk.md). A declining radial stress gives $A>0$: random motions supply some support, so mean stellar rotation is slower than cold-gas circular rotation. For $A\sigma^2\ll V_c^2$, $V_c-\bar v_\phi\simeq A\sigma^2/(2V_c)$. The condition $\sigma<V_c$ alone is insufficient; one also needs $A\sigma^2\le V_c^2$.

There is no universal numerical coefficient expressible from $V_c$ and $\sigma$ alone. For constant [velocity dispersion](../../../../../../velocity-dispersion.md) and $\nu\propto R^{-p}$, $A=p$. Thus $p=2$ gives the often-used estimate $\bar v_\phi=\sqrt{V_c^2-2\sigma^2}$, while $p=1$ gives a different answer with the same $V_c$ and $\sigma$. For an [exponential galactic disk](../../../../../../exponential-galactic-disk.md) tracer with $\nu\propto e^{-R/R_d}$ and $\sigma^2\propto e^{-R/R_\sigma}$, the [exponential-disk asymmetric drift](../../../../../../exponential-disk-asymmetric-drift.md) has $A=R(R_d^{-1}+R_\sigma^{-1})$.

Real [galactic disks](../../../../../../galactic-disk.md) generally have anisotropic [velocity dispersions](../../../../../../velocity-dispersion.md), often $\sigma_R>\sigma_\phi>\sigma_z$. In the small-random-motion [epicyclic motion](../../../../../../epicyclic-motion.md) limit for a flat [galaxy rotation curve](../../../../../../galaxy-rotation-curve.md), $\sigma_\phi^2/\sigma_R^2\simeq1/2$, so even the non-gradient term matters. The [velocity ellipsoid](../../../../../../velocity-ellipsoid.md) can tilt, and bars or spiral structure can violate steady axisymmetry. Age-dependent [galactic disk heating](../../../../../../galactic-disk-heating.md) makes the lag population dependent. Gas has finite turbulent and thermal stresses too, though a cold gas disk often approximates $V_c$ much better than a hot [stellar population](../../../../../../stellar-population.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
