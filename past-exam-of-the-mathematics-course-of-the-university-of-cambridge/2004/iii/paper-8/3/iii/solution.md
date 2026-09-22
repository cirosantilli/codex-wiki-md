<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the canonical representatives of [functionals](../../../../../../functional.md) of $u$: $P_f=f\partial^{-1}$, $P_g=g\partial^{-1}$. The [formal pseudodifferential composition rule](../../../../../../formal-pseudodifferential-composition-rule.md) gives

$$
P_fP_g=fg\partial^{-2}-fg'\partial^{-3}+fg''\partial^{-4}+\cdots,
$$

and the reversed product has $f,g$ exchanged. Therefore

$$
[P_f,P_g]=(gf'-fg')\partial^{-3}+(fg''-gf'')\partial^{-4}+\cdots.
$$

Multiplying by $L=\partial^2+u$ on the left, only the leading displayed [commutator](../../../../../../commutator.md) term can produce a residue. Differentiation of its [coefficient](../../../../../../coefficient.md) produces powers at most $\partial^{-2}$, and multiplication by $u$ produces powers at most $\partial^{-3}$. Thus

$$
\operatorname{res}\bigl(L[P_f,P_g]\bigr)=gf'-fg',
$$

and, with the trace convention of part (i),

$$
\boxed{\{l_{P_f},l_{P_g}\}(L)=\int(gf'-fg')\,dx=-2\int fg'\,dx.}
$$

There is no $u$ dependence in this bracket.

Moreover $\operatorname{res}(P_fL)=fu$, so $l_{P_f}=\int fu\,dx$ and $\delta l_{P_f}/\delta u=f$. If $K(x,y)=\{u(x),u(y)\}$ is the distributional field bracket, it is characterized by

$$
\iint f(x)g(y)K(x,y)\,dx\,dy=-2\int f(x)g'(x)\,dx.
$$

Since $\int\partial_x\delta(x-y)g(y)\,dy=g'(x)$, the answer is

$$
\boxed{\{u(x),u(y)\}=-2\partial_x\delta(x-y)=2\partial_y\delta(x-y).}
$$

The [Dirac delta](../../../../../../dirac-delta-function.md) is periodic in the periodic setting, or the ordinary [Dirac delta](../../../../../../dirac-delta-function.md) on the real line with admissible test [functions](../../../../../../function-split.md). This is the [first Hamiltonian structure of the KdV equation](../../../../../../first-hamiltonian-structure-of-the-kdv-equation.md), with [Poisson operator](../../../../../../poisson-operator.md) $-2\partial_x$. Its skewness follows by [integration by parts](../../../../../../integration-by-parts.md); its [coefficients](../../../../../../coefficient.md) are constant, so the [functional](../../../../../../functional.md) [Jacobi identity](../../../../../../jacobi-identity.md) has no coefficient-variation terms.

A qualification is needed if the displayed trace formula is interpreted as a bracket on the reduced space for arbitrary operator representatives. Multiplication by a [function](../../../../../../function-split.md) $h$ gives $l_{m_h}(\partial^2+u)=0$, yet direct expansion gives

$$
\operatorname{res}\bigl(L[m_h,g\partial^{-1}]\bigr)
=2(gh')'-gh'',\qquad
\operatorname{Tr}\bigl(L[m_h,g\partial^{-1}]\bigr)=-\int gh''\,dx.
$$

With $h=g=\cos x$ on a period $[0,2\pi]$, the latter is $\pi$. Hence the formula does not descend through every possible representative of a [functional](../../../../../../functional.md) on this reduced [affine space](../../../../../../affine-space.md). The requested $f\partial^{-1},g\partial^{-1}$ representatives, used consistently for variational gradients, give the well-defined constant field bracket just computed; a general restriction from the ambient operator algebra needs an appropriate reduction.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
