# Paper 17

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper17.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper17.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For a [symplectic vector space](../../../linear-algebra.md#symplectic-vector-space) $(V,\omega)$ and a [vector subspace](../../../vector-space.md#vector-subspace) $W$, the [symplectic orthogonal complement](../../../linear-algebra.md#symplectic-orthogonal-complement) is

$$
W^\omega=\{v\in V:\omega(v,w)=0\text{ for every }w\in W\}.
$$

[Nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form) identifies $V$ with its [dual space](../../../linear-algebra.md#dual-space), so $\dim W^\omega=\dim V-\dim W$. If $W$ is a [symplectic subspace](../../../linear-algebra.md#symplectic-subspace), $W\cap W^\omega=0$, and hence $V=W\oplus W^\omega$; the restriction to $W^\omega$ is also nondegenerate.

Here is an inductive construction of a [symplectic basis](../../../linear-algebra.md#symplectic-basis). Choose $e_1\ne0$. [Nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form) supplies $f_1$ with $\omega(e_1,f_1)=1$. The plane $P=\operatorname{span}(e_1,f_1)$ is a [symplectic subspace](../../../linear-algebra.md#symplectic-subspace), and its [symplectic orthogonal complement](../../../linear-algebra.md#symplectic-orthogonal-complement) gives $V=P\oplus P^\omega$. Repeat on $P^\omega$. The process ends in dimension zero, since each step removes two dimensions and a one-dimensional alternating form is degenerate. We obtain $e_1,f_1,\ldots,e_n,f_n$ with

$$
\omega(e_i,e_j)=\omega(f_i,f_j)=0,\qquad\omega(e_i,f_j)=\delta_{ij}.
$$

The [linear map](../../../vector-space.md#linear-map) taking the coordinate vectors of $\mathbb R^{2n}$ to this basis pulls $\omega$ back to $\sum_jdx_j\wedge dy_j$, proving the asserted normal form.

Now split $V=C\oplus D$ with $D=C^\omega$, and choose [symplectic bases](../../../linear-algebra.md#symplectic-basis) on both planes. Parametrize $\Gamma_A$ by $v\mapsto(Av,v)$. Orthogonality removes the cross terms, and a two-dimensional alternating form transforms by the [determinant](../../../linear-algebra.md#determinant), so

$$
\omega|_{\Gamma_A}\longleftrightarrow A^*\omega_C+\omega_D=(1+\det A)\omega_D.
$$

Consequently the correct [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form) criterion is

$$
\boxed{\Gamma_A\text{ is symplectic}\iff\det A\ne-1.}
$$

The strict inequality printed in the PDF requires an extra orientation condition: it says that the [symplectic orientation](../../../symplectic-geometry.md#symplectic-orientation) on the graph agrees with the orientation transported from $D$. It is not equivalent to being a [symplectic subspace](../../../linear-algebra.md#symplectic-subspace). For example, $A=\operatorname{diag}(-2,1)$ has [determinant](../../../linear-algebra.md#determinant) $-2$ and gives a nondegenerate restriction $-\omega_D$. This is the [orientation criterion for a graph of symplectic planes](../../../linear-algebra.md#orientation-criterion-for-a-graph-of-symplectic-planes).

This same map supplies the requested obstruction. Orient $C$ and $\Gamma_A$ by their restricted [symplectic forms](../../../symplectic-geometry.md#symplectic-form). If $(d_1,d_2)$ is a positive basis of $D$, then $(Ad_1+d_1,Ad_2+d_2)$ is negatively oriented in $\Gamma_A$. The coordinate transformation from a basis of $C$ followed by these graph vectors to a basis of $C\oplus D$ has [determinant](../../../linear-algebra.md#determinant) $1$. Reversing the graph basis to give its positive orientation therefore makes the oriented direct sum $C\oplus\Gamma_A$ negative relative to the ambient [symplectic orientation](../../../symplectic-geometry.md#symplectic-orientation).

Two distinct complex lines in standard $\mathbb C^2$ have the opposite behaviour: complex bases of the two lines give a complex-linear [isomorphism](../../../algebra.md#isomorphism) $\mathbb C\oplus\mathbb C\to\mathbb C^2$, whose real [determinant](../../../linear-algebra.md#determinant) is the positive number $|\det_{\mathbb C}|^2$. Their complex orientations are their [symplectic orientations](../../../symplectic-geometry.md#symplectic-orientation). A [symplectic linear map](../../../linear-algebra.md#symplectic-linear-map) preserves both the ambient and each plane's [symplectic orientation](../../../symplectic-geometry.md#symplectic-orientation), so it cannot change this sign. Thus **the pair with $A=\operatorname{diag}(-2,1)$ cannot be the image of a pair of complex lines**. Interchanging the planes does not change the sign, since both dimensions are even.

## 2

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) is a smooth even-dimensional manifold $X^{2n}$ with a closed, nondegenerate [differential two-form](../../../differential-form.md#2-form) $\omega$. A [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) $L\subset X$ has dimension $n$ and $\omega|_{TL}=0$; equivalently $T_xL=(T_xL)^\omega$ at every point.

On $T^*M$, let $\pi:T^*M\to M$ and define the [canonical one-form on a cotangent bundle](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) by $\theta_{(q,p)}(v)=p(d\pi(v))$. In local coordinates $\theta=\sum_i p_i\,dq_i$, so our sign convention gives

$$
\omega_0=-d\theta=\sum_i dq_i\wedge dp_i.
$$

The intrinsic definition of $\theta$ makes this form globally defined. It is closed because $d^2=0$, and its displayed coordinate matrix is invertible. The [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle) pulls $\theta$, and therefore $\omega_0$, back to zero and has half the total dimension. It is a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold).

We prove the [Weinstein neighborhood theorem](../../../symplectic-geometry.md#weinstein-neighborhood-theorem), rather than merely invoking it. Along a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) $L\subset(X,\omega)$, choose a [compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure) $J$; its existence is proved by the metric construction in Question 5. Then $JL$ at the tangent-bundle level means $J(TL)$, and

$$
TX|_L=TL\oplus J(TL).
$$

Indeed, $Jv\in TL$ with $v\in TL$ would imply $0=\omega(v,Jv)$, forcing $v=0$. Also $\omega(Ju,Jv)=\omega(u,v)=0$ for $u,v\in TL$, so $J(TL)$ is a [Lagrangian complement](../../../symplectic-geometry.md#lagrangian-complement). Identify a normal vector $n\in J(TL)$ with the covector $\eta(v)=\omega(v,n)$. This is a vector-bundle [isomorphism](../../../algebra.md#isomorphism) with $T^*L$, and under it

$$
\omega((v,\eta),(w,\zeta))=\zeta(v)-\eta(w),
$$

which is exactly the form $\omega_0$ along the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle). The [tubular neighborhood theorem](../../../differential-geometry.md#tubular-neighborhood-theorem) therefore supplies a smooth map $F$ from a neighborhood of that section to a neighborhood of $L$, restricting to the identity and with this derivative along $L$.

Write $\omega_1=F^*\omega$ and $\delta=\omega_1-\omega_0$. This [closed differential form](../../../differential-form.md#closed-differential-form) vanishes as an entire [bilinear form](../../../linear-algebra.md#bilinear-form) along the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle). The [relative Poincaré lemma](../../../differential-form.md#relative-poincare-lemma) gives $\delta=d\beta$ with $\beta$ zero along the section. Explicitly, if $r_s(q,p)=(q,sp)$ and $R=\sum p_i\partial_{p_i}$, use

$$
\beta=\int_0^1\frac1s r_s^*(\iota_R\delta)\,ds.
$$

The homotopy identity gives $d\beta=\delta-r_0^*\delta=\delta$; the vanishing at the section ensures smoothness of this integral. The forms $\omega_t=\omega_0+t\delta$ are nondegenerate on a sufficiently small neighborhood of the section for all $0\leq t\leq1$. Solve uniquely

$$
\iota_{Y_t}\omega_t=-\beta.
$$

The [vector field](../../../calculus.md#vector-field) $Y_t$ vanishes on the section. After another neighborhood shrink its [flow](../../../graph-theory.md#flow) $\phi_t$ exists up to time one and fixes the section. For noncompact $L$, the sizes of these neighborhoods may vary with the base point; no [compactness](../../../topology.md#compact-space) of $L$ is required for the local conclusion. By [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula),

$$
\frac d{dt}\phi_t^*\omega_t
=\phi_t^*(\delta+d\iota_{Y_t}\omega_t)=0.
$$

Thus $(F\circ\phi_1)^*\omega=\omega_0$. This establishes the universal neighborhood model, with the [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) identified with the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle).

For the section $s_\alpha(q)=(q,\alpha_q)$, the canonical [differential one-form](../../../differential-form.md#one-form) satisfies $s_\alpha^*\theta=\alpha$. Hence

$$
\boxed{s_\alpha^*\omega_0=-d\alpha,\qquad\Gamma_\alpha\text{ is Lagrangian}\iff d\alpha=0.}
$$

Its dimension is already half that of $T^*M$, so vanishing of this pullback is sufficient as well as necessary.

Suppose now that a smooth open six-dimensional region were a [fiber bundle](../../../fiber-bundle.md) with [Lagrangian submanifolds](../../../symplectic-geometry.md#lagrangian-submanifold) diffeomorphic to $S^3$ as its fibres. Fix one compact fibre $L$. Smooth local triviality and [compactness](../../../topology.md#compact-space) imply that the other sufficiently nearby fibres are $C^1$-close embeddings of $L$. In the [Weinstein neighborhood](../../../symplectic-geometry.md#weinstein-neighborhood-theorem), projection to $L$ restricts on each such fibre to a [local diffeomorphism](../../../calculus.md#local-diffeomorphism) close to the identity. It has degree one, and [compactness](../../../topology.md#compact-space) makes it a [covering map](../../../algebraic-topology.md#covering-space), so it is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism). Each nearby fibre is therefore a graph of a [closed differential one-form](../../../differential-form.md#closed-differential-one-form) $\alpha$ on $S^3$. Since $H^1(S^3;\mathbb R)=0$, this is $df$ for a smooth real function $f$. A maximum of $f$ exists by [compactness](../../../topology.md#compact-space), and there $df=0$. The graph meets the original [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle), contradicting disjointness of different fibres. **No such Lagrangian three-sphere fibration exists.** More generally this is the [compact first-cohomology obstruction to a Lagrangian fibration](../../../symplectic-geometry.md#compact-first-cohomology-obstruction-to-a-lagrangian-fibration).

## 3

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Fix the sign convention $\iota_{\xi_M}\omega=-d\mu^\xi$, where $\xi_M$ is the [fundamental vector field](../../../lie-theory.md#fundamental-vector-field) and $\mu^\xi=\langle\mu,\xi\rangle$. A [Hamiltonian group action](../../../symplectic-geometry.md#hamiltonian-group-action) is a symplectic [Lie group action](../../../lie-theory.md#lie-group-action) together with an equivariant [moment map](../../../symplectic-geometry.md#moment-map) $\mu:M\to\mathfrak g^*$ satisfying this identity for every $\xi\in\mathfrak g$. Equivariance means $\mu(gx)=\operatorname{Ad}_{g^{-1}}^*\mu(x)$. Merely requiring each fundamental field to have some Hamiltonian is the weaker condition of a [weakly Hamiltonian action](../../../symplectic-geometry.md#weakly-hamiltonian-action).

For a [circle group](../../../lie-theory.md#circle-group) action, identify its Lie algebra with $\mathbb R$, and let $Y$ generate the action. Put $Z=\mu^{-1}(t)$ and let $i:Z\hookrightarrow M$. Since $t$ is a [regular value](../../../differential-geometry.md#regular-value),

$$
T_xZ=\ker d\mu_x=\{v:\omega(Y_x,v)=0\}.
$$

The action is free, so $Y_x\ne0$. The [symplectic orthogonal complement](../../../linear-algebra.md#symplectic-orthogonal-complement) of this hyperplane is exactly $\mathbb RY_x$, which is contained in $T_xZ$. Thus

$$
\ker(i^*\omega)_x=\mathbb RY_x.
$$

The free action of the compact [circle group](../../../lie-theory.md#circle-group) is proper, and the quotient $Q=Z/S^1$ is a [smooth manifold](../../../differential-geometry.md#smooth-manifold) with projection $\pi:Z\to Q$ a [principal bundle](../../../fiber-bundle.md#principal-bundle). The form $i^*\omega$ is invariant and kills the orbit directions, hence is basic and descends to a unique two-form $\omega_Q$ satisfying $\pi^*\omega_Q=i^*\omega$. It is closed because pullback by a [submersion](../../../differential-geometry.md#submersion) detects [differential forms](../../../differential-form.md). If a quotient tangent vector annihilates $\omega_Q$, a lift lies in the displayed [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and hence projects to zero. Therefore $\omega_Q$ is nondegenerate. This proves [symplectic reduction](../../../symplectic-geometry.md#symplectic-reduction) directly.

If $L\subset Q$ is a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold), its inverse image $\widetilde L=\pi^{-1}(L)$ is a smooth [circle bundle](../../../fiber-bundle.md#circle-bundle) over $L$. The restricted [symplectic form](../../../symplectic-geometry.md#symplectic-form) is $\pi^*(\omega_Q|_L)=0$. If $\dim M=2N$, then $\dim Q=2N-2$, $\dim L=N-1$, and $\dim\widetilde L=N$, proving that $\widetilde L$ is Lagrangian. This is the [Lagrangian lift through circle reduction](../../../symplectic-geometry.md#lagrangian-lift-through-circle-reduction).

For scalar multiplication on $\mathbb C^{n+1}$, the generator is $Y=\sum_j(-y_j\partial_{x_j}+x_j\partial_{y_j})$. Direct contraction gives

$$
\iota_Y\omega_{st}=-\sum_j(x_jdx_j+y_jdy_j),\qquad\boxed{\mu(z)=\tfrac12|z|^2.}
$$

Choose $t>0$. Its level is the sphere of radius $R=\sqrt{2t}$ and its quotient is $\mathbb{CP}^n$. [Complex conjugation](../../../complex-analysis.md#complex-conjugation) on the sphere reverses the ambient [symplectic form](../../../symplectic-geometry.md#symplectic-form) and descends to an [anti-symplectic involution](../../../symplectic-geometry.md#anti-symplectic-involution) of the quotient. Its fixed set is $\mathbb{RP}^n$: a projective point fixed by conjugation has a real representative after a phase change. For two tangent vectors to this fixed set, anti-symplecticity makes the reduced form equal to its negative, so it vanishes. The real dimension is $n$, half the quotient dimension, proving the [Lagrangian fixed locus of an anti-symplectic involution](../../../symplectic-geometry.md#lagrangian-fixed-locus-of-an-anti-symplectic-involution) property.

The lifted [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) can be written explicitly as

$$
\boxed{\widetilde L=\{e^{i\theta}x:x\in\mathbb R^{n+1},\ |x|=R\}
\cong(S^n\times S^1)/((x,\zeta)\sim(-x,-\zeta)).}
$$

The only redundancy in this parametrization is the displayed free involution: two nonzero real representatives on the same complex ray differ by a real sign. The quotient embeds smoothly in the sphere, and projection to $[x]\in\mathbb{RP}^n$ exhibits its [circle bundle](../../../fiber-bundle.md#circle-bundle) structure. Its Lagrangian property follows from the reduction argument, including the case $n=0$.

## 4

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

**False.** Give $E=TS^2\to S^2$ a fibrewise area form. This is a rank-two [symplectic vector bundle](../../../fiber-bundle.md#symplectic-vector-bundle). A [Lagrangian subbundle](../../../fiber-bundle.md#lagrangian-subbundle) would be a real line subbundle $L\subset TS^2$. Real [line bundles](../../../ringed-space.md#line-bundle) are classified by their first [Stiefel–Whitney class](../../../fiber-bundle.md#stiefel-whitney-class) in $H^1(B;\mathbb Z/2)$; since this group vanishes for $S^2$, $L$ would be trivial. A nonzero section of $L$ would therefore be a nowhere-vanishing tangent [vector field](../../../calculus.md#vector-field) on $S^2$. The [Hairy ball theorem](../../../fiber-bundle.md#hairy-ball-theorem) rules this out: every continuous tangent [vector field](../../../calculus.md#vector-field) on an even-dimensional sphere has a zero. Hence $TS^2$ does not even have one [Lagrangian subbundle](../../../fiber-bundle.md#lagrangian-subbundle), let alone a splitting into two. Fibrewise existence of [Lagrangian subspaces](../../../symplectic-geometry.md#lagrangian-subspace) does not guarantee a globally continuous choice.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

**True.** Use the normalization in which the blowup weight $\lambda$ is the area of an exceptional projective line, equivalently the capacity $\pi r^2$ of the ball removed. The auxiliary volume formula for a point [symplectic blowup](../../../symplectic-geometry.md#symplectic-blowup) in real dimension $2n$ is

$$
\int_{\widetilde X}\frac{\widetilde\omega^n}{n!}
=\int_X\frac{\omega^n}{n!}-\frac{\lambda^n}{n!}.
$$

It applies to each successive blowup, irrespective of where the point is chosen. Geometrically the removed standard ball has volume $\pi^nr^{2n}/n!$, while its replacement divisor has zero $2n$-dimensional volume. If $V$ is the original [symplectic volume](../../../symplectic-geometry.md#symplectic-volume), after $k$ equal-weight blowups the volume is $V-k\lambda^n/n!$. A nonempty closed [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) has strictly positive volume, so

$$
\boxed{k<\frac{n!V}{\lambda^n}.}
$$

This finite upper bound suffices; it does not assert that every number below the bound is realizable. A convention taking the weight to be the radius instead changes the fixed decrement to $\pi^n\lambda^{2n}/n!$, with the same conclusion.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

**False even when both base and fibre are closed and oriented.** Take the [Hopf fibration](../../../algebraic-topology.md#hopf-fibration) $h:S^3\to S^2$, and define the smooth [fiber bundle](../../../fiber-bundle.md) $p:S^3\times S^1\to S^2$ by $p(x,\theta)=h(x)$. Its local trivializations are the Hopf trivializations times $S^1$, and its fibre is $S^1\times S^1=T^2$.

The [Künneth theorem](../../../cohomology.md#kunneth-theorem) for [cohomology](../../../cohomology.md) over a field says $H^k(A\times B;\mathbb R)=\bigoplus_{i+j=k}H^i(A;\mathbb R)\otimes H^j(B;\mathbb R)$ for these compact manifolds. Here it gives $H^2(S^3\times S^1;\mathbb R)=0$. If a [symplectic form](../../../symplectic-geometry.md#symplectic-form) $\omega$ existed on this closed four-manifold, it would be exact, $\omega=d\eta$. Since $d\omega=0$,

$$
\int_{S^3\times S^1}\omega\wedge\omega
=\int_{S^3\times S^1}d(\eta\wedge\omega)=0
$$

by [Stokes theorem](../../../calculus.md#stokes-theorem). But $\omega^2$ is a positive volume form in the [symplectic orientation](../../../symplectic-geometry.md#symplectic-orientation), so its integral is positive. This contradiction proves the claim fails. The mere bundle structure does not ensure that a fibrewise area class extends to the total space.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

**True for a smooth complex projective surface**, the usual manifold convention in this question. Choose an [ample divisor](../../../cartier-divisor.md#ample-cartier-divisor) $H$. The auxiliary pencil-existence theorem states that, for all sufficiently large $m$, a general two-dimensional space of sections of $\mathcal O_X(mH)$ defines a [Lefschetz pencil](../../../symplectic-geometry.md#lefschetz-pencil): its base points are transverse and finite, its general fibre is a smooth connected curve, and each singular fibre has exactly one ordinary node, with distinct critical values. High powers separate the required jets, so a generic pencil has precisely these singularities.

Choose such an $m$ divisible by four, and write $D=mH$. The [adjunction formula](../../../complex-geometry.md#adjunction-formula) for a smooth connected curve of class $D$ on a smooth projective surface is $2g-2=D\cdot(D+K_X)$. Consequently

$$
g=1+\frac{m^2H^2+mK_X\cdot H}{2}.
$$

Writing $m=4\ell$ gives $g=1+8\ell^2H^2+2\ell K_X\cdot H$, an odd integer. Thus **a sufficiently positive four-divisible polarization gives an odd-genus [Lefschetz pencil](../../../symplectic-geometry.md#lefschetz-pencil)**. The surface is taken to be smooth; a singular projective variety need not support a [Lefschetz pencil](../../../symplectic-geometry.md#lefschetz-pencil) in this smooth-manifold sense.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

**True.** The [Künneth theorem](../../../cohomology.md#kunneth-theorem) gives the [Poincaré polynomial](../../../homology.md#poincare-polynomial)

$$
P_{S^4\times T^4}(t)=(1+t^4)(1+t)^4,
$$

so $b_2=6$ and $b_4=2$. The proposed equality also gives $b_0=b_8=1$. Even if [compactness](../../../topology.md#compact-space) was not stated separately, these two numbers force the putative eight-manifold to be connected and compact: the top ordinary real [cohomology](../../../cohomology.md) of a connected noncompact manifold is zero.

The auxiliary [Hard Lefschetz theorem on de Rham cohomology](../../../complex-geometry.md#hard-lefschetz-theorem-on-de-rham-cohomology) says that, on a compact [Kähler manifold](../../../complex-geometry.md#kahler-manifold) of complex dimension $n$, $L^{n-k}:H^k\to H^{2n-k}$ is an [isomorphism](../../../algebra.md#isomorphism), where $L\alpha=[\omega]\smile\alpha$. Here $n=4$, so $L^2:H^2\to H^6$ is [injective](../../../algebra.md#injective-function). If $L\alpha=0$, then $L^2\alpha=0$ and therefore $\alpha=0$. Thus $L:H^2\to H^4$ is [injective](../../../algebra.md#injective-function), forcing $b_2\leq b_4$. The inequality $6\leq2$ is impossible. Hence **these [Betti numbers](../../../homology.md#betti-number) cannot occur for a Kähler eight-manifold**.

## 5

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure) is a smooth endomorphism $J:TX\to TX$ satisfying $J^2=-I$, preserving $\omega$, and making $g_J(u,v)=\omega(u,Jv)$ a positive-definite [inner product](../../../linear-algebra.md#inner-product). Preservation and $J^2=-I$ make this [bilinear form](../../../linear-algebra.md#bilinear-form) symmetric.

To construct one, choose any [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $h$ and define $A$ by $h(Au,v)=\omega(u,v)$. The endomorphism $A$ is skew-adjoint and invertible. Consequently $-A^2$ is positive definite and self-adjoint. Let $B=(-A^2)^{1/2}$ be its positive square root and set

$$
\boxed{J=B^{-1}A.}
$$

The [spectral theorem](../../../hilbert-space.md#spectral-theorem) gives $B$ fibrewise, and the positive-square-root operation is smooth on positive-definite matrices, so this defines a smooth endomorphism. Since $A$ commutes with $B$, $J^2=-I$. Also $J^*=-J$, so $J^*J=I$. Commutation then gives

$$
\omega(Ju,Jv)=h(AJu,Jv)=h(Au,v)=\omega(u,v),\qquad
\omega(u,Ju)=h(Bu,u)>0\quad(u\ne0).
$$

This is the [metric construction of a compatible almost complex structure](../../../complex-geometry.md#metric-construction-of-a-compatible-almost-complex-structure), proving nonemptiness.

If we start with $h=g_J$ for an already compatible $J$, then $h(Ju,v)=\omega(u,v)$, so $A=J$, $B=I$, and the construction recovers $J$. For two compatible structures, linearly interpolate their metrics,

$$
h_t=(1-t)g_{J_0}+t g_{J_1},\qquad0\leq t\leq1,
$$

and apply the construction to $h_t$. This is a continuous smooth-in-$t$ path with endpoints $J_0,J_1$. Thus **the space is nonempty and path connected**. Interpolating instead to a single fixed auxiliary metric actually gives the [contractibility of compatible almost complex structures](../../../complex-geometry.md#contractibility-of-compatible-almost-complex-structures).

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Let $\lambda=\tfrac12\sum_j(x_jdy_j-y_jdx_j)$ on $\mathbb C^3$, so $d\lambda=\omega_{st}$. On a projective line, work in the affine coordinate $w=\rho e^{i\theta}$ and lift it to the unit three-sphere by

$$
s(w)=\frac{(w,1)}{\sqrt{1+|w|^2}}.
$$

This sphere lies in a complex two-plane in $\mathbb C^3$. The defining reduction identity for the [Fubini-Study form](../../../complex-geometry.md#fubini-study-form) gives $\Omega=s^*\omega_{st}$ on this chart. Differentiating the lift, or using the fact that real radial rescaling contributes no imaginary part to $\bar z\,dz$, gives

$$
s^*\lambda=\frac12\frac{\rho^2}{1+\rho^2}\,d\theta,
\qquad
\Omega=\frac{\rho}{(1+\rho^2)^2}\,d\rho\wedge d\theta.
$$

The missing point at infinity has zero area, so

$$
\boxed{\int_H\Omega=2\pi\int_0^\infty\frac{\rho\,d\rho}{(1+\rho^2)^2}=\pi.}
$$

This normalization is important: it differs from conventions in which a projective line has area $1$ or $2\pi$.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Define

$$
F:B^4(1)\longrightarrow\mathbb{CP}^2\setminus\{z_3=0\},\qquad
F(w_1,w_2)=[w_1:w_2:\sqrt{1-|w|^2}].
$$

Every projective point with $z_3\ne0$ has a unique unit representative whose third coordinate is positive real, so $F$ is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism). More explicitly, in the affine coordinate $u=(z_1/z_3,z_2/z_3)$ its inverse is $w=u/\sqrt{1+|u|^2}$. Lift $F$ to the unit sphere by $\widetilde F(w)=(w,\sqrt{1-|w|^2})$. The last coordinate is real, so its contribution $dx_3\wedge dy_3$ pulls back to zero. The reduction identity therefore yields

$$
\boxed{F^*\Omega=\widetilde F^*\omega_{st}=\omega_{st}|_{\mathbb C^2}.}
$$

This proves the [symplectic ball chart in complex projective space](../../../complex-geometry.md#symplectic-ball-chart-in-complex-projective-space) directly, including the precise unit radius.

For the final unheaded request, embed the two disjoint balls in this chart. Fix arbitrary $0<\rho_i<r_i$, and choose intermediate radii $\rho_i<\rho_i'<r_i$. On the images of the balls of radius $\rho_i'$, transport the standard [complex structure](../../../complex-geometry.md#complex-structure) by the given [symplectic embeddings](../../../symplectic-geometry.md#symplectic-embedding). It is compatible with $\Omega$. Their smaller closed neighborhoods are compact and disjoint. Choose a global [Riemannian metric](../../../differential-geometry.md#riemannian-metric) agreeing there with the associated compatible metrics, using a [partition of unity](../../../differential-geometry.md#partition-of-unity) outside these neighborhoods, and apply the metric construction. The resulting global [compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure) $J$ agrees with the transported standard structure on each ball of radius $\rho_i$ and on a slightly larger neighborhood. This extends metrics, rather than averaging [almost complex structures](../../../complex-geometry.md#almost-complex-manifold).

Let $p_1,p_2$ be the centres. They are distinct. The degree-one [J-holomorphic curve](../../../symplectic-geometry.md#pseudoholomorphic-curve) supplied in the question has total area $\pi$, because its [homology class](../../../homology.md#homology-class) is the projective line class. We use the sharp Euclidean version of the [Monotonicity theorem for a J-holomorphic curve](../../../symplectic-geometry.md#monotonicity-theorem-for-a-j-holomorphic-curve): a nonconstant holomorphic curve through the centre of a standard complex ball, with no boundary in the ball and counted with its parametrization multiplicities, has area in the radius-$\rho$ ball at least $\pi\rho^2$. This includes branched points: their density is a positive integer $m$, and the stronger lower bound is $m\pi\rho^2$. One way to see the constant is that complex curves are calibrated [minimal surfaces](../../../second-fundamental-form.md#minimal-surface); their stationary area ratio $\operatorname{area}(C\cap B(\rho))/\rho^2$ is nondecreasing and its limit at the centre is $m\pi$.

The closed degree-one curve cannot stay entirely inside either chart ball: there the form is exact, so [Stokes theorem](../../../calculus.md#stokes-theorem) would give zero total area, contradicting its positive area. Thus the branch through each centre crosses the surrounding spheres, and the stated monotonicity bound applies to each restriction. The two ball images are disjoint, so their area contributions add without overlap. It follows that

$$
\pi\rho_1^2+\pi\rho_2^2\leq\int_C\Omega=\pi.
$$

Letting both smaller radii increase to their original radii gives

$$
\boxed{r_1^2+r_2^2\leq1.}
$$

This [two-ball packing obstruction in the projective plane](../../../complex-geometry.md#two-ball-packing-obstruction-in-the-projective-plane) is sharper than volume alone: a volume comparison would only give $r_1^4+r_2^4\leq1$.

## 6

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [J-holomorphic curve](../../../symplectic-geometry.md#pseudoholomorphic-curve) is a map $u:(\Sigma,j)\to(X,J)$ from a [Riemann surface](../../../complex-analysis.md#riemann-surfaces) satisfying $du\circ j=J\circ du$. The target [almost complex structure](../../../complex-geometry.md#almost-complex-manifold) need not be integrable; the equation still behaves like a nonlinear elliptic version of complex analysis. On a [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) it is particularly effective when $J$ is compatible with $\omega$, because complex analysis then controls [symplectic area](../../../symplectic-geometry.md#symplectic-area). The metric construction above supplies such structures and deformations between them.

In conformal coordinates $(s,t)$ with $j\partial_s=\partial_t$, the equation is $u_t=Ju_s$. With $g=\omega(\cdot,J\cdot)$, an arbitrary map satisfies

$$
\frac12(|u_s|^2+|u_t|^2)
=\omega(u_s,u_t)+\frac12|u_t-Ju_s|^2.
$$

This follows by expanding the last square and using $g(Ju_s,u_t)=\omega(u_s,u_t)$. Integrating proves the [Energy identity for a J-holomorphic curve](../../../symplectic-geometry.md#energy-identity-for-a-j-holomorphic-curve). In particular,

$$
E(u)=\int_\Sigma u^*\omega
$$

for a [J-holomorphic curve](../../../symplectic-geometry.md#pseudoholomorphic-curve), and its energy depends only on its [homology class](../../../homology.md#homology-class) when the domain is closed. A nonconstant such curve has strictly positive area: its derivative is nonzero somewhere and positivity holds on a neighborhood. It also minimizes energy among maps in the same [homology class](../../../homology.md#homology-class) with the same domain [conformal structure](../../../geometry-and-topology.md#conformal-structure). Thus analytic bounds can be obtained from topological information.

The equation is the zero set of the [Cauchy–Riemann operator](../../../symplectic-geometry.md#cauchy-riemann-operator) $\bar\partial_Ju=\tfrac12(du+J\circ du\circ j)$. Linearization at a solution, with respect to a connection, has the form

$$
D_u\xi=\tfrac12\bigl(\nabla\xi+J\nabla\xi\circ j+(\nabla_\xi J)du\circ j\bigr).
$$

The last term has differential order zero. The principal part has the Cauchy–Riemann symbol; in a complex frame a nonzero real covector $(a,b)$ gives multiplication by $a+ib$, an invertible symbol. This establishes ellipticity. On a closed domain the resulting operator between suitable [Sobolev spaces](../../../sobolev-space.md) is a [Fredholm operator](../../../functional-analysis.md#fredholm-operator). The [Riemann-Roch index for a real Cauchy-Riemann operator](../../../symplectic-geometry.md#riemann-roch-index-for-a-real-cauchy-riemann-operator) is $2n(1-g)+2c_1(A)$ for a fixed genus-$g$ domain, where $2n=\dim X$ and $A=u_*[\Sigma]$. For spheres, removing the six real dimensions of domain reparametrization gives

$$
\dim\mathcal M_A=2n+2c_1(A)-6,
$$

provided the curve is simple and regular. Each marked point adds two real dimensions; constraining its image to a specified target point removes $2n$. These are the [dimension formula for regular J-holomorphic spheres](../../../symplectic-geometry.md#dimension-formula-for-regular-j-holomorphic-spheres) and its incidence version.

Here regular means that $D_u$ is [surjective](../../../algebra.md#surjective-function). Then the [implicit function theorem](../../../calculus.md#implicit-function-theorem) makes the [moduli space](../../../geometry-and-topology.md#moduli-space) locally smooth of this index. The [generic transversality for simple holomorphic spheres](../../../symplectic-geometry.md#generic-transversality-for-simple-holomorphic-spheres) theorem asserts that a residual set of smooth compatible $J$ makes all simple spheres in specified countably many classes regular, and that generic incidence constraints and generic one-parameter deformations are transverse. It does not assert regularity for all multiple covers. This distinction matters whenever one tries to count curves. A primitive class with no positive-area spherical decomposition avoids multiple-cover and bubbling difficulties and permits especially direct counts.

The other central ingredient is [Gromov compactness for spheres](../../../symplectic-geometry.md#gromov-compactness-for-spheres). On a compact symplectic target, a sequence of holomorphic spheres with uniformly bounded area and smoothly converging tame [almost complex structures](../../../complex-geometry.md#almost-complex-manifold) has a subsequence converging to a finite bubble tree, smoothly away from finitely many domain points after reparametrizations. The areas and [homology classes](../../../homology.md#homology-class) of the nonconstant components add to those of the original maps; constant components account for stable marked configurations. This is [compactness](../../../topology.md#compact-space) of stable maps, not ordinary smooth [compactness](../../../topology.md#compact-space) of the original parametrizations.

The proof mechanism explains why bubbling is indispensable. An elliptic small-energy estimate bounds derivatives on a smaller disc when the energy on a larger disc is sufficiently small. Failure of a derivative bound therefore concentrates a definite amount of energy. Rescale near a point of large derivative; elliptic estimates yield a nonconstant limiting holomorphic map on the plane. Its finite energy allows the point at infinity to be filled in by the [removal of a finite-energy holomorphic puncture](../../../symplectic-geometry.md#removal-of-a-finite-energy-holomorphic-puncture) theorem, producing a sphere. Repeating extracts further spheres. Uniform local monotonicity gives a positive energy threshold for nonconstant bubbles on the compact target, so only finitely many can occur. Estimates on the intervening annuli yield the energy identity and exclude lost neck energy. These statements give the analytic content behind the [compactness](../../../topology.md#compact-space) theorem, while identifying the exact place where a smooth limit alone fails.

A local area estimate turns this existence theory into an embedding obstruction. In a standard complex ball, holomorphic curves are calibrated by the standard [symplectic form](../../../symplectic-geometry.md#symplectic-form), so their parametrized [symplectic area](../../../symplectic-geometry.md#symplectic-area) is their Riemannian area. They are stationary [minimal surfaces](../../../second-fundamental-form.md#minimal-surface). The minimal-surface monotonicity formula says that $\operatorname{area}(C\cap B(\rho))/\rho^2$ is nondecreasing wherever the curve has no boundary in the ball. At a point of multiplicity $m$, its limiting density is $m\pi$. Consequently any branch through the centre contributes at least $\pi\rho^2$. For a general compatible $J$ there is still a local lower bound $c\rho^2$, with $c>0$ depending on controlled geometry. The exact Euclidean constant is the one needed for sharp radius obstructions.

Here is a global existence argument that feeds this estimate. Put

$$
Y=S^2(a)\times T^{2n-2},\qquad F=[S^2\times\{q\}],
$$

with the product [symplectic form](../../../symplectic-geometry.md#symplectic-form), sphere area $a$, and a constant [symplectic form](../../../symplectic-geometry.md#symplectic-form) on the [torus](../../../topology.md#torus). Since the [torus](../../../topology.md#torus) has zero second [homotopy group](../../../algebraic-topology.md#homotopy-group), every spherical class is $kF$ for an integer $k$. A nonconstant holomorphic sphere in this class has area $ka>0$, so $k\geq1$. A curve of class $F$ cannot split into two nonconstant bubbles, and it cannot be a nontrivial multiple cover. This supplies the [compactness](../../../topology.md#compact-space) required for [fibre spheres in a sphere-torus product](../../../symplectic-geometry.md#fibre-spheres-in-a-sphere-torus-product).

For the product [complex structure](../../../complex-geometry.md#complex-structure), every sphere of class $F$ has constant [torus](../../../topology.md#torus) projection: it lifts to a holomorphic map from the sphere to $\mathbb C^{n-1}$, whose coordinates are constant. Its sphere projection has degree one. Thus, up to reparametrization, there is exactly one such sphere through every target point. It is regular because its pulled-back [tangent bundle](../../../fiber-bundle.md#tangent-bundle) is $\mathcal O(2)\oplus\mathcal O^{n-1}$ on $\mathbb{CP}^1$, and the first [cohomology](../../../cohomology.md) of each summand vanishes. Its linearized [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator) therefore has zero [cokernel](../../../linear-algebra.md#cokernel).

Since $c_1(F)=2$, the [moduli space](../../../geometry-and-topology.md#moduli-space) with one marked point has expected real dimension $2n$. Imposing passage through a fixed point gives dimension zero. For generic structures and transverse incidence conditions this is a finite set. Along a generic path of structures its one-point solutions form a compact one-dimensional cobordism: [compactness](../../../topology.md#compact-space) holds because splitting and multiple covers were excluded. Its boundary contains the endpoint solutions. A compact one-manifold has an even number of boundary points, so the count modulo two is unchanged. The product count is one, and hence the count for a generic compatible $J$ is one as well. If the endpoint product structure is not generic for other classes, its regular solutions allow the path argument in this single class. Approximating an arbitrary compatible $J$ by generic structures and applying [compactness](../../../topology.md#compact-space) supplies a limiting sphere of class $F$ through the prescribed point. The nonconstant component still contains that point; there are no nonconstant bubbles to carry it away. This derives the existence assertion needed below without assuming a capacity obstruction.

Now suppose a [symplectic embedding](../../../symplectic-geometry.md#symplectic-embedding) sends $B^{2n}(r)$ into the [symplectic cylinder](../../../symplectic-geometry.md#symplectic-cylinder) $B^2(R)\times\mathbb R^{2n-2}$. Choose $0<\rho<\rho'<r$. The image of the closed radius-$\rho'$ ball is compact. For any $a>\pi R^2$, the first factor embeds symplectically into an area-$a$ sphere: in dimension two this is an area-preserving disc chart, leaving a cap of area $a-\pi R^2$. Enclose the remaining compact coordinate projection in a sufficiently large rectangular fundamental domain of a symplectic [torus](../../../topology.md#torus). The compact ball image thereby embeds into $S^2(a)\times T^{2n-2}$.

Choose a compatible $J$ agreeing with the transported standard [complex structure](../../../complex-geometry.md#complex-structure) near the radius-$\rho$ ball, by extending its associated metric and applying the polar construction. The sphere of class $F$ through the centre has area $a$. It cannot be contained in the ball image, where the [symplectic form](../../../symplectic-geometry.md#symplectic-form) is exact. Euclidean monotonicity therefore gives $a\geq\pi\rho^2$. The choices of $a>\pi R^2$ and $\rho<r$ were arbitrary, so

$$
\boxed{B^{2n}(r)\hookrightarrow B^2(R)\times\mathbb R^{2n-2}\text{ symplectically}\quad\Longrightarrow\quad r\leq R.}
$$

For $n=1$ the same conclusion is simply area comparison; for $n\geq2$ the cylinder has infinite volume, so this proof detects a restriction that volume misses. This is the [Gromov non-squeezing theorem](../../../symplectic-geometry.md#non-squeezing-theorem), derived from the curve existence and sharp area estimates above.

The associated [Gromov width](../../../symplectic-geometry.md#gromov-width) is

$$
c_G(U,\omega)=\sup\{\pi r^2:B^{2n}(r)\text{ admits a symplectic embedding into }(U,\omega)\}.
$$

Composition of embeddings proves monotonicity. Rescaling coordinates in a ball proves $c_G(U,c\omega)=c\,c_G(U,\omega)$ for $c>0$. Non-squeezing, together with the evident inclusions, gives

$$
\boxed{c_G(B^{2n}(R))=c_G(B^2(R)\times\mathbb R^{2n-2})=\pi R^2.}
$$

These are the normalization, monotonicity and conformality properties of a [symplectic capacity](../../../symplectic-geometry.md#symplectic-capacity). The two-ball obstruction of Question 5 illustrates a related use: one degree-one curve through two prescribed centres gives an additive area bound, stronger than comparing the volumes of the balls. The common method is to arrange standard complex geometry in the region one wants to measure, obtain a global holomorphic curve by deformation and [compactness](../../../topology.md#compact-space), and compare its globally fixed area with local monotonicity lower bounds.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
