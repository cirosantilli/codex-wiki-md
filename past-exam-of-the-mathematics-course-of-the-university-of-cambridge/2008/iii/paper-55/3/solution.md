<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $T=\tfrac12\int|\nabla\phi|^2d^nx$ and $W=\int U(\phi)d^nx$. For a sufficiently regular [finite-energy field configuration](../../../../../finite-energy-field-configuration.md) with vacuum asymptotics, the scaled field $\phi_\lambda(x)=\phi(\lambda x)$ stays in the same boundary sector. Changing variables gives the [Derrick scaling](../../../../../derrick-scaling.md) formula

$$
V(\phi_\lambda)=\lambda^{2-n}T+\lambda^{-n}W.
$$

A static solution must be stationary under this variation, so the [Derrick virial identity](../../../../../derrick-virial-identity.md) is

$$
\boxed{(n-2)T+nW=0.}
$$

For $n>2$, both terms are nonnegative, so both vanish and the field is constant at a vacuum. Hence **there are no nonconstant smooth finite-energy static solitons of this scalar type for $n>2$**. For $n=1$ the identity is $T=W$, allowing [kinks](../../../../../scalar-field-kink.md). For $n=2$ it requires $W=0$: a nonzero potential contribution excludes a static soliton, but the scaling identity alone does not exclude a purely derivative energy.

There is a useful refinement specific to the unconstrained flat target $\mathbb R^l$. If $U$ is differentiable and nonnegative, $W=0$ implies $U(\phi(x))=0$ and $\nabla_\phi U=0$ on the image. The static [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md) then give $\Delta\phi=0$. Each first derivative is an entire harmonic function in [L2 space](../../../../../l2-space-is-a-hilbert-space.md). Its mean-value bound over a disk of radius $R$ is at most its total squared norm divided by $\pi R^2$; letting $R\to\infty$ shows that derivative is zero. Thus even the exceptional two-dimensional case has only constant smooth finite-energy solutions into this flat target. This [two-dimensional flat-target Derrick obstruction](../../../../../two-dimensional-flat-target-derrick-obstruction.md) uses the field equations in addition to the scale identity.

The [Yang-Mills theory](../../../../../yang-mills-theory.md) with a [Higgs field](../../../../../higgs-field.md) escapes the original scaling because the gauge curvature is quadratic in spatial scaling. In three dimensions use $A_i^\lambda(x)=\lambda A_i(\lambda x)$ and $\Phi^\lambda(x)=\Phi(\lambda x)$. Then $F^\lambda_{ij}=\lambda^2F_{ij}(\lambda x)$ and $D_i^\lambda\Phi^\lambda=\lambda D_i\Phi(\lambda x)$. Writing the magnetic, Higgs-gradient and Higgs-potential energies as $V_B,V_D,V_U$, the [Derrick scaling of Yang-Mills-Higgs energy](../../../../../derrick-scaling-of-yang-mills-higgs-energy.md) gives

$$
V_\lambda=\lambda V_B+\lambda^{-1}V_D+\lambda^{-3}V_U,
\qquad V_B=V_D+3V_U
$$

at stationarity. These terms can balance. In particular, the zero-potential [Bogomolny-Prasad-Sommerfield monopole](../../../../../bogomolny-prasad-sommerfield-monopole.md) has $V_B=V_D\ne0$.

For a [nonlinear sigma model](../../../../../nonlinear-sigma-model.md) in two dimensions, the [harmonic map](../../../../../harmonic-map.md) energy is purely quadratic in first derivatives and is scale invariant: $V_\lambda=V$. Its target is a curved manifold, not the unconstrained Euclidean target of the refinement above. Its equation is the nonlinear harmonic-map equation, not componentwise $\Delta\phi=0$. The [Derrick theorem](../../../../../derrick-s-theorem.md) therefore gives no obstruction. Nonconstant finite-energy maps into $S^2$, as in the [O3 nonlinear sigma model](../../../../../o3-nonlinear-sigma-model.md), provide examples with nonzero degree.

For the complex theory, regard $\phi$ and $\bar\phi$ as independent variables in the variation, and write $s=|\phi|^2$, $U=U(s)$. Variation in $\bar\phi$ gives

$$
\frac{\partial\mathcal L}{\partial\bar\phi}=-U'(s)\phi,\qquad
\frac{\partial\mathcal L}{\partial(\partial_\mu\bar\phi)}=\frac12\partial^\mu\phi.
$$

Thus

$$
\boxed{\phi_{tt}-\Delta\phi+2U'(|\phi|^2)\phi=0.}
$$

The factor 2 follows from the printed $1/2$ normalization of the complex kinetic term; equivalently vary its two real components.

A [non-topological soliton](../../../../../non-topological-soliton.md) is a localized finite-energy persistent field solution with no protecting winding or other nontrivial topological sector. In this complex theory a [Q-ball](../../../../../q-ball.md) has a stationary spatial profile and a rotating phase,

$$
\phi(t,x)=e^{i\omega t}f(x),\qquad f(x)\to0\text{ at infinity},
$$

with real $f$. It is not static as a field even though its energy density is time-independent. The global phase symmetry gives the [Noether charge](../../../../../noether-charge.md)

$$
Q=\int\operatorname{Im}(\bar\phi\phi_t)d^nx=\omega I,
\qquad I=\int f^2d^nx.
$$

The profile equation is $-\Delta f+2U'(f^2)f-\omega^2f=0$. Its energy is $T+W+\omega^2I/2$. To vary the size at fixed charge one must also vary the frequency, because scaling $f$ at fixed $\omega$ would change $Q$. Eliminating $\omega=Q/I$ gives [charge-constrained scalar-field scaling](../../../../../charge-constrained-scalar-field-scaling.md):

$$
E_Q[f_\lambda]=\lambda^{2-n}T+\lambda^{-n}W+\lambda^n\frac{Q^2}{2I}.
$$

The new positive-power term can balance the other terms for $n>1$, including $n>2$, so the static [Derrick theorem](../../../../../derrick-s-theorem.md) does not rule out these solutions. Equivalently, at fixed frequency the profile extremizes $T+\int[U(f^2)-\omega^2f^2/2]$, whose effective potential need not be nonnegative. This explains both the time dependence and the charge constraint behind the evasion; a complex field by itself is not enough.

For an explicit example take the [sextic unique-vacuum Q-ball potential](../../../../../sextic-unique-vacuum-q-ball-potential.md)

$$
\boxed{U(|\phi|^2)=|\phi|^2-|\phi|^4+|\phi|^6.}
$$

It is nonnegative, since $U(s)=s[(s-1/2)^2+3/4]$, and its only vacuum is zero. Its small-field mass squared is $2U'(0)=2$, while $\min_{s>0}2U(s)/s=3/2$. It supports localized [Q-balls](../../../../../q-ball.md), for example radial ones in three dimensions with $3/2<\omega^2<2$. In that range the profile potential is positive quadratic near zero but negative somewhere away from zero, permitting a localized nontrivial profile. This example uses a conserved phase charge and no vacuum winding.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
