<h1 id="1/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [general-order Cauchy-Kovalevskaya theorem](../../../../../../../general-order-cauchy-kovalevskaya-theorem.md) applies to analytic data on a [non-characteristic hypersurface](../../../../../../../non-characteristic-hypersurface.md). In local coordinates $(t,z)$, a [real analytic](../../../../../../../real-analytic-function.md) system of order $m$ in an unknown vector $U$ is in normal form when

$$
\partial_t^mU=F\bigl(t,z,\{\partial_t^j\partial_z^\alpha U:j<m,\ j+|\alpha|\le m\}\bigr),
$$

with $F$ [real analytic](../../../../../../../real-analytic-function.md) near the initial jet. Analytic data $\partial_t^jU(0,z)=h_j(z)$ for $0\le j<m$ determine a unique [real analytic](../../../../../../../real-analytic-function.md) solution near each initial point. More general systems, including different orders for the components, have the same conclusion after solving for the highest [normal derivatives](../../../../../../../normal-derivative.md): the corresponding coefficient matrix, or highest-derivative Jacobian for a nonlinear system, must be invertible. This is the system's [non-characteristic hypersurface](../../../../../../../non-characteristic-hypersurface.md) condition. The uniqueness asserted by the [Cauchy-Kovalevskaya theorem](../../../../../../../cauchy-kovalevskaya-theorem.md) is initially uniqueness in the [real analytic](../../../../../../../real-analytic-function.md) class.

A [real analytic](../../../../../../../real-analytic-function.md) coordinate change flattens a [real analytic](../../../../../../../real-analytic-function.md) initial [hypersurface](../../../../../../../hypersurface.md). Non-characteristicity permits solving for its highest [normal derivatives](../../../../../../../normal-derivative.md) by the [real analytic](../../../../../../../real-analytic-function.md) [implicit function theorem](../../../../../../../implicit-function-theorem.md). Introduce all [derivatives](../../../../../../../derivative.md) through order $m-1$ as additional unknowns. Their [normal derivatives](../../../../../../../normal-derivative.md) are either another jet variable, a tangential first [derivative](../../../../../../../derivative.md) of a jet variable, or the right-hand side of the original equation. This gives a first-order [real analytic](../../../../../../../real-analytic-function.md) system. The derivative-compatibility identities have zero initial data and are preserved by the system; equivalently, its [real analytic](../../../../../../../real-analytic-function.md) coefficient recurrence reproduces the [derivatives](../../../../../../../derivative.md) of $U$. This explains both reductions, rather than assuming arbitrary [real analytic](../../../../../../../real-analytic-function.md) [hypersurfaces](../../../../../../../hypersurface.md) are already flat.

For the first example, the [principal symbol](../../../../../../../principal-symbol-of-a-partial-differential-equation.md) of the [Laplace equation](../../../../../../../laplace-equation.md) at the conormal $dx_1$ is $1$, so the plane is a [non-characteristic hypersurface](../../../../../../../non-characteristic-hypersurface.md). The theorem therefore applies to [real analytic](../../../../../../../real-analytic-function.md) $u|_{x_1=0}$ and $\partial_1u|_{x_1=0}$:

$$
\boxed{\text{analytic local existence and analytic uniqueness hold for Laplace Cauchy data}.}
$$

This does not give [Hadamard well-posedness](../../../../../../../well-posed-problem.md) in smooth or [Sobolev space](../../../../../../../sobolev-space-split.md) [norms](../../../../../../../norm.md). For $n\ge2$, the harmonic functions

$$
u_N(x)=\frac{e^{-\sqrt N}}N\sinh(Nx_1)\cos(Nx_2)
$$

have zero value data and [normal derivative](../../../../../../../normal-derivative.md) data $e^{-\sqrt N}\cos(Nx_2)$ tending to zero with every fixed tangential [derivative](../../../../../../../derivative.md). At any fixed $x_1=\delta>0$, however, $u_N(\delta,0)$ diverges. Thus the elliptic [Cauchy problem for a partial differential equation](../../../../../../../cauchy-problem.md) is unstable despite [real analytic](../../../../../../../real-analytic-function.md) solvability. The exceptional case $n=1$ is the elementary affine ordinary differential equation and has no such tangential high-frequency instability.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
