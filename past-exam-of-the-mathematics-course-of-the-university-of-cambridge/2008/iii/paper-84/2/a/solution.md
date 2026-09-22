<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $k_1>k_2$ and let both original and injected fluids initially have [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\mu$. Assume sharp displacement fronts, constant [porosity](../../../../../../porosity.md) and negligible exchange between layers. The imposed pressure difference gives [Darcy velocities](../../../../../../darcy-velocity.md) $q_i^0=k_i\Delta P/(\mu L)$ and [interstitial velocities](../../../../../../pore-velocity.md) $u_i^0=q_i^0/\phi$. The two arrival times are therefore

$$
\boxed{t_a=\frac{\phi\mu L^2}{k_1\Delta P},
\qquad t_s=\frac{\phi\mu L^2}{k_2\Delta P}
=\frac{k_1}{k_2}t_a.}
$$

If $A_i$ is the flow cross-section of layer $i$, its volume discharge is $Q_i^0=A_iq_i^0$. Equal viscosities make the hydraulic resistance independent of front position, so the total fluid discharge $Q_1^0+Q_2^0$ stays constant. The injected-fluid component at the outflow well is

$$
Q_{\rm inj}(t)=Q_1^0\mathbf1_{t\ge t_a}
+Q_2^0\mathbf1_{t\ge t_s}.
$$

It jumps from zero to the high-permeability discharge at the first breakthrough, then to the total discharge at the second. Before a layer breaks through, its outflow is original reservoir fluid. Cross-sections are needed to state an absolute volume discharge or its partition; the arrival times do not require them.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
