<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\tau_\nu$ increase downward and let $\mu>0$ be the outward direction cosine. Assume a plane-parallel, static, nonscattering atmosphere in [local thermodynamic equilibrium](../../../../../../local-thermodynamic-equilibrium.md), so the source function is $B_\nu[T(P)]$. Hydrostatic balance gives

$$
d\tau_\nu=\frac{\kappa_\nu(P,T)}{g}\,dP.
$$

The [formal solution of the radiative transfer equation](../../../../../../formal-solution-of-the-radiative-transfer-equation.md) between $P_1>P_2$, corresponding to $\tau_1>\tau_2$, is

$$
\boxed{I_\nu(P_2,\mu)
=I_{\nu,1}e^{-(\tau_1-\tau_2)/\mu}
+\int_{\tau_2}^{\tau_1}
B_\nu[T(t)]e^{-(t-\tau_2)/\mu}\frac{dt}{\mu}}.
$$

For an isothermal atmosphere, $B_\nu(T)$ is constant and

$$
\boxed{I_\nu(P_2,\mu)
=I_{\nu,1}e^{-\Delta\tau_\nu/\mu}
+B_\nu(T)(1-e^{-\Delta\tau_\nu/\mu})}.
$$

If the lower boundary is itself thermalized, $I_{\nu,1}=B_\nu(T)$ and the upward intensity remains the blackbody value.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
