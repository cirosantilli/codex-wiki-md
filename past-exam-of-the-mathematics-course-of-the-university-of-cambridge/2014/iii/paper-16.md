# Paper 16

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_16.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_16.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $Q$ be the configuration [smooth manifold](../../../differential-geometry.md#smooth-manifold), and let $L(t,q,v)$ be a [smooth](../../../analysis.md#smooth-function) [Lagrangian](../../../calculus-of-variations.md#lagrangian) on its [tangent bundle](../../../fiber-bundle.md#tangent-bundle). For a path with fixed endpoints, its [action](../../../classical-mechanics.md#action) is

$$
S[q]=\int_a^b L(t,q(t),\dot q(t))\,dt.
$$

The [principle of stationary action](../../../classical-mechanics.md#principle-of-stationary-action) requires the [first variation](../../../calculus-of-variations.md#first-variation) to vanish for every fixed-endpoint [variation](../../../calculus-of-variations.md#variation). In a coordinate chart take $q_s=q+s\eta$, with $\eta(a)=\eta(b)=0$. Differentiation under the integral and [integration by parts](../../../calculus.md#integration-by-parts) give

$$
\left.\frac d{ds}S[q_s]\right|_{s=0}
=\int_a^b\left(\frac{\partial L}{\partial q^i}\eta^i+\frac{\partial L}{\partial v^i}\dot\eta^i\right)dt
=\int_a^b\left(\frac{\partial L}{\partial q^i}-\frac d{dt}\frac{\partial L}{\partial v^i}\right)\eta^i\,dt.
$$

Repeated coordinate indices are summed. The endpoint term vanishes. Since compactly supported [variations](../../../calculus-of-variations.md#variation) can be chosen independently in each coordinate, the [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) yields the [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation)

$$
\boxed{\frac d{dt}\frac{\partial L}{\partial\dot q^i}=\frac{\partial L}{\partial q^i}.}
$$

Conversely these equations make the displayed [first variation](../../../calculus-of-variations.md#first-variation) zero for every fixed-endpoint [variation](../../../calculus-of-variations.md#variation). Variations localized in coordinate charts establish the same assertion for paths on $Q$. Thus **the [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) are exactly the stationary-path condition**, not necessarily a condition for an [action](../../../classical-mechanics.md#action) minimum.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The passage to [Hamiltonian mechanics](../../../classical-mechanics.md#hamiltonian-mechanics) uses the [Legendre transform in mechanics](../../../classical-mechanics.md#legendre-transform-in-mechanics). Assume a [regular Lagrangian](../../../classical-mechanics.md#regular-lagrangian): the velocity [Hessian matrix](../../../calculus.md#hessian-matrix) $(\partial^2L/\partial v^i\partial v^j)$ is invertible. Then

$$
p_i=\frac{\partial L}{\partial v^i}
$$

defines a locally invertible map from the [tangent bundle](../../../fiber-bundle.md#tangent-bundle) to the [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle). Write its local inverse as $v=v(t,q,p)$ and define the [Hamiltonian](../../../classical-mechanics.md#hamiltonian)

$$
H(t,q,p)=p_iv^i-L(t,q,v).
$$

Differentiating this expression, all terms containing $dv$ cancel because $p_i=L_{v^i}$. Hence

$$
dH=v^i\,dp_i-L_{q^i}\,dq^i-L_t\,dt,
\qquad H_{p_i}=v^i,\quad H_{q^i}=-L_{q^i}.
$$

The [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) become [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations):

$$
\boxed{\dot q^i=H_{p_i},\qquad\dot p_i=-H_{q^i}.}
$$

Conversely, a solution of [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations) satisfies $\dot q=v(t,q,p)$, hence $p=L_v(t,q,\dot q)$, and $\dot p=L_q$ recovers the [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation). This proves local equivalence of the two descriptions.

On the [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle), choose the canonical [symplectic form](../../../symplectic-geometry.md#symplectic-form) $\omega_{\mathrm{can}}=\sum_i dq^i\wedge dp_i=-d\lambda$ and the convention $\iota_{X_H}\omega_{\mathrm{can}}=dH$. Then $X_H=\sum_i(H_{p_i}\partial_{q^i}-H_{q^i}\partial_{p_i})$, so its integral curves are exactly the phase-space equations above. **This sign convention is used throughout these solutions.** For a [hyperregular Lagrangian](../../../classical-mechanics.md#hyperregular-lagrangian), the [Legendre transform in mechanics](../../../classical-mechanics.md#legendre-transform-in-mechanics) is globally invertible and gives global equivalence; regularity alone only gives local equivalence. A singular velocity [Hessian matrix](../../../calculus.md#hessian-matrix) may instead produce constraints, so the ordinary unconstrained argument does not apply to every [Lagrangian](../../../calculus-of-variations.md#lagrangian).

## 2

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) is a [smooth manifold](../../../differential-geometry.md#smooth-manifold) $M$ equipped with a [differential two-form](../../../differential-form.md#2-form) $\omega$ such that

$$
\boxed{d\omega=0,\qquad\omega_p(v,w)=0\text{ for all }w\in T_pM\Longrightarrow v=0.}
$$

The first condition says it is a [closed differential form](../../../differential-form.md#closed-differential-form); the second says it is pointwise [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form). A nondegenerate skew-symmetric matrix has even size, so the dimension is $2n$. Equivalently, $\omega^n$ is a nowhere-zero top-degree [differential form](../../../differential-form.md). It supplies an [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) and the [volume form](../../../differential-form.md#volume-form) $\omega^n/n!$. These are the defining conditions on the [symplectic form](../../../symplectic-geometry.md#symplectic-form).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Odd-dimensional [spheres](../../../geometry-and-topology.md#sphere) cannot carry a [symplectic form](../../../symplectic-geometry.md#symplectic-form), by even-dimensionality. For $S^{2m}$ with $m\geq2$, the second [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) group vanishes. Any hypothetical [symplectic form](../../../symplectic-geometry.md#symplectic-form) would therefore be $\omega=d\alpha$. The [symplectic cohomology obstruction](../../../symplectic-geometry.md#symplectic-cohomology-obstruction) gives

$$
\int_{S^{2m}}\omega^m
=\int_{S^{2m}}d(\alpha\wedge\omega^{m-1})=0
$$

by the [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem). But the [symplectic orientation](../../../symplectic-geometry.md#symplectic-orientation) makes $\omega^m$ a positive [volume form](../../../differential-form.md#volume-form), whose integral on this nonempty compact manifold is positive. This is a contradiction.

The oriented area form on $S^2$ is nondegenerate and automatically closed, since a two-dimensional manifold has no nonzero three-forms. Thus **among positive-dimensional spheres, exactly $S^2$ admits a symplectic structure**:

$$
\boxed{n=2\quad\text{for }n\geq1.}
$$

If zero-dimensional [symplectic manifolds](../../../symplectic-geometry.md#symplectic-manifold) are admitted, $S^0$ also qualifies: its zero two-form is nondegenerate on the zero [tangent spaces](../../../differential-geometry.md#tangent-space). This is a convention-dependent additional case, not another positive-dimensional example.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**There are no symplectic structures on the [Möbius strip](../../../topology.md#mobius-band).** A [symplectic form](../../../symplectic-geometry.md#symplectic-form) on a surface would be a nowhere-vanishing two-form, hence would provide an [orientation](../../../algebraic-topology.md#orientation-of-a-simplex). The [Möbius strip](../../../topology.md#mobius-band) is nonorientable: transport around its core reverses a transverse direction and therefore reverses any local [orientation](../../../algebraic-topology.md#orientation-of-a-simplex). This is incompatible with such a two-form. The argument applies whether the boundary is included or only the interior is considered.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

A [symplectic vector field](../../../symplectic-geometry.md#symplectic-vector-field) satisfies $\mathcal L_X\omega=0$, so its local flow consists of [symplectomorphisms](../../../symplectic-geometry.md#symplectomorphism). By [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) and $d\omega=0$, this is equivalent to the [differential one-form](../../../differential-form.md#one-form) $\iota_X\omega$ being closed. In the convention fixed above, a [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) satisfies $\iota_X\omega=dH$ for a globally defined smooth function $H$. It is therefore a [symplectic vector field](../../../symplectic-geometry.md#symplectic-vector-field), but the converse requires this closed one-form to be exact.

On the [torus](../../../topology.md#torus) with $\omega=dx\wedge dy$,

$$
\iota_{\partial_x}\omega=dy,\qquad d(dy)=0.
$$

Thus $\partial_x$ is a [symplectic vector field](../../../symplectic-geometry.md#symplectic-vector-field). The closed [differential one-form](../../../differential-form.md#one-form) $dy$ is not exact on the [torus](../../../topology.md#torus): its integral on the loop $\gamma(s)=[(0,s)]$, $0\leq s\leq1$, equals one, while the integral of an exact one-form around any closed loop is zero. **The vector field is symplectic but not Hamiltonian.** The local candidate $H=y$ does not descend to a single-valued function on $\mathbb R^2/\mathbb Z^2$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) of $H$ solves

$$
\frac d{dt}\phi_H^t(p)=X_H(\phi_H^t(p)),\qquad\phi_H^0(p)=p,
\qquad\iota_{X_H}\omega=dH.
$$

Compactness and the absence of a boundary make this [smooth](../../../analysis.md#smooth-function) [vector field](../../../calculus.md#vector-field) complete, so the flow exists for all real $t$. The defining equation and [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) give

$$
\mathcal L_{X_H}\omega=d\iota_{X_H}\omega+\iota_{X_H}d\omega=d^2H=0.
$$

Therefore the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) differentiation rule yields

$$
\frac d{dt}(\phi_H^t)^*\omega=(\phi_H^t)^*(\mathcal L_{X_H}\omega)=0,
$$

so $(\phi_H^t)^*\omega=\omega$. Pullback commutes with the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms), and consequently

$$
\boxed{(\phi_H^t)^*\left(\frac{\omega^n}{n!}\right)=\frac{\omega^n}{n!}.}
$$

Thus the flow preserves the [symplectic volume](../../../symplectic-geometry.md#symplectic-volume), in fact the entire [symplectic form](../../../symplectic-geometry.md#symplectic-form).

## 3

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

[Moser's trick](../../../symplectic-geometry.md#moser-s-trick) turns variation of [symplectic forms](../../../symplectic-geometry.md#symplectic-form) into an equation for a time-dependent [vector field](../../../calculus.md#vector-field). Let $\omega_t$, $0\leq t\leq1$, be a smooth path of [symplectic forms](../../../symplectic-geometry.md#symplectic-form) on a compact manifold without boundary, with a constant [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class. Choose a smooth family of one-forms $\alpha_t$ such that $\dot\omega_t=d\alpha_t$. Such a smooth choice can be made using a fixed auxiliary metric; the essential requirement is this exactness throughout the path.

Nondegeneracy uniquely determines $X_t$ by

$$
\iota_{X_t}\omega_t=-\alpha_t.
$$

Let $f_t$ be its flow, with $f_0=\mathrm{id}$. Compactness ensures existence over the whole parameter interval. By [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula),

$$
\frac d{dt}f_t^*\omega_t
=f_t^*(\dot\omega_t+\mathcal L_{X_t}\omega_t)
=f_t^*(d\alpha_t+d\iota_{X_t}\omega_t)=0.
$$

Thus

$$
\boxed{f_t^*\omega_t=\omega_0.}
$$

The path is made constant by a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) moving with $X_t$. Every interpolating form must be nondegenerate; equal endpoint cohomology alone does not ensure that every linearly interpolated form is a [symplectic form](../../../symplectic-geometry.md#symplectic-form). On a noncompact manifold one instead needs completeness of this flow, or restricts to a sufficiently small neighborhood, as in the local argument below.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Symplectic Darboux theorem](../../../symplectic-geometry.md#darboux-theorem-symplectic-geometry) says that every point of a $2n$-dimensional [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) has local coordinates $(q^1,\ldots,q^n,p_1,\ldots,p_n)$ in which

$$
\boxed{\omega=\sum_{i=1}^n dq^i\wedge dp_i.}
$$

First choose linear coordinates at the point so the form there is standard. The required [symplectic basis](../../../linear-algebra.md#symplectic-basis) can be constructed inductively: choose $e,f$ with $\omega(e,f)=1$, split off their span, and repeat on its nondegenerate [symplectic orthogonal complement](../../../linear-algebra.md#symplectic-orthogonal-complement). Extend these coordinates to a chart centered at zero.

Let $\omega_0$ be the constant standard form in this chart and $\eta=\omega-\omega_0$. The closed form $\eta$ vanishes at zero. On a small star-shaped ball the radial [Poincaré lemma](../../../differential-form.md#poincare-lemma) supplies a primitive

$$
\alpha_x(v)=\int_0^1 t\,\eta_{tx}(x,v)\,dt,\qquad d\alpha=\eta.
$$

Since $\eta_0=0$, this primitive is $O(|x|^2)$. The interpolating forms $\omega_t=\omega_0+t\eta$ are nondegenerate on a common smaller ball, because they all agree with $\omega_0$ at zero and $t$ ranges over a compact interval.

Apply the local version of [Moser's trick](../../../symplectic-geometry.md#moser-s-trick): solve $\iota_{X_t}\omega_t=-\alpha$. The [vector fields](../../../calculus.md#vector-field) are $O(|x|^2)$ and fix zero. On a sufficiently small ball their flows exist for $0\leq t\leq1$ and remain inside the coordinate chart; the quadratic bound makes their displacement smaller than the available margin. The same pullback calculation gives $f_1^*\omega=\omega_0$. Thus $f_1$ is a local [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism) from the standard ball into $M$, and its inverse supplies the desired [Darboux chart](../../../symplectic-geometry.md#darboux-chart). **There are no local symplectic invariants beyond dimension.**

## 4

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $\pi:T^*L\to L$ be the [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle) projection. The [canonical one-form on a cotangent bundle](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) is intrinsically defined by

$$
\lambda_{(q,p)}(V)=p(d\pi(V)).
$$

No metric or coordinate choice is needed. In local coordinates $\lambda=\sum_i p_i\,dq^i$. Choose

$$
\boxed{\omega_{\mathrm{can}}=-d\lambda=\sum_i dq^i\wedge dp_i.}
$$

It is closed because $d^2=0$, and its coordinate matrix is $\begin{pmatrix}0&I\\-I&0\end{pmatrix}$, which is invertible. The intrinsic definition of $\lambda$ makes the forms agree under all cotangent coordinate changes. This is the canonical [symplectic form](../../../symplectic-geometry.md#symplectic-form); choosing $d\lambda$ instead is the opposite common sign convention.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) of a $2n$-dimensional [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) is an embedded $n$-dimensional submanifold on which the [symplectic form](../../../symplectic-geometry.md#symplectic-form) restricts to zero. The dimension requirement distinguishes it from a lower-dimensional [isotropic submanifold](../../../symplectic-geometry.md#isotropic-submanifold).

A [differential one-form](../../../differential-form.md#one-form) $\sigma$ on $L$ gives an embedded section of its [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle), since $\pi\circ\sigma=\mathrm{id}$. Directly from the [canonical one-form on a cotangent bundle](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle),

$$
\sigma^*\lambda=\sigma,\qquad\sigma^*\omega_{\mathrm{can}}=-d\sigma.
$$

Its graph already has half the ambient dimension. Therefore

$$
\boxed{\operatorname{graph}(\sigma)\text{ is Lagrangian}\iff d\sigma=0.}
$$

This proves the [graph of a closed one-form is Lagrangian](../../../symplectic-geometry.md#graph-of-a-closed-one-form-is-lagrangian) criterion, in both directions.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Use the [Weinstein neighborhood theorem](../../../symplectic-geometry.md#weinstein-neighborhood-theorem): a neighborhood of a compact [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) is [symplectomorphic](../../../symplectic-geometry.md#symplectomorphism) to a neighborhood of the zero section of its [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle), with the identification equal to the identity on that submanifold. Take the canonical sign $-d\lambda$ in this identification. We also use [C1 openness of diffeomorphisms](../../../geometry-and-topology.md#c1-openness-of-diffeomorphisms): on a compact manifold, all smooth self-maps sufficiently close in the $C^1$ topology to a fixed [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) are themselves [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism).

In $M\times M$ put $\Omega=-\operatorname{pr}_1^*\omega+\operatorname{pr}_2^*\omega$. The diagonal $\Delta$ is [Lagrangian](../../../calculus-of-variations.md#lagrangian). For a [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism) $\phi$, its graph $\Gamma_\phi$ is also [Lagrangian](../../../calculus-of-variations.md#lagrangian), because its pullback of $\Omega$ is $-\omega+\phi^*\omega=0$.

If $\phi$ is sufficiently $C^1$-close to the identity, $\Gamma_\phi$ lies in the fixed Weinstein neighborhood of $\Delta$. Its image in $T^*\Delta$ is transverse to the cotangent fibers and is a section: the projection of that image to $\Delta\cong M$ is $C^1$-close to the identity, hence is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) on compact $M$. Reparametrizing by this projection identifies the image with $\operatorname{graph}(\sigma)$ for a small [differential one-form](../../../differential-form.md#one-form) $\sigma$.

The preceding [graph of a closed one-form is Lagrangian](../../../symplectic-geometry.md#graph-of-a-closed-one-form-is-lagrangian) criterion gives $d\sigma=0$. Since $H^1_{\mathrm{dR}}(M)=0$, the [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) definition gives $\sigma=df$. Intersections with the zero section are precisely the [critical points](../../../analysis.md#critical-point) of $f$; under the neighborhood identification these are the intersections $\Gamma_\phi\cap\Delta$, hence the [fixed points](../../../function.md#fixed-point) of $\phi$.

On a nonempty compact manifold without boundary, $f$ has a maximum and a minimum. If it is nonconstant, these occur at distinct [critical points](../../../analysis.md#critical-point). If it is constant, $df=0$ everywhere, so the whole graph is the diagonal and every point is fixed. **For positive-dimensional $M$, there are at least two distinct fixed points.** This is the [nearby exact Lagrangian intersection lemma](../../../symplectic-geometry.md#nearby-exact-lagrangian-intersection-lemma) applied to the diagonal. No connectedness assumption is needed.

The usual positive-dimensional convention is necessary for the assertion: if zero-dimensional [symplectic manifolds](../../../symplectic-geometry.md#symplectic-manifold) are allowed, a single-point $M$ has $H^1=0$ and only one [fixed point](../../../function.md#fixed-point). That is a literal exception to the printed statement.

## 5

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [Hamiltonian group action](../../../symplectic-geometry.md#hamiltonian-group-action) is a [smooth](../../../analysis.md#smooth-function) [Lie group action](../../../lie-theory.md#lie-group-action) of $G$ on $(M,\omega)$ by [symplectomorphisms](../../../symplectic-geometry.md#symplectomorphism), together with an equivariant [moment map](../../../symplectic-geometry.md#moment-map) $\mu:M\to\mathfrak g^*$. For $\xi\in\mathfrak g$, let $\xi_M(p)=\left.\frac d{dt}\right|_0\exp(t\xi)\cdot p$ be its [fundamental vector field](../../../lie-theory.md#fundamental-vector-field). In our sign convention the defining identities are

$$
\boxed{d\langle\mu,\xi\rangle=\iota_{\xi_M}\omega,\qquad
\mu(g\cdot p)=\operatorname{Ad}_g^*\mu(p).}
$$

Here the left [coadjoint action](../../../lie-theory.md#coadjoint-representation) means $(\operatorname{Ad}_g^*\nu)(\xi)=\nu(\operatorname{Ad}_{g^{-1}}\xi)$. Each component $\mu^\xi$ is therefore a [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function) for the corresponding infinitesimal action. Equivariance is part of the definition; merely requiring each infinitesimal generator to be a [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) is the weaker condition of a [weakly Hamiltonian action](../../../symplectic-geometry.md#weakly-hamiltonian-action). Reversing the defining sign of [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) reverses the [moment map](../../../symplectic-geometry.md#moment-map) sign as well.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Use the normalization in which a projective line has area $2\pi$. On the affine chart of [Complex projective space](../../../algebraic-topology.md#complex-projective-space) where $Z_0\ne0$, set $w_j=Z_j/Z_0$ and $S=1+\sum_j|w_j|^2$. Define the [Fubini-Study form](../../../complex-geometry.md#fubini-study-form) by

$$
\boxed{\omega_{\mathrm{FS}}=i\partial\bar\partial\log S
=i\sum_{j,k}\frac{S\delta_{jk}-\bar w_jw_k}{S^2}\,dw_j\wedge d\bar w_k.}
$$

On another chart the corresponding potential differs by $\log|h|^2$ for a nowhere-zero [holomorphic function](../../../complex-analysis.md#holomorphic-function) $h$, whose $\partial\bar\partial$ is zero. Thus these local [differential forms](../../../differential-form.md) glue to a global form. It is real and closed. Its Hermitian coefficient matrix is positive definite, since for $v\ne0$ the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\sum_{j,k}\frac{S\delta_{jk}-\bar w_jw_k}{S^2}v_j\bar v_k
=\frac{S|v|^2-|\sum_j\bar w_jv_j|^2}{S^2}\geq\frac{|v|^2}{S^2}>0.
$$

Hence it is a [Kähler form](../../../complex-geometry.md#kahler-form) and in particular a [symplectic form](../../../symplectic-geometry.md#symplectic-form).

On a [complex projective line](../../../algebraic-topology.md#complex-projective-line) with $w=x+iy$ this is $2(1+|w|^2)^{-2}dx\wedge dy$, whose total area is $2\pi$. Thus $[\omega_{\mathrm{FS}}/(2\pi)]$ is the positive generator, equivalently $c_1(\mathcal O(1))$. Another common normalization uses half this form and gives line area $\pi$; the scale must be carried consistently into [symplectic reduction](../../../symplectic-geometry.md#symplectic-reduction).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [Marsden-Weinstein theorem](../../../symplectic-geometry.md#marsden-weinstein-theorem) says that for a [Hamiltonian group action](../../../symplectic-geometry.md#hamiltonian-group-action), if $c$ is a [regular value](../../../differential-geometry.md#regular-value) fixed by the [coadjoint action](../../../lie-theory.md#coadjoint-representation) and $G$ acts freely and properly on $\mu^{-1}(c)$, then

$$
M_c=\mu^{-1}(c)/G
$$

is a [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) with a unique form characterized by $\pi^*\omega_c=\iota^*\omega$, where $\iota$ includes the level set and $\pi$ is the quotient projection. Its dimension is $\dim M-2\dim G$.

Equip $\mathbb C^{n+1}$ with the [standard symplectic form](../../../symplectic-geometry.md#standard-symplectic-form)

$$
\omega_{\mathbb C}=\sum_{j=0}^n dx_j\wedge dy_j=\frac i2\sum_{j=0}^n dz_j\wedge d\bar z_j.
$$

Let the [circle group](../../../lie-theory.md#circle-group) act by $e^{i\theta}\cdot z=e^{i\theta}z$. Its generator is $X=\sum_j(-y_j\partial_{x_j}+x_j\partial_{y_j})$, and

$$
\iota_X\omega_{\mathbb C}=-d\left(\frac12|z|^2\right).
$$

Consequently the [moment map](../../../symplectic-geometry.md#moment-map) in our convention is $\mu(z)=-|z|^2/2$. It is invariant, hence equivariant because the [circle group](../../../lie-theory.md#circle-group) is abelian. The level $\mu^{-1}(-1)$ is the sphere of radius $\sqrt2$; it is regular, the [circle group](../../../lie-theory.md#circle-group) acts freely there, and properness follows from compactness of the group. The quotient is [Complex projective space](../../../algebraic-topology.md#complex-projective-space), by $z\mapsto[z]$, a scaled [Hopf fibration](../../../algebraic-topology.md#hopf-fibration). The [Marsden-Weinstein theorem](../../../symplectic-geometry.md#marsden-weinstein-theorem) therefore produces a reduced [symplectic form](../../../symplectic-geometry.md#symplectic-form) on $\mathbb{CP}^n$.

To identify it rather than only assert its existence, use the primitive

$$
\lambda_0=\frac12\sum_j(x_jdy_j-y_jdx_j)
=\frac1{4i}\sum_j(\bar z_jdz_j-z_jd\bar z_j),\qquad d\lambda_0=\omega_{\mathbb C}.
$$

On the affine chart choose the local section $s(w)=\sqrt2(1,w)/\sqrt S$ of the quotient. Direct substitution gives

$$
s^*\lambda_0=\frac1{2iS}\sum_j(\bar w_jdw_j-w_jd\bar w_j)
=\frac1{2i}(\partial-\bar\partial)\log S.
$$

Differentiating, using $\bar\partial\partial=-\partial\bar\partial$, gives

$$
\boxed{\omega_c=s^*\omega_{\mathbb C}=d(s^*\lambda_0)=i\partial\bar\partial\log S=\omega_{\mathrm{FS}}.}
$$

This is the [Fubini-Study form from circle reduction](../../../complex-geometry.md#fubini-study-form-from-circle-reduction). The unit sphere instead produces half this form; our radius $\sqrt2$ is exactly what gives the $2\pi$ line-area normalization used above.

## 6

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

An [almost complex structure](../../../complex-geometry.md#almost-complex-manifold) is a smooth bundle endomorphism $J:TM\to TM$ with $J^2=-I$. It is an $\omega$-[compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure) when

$$
\boxed{\omega(Jv,Jw)=\omega(v,w),\qquad\omega(v,Jv)>0\quad(v\ne0).}
$$

These conditions make $g_J(v,w)=\omega(v,Jw)$ a [Riemannian metric](../../../differential-geometry.md#riemannian-metric). In particular it is symmetric: invariance and $J^2=-I$ give $\omega(Jv,w)=-\omega(v,Jw)$, and skew-symmetry then gives $g_J(w,v)=g_J(v,w)$. Positivity is the second condition. Moreover $J$ is an isometry for $g_J$. Compatibility does not require that the [almost complex structure](../../../complex-geometry.md#almost-complex-manifold) be integrable.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For a [Riemann surface](../../../complex-analysis.md#riemann-surfaces) $(\Sigma,j)$ and an [almost complex manifold](../../../complex-geometry.md#almost-complex-manifold) $(M,J)$, a [J-holomorphic curve](../../../symplectic-geometry.md#pseudoholomorphic-curve) is a [smooth](../../../analysis.md#smooth-function) map $u:\Sigma\to M$ satisfying

$$
\boxed{du\circ j=J\circ du,\qquad\bar\partial_Ju:=\frac12(du+J\circ du\circ j)=0.}
$$

Thus its differential is complex-linear at every point. In oriented local coordinates $s,t$ with $j\partial_s=\partial_t$, this is $u_t=Ju_s$, equivalently $u_s+Ju_t=0$. No integrability of the target [almost complex structure](../../../complex-geometry.md#almost-complex-manifold) is required. Constant maps satisfy the definition; some usages reserve the word curve for nonconstant maps, so that restriction should be stated separately when intended.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Choose a [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $h$ on $\Sigma$ compatible with its [complex structure](../../../complex-geometry.md#complex-structure) $j$, and use $g_J=\omega(\cdot,J\cdot)$ on the target. The [Dirichlet energy of a map](../../../differential-geometry.md#dirichlet-energy-of-a-map) is

$$
E(u)=\frac12\int_\Sigma|du|_{h,g_J}^2\,d\operatorname{vol}_h.
$$

It is independent of the particular conformal representative $h$: rescaling $h$ multiplies the squared differential norm by the inverse factor and the area element by the same factor. For a [J-holomorphic curve](../../../symplectic-geometry.md#pseudoholomorphic-curve), the [Energy identity for a J-holomorphic curve](../../../symplectic-geometry.md#energy-identity-for-a-j-holomorphic-curve) is

$$
\boxed{E(u)=\int_\Sigma u^*\omega.}
$$

To prove it, take an oriented $h$-orthonormal frame $e_1,e_2=je_1$ and put $a=du(e_1)$, $b=du(e_2)$. The [J-holomorphic curve](../../../symplectic-geometry.md#pseudoholomorphic-curve) equation says $b=Ja$. The pointwise energy density is therefore $\frac12(|a|_{g_J}^2+|Ja|_{g_J}^2)=|a|_{g_J}^2$, while the pulled-back area density is $\omega(a,Ja)=|a|_{g_J}^2$. Integrating proves the identity.

More generally, the same frame gives

$$
\frac12(|a|^2+|b|^2)-\omega(a,b)=\frac12|b-Ja|^2.
$$

With the full tensor [norm](../../../functional-analysis.md#norm) of $\bar\partial_Ju$, its two frame components are $(a+Jb)/2$ and $(b-Ja)/2$, so their squared norms sum to $\frac12|b-Ja|^2$. Hence the full identity is

$$
E(u)=\int_\Sigma u^*\omega+\int_\Sigma|\bar\partial_Ju|^2\,d\operatorname{vol}_h.
$$

This also fixes the normalization of the error term. **The energy is nonnegative and vanishes exactly when $du=0$.** The formulas apply whenever the relevant integrals are defined, in particular on compact source surfaces.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

**No nonconstant [J-holomorphic curve](../../../symplectic-geometry.md#pseudoholomorphic-curve) with this closed connected source exists.** The [standard symplectic form](../../../symplectic-geometry.md#standard-symplectic-form) on $\mathbb R^{2n}$ is exact; for instance

$$
\omega_0=d\lambda_0,\qquad\lambda_0=\frac12\sum_j(x_jdy_j-y_jdx_j).
$$

The [Energy identity for a J-holomorphic curve](../../../symplectic-geometry.md#energy-identity-for-a-j-holomorphic-curve) and the [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem) give

$$
E(u)=\int_\Sigma u^*\omega_0
=\int_\Sigma d(u^*\lambda_0)
=\int_{\partial\Sigma}u^*\lambda_0=0.
$$

The target metric from the [compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure) is positive definite, so the nonnegative continuous energy density must vanish everywhere. Thus $du=0$. Connectedness of $\Sigma$ makes $u$ constant. This argument uses exactness and compatibility, and works even when $J$ is nonintegrable; it does not require the ordinary holomorphic maximum principle on the target.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
