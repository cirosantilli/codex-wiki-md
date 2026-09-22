<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the $L^2(S^2)$ data [norm](../../../../../../../norm.md). The coefficients of the measurement error are $e_n^m=b_n^m-a_n^m$, so [Parseval's identity](../../../../../../../parseval-identity.md) gives

$$
\sum_{n,m}|e_n^m|^2\le\delta^2.
$$

An unregularized continuation of these measurements to $r=R$ replaces $a_n^m$ by $b_n^m$ in the outgoing [spherical harmonic](../../../../../../../spherical-harmonic.md) expansion. Whenever this continuation has a finite trace, its error is

$$
\|g^\delta-g\|^2=k^2\sum_{n,m}|h_n^{(1)}(kR)|^2|e_n^m|^2.
$$

Choose a measurement error supported on a single normalized [spherical harmonic](../../../../../../../spherical-harmonic.md), with $e_N^0=\delta$ and all other coefficients zero. The data error has [norm](../../../../../../../norm.md) exactly $\delta$, but

$$
\boxed{\|g^\delta-g\|=\delta k|h_N^{(1)}(kR)|\longrightarrow\infty\quad(N\to\infty).}
$$

This [perturbation theory](../../../../../../../perturbation-theory.md) is a finite expansion, so it defines an actual outgoing solution of the [Helmholtz equation](../../../../../../../helmholtz-equation.md) outside any sphere of positive radius. It is not merely an example of nonconvergent formal coefficients. Taking instead $e_N^0=|d_N|^{-1}$ gives data errors tending to zero and trace errors of [norm](../../../../../../../norm.md) one, which directly proves discontinuity of inversion. General square-summable measurement noise can even violate the [spherical far-field range condition](../../../../../../../spherical-far-field-range-condition.md), leaving no $L^2$ continuation to the chosen sphere.

For obstacle reconstruction one would continue the field toward the unknown boundary and look for a surface on which $u_i+u_s=0$, the [Dirichlet boundary condition](../../../../../../../dirichlet-boundary-condition.md). The [unbounded spherical far-to-near-field continuation](../../../../../../../unbounded-spherical-far-to-near-field-continuation.md) shows why small far-field errors can cause arbitrarily large errors in the field used to estimate that surface. Locally, a differentiable normal displacement $\eta$ of a candidate boundary must obey the linearized condition $\Delta u_s+\eta\,\partial_n(u_i+u_s)=0$. Thus a large continued-field error, or a small [normal derivative](../../../../../../../normal-derivative.md), defeats an uncontrolled boundary estimate.

There is a necessary qualification to the wording about errors in the scatterer itself. The calculation proves an unbounded **field-continuation error**. An arbitrary perturbed outgoing field need not correspond to any Dirichlet obstacle, and no admissible class or metric on obstacle shapes is specified. It therefore does not by itself prove an arbitrarily large geometric error in every constrained reconstruction method. Such a claim requires a shape model and an analysis of the boundary-extraction step. The instability displayed here is exactly the mechanism that an unregularized reconstruction must control.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 80](../../../../paper-80-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
