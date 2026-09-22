<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In [conformal gauge](../../../../../../conformal-gauge.md), $\gamma_{\mu\nu}=e^{2\omega}\operatorname{diag}(-1,1)$. The [Weyl invariance](../../../../../../weyl-transformation.md) of the [Polyakov action](../../../../../../polyakov-action.md) removes $\omega$, leaving

$$
I_{\mathrm{conf}}=\frac T2\int_{t_i}^{t_f}dt\int_0^\ell d\sigma\,
(\dot X^2-X'^2).
$$

Its complete variation is

$$
\delta I_{\mathrm{conf}}=
T\int dt\,d\sigma\,(X''-\ddot X)\cdot\delta X
+T\left[\int_0^\ell d\sigma\,\dot X\cdot\delta X\right]_{t_i}^{t_f}
-T\int dt\,[X'\cdot\delta X]_0^\ell.
$$

Fix the [string embedding map](../../../../../../string-embedding-map.md) on the initial and final time slices. The interior [Euler-Lagrange field equation](../../../../../../euler-lagrange-field-equation.md) is the [wave equation](../../../../../../wave-equation-split.md)

$$
\boxed{\ddot X^m-X^{m\prime\prime}=0.}
$$

At each spatial endpoint the remaining variation vanishes under either [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md), $\delta X^m=0$, or [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md), $X^{m\prime}=0$, independently for each target-space component. Thus **a fixed endpoint or a free endpoint makes the boundary contribution vanish**. Fixing a spatial point throughout time imposes [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) on its spatial coordinates, while the time coordinate may retain [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md).

The independent [metric tensor](../../../../../../metric-tensor.md) equation must also be retained after [gauge fixing](../../../../../../gauge-fixing.md). Its [Virasoro constraints](../../../../../../virasoro-constraint.md) are

$$
\dot X\cdot X'=0,\qquad \dot X^2+X'^2=0.
$$

Together with the [wave equation](../../../../../../wave-equation-split.md), these ensure equivalence to the [Nambu–Goto action](../../../../../../nambu-goto-action.md); varying only the already fixed metric would lose these [Virasoro constraints](../../../../../../virasoro-constraint.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
