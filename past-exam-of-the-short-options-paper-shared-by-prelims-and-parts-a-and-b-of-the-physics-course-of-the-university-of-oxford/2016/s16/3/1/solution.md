<h1 id="s16/3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take electrostatic perturbations proportional to $e^{i(kz-\omega t)}$, with [ions](../../../../../ion.md) immobile on the fast [electron](../../../../../electron.md) [time scale](../../../../../time-scale.md). Linearized Vlasov gives $f_1=-i(qE_1/m)(\partial f_0/\partial v_z)/(\omega-kv_z)$. Integrating over transverse velocities gives $F_0(v_z)=n_0\sqrt{m/(2\pi k_BT)}e^{-mv_z^2/(2k_BT)}$. Combine the perturbed [charge density](../../../../../charge-density.md) with [Poisson's equation](../../../../../poisson-s-equation.md):

$$
1+\frac{e^2}{\epsilon_0mk}\int\frac{F_0'(v_z)}{\omega-kv_z}dv_z=0.
$$

Since $F_0'=-mv_zF_0/(k_BT)$, this is precisely

$$
\boxed{1-\frac{2n_0e^2}{\sqrt\pi\epsilon_0mk}\left(\frac m{2k_BT}\right)^{3/2}\int\frac{v_ze^{-mv_z^2/(2k_BT)}}{\omega-kv_z}dv_z=0.}
$$

The [pole](../../../../../pole.md) selects particles moving at [phase speed](../../../../../phase-speed.md). A causal initial-value prescription specifies how the [contour](../../../../../complex-integration-contour.md) passes it and produces resonant [energy](../../../../../energy-split.md) exchange, including [Landau damping](../../../../../landau-damping.md) for a decreasing Maxwellian. A bare real [improper integral](../../../../../improper-integral.md) without that prescription is incomplete. The unclosed brace in the printed Maxwellian exponent is typographical; the normalized Gaussian above fixes its meaning.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [3](../../3.md)
3. [S16](../../../s16.md)
4. [2016](../../../../2016-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
