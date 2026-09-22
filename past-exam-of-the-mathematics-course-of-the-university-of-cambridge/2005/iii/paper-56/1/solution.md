<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The nonexistence conclusion concerns nonconstant fields: a constant [scalar-field vacuum](../../../../../scalar-field-vacuum.md) with $U=0$ is a zero-energy [critical point of an energy functional](../../../../../critical-point-of-an-energy-functional.md) in every dimension. Assume the potential is smooth, so the classical [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is well defined. Write the two nonnegative [energy](../../../../../energy.md) terms as

$$
T=\frac12\int|\nabla\phi|^2\,d^Dx,\qquad
V=\int U(\phi)\,d^Dx.
$$

For the admissible [Derrick scaling](../../../../../derrick-scaling.md) $\phi_\lambda(x)=\phi(\lambda x)$,

$$
E(\phi_\lambda)=\lambda^{2-D}T+\lambda^{-D}V.
$$

Stationarity at $\lambda=1$ gives the [Derrick virial identity](../../../../../derrick-virial-identity.md)

$$
\boxed{(2-D)T-DV=0.}
$$

For $D>2$, both terms have nonpositive sign, forcing $T=V=0$ and hence a constant vacuum. For $D=2$, scaling alone only proves $V=0$; the gradient term is scale invariant, so it must not simply be declared zero.

The [two-dimensional flat-target Derrick obstruction](../../../../../two-dimensional-flat-target-derrick-obstruction.md) supplies that remaining step. Since $U\geq0$ and its integral is zero, continuity gives $U(\phi(x))=0$ everywhere; smooth nonnegative $U$ has $U'(\phi(x))=0$ at those values. The field equation $\Delta\phi=U'(\phi)$ therefore becomes $\Delta\phi=0$. Each $\partial_i\phi$ is an entire [harmonic function](../../../../../harmonic-function.md) in $L^2(\mathbb R^2)$. Its [mean value property](../../../../../mean-value-property-for-harmonic-functions.md) and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) give, for every radius $R$,

$$
|\partial_i\phi(x_0)|
\leq\frac{\|\partial_i\phi\|_{L^2(\mathbb R^2)}}{\sqrt{\pi R^2}}.
$$

Let $R\to\infty$ to get $\partial_i\phi=0$. Thus $D=2$ also has only constant [stationary field configurations](../../../../../critical-point-of-an-energy-functional.md) of finite [energy](../../../../../energy.md). The unconstrained real scalar target is essential in this argument; the spherical target in Question 2 has different field equations.

In $D=1$ the field equation is $\phi''=U'(\phi)$. Multiplication by $\phi'$ gives the [first integral](../../../../../first-integral.md)

$$
\frac12(\phi')^2-U(\phi)=K.
$$

Finite [energy](../../../../../energy.md) makes $\frac12(\phi')^2+U(\phi)$ an [integrable](../../../../../integrability.md) nonnegative function, so along some sequence $x_n\to+\infty$ it tends to zero. Evaluating the constant [first integral](../../../../../first-integral.md) on that sequence gives $K=0$. Choose

$$
\boxed{W(u)=\int_{u_*}^{u}\sqrt{2U(s)}\,ds,\qquad U(u)=\frac12(W'(u))^2.}
$$

Consequently $(\phi')^2=2U(\phi)$ and

$$
\boxed{\frac{d\phi}{dx}=\pm\frac{dW}{d\phi}.}
$$

For a nonconstant entire solution the sign is fixed. Indeed a finite-$x$ zero of $\phi'$ would have $U(\phi)=U'(\phi)=0$; uniqueness of the smooth second-order equation with initial data $(\phi,\phi')=(v,0)$ would make the solution the constant vacuum. Thus $\phi'$ never vanishes in a nonconstant solution. Conversely a smooth solution of the displayed first-order equation satisfies $\phi''=U'(\phi)$ wherever it is nonconstant.

Under the usual soliton boundary conditions $\phi(x)\to v_\pm$ as $x\to\pm\infty$, with $v_\pm$ in the [vacuum manifold](../../../../../vacuum-manifold.md) $\{U=0\}$, the two endpoint components label the [topological sector](../../../../../topological-sector.md). For isolated [scalar-field vacua](../../../../../scalar-field-vacuum.md) this is an ordered pair of vacuum labels, not necessarily one universally normalized integer. More explicitly, for any smooth $F$, the [topological current](../../../../../topological-current.md)

$$
j_F^\mu=\epsilon^{\mu\nu}\partial_\nu F(\phi),\qquad
\partial_\mu j_F^\mu=0,\qquad
Q_F=\int j_F^0\,dx=F(v_+)-F(v_-)
$$

is identically conserved, taking $\epsilon^{01}=1$ and boundary conditions fixed during evolution. The choices $F(u)=u$ and $F(u)=W(u)$ give the field-difference charge and the kink [energy](../../../../../energy.md) charge. The [square completion for a one-dimensional kink](../../../../../square-completion-for-a-one-dimensional-kink.md) gives

$$
E=\frac12\int(\phi'\mp W'(\phi))^2\,dx
\pm[W(v_+)-W(v_-)],
\qquad
\boxed{E\geq|W(v_+)-W(v_-)|.}
$$

The first-order critical solution saturates this [Bogomolny bound](../../../../../bogomolny-bound.md). A nonzero difference between endpoint vacuum components prevents continuous deformation to a vacuum while those boundary conditions remain fixed. Finite [energy](../../../../../energy.md) alone need not give finite endpoint values for arbitrary potentials, so these topological labels use the stated vacuum boundary conditions.

To evade the scalar-only obstruction, introduce a [gauge field](../../../../../gauge-field.md) and a charged, generally multicomponent [Higgs field](../../../../../higgs-field.md). For a Yang-Mills-Higgs [energy](../../../../../energy.md) write $E=T_H+V+E_B$, where $T_H$ contains $|D_i\Phi|^2$ and $E_B$ contains $|F_{ij}|^2$. Rescale $\Phi_\lambda(x)=\Phi(\lambda x)$ and $A_{i,\lambda}(x)=\lambda A_i(\lambda x)$. Then $D_i\Phi$ scales by $\lambda$, while $F_{ij}$ scales by $\lambda^2$, so

$$
E_\lambda=\lambda^{2-D}T_H+\lambda^{-D}V+\lambda^{4-D}E_B,
\qquad
\boxed{(2-D)T_H-DV+(4-D)E_B=0.}
$$

The magnetic term supplies the missing opposing scaling power. In $D=2$ the relation is $E_B=V$, permitting [Abelian Higgs vortices](../../../../../nielsen-olesen-vortex.md); in $D=3$ it is $E_B=T_H+3V$, permitting ['t Hooft-Polyakov monopoles](../../../../../t-hooft-polyakov-monopole.md). In the monopole Bogomolny limit $V=0$, $B_i=\pm D_i\Phi$ achieves $E_B=T_H$. Also, asymptotic ordinary derivatives need not vanish when a Higgs phase winds: the relevant vanishing quantity is the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md). This allows nontrivial boundary winding with finite [energy](../../../../../energy.md). Merely appending a gauge potential to a neutral one-component real field would not by itself furnish that Higgs mechanism.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
