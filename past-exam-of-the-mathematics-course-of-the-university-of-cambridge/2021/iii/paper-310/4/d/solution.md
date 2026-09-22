<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The supplied superhorizon evolution equation is

$$
\frac{d\mathcal R}{d\ln a}
=-\frac{\delta P_{\rm nad}}{\bar\rho+\bar P},
\qquad
\delta P_{\rm nad}=\delta P-
\frac{\bar P'}{\bar\rho'}\delta\rho.
$$

For an [adiabatic cosmological perturbation](../../../../../../adiabatic-initial-conditions.md), $\delta P=(\bar P'/\bar\rho')\delta\rho$, so $\delta P_{\rm nad}=0$ and the [comoving curvature perturbation](../../../../../../comoving-curvature-perturbation.md) $\mathcal R$ is conserved on [superhorizon scales](../../../../../../superhorizon-scale.md).

For photons and [cold dark matter](../../../../../../cold-dark-matter.md), put $A=\bar\rho_\gamma$, $C=\bar\rho_c$, and use $\bar P=A/3$, $A'=-4\mathcal H A$, and $C'=-3\mathcal H C$. Then

$$
\frac{\bar P'}{\bar\rho'}=\frac{4A}{3(4A+3C)}.
$$

The [cosmological entropy perturbation](../../../../../../cosmological-entropy-perturbation.md) $S=\delta_c-3\delta_\gamma/4$ implies $\delta_c=S+3\delta_\gamma/4$, so the adiabatic part cancels and

$$
\delta P_{\rm nad}
=-\frac{4AC}{3(4A+3C)}S.
$$

Since $\bar\rho+\bar P=C+4A/3$, the curvature evolves as

$$
\boxed{\frac{d\mathcal R}{d\ln a}
=\frac{4\bar\rho_\gamma\bar\rho_c}
{(4\bar\rho_\gamma+3\bar\rho_c)^2}S}.
$$

In the sign convention requested in the question, $d\mathcal R/d\ln a=-fS$, this means

$$
\boxed{f(\bar\rho_\gamma,\bar\rho_c)
=-\frac{4\bar\rho_\gamma\bar\rho_c}
{(4\bar\rho_\gamma+3\bar\rho_c)^2}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
