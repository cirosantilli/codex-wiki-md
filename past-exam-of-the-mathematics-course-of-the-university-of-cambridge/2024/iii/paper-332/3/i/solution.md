<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $d(z,t)$ be the local water-film thickness. To first order in the interface amplitudes,

$$
d=h+(\eta_2-\eta_1)e^{i\alpha z+\sigma t}.
$$

The [lubrication theory](../../../../../../lubrication-theory.md) flux down the vertical surface, with a [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) at the ice and a [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md) at the water-air interface, is

$$
q=\frac{d^3}{3\nu}
\left(g-\frac1\rho p_z\right).
$$

For the unperturbed film $p_z=0$, so

$$
q=\frac{gh^3}{3\nu},
\qquad
\boxed{h=\left(\frac{3\nu q}{g}\right)^{1/3}}.
$$

The linearized [Young–Laplace equation](../../../../../../young-laplace-equation.md) gives the capillary-pressure perturbation

$$
p'=\gamma\alpha^2\eta_2e^{i\alpha z+\sigma t},
\qquad
p'_z=i\gamma\alpha^3\eta_2e^{i\alpha z+\sigma t}.
$$

Because the prescribed [volume flux](../../../../../../volumetric-flow-rate.md) is uniform, its first-order perturbation must vanish. [Linearization](../../../../../../linearization.md) of the flux law gives

$$
0=\frac{gh^2}{\nu}(\eta_2-\eta_1)
-\frac{ih^3\gamma\alpha^3}{3\rho\nu}\eta_2.
$$

Thus, with $\Gamma=\gamma/(3\rho g)$,

$$
\eta_2(1-i\Gamma\alpha^3h)=\eta_1,
$$

and hence

$$
\boxed{
\eta_2=\frac{\eta_1}
{1-i\Gamma\alpha^3h}}.
$$

The complex amplitude ratio records the phase shift caused by [surface tension](../../../../../../surface-tension.md) in the [long-wave approximation](../../../../../../long-wave-approximation.md).

## ↑ Ancestors (11)

1. [I](../i.md)
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
