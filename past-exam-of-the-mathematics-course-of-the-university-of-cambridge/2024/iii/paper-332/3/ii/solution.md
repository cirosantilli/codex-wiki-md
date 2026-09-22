<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The unperturbed [temperature](../../../../../../temperature.md) is linear in each material. Continuity of the conductive [heat flux](../../../../../../heat-flux-density.md) at $x=h$ gives

$$
k_w\frac{T_m-T_h}{h}
=k_a\frac{T_h-T_a}{\delta}.
$$

On defining

$$
\epsilon=\frac{k_a}{k_w}\frac h\delta,
$$

this becomes $T_m-T_h=\epsilon(T_h-T_a)$. Therefore

$$
\boxed{
T_m-T_h=
\frac{\epsilon}{1+\epsilon}(T_m-T_a)}.
$$

Let $\rho_i$ be the ice [mass density](../../../../../../density.md) and $L_f$ its [latent heat](../../../../../../latent-heat.md) of fusion per unit mass. The ice is isothermal in this model, so the [Stefan condition](../../../../../../stefan-condition.md) equates latent-heat production to the [heat flux](../../../../../../heat-flux-density.md) conducted through the water:

$$
\rho_iL_fV
=k_w\frac{T_m-T_h}{h}.
$$

Consequently the unperturbed lateral solidification speed is

$$
\boxed{
V=\frac{k_w}{\rho_iL_fh}
\frac{\epsilon}{1+\epsilon}(T_m-T_a)
=\frac{k_a}{\rho_iL_f\delta}
\frac{T_m-T_a}{1+\epsilon}}.
$$

The material parameters are the [thermal conductivities](../../../../../../thermal-conductivity.md) $k_w,k_a$, ice density $\rho_i$, and specific latent heat $L_f$; the geometric thermal length is $\delta$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
