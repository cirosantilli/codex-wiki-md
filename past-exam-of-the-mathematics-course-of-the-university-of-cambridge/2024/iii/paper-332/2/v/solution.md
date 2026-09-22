<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Define the dimensionless stagnant-layer depth and time by

$$
\eta=\frac hH,
\qquad
\tau=\frac{\kappa t}{H^2},
$$

so $H^2/\kappa$ is the [thermal diffusion time](../../../../../../thermal-diffusion-time.md). The maximizing interface temperature gives

$$
T_h-T_s=\Delta T\left(1-\frac35\theta\right).
$$

Equating conductive and convective [heat fluxes](../../../../../../heat-flux-density.md) therefore gives the algebraic relation

$$
\boxed{
\frac{1-3\theta/5}{\eta}
=\mathcal F\theta^{5/3}}.
$$

Since $k=\rho c_p\kappa$, where $c_p$ is the [specific heat capacity](../../../../../../specific-heat-capacity.md), the bulk heat balance in the convecting depth $H-h$ becomes

$$
\boxed{
(1-\eta)\frac{d\theta}{d\tau}
=-\mathcal F\theta^{5/3}}.
$$

Retaining the heat capacity of the thin stagnant layer changes this only by relative order $\eta$.

For $\mathcal F\gg1$ and $\theta=O(1)$, the flux relation gives $\eta=O(\mathcal F^{-1})$. The leading equation is consequently

$$
\frac{d\theta}{d\tau}
=-\mathcal F\theta^{5/3}.
$$

Separating variables and using $\theta(0)=1$ gives

$$
\theta^{-2/3}=1+\frac23\mathcal F\tau,
$$

hence

$$
\boxed{
\theta(\tau)=
\left(1+\frac23\mathcal F\tau\right)^{-3/2}}.
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
