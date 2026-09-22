<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\rho=t\wedge\tau_0\wedge\tau_1$ and apply the [Itô formula](../../../../../../ito-s-lemma.md) to $u(t-s,B_s)$ for $0\leq s\leq\rho$. The [heat equation](../../../../../../heat-equation.md) cancels the drift, so the stopped process is a bounded [martingale](../../../../../../martingale-split.md). The [optional sampling theorem for a supermartingale](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives $u(t,x)=\mathbb E_x[u(t-\rho,B_\rho)]$. On the three mutually exclusive terminal events, the initial and [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) identify this value as

$$
u(t,x)=\mathbb E_x\!\left[g(B_t)\mathbf1_{\{t<\tau_0\wedge\tau_1\}}+f_1(t-\tau_0)\mathbf1_{\{\tau_0<t\wedge\tau_1\}}+f_2(t-\tau_1)\mathbf1_{\{\tau_1<t\wedge\tau_0\}}\right].
$$

This is the [probabilistic representation of the heat equation with time-dependent Dirichlet data](../../../../../../probabilistic-representation-of-the-heat-equation-with-time-dependent-dirichlet-data.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
