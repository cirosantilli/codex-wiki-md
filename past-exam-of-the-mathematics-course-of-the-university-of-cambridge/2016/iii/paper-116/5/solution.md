<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Fix a reference path $\gamma_*$ from $L_0$ to $L_1$. By path connectedness, a path $\gamma$ can be joined to it by a smooth homotopy strip $u:[0,1]_s\times[0,1]_t\to M$ with

$$
u(0,t)=\gamma_*(t),\quad u(1,t)=\gamma(t),\quad u(s,0)\in L_0,\quad u(s,1)\in L_1.
$$

Smooth homotopies may be used by the relative smoothing theorem; piecewise smooth homotopies give the same integrals. Orient the square by $ds\wedge dt$ and define the [Lagrangian path-area functional](../../../../../lagrangian-path-area-functional.md) by

$$
\boxed{\mathcal A(\gamma)=-\int_{[0,1]^2}u^*\omega.}
$$

Here $\mathcal A$ denotes the functional called $A$ in the question. The minus sign is the convention for which downward [gradient flow](../../../../../gradient-flow.md) is $J$-holomorphic on the standard oriented strip.

For [relative symplectic-area independence](../../../../../relative-symplectic-area-independence.md), glue two choices, with one orientation reversed, along their common reference and final paths. The resulting oriented surface is a relative $2$-cycle $Z$ in $(M,L_0\cup L_1)$. Since $H_2(M,L_0\cup L_1)=0$, it bounds a relative $3$-chain: as an absolute chain, $Z=\partial B+C$ for a chain $C$ supported in $L_0\cup L_1$. The [symplectic form](../../../../../symplectic-form.md) is closed, and it restricts to zero on each [Lagrangian submanifold](../../../../../lagrangian-submanifold.md). Using piecewise smooth relative chains, [Stokes theorem](../../../../../stokes-theorem.md) gives

$$
\int_Z\omega=\int_Bd\omega+\int_C\omega=0.
$$

Equivalently, integration of the closed [symplectic form](../../../../../symplectic-form.md) defines the zero pairing on the zero relative [homology](../../../../../homology-split.md) group. The two strips therefore define the same value of $\mathcal A$.

Choosing a different reference path changes every value by the negative area of one fixed connecting strip, independent of $\gamma$. Changing the initially assigned reference value also adds a constant. Path connectedness ensures that this is **one global constant**, rather than an independent constant on each component.

For the first variation, let $\xi(t)$ be a [variation vector field](../../../../../variation-vector-field.md) along $\gamma$, with $\xi(0)\in T_{\gamma(0)}L_0$ and $\xi(1)\in T_{\gamma(1)}L_1$. Differentiate the defining strip integral. [Stokes theorem](../../../../../stokes-theorem.md), or the variation formula for the integral of a closed [differential form](../../../../../differential-form-split.md), reduces it to the final edge; the side edges give zero because their variations and tangent vectors lie in the [Lagrangian submanifolds](../../../../../lagrangian-submanifold.md). With the chosen sign,

$$
\boxed{(d\mathcal A)_\gamma(\xi)=-\int_0^1\omega(\xi(t),\dot\gamma(t))\,dt
=\int_0^1\omega(\dot\gamma(t),\xi(t))\,dt.}
$$

If this vanishes for every admissible $\xi$, it in particular vanishes for every field supported in $(0,1)$. Nondegeneracy of the [symplectic form](../../../../../symplectic-form.md), together with the [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md), forces $\dot\gamma(t)=0$ in the interior and hence everywhere by smoothness. Conversely, a constant path makes the displayed integral zero. The constant must lie in both endpoint submanifolds. Thus

$$
\boxed{\operatorname{Crit}(\mathcal A)=\{\gamma(t)\equiv x:x\in L_0\cap L_1\}.}
$$

No transverse-intersection assumption is required; the critical set can be empty or have positive dimension.

A [compatible almost complex structure](../../../../../compatible-almost-complex-structure.md) is a smooth bundle map $J:TM\to TM$ such that

$$
J^2=-I,\qquad\omega(Jv,Jw)=\omega(v,w),\qquad\omega(v,Jv)>0\quad(v\ne0).
$$

These conditions make

$$
\boxed{g(v,w)=\omega(v,Jw)}
$$

a [Riemannian metric](../../../../../riemannian-metric.md). Its symmetry follows from the $J$-invariance and skew symmetry of $\omega$, and its positivity is the final compatibility condition. It also satisfies $g(Jv,w)=\omega(v,w)$.

Use the formal $L^2$ metric on the [path space](../../../../../path-space.md),

$$
G_\gamma(\xi,\eta)=\int_0^1g(\xi(t),\eta(t))\,dt.
$$

The variation formula becomes

$$
(d\mathcal A)_\gamma(\xi)=G_\gamma(J\dot\gamma,\xi),\qquad\operatorname{grad}\mathcal A=J\dot\gamma.
$$

Thus a formal downward flow $s\mapsto u(s,\cdot)$ satisfies

$$
\boxed{\partial_su+J(u)\partial_tu=0,\qquad u(s,0)\in L_0,\quad u(s,1)\in L_1.}
$$

Put the standard complex structure $j$ on the strip, with $j\partial_s=\partial_t$. The [J-holomorphic curve](../../../../../pseudoholomorphic-curve.md) equation $du\circ j=J\circ du$ says $u_t=Ju_s$, which is equivalent to the displayed flow equation because $J^2=-I$. The converse is identical: a smooth [J-holomorphic curve](../../../../../pseudoholomorphic-curve.md) on the strip with the specified [Lagrangian boundary conditions](../../../../../lagrangian-boundary-condition.md) gives a formal downward trajectory of $\mathcal A$.

As a sign check, along such a strip,

$$
\frac{d}{ds}\mathcal A(u(s,\cdot))=-\int_0^1|u_s|_g^2\,dt,
\qquad\omega(u_s,u_t)=\omega(u_s,Ju_s)=|u_s|_g^2.
$$

The drop in $\mathcal A$ therefore equals the positive [symplectic area](../../../../../symplectic-area.md) swept out by the strip. The word formal matters: the $L^2$ calculation gives the interior equation and its [Lagrangian boundary conditions](../../../../../lagrangian-boundary-condition.md); it does not assert that arbitrary smooth initial paths produce a well-posed ordinary flow on the smooth [path space](../../../../../path-space.md). In particular, the expression $J\dot\gamma$ need not satisfy the endpoint tangent restrictions for an arbitrary initial path. The claimed correspondence concerns smooth solutions of the strip equation.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 116](../../paper-116-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
