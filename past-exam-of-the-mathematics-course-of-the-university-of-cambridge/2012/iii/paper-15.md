# Paper 15

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_15.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_15.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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

## 1

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle) coordinates $(q^1,\ldots,q^n,p_1,\ldots,p_n)$, the [Liouville one-form](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) and the canonical [symplectic form](../../../symplectic-geometry.md#symplectic-form) are

$$
\alpha=\sum_i p_i\,dq^i,\qquad
\omega=-d\alpha=\sum_i dq^i\wedge dp_i.
$$

The [twisted cotangent symplectic form](../../../symplectic-geometry.md#twisted-cotangent-symplectic-form) is closed: [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) commutes with the [exterior derivative](../../../differential-form.md#exterior-derivative), so

$$
d\omega_\sigma=d\omega+\pi^*(d\sigma)=0.
$$

To prove the form is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form), write a tangent vector in these coordinates as $(u,v)$ and test its pairing with an arbitrary vertical vector $(0,w)$. The base [differential two-form](../../../differential-form.md#2-form) has zero pairing with vertical vectors, hence

$$
\omega_\sigma((u,v),(0,w))=u^iw_i.
$$

A vector in the [kernel of a linear map](../../../linear-algebra.md#kernel-of-a-linear-map) therefore has $u=0$. Pairing it next with every $(z,0)$ gives $-z^iv_i=0$, so $v=0$. Thus the kernel is zero at every point, independently of the size or rank of $\sigma$. Together with closedness, this proves **$\omega_\sigma$ is a [symplectic form](../../../symplectic-geometry.md#symplectic-form)**. The argument is local only for convenience; the [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) property is intrinsic and the coordinate charts cover the whole [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [differential one-form](../../../differential-form.md#one-form) $\theta$ defines a smooth [section of a vector bundle](../../../fiber-bundle.md#section-of-a-vector-bundle), and its [one-form graph](../../../symplectic-geometry.md#graph-of-a-differential-one-form) is an embedded copy of $X$ because $\pi\circ\theta=\operatorname{id}_X$. The defining property of the [Liouville one-form](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) gives $\theta^*\alpha=\theta$. Consequently

$$
\theta^*\omega_\sigma=-d\theta+(\pi\circ\theta)^*\sigma=\sigma-d\theta.
$$

The [one-form graph](../../../symplectic-geometry.md#graph-of-a-differential-one-form) has dimension $n$, half the dimension of the [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle). It is therefore a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) precisely when this [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) vanishes:

$$
\boxed{\theta(X)\text{ is Lagrangian in }(T^*X,\omega_\sigma)
\quad\Longleftrightarrow\quad d\theta=\sigma.}
$$

This is the [twisted Lagrangian graph criterion](../../../symplectic-geometry.md#twisted-lagrangian-graph-criterion).

Now suppose the projection restricts to a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) on a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) $L$. Its inverse followed by the inclusion defines a smooth section $s:X\to T^*X$, hence a global [differential one-form](../../../differential-form.md#one-form) $\theta$ with image $L$. The criterion forces $\sigma=d\theta$, so its class in [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) is zero. Thus **$[\sigma]\ne0$ rules out every such Lagrangian section**. This [cohomological obstruction to a Lagrangian section](../../../symplectic-geometry.md#cohomological-obstruction-to-a-lagrangian-section) concerns graphs over the entire base; it does not claim that all [Lagrangian submanifolds](../../../symplectic-geometry.md#lagrangian-submanifold) are absent.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**Yes.** Choose a global [differential one-form](../../../differential-form.md#one-form) $\beta$ with $d\beta=\sigma$, and use the [cotangent fiber translation](../../../symplectic-geometry.md#cotangent-fiber-translation)

$$
T_\beta(q,p)=(q,p+\beta_q).
$$

It is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) with inverse $T_{-\beta}$, and $\pi\circ T_\beta=\pi$. Directly from the [Liouville one-form](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle),

$$
T_\beta^*\alpha=\alpha+\pi^*\beta.
$$

The sign convention $\omega=-d\alpha$ therefore gives

$$
\boxed{T_\beta^*\omega_\sigma
=\omega-\pi^*(d\beta)+\pi^*\sigma=\omega.}
$$

Thus $T_\beta:(T^*X,\omega)\to(T^*X,\omega_\sigma)$ is the required [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism). Equivalently, $T_{-\beta}^*\omega=\omega_\sigma$ gives the inverse direction. This [translation equivalence of exact twisted cotangent bundles](../../../symplectic-geometry.md#translation-equivalence-of-exact-twisted-cotangent-bundles) is global even when $X$ is not compact; no completeness argument for a [Moser theorem](../../../symplectic-geometry.md#moser-s-trick) flow is needed.

## 2

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Put $\xi_t=\ker\alpha_t$, the [contact distribution](../../../differential-geometry.md#contact-distribution). If $\dim M=2r+1$, the [contact form](../../../differential-geometry.md#contact-form) condition is $\alpha_t\wedge(d\alpha_t)^r\ne0$. It implies that $d\alpha_t|_{\xi_t}$ is a [symplectic form](../../../symplectic-geometry.md#symplectic-form) on each contact hyperplane: inserting a vector transverse to $\xi_t$ in that volume form leaves the nonzero top exterior power $(d\alpha_t|_{\xi_t})^r$. Hence there is a unique smooth [time-dependent vector field](../../../calculus.md#time-dependent-vector-field) $Y_t\in\xi_t$ satisfying

$$
(\iota_{Y_t}d\alpha_t)|_{\xi_t}=-\dot\alpha_t|_{\xi_t}.
$$

Its smoothness follows by inverting the smoothly varying [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) matrix of this [contact distribution symplectic form](../../../differential-geometry.md#contact-distribution-symplectic-form). This is the [horizontal generator of contact stability](../../../differential-geometry.md#horizontal-generator-of-contact-stability).

Let $R_t$ be the [Reeb vector field](../../../differential-geometry.md#reeb-vector-field) of $\alpha_t$. The one-form $\dot\alpha_t+\iota_{Y_t}d\alpha_t$ vanishes on $\xi_t$, so it is $h_t\alpha_t$. Evaluating on $R_t$, using $\alpha_t(R_t)=1$ and $\iota_{R_t}d\alpha_t=0$, identifies the coefficient:

$$
h_t=\dot\alpha_t(R_t),\qquad
\dot\alpha_t+\iota_{Y_t}d\alpha_t=h_t\alpha_t.
$$

By [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula), the [Lie derivative of a differential form](../../../differential-form.md#lie-derivative-of-a-differential-form) is

$$
\mathcal L_{Y_t}\alpha_t=\iota_{Y_t}d\alpha_t+d(\alpha_t(Y_t))
=\iota_{Y_t}d\alpha_t,
$$

because $Y_t$ lies in the contact hyperplane.

Let $\rho_t$ solve $\partial_t\rho_t=Y_t\circ\rho_t$, with $\rho_0=\operatorname{id}_M$. Since $M$ is compact without boundary and $Y_t$ is smooth on the closed time interval, its solutions cannot escape and exist for the entire interval. Reversing the time-dependent equation supplies a smooth inverse for each $\rho_t$. Thus these [flow maps](../../../dynamical-systems.md#flow-map) give a [smooth isotopy](../../../differential-geometry.md#smooth-isotopy). Differentiating the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) along this isotopy yields

$$
\frac d{dt}(\rho_t^*\alpha_t)
=\rho_t^*(\dot\alpha_t+\mathcal L_{Y_t}\alpha_t)
=(h_t\circ\rho_t)\rho_t^*\alpha_t.
$$

For each base point this is a scalar linear equation for a covector, initially $\alpha_0$. Its solution is

$$
\boxed{\rho_t^*\alpha_t=u_t\alpha_0,\qquad
u_t(x)=\exp\left(\int_0^t h_s(\rho_s(x))\,ds\right)>0.}
$$

By [finite-time flow completeness on a compact manifold](../../../calculus.md#finite-time-flow-completeness-on-a-compact-manifold), this construction gives the whole time interval. The [contact conformal factor along an isotopy](../../../differential-geometry.md#contact-conformal-factor-along-an-isotopy) is smooth in $(t,x)$ and nowhere zero, proving [Gray stability theorem](../../../differential-geometry.md#gray-stability-theorem). The precise domains here are $\rho_t:M\to M$ and $\rho:M\times[0,1]\to M$; the extra time factor attached to the already indexed $\rho_t$ in the source is a notational slip. The proof produces the required family on its whole specified interval. If a parameter domain of all $\mathbb R$ is intended, extend the smooth field slightly beyond $[0,1]$, multiply it by a time cutoff, and use compactness to obtain the extended isotopy $\rho:M\times\mathbb R\to M$. Its restriction to $[0,1]$ is unchanged.

## 3

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

We prove the [Weinstein neighborhood theorem](../../../symplectic-geometry.md#weinstein-neighborhood-theorem) with the canonical sign convention $\omega_0=-d\alpha$. The essential first step is to match the two [symplectic forms](../../../symplectic-geometry.md#symplectic-form) as bilinear forms on the entire tangent space along $X$, not only after pulling them back to $TX$.

Here is the needed [symplectic splitting along a Lagrangian submanifold](../../../symplectic-geometry.md#symplectic-splitting-along-a-lagrangian-submanifold). Write $E=TM|_X$ and $L=TX$. Choose a smooth [vector bundle](../../../fiber-bundle.md#vector-bundle) complement $N$ of $L$, for example using a [Riemannian metric](../../../differential-geometry.md#riemannian-metric). Since $L$ is a [Lagrangian subspace](../../../symplectic-geometry.md#lagrangian-subspace) in every fiber, the pairing map

$$
N\longrightarrow L^*,\qquad v\longmapsto\bigl(u\longmapsto\omega(u,v)\bigr)
$$

is an isomorphism: its kernel is $N\cap L^\omega=N\cap L=0$, and both bundles have rank $n$. Let $s:L^*\to N$ be its inverse and put $b(\eta,\zeta)=\omega(s\eta,s\zeta)$. Define $a:L^*\to L$ by

$$
\zeta(a\eta)=-\tfrac12 b(\eta,\zeta),
$$

and set $\widetilde s=s+a$. Nondegeneracy of the dual pairing gives a unique smooth $a$. Since $b$ is alternating,

$$
\omega(\widetilde s\eta,\widetilde s\zeta)
=b(\eta,\zeta)-\eta(a\zeta)+\zeta(a\eta)=0.
$$

Thus $K=\widetilde s(L^*)$ is a smooth [Lagrangian complement](../../../symplectic-geometry.md#lagrangian-complement) to $L$. The map

$$
A:TX\oplus T^*X\longrightarrow TM|_X,\qquad
A(u,\eta)=u+\widetilde s\eta
$$

is a [vector bundle isomorphism](../../../fiber-bundle.md#vector-bundle-isomorphism), is the identity on $TX$, and satisfies

$$
\omega(A(u,\eta),A(v,\zeta))=\zeta(u)-\eta(v)
=\omega_0((u,\eta),(v,\zeta)).
$$

The last equality uses the canonical splitting of the tangent bundle of $T^*X$ along its [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle).

Choose a [Riemannian metric](../../../differential-geometry.md#riemannian-metric) near $X$ for which $K$ is orthogonal to $TX$. The [tubular neighborhood](../../../differential-geometry.md#tubular-neighborhood) construction using its [Riemannian exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry) gives a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism)

$$
\psi:W\subset T^*X\longrightarrow W'\subset M,\qquad
\psi(q,p)=\exp_q(\widetilde s_qp),
$$

after shrinking around the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle). It restricts to the given inclusion of $X$ and has differential $A$ along it. Consequently $\beta=\psi^*\omega$ and $\omega_0$ agree pointwise as ambient bilinear forms at every point of the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle).

We use the following precise [relative Moser theorem](../../../symplectic-geometry.md#relative-moser-theorem). If two closed [symplectic forms](../../../symplectic-geometry.md#symplectic-form) $\gamma_0,\gamma_1$ near a compact embedded submanifold $S$ agree as ambient bilinear forms along $S$, then, on smaller neighborhoods, there is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $\kappa$ fixing $S$ pointwise with $\kappa^*\gamma_1=\gamma_0$. One sufficient version allows a symplectic path $\gamma_t$ with $\partial_t\gamma_t=d\eta_t$ and $\eta_t=0$ as ambient covectors along $S$: solve $\iota_{Z_t}\gamma_t=-\eta_t$ and use its flow. The [vector field](../../../calculus.md#vector-field) vanishes on $S$, so the flow fixes $S$, and compactness permits a common smaller neighborhood for the full time interval.

For completeness, all hypotheses can be checked directly here. Put $\delta=\beta-\omega_0$ and $\gamma_t=\omega_0+t\delta$. At the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle), every $\gamma_t$ equals $\omega_0$. The [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) property is open, and compactness of $X\times[0,1]$ allows a single smaller neighborhood on which all $\gamma_t$ are [symplectic forms](../../../symplectic-geometry.md#symplectic-form). Choose it fiberwise star-shaped. Write $H_s(q,p)=(q,sp)$ and let $E$ be the vertical radial [vector field](../../../calculus.md#vector-field). The [radial homotopy primitive near a zero section](../../../differential-form.md#radial-homotopy-primitive-near-a-zero-section)

$$
\eta=\int_0^1 s^{-1}H_s^*(\iota_E\delta)\,ds
$$

is smooth, is zero as an ambient covector along the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle), and satisfies

$$
d\eta=\delta-H_0^*\delta=\delta.
$$

The [radial homotopy operator](../../../differential-form.md#radial-homotopy-operator) gives this identity, using $d\delta=0$ and $H_0^*\delta=\pi^*i_0^*\delta=0$. Smoothness at $s=0$ follows because contraction with $E$ supplies a factor of $s$ after evaluation at $(q,sp)$; the vanishing of $\delta$ along $X$ supplies additional vanishing. Therefore solve $\iota_{Z_t}\gamma_t=-\eta$. By [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula), its [flow maps](../../../dynamical-systems.md#flow-map) $\kappa_t$ satisfy

$$
\frac d{dt}(\kappa_t^*\gamma_t)
=\kappa_t^*\bigl(\delta+d(\iota_{Z_t}\gamma_t)\bigr)=0.
$$

After shrinking the starting neighborhood, these flows exist for $0\leq t\leq1$ and fix $X$. This is a relative local construction, not an assertion of completeness throughout the noncompact [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle).

Finally set $\varphi=\psi\circ\kappa_1$, let $U_0$ be its sufficiently small domain, and let $U=\varphi(U_0)$. Then

$$
\boxed{\varphi^*\omega=\kappa_1^*\beta=\omega_0,
\qquad \varphi\circ i_0=i.}
$$

Thus the map is a [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism) of neighborhoods and agrees with the specified inclusion at every point of $X$.

## 4

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a covector $p\in T_x^*X$, define the [cotangent lift of a diffeomorphism](../../../symplectic-geometry.md#cotangent-lift-of-a-diffeomorphism) by

$$
\boxed{f_\#(x,p)=\bigl(f(x),p\circ(df_x)^{-1}\bigr).}
$$

The inverse derivative here maps $T_{f(x)}X$ to $T_xX$. This is a smooth [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), its inverse is $(f^{-1})_\#$, and it satisfies $\pi\circ f_\#=f\circ\pi$.

For $v\in T_{(x,p)}T^*X$, the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) and the defining formula for the [Liouville one-form](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) give

$$
\begin{aligned}
(f_\#^*\alpha)_{(x,p)}(v)
&=(p\circ(df_x)^{-1})\bigl(d\pi_{f_\#(x,p)}df_\#(v)\bigr)\\
&=(p\circ(df_x)^{-1})(df_xd\pi_{(x,p)}v)\\
&=p(d\pi_{(x,p)}v)=\alpha_{(x,p)}(v).
\end{aligned}
$$

Hence **$f_\#^*\alpha=\alpha$**, and applying the [exterior derivative](../../../differential-form.md#exterior-derivative) also proves $f_\#^*\omega=\omega$. The [cotangent lift of a diffeomorphism](../../../symplectic-geometry.md#cotangent-lift-of-a-diffeomorphism) thus preserves both canonical forms, with no extra choice of metric or connection.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

First observe that the [Liouville one-form](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) is zero as an ambient covector exactly on the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle). Indeed, $\alpha_{(x,p)}=p\circ d\pi$, and $d\pi$ is surjective. Since $dg$ is invertible, $g^*\alpha=\alpha$ therefore implies that $g$ maps the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle) onto itself. It induces a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $f:X\to X$ defined by $g(x,0)=(f(x),0)$.

The map $g$ is a [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism), since it preserves $-d\alpha$. Let $E=\sum_i p_i\partial_{p_i}$ be the vertical [Liouville vector field](../../../symplectic-geometry.md#liouville-vector-field). With the chosen sign convention,

$$
\iota_E\omega=-\alpha.
$$

Preservation of both $\omega$ and $\alpha$ forces $g_*E=E$ because $\omega$ is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form). Its complete [cotangent fiber-dilation flow](../../../symplectic-geometry.md#cotangent-fiber-dilation-flow) is

$$
D_s(x,p)=(x,e^sp),\qquad s\in\mathbb R.
$$

Uniqueness of integral curves gives $g\circ D_s=D_s\circ g$. If $g(x,p)=(y,P)$, let $s\to-\infty$. Continuity and this commutation yield

$$
(f(x),0)=g(x,0)=\lim_{s\to-\infty}g(x,e^sp)
=\lim_{s\to-\infty}(y,e^sP)=(y,0).
$$

Thus $y=f(x)$ for every $p$: the whole cotangent fiber over $x$ maps into the fiber over $f(x)$. This step proves that $g$ covers $f$; it was not assumed.

Now write $g(x,p)=(f(x),P(x,p))$. For any $u\in T_xX$, choose a tangent vector to $T^*X$ projecting to $u$. Evaluating $g^*\alpha=\alpha$ on it gives

$$
P(x,p)(df_xu)=p(u).
$$

Since $df_x$ is invertible, $P(x,p)=p\circ(df_x)^{-1}$. Therefore

$$
\boxed{g=f_\#,\qquad f=\pi\circ g\circ i_0,}
$$

and $f$ is unique. This [rigidity of cotangent Liouville-form preservation](../../../symplectic-geometry.md#rigidity-of-cotangent-liouville-form-preservation) uses smoothness at the [zero section](../../../fiber-bundle.md#zero-section-of-a-vector-bundle); it follows from the canonical form and its dilation dynamics on the entire [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For any positive-dimensional $X$, choose a smooth function $h$ with $dh$ not identically zero. A nonconstant smooth bump in a coordinate chart supplies one on an arbitrary [smooth manifold](../../../differential-geometry.md#smooth-manifold). Translate by this [exact differential form](../../../differential-form.md#exact-differential-form):

$$
T_{dh}(x,p)=(x,p+dh_x).
$$

The [cotangent fiber translation](../../../symplectic-geometry.md#cotangent-fiber-translation) identities give

$$
\boxed{T_{dh}^*\omega=\omega,\qquad
T_{dh}^*\alpha=\alpha+\pi^*(dh)\ne\alpha.}
$$

Thus a [nontrivial exact fiber translation](../../../symplectic-geometry.md#nontrivial-exact-fiber-translation) is a [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism) that fails to preserve the [Liouville one-form](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle). For example, on $T^*\mathbb R$ one can take $T(q,p)=(q,p+1)$: it preserves $dq\wedge dp$ but changes $p\,dq$ to $(p+1)\,dq$.

If dimension zero is admitted, $T^*X=X$ and $\alpha=0$, so every [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) preserves $\alpha$ and this requested distinction is impossible. The example therefore applies in positive dimension, as required for a nonzero [differential one-form](../../../differential-form.md#one-form).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
