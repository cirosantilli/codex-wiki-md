# Paper 140

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_140.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_140.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
  - [c](#3/c)
    - [Solution](#3/c/solution)
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
  - [e](#6/e)
    - [Solution](#6/e/solution)

## 1

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

[Moser theorem](../../../symplectic-geometry.md#moser-s-trick) says that if $M$ is a [compact](../../../topology.md#compact-space) [smooth manifold](../../../differential-geometry.md#smooth-manifold) without boundary and $\omega_t$, $0\leq t\leq1$, is a smooth family of [symplectic forms](../../../symplectic-geometry.md#symplectic-form) with constant [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class, then there is a [smooth isotopy](../../../differential-geometry.md#smooth-isotopy) $\psi_t$, with $\psi_0=\mathrm{id}$, such that

$$
\boxed{\psi_t^*\omega_t=\omega_0.}
$$

Thus the endpoints are [symplectomorphic](../../../symplectic-geometry.md#symplectomorphism). The hypothesis is a whole path of [symplectic forms](../../../symplectic-geometry.md#symplectic-form), not merely equality of the endpoint [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) classes.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism) is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), so it preserves the [genus of a surface](../../../topology.md#genus-of-a-surface). It also preserves the [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) determined by the [symplectic form](../../../symplectic-geometry.md#symplectic-form) and, by integration of a [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form), preserves the [symplectic area](../../../symplectic-geometry.md#symplectic-area).

Conversely, equal [genus of a surface](../../../topology.md#genus-of-a-surface) gives a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $f:\Sigma_0\to\Sigma_1$. We can choose $f$ to preserve the [orientations](../../../algebraic-topology.md#orientation-of-a-simplex) determined by $\omega_0,\omega_1$: if necessary, compose with an [orientation-reversing diffeomorphism](../../../differential-geometry.md#orientation-reversing-diffeomorphism) of the standard [closed orientable surface](../../../topology.md#closed-orientable-surface) of that [genus of a surface](../../../topology.md#genus-of-a-surface), obtained by reflection of a symmetric handle model. On $\Sigma_0$ put $\eta=f^*\omega_1$. Both $\eta$ and $\omega_0$ are positive [volume forms](../../../differential-form.md#volume-form) for the same [orientation](../../../algebraic-topology.md#orientation-of-a-simplex), and their integrals agree. By [top-degree de Rham cohomology](../../../differential-form.md#top-degree-de-rham-cohomology), $[\eta]=[\omega_0]$.

The family $\omega_t=(1-t)\omega_0+t\eta$ consists of positive [volume forms](../../../differential-form.md#volume-form), hence [symplectic forms](../../../symplectic-geometry.md#symplectic-form) in dimension two, with constant [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class. [Moser theorem](../../../symplectic-geometry.md#moser-s-trick) supplies $\psi$ with $\psi^*\eta=\omega_0$. Consequently

$$
\boxed{(f\circ\psi)^*\omega_1=\omega_0.}
$$

Therefore **the [genus of a surface](../../../topology.md#genus-of-a-surface) and [symplectic area](../../../symplectic-geometry.md#symplectic-area) classify [compact](../../../topology.md#compact-space) [connected](../../../geometry-and-topology.md#connected-space) [symplectic surfaces](../../../symplectic-geometry.md#symplectic-surface)**.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

There is an [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) convention in this statement: the two [volume forms](../../../differential-form.md#volume-form) must be positive for one fixed [orientation](../../../algebraic-topology.md#orientation-of-a-simplex), as is usual in [Moser theorem for volume forms](../../../symplectic-geometry.md#moser-theorem-for-volume-forms). Without that convention, the stated necessity is false. For example, on an oriented [two-sphere](../../../geometry-and-topology.md#two-sphere), take a positive [volume form](../../../differential-form.md#volume-form) $\beta_0$ and an [orientation-reversing diffeomorphism](../../../differential-geometry.md#orientation-reversing-diffeomorphism) $r$, and set $\beta_1=r^*\beta_0$. Then $(r^{-1})^*\beta_1=\beta_0$ but $\int\beta_1=-\int\beta_0$. We prove the intended result with a common [orientation](../../../algebraic-topology.md#orientation-of-a-simplex).

If $\phi^*\beta_1=\beta_0$, positivity forces $\phi$ to preserve the [orientation](../../../algebraic-topology.md#orientation-of-a-simplex), and integration of the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) gives equality of the integrals.

For sufficiency, [top-degree de Rham cohomology](../../../differential-form.md#top-degree-de-rham-cohomology) gives a [differential form](../../../differential-form.md) $\alpha$ of degree $n-1$ with $\beta_1-\beta_0=d\alpha$. Put $\beta_t=(1-t)\beta_0+t\beta_1$. Positivity makes every $\beta_t$ a [volume form](../../../differential-form.md#volume-form). The [interior product of a differential form](../../../differential-form.md#interior-product) gives an [linear isomorphism](../../../vector-space.md#linear-isomorphism)

$$
T_pM\longrightarrow\Lambda^{n-1}T_p^*M,\qquad v\longmapsto\iota_v\beta_t.
$$

Thus there is a unique smooth time-dependent [vector field](../../../calculus.md#vector-field) $X_t$ satisfying $\iota_{X_t}\beta_t=-\alpha$. Since $M$ is [compact](../../../topology.md#compact-space), its [local flow](../../../differential-geometry.md#local-flow) exists throughout $0\leq t\leq1$ and defines a [smooth isotopy](../../../differential-geometry.md#smooth-isotopy) $\phi_t$ starting at the identity. By [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula), and since a top-degree [differential form](../../../differential-form.md) has zero [exterior derivative](../../../differential-form.md#exterior-derivative),

$$
\frac{d}{dt}\phi_t^*\beta_t
=\phi_t^*\bigl(d\alpha+\mathcal L_{X_t}\beta_t\bigr)
=\phi_t^*\bigl(d\alpha+d\iota_{X_t}\beta_t\bigr)=0.
$$

Hence

$$
\boxed{\phi_1^*\beta_1=\beta_0.}
$$

The zero-dimensional case, a single point, is immediate from equality of the integrals.

## 2

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\dim V=2n$ and let $V_+=\ker(S-I)$ and $V_-=\ker(S+I)$ be the two [eigenspaces](../../../linear-operator-theory.md#eigenspace). The [involution](../../../group-theory.md#involution) identity gives a [direct sum](../../../vector-space.md#direct-sum), since

$$
v=\frac{v+Sv}{2}+\frac{v-Sv}{2},\qquad V=V_+\oplus V_-.
$$

For $u,v$ in either one of these [eigenspaces](../../../linear-operator-theory.md#eigenspace), the [anti-symplectic involution](../../../symplectic-geometry.md#anti-symplectic-involution) identity implies

$$
\Omega(u,v)=\Omega(Su,Sv)=-\Omega(u,v),
$$

so both are [isotropic subspaces of a symplectic vector space](../../../linear-algebra.md#isotropic-subspace-of-a-symplectic-vector-space). Such a subspace has dimension at most $n$: $W\subset W^\Omega$ and the [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form) $\Omega$ gives $\dim W^\Omega=2n-\dim W$, where $W^\Omega$ is the [symplectic orthogonal complement](../../../linear-algebra.md#symplectic-orthogonal-complement). As their dimensions add to $2n$, both have dimension $n$. Therefore

$$
\boxed{\operatorname{Fix}(S)=V_+\text{ is a Lagrangian subspace}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the decomposition into [Lagrangian subspaces](../../../symplectic-geometry.md#lagrangian-subspace) $V=V_+\oplus V_-$ from part (a). The [bilinear form](../../../linear-algebra.md#bilinear-form) $\Omega$ pairs $V_+$ and $V_-$ nondegenerately: a [vector](../../../vector-space.md#vector) in either summand annihilating the other already annihilates its own summand and hence all of $V$, so is zero.

Choose a [basis](../../../vector-space.md#basis) $e_1,\ldots,e_n$ of $V_+$. The [linear map](../../../vector-space.md#linear-map)

$$
V_-\longrightarrow V_+^*,\qquad f\longmapsto\bigl(e\longmapsto\Omega(e,f)\bigr)
$$

is an [linear isomorphism](../../../vector-space.md#linear-isomorphism). Let $f_j$ correspond to the [dual basis](../../../linear-algebra.md#dual-basis) of the $e_i$. Then $\Omega(e_i,f_j)=\delta_{ij}$, and the pairings within each summand vanish. Thus

$$
\boxed{(e_1,\ldots,e_n,f_1,\ldots,f_n)\text{ is a symplectic basis},\quad Se_i=e_i,\quad Sf_i=-f_i.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $p\in\operatorname{Fix}(\sigma)$, differentiation gives $(d\sigma_p)^2=I$ and $(d\sigma_p)^*\omega_p=-\omega_p$. Thus $d\sigma_p$ is an [anti-symplectic involution](../../../symplectic-geometry.md#anti-symplectic-involution) of the [symplectic vector space](../../../linear-algebra.md#symplectic-vector-space) $T_pM$. By part (a), its $+1$ [eigenspace](../../../linear-operator-theory.md#eigenspace) is a [Lagrangian subspace](../../../symplectic-geometry.md#lagrangian-subspace).

In the local [manifold chart](../../../differential-geometry.md#manifold-chart) supplied in the question, $\sigma$ is linear, so its [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) is the intersection of the chart with this $+1$ [eigenspace](../../../linear-operator-theory.md#eigenspace). Therefore the [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) is an [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) and

$$
T_p\operatorname{Fix}(\sigma)=\ker(d\sigma_p-I).
$$

Every such [tangent space](../../../differential-geometry.md#tangent-space) has half the ambient dimension and the [symplectic form](../../../symplectic-geometry.md#symplectic-form) vanishes on it. Hence **every nonempty [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) is a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold)**. The [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) itself need not be [connected](../../../geometry-and-topology.md#connected-space).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $\sigma(z)=\overline z$, componentwise [complex conjugation](../../../complex-analysis.md#complex-conjugation). Interpret the printed $|z^2|$ in the potential as $|z|^2=\sum_j|z_j|^2$. With $D=1+|z|^2$, the local [Fubini-Study form](../../../complex-geometry.md#fubini-study-form) is

$$
\widetilde\omega_{FS}=\frac{i}{2}\sum_{j,k}
\left(\frac{\delta_{jk}}D-\frac{\overline z_jz_k}{D^2}\right)dz_j\wedge d\overline z_k.
$$

Its [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) under $\sigma$ is

$$
\sigma^*\widetilde\omega_{FS}
=\frac{i}{2}\sum_{j,k}
\left(\frac{\delta_{jk}}D-\frac{z_j\overline z_k}{D^2}\right)d\overline z_j\wedge dz_k
=-\widetilde\omega_{FS},
$$

where the last equality swaps $j,k$ and uses antisymmetry of the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms). Since $\sigma^2=I$, it is an [anti-symplectic involution](../../../symplectic-geometry.md#anti-symplectic-involution), with [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) $\mathbb R^n$. Part (c) gives

$$
\boxed{\mathbb R^n\subset(\mathbb C^n,\widetilde\omega_{FS})\text{ is Lagrangian}.}
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

As usual for [Complex projective space](../../../algebraic-topology.md#complex-projective-space) and [Real projective space](../../../algebraic-topology.md#real-projective-space), [homogeneous coordinates](../../../projective-space.md#homogeneous-coordinate) are represented by nonzero vectors. Componentwise [complex conjugation](../../../complex-analysis.md#complex-conjugation) descends to the [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism)

$$
\tau:\mathbb{CP}^n\longrightarrow\mathbb{CP}^n,\qquad [z]\longmapsto[\overline z].
$$

It is well defined because $\overline{\lambda z}=\overline\lambda\,\overline z$, and $\tau^2=I$. Every standard [manifold chart](../../../differential-geometry.md#manifold-chart) is invariant under $\tau$, with $\varphi_i\circ\tau=\sigma\circ\varphi_i$. Part (d) and the gluing of the [Fubini-Study form](../../../complex-geometry.md#fubini-study-form) therefore imply $\tau^*\omega_{FS}=-\omega_{FS}$.

A point $[z]$ in the [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) satisfies $\overline z=\lambda z$. Applying [complex conjugation](../../../complex-analysis.md#complex-conjugation) again gives $|\lambda|=1$. Choose $a\ne0$ with $a/\overline a=\lambda$; then $\overline{az}=az$, so $[z]$ has a real representative. Conversely every real representative determines a point in the [fixed-point set](../../../riemannian-geometry.md#fixed-point-set). Hence $\operatorname{Fix}(\tau)=\mathbb{RP}^n$, and part (c) gives

$$
\boxed{\mathbb{RP}^n\subset(\mathbb{CP}^n,\omega_{FS})\text{ is a Lagrangian submanifold}.}
$$

## 3

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Take the usual convention that the [smooth isotopy](../../../differential-geometry.md#smooth-isotopy) starts at $\rho_0=\mathrm{id}$. The [exterior derivative](../../../differential-form.md#exterior-derivative) commutes with a [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form), so

$$
d(\rho_t^*\lambda-\lambda)
=\rho_t^*d\lambda-d\lambda
=\omega-\rho_t^*\omega.
$$

Consequently

$$
\boxed{\rho_t^*\lambda-\lambda\text{ is closed for every }t
\iff \rho_t^*\omega=\omega\text{ for every }t.}
$$

The right-hand condition says precisely that $\rho_t$ is a [symplectic isotopy](../../../symplectic-geometry.md#symplectic-isotopy).

Here an [exact symplectic manifold](../../../symplectic-geometry.md#exact-symplectic-manifold) is necessarily noncompact in positive dimension: if $\dim M=2n$ and $\omega=-d\lambda$, then $\omega^n=-d(\lambda\wedge\omega^{n-1})$, contradicting the positive [symplectic volume](../../../symplectic-geometry.md#symplectic-volume) and the [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem) on a [compact](../../../topology.md#compact-space) [smooth manifold](../../../differential-geometry.md#smooth-manifold) without boundary. Thus the paper's introductory word “closed” must here be read as “without boundary”, as its parenthesis suggests, rather than as including [compactness](../../../topology.md#compact-space).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) convention $\iota_{X_t}\omega=dH_t$, which is forced by the sign of the formula in this part. This is the opposite of the default sign in the linked general article. Since $d\lambda=-\omega$, [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) gives

$$
\mathcal L_{X_t}\lambda
=d(\iota_{X_t}\lambda)+\iota_{X_t}d\lambda
=d(\iota_{X_t}\lambda-H_t).
$$

Differentiate the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) along the [smooth isotopy](../../../differential-geometry.md#smooth-isotopy) and integrate from $0$ to $t$:

$$
\begin{aligned}
\rho_t^*\lambda-\lambda
&=\int_0^t\rho_s^*\mathcal L_{X_s}\lambda\,ds\\
&=d\int_0^t(\iota_{X_s}\lambda-H_s)\circ\rho_s\,ds.
\end{aligned}
$$

Thus the required [exact differential form](../../../differential-form.md#exact-differential-form) has the explicit primitive

$$
\boxed{F_t=\int_0^t(\iota_{X_s}\lambda-H_s)\circ\rho_s\,ds,\qquad\rho_t^*\lambda-\lambda=dF_t.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Differentiating the assumed primitive identity and using [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) gives

$$
d\dot F_t=\rho_t^*\mathcal L_{X_t}\lambda
=\rho_t^*\bigl(d(\iota_{X_t}\lambda)-\iota_{X_t}\omega\bigr).
$$

Apply the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) by $\rho_t^{-1}$ and rearrange:

$$
\boxed{\iota_{X_t}\omega=dH_t,\qquad
H_t=\iota_{X_t}\lambda-\dot F_t\circ\rho_t^{-1}.}
$$

This smooth family of [Hamiltonian functions](../../../symplectic-geometry.md#hamiltonian-function) proves that $\rho_t$ is a [Hamiltonian isotopy](../../../symplectic-geometry.md#hamiltonian-isotopy) in the convention of part (b).

To connect this with the preceding assertion that every $\rho_t^*\lambda-\lambda$ is an [exact differential form](../../../differential-form.md#exact-differential-form), the smooth choice of primitives causes no additional obstruction. Fix $p_0\in M$ and normalize $F_t(p_0)=0$. Define $F_t(p)$ by the [line integral](../../../calculus.md#line-integral) of $\rho_t^*\lambda-\lambda$ from $p_0$ to $p$. The [fundamental theorem for line integrals](../../../calculus.md#fundamental-theorem-for-line-integrals) makes this independent of the path. Near any $p$, use one fixed path to a nearby chart center followed by coordinate line segments; this expression is smooth jointly in $t,p$. Thus these normalized primitives form the required smooth family.

## 4

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $\pi:T^*X\to X$ be the [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle) projection and $\lambda$ its [canonical one-form on a cotangent bundle](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle), defined by $\lambda_{(x,\xi)}(v)=\xi(d\pi(v))$. Use the [symplectic form](../../../symplectic-geometry.md#symplectic-form) $\omega=-d\lambda$, so in local coordinates $\omega=\sum_jdx_j\wedge d\xi_j$.

The graph map $s_\beta(x)=(x,\beta_x)$ is a [smooth embedding](../../../differential-geometry.md#smooth-embedding), with $s_\beta^*\lambda=\beta$, and hence

$$
s_\beta^*\omega=-d\beta.
$$

Its image has dimension $\dim X$, half the dimension of $T^*X$. By the definition of a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold),

$$
\boxed{\operatorname{graph}(\beta)\text{ is Lagrangian}\iff d\beta=0.}
$$

This is the [graph of a closed one-form is Lagrangian](../../../symplectic-geometry.md#graph-of-a-closed-one-form-is-lagrangian) criterion. The opposite conventional sign for the [symplectic form](../../../symplectic-geometry.md#symplectic-form) gives the same criterion.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [cotangent fiber translation](../../../symplectic-geometry.md#cotangent-fiber-translation) $f$ is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), with inverse $(x,\xi)\mapsto(x,\xi-\beta_x)$. Because $\pi\circ f=\pi$, the definition of the [canonical one-form on a cotangent bundle](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) gives

$$
f^*\lambda=\lambda+\pi^*\beta.
$$

Taking the [exterior derivative](../../../differential-form.md#exterior-derivative) yields

$$
\boxed{f^*\omega=\omega-\pi^*d\beta.}
$$

If $\beta$ is a [closed differential form](../../../differential-form.md#closed-differential-form), this is $f^*\omega=\omega$, proving that **the [cotangent fiber translation](../../../symplectic-geometry.md#cotangent-fiber-translation) is a [symplectomorphism](../../../symplectic-geometry.md#symplectomorphism)**.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Write the [exact differential form](../../../differential-form.md#exact-differential-form) as $\beta=dh$ and take the [cotangent fiber translation](../../../symplectic-geometry.md#cotangent-fiber-translation) family $\rho_t(x,\xi)=(x,\xi+t\,dh_x)$. Its generating [vector field](../../../calculus.md#vector-field) is vertical and in local coordinates is

$$
X=\sum_j\frac{\partial h}{\partial x_j}\frac{\partial}{\partial\xi_j}.
$$

With $\omega=\sum_jdx_j\wedge d\xi_j$ and the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) convention from Question 3,

$$
\boxed{\iota_X\omega=-\pi^*dh=dH,\qquad H=-h\circ\pi.}
$$

Thus $\rho_t$ is a [Hamiltonian isotopy](../../../symplectic-geometry.md#hamiltonian-isotopy) and $f=\rho_1$ is a [Hamiltonian diffeomorphism](../../../symplectic-geometry.md#hamiltonian-isotopy). The [local flow](../../../differential-geometry.md#local-flow) is explicitly defined for every real $t$, regardless of [compactness](../../../topology.md#compact-space). With the alternative convention $\iota_{X_H}\omega=-dH$, the same family is generated by $H=h\circ\pi$.

The definition in the question does not require compact support for the [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function); the displayed [Hamiltonian diffeomorphism](../../../symplectic-geometry.md#hamiltonian-isotopy) uses that definition.

## 5

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure) is a smooth bundle map $J:TM\to TM$ such that, for all [tangent vectors](../../../differential-geometry.md#tangent-vector) $u,v$,

$$
\boxed{J^2=-I,\qquad\omega(Ju,Jv)=\omega(u,v),\qquad\omega(u,Ju)>0\quad(u\ne0).}
$$

It determines the [Riemannian metric](../../../differential-geometry.md#riemannian-metric)

$$
\boxed{g(u,v)=\omega(u,Jv).}
$$

Indeed, the invariance of the [symplectic form](../../../symplectic-geometry.md#symplectic-form) under $J$ and its antisymmetry imply $\omega(v,Ju)=\omega(u,Jv)$, so $g$ is symmetric; the positivity condition makes it positive definite. A [compatible triple](../../../complex-geometry.md#compatible-triple) consists of this [symplectic form](../../../symplectic-geometry.md#symplectic-form), this [compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure), and this [Riemannian metric](../../../differential-geometry.md#riemannian-metric). Useful equivalent identities are $\omega(u,v)=g(Ju,v)$ and $g(Ju,Jv)=g(u,v)$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

At a point $p$, write $W=T_pL$ and take the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) with respect to the [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $g$. The [compatible triple](../../../complex-geometry.md#compatible-triple) identity gives

$$
g(Ju,v)=\omega(u,v).
$$

If $L$ is a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold), then $\omega(u,v)=0$ for $u,v\in W$, so $JW\subset W^\perp$. Both have dimension $\frac12\dim M$, hence equality.

Conversely, if $JW=W^\perp$, equality of dimensions gives $\dim W=\frac12\dim M$, and $g(Ju,v)=0$ for $u,v\in W$ gives $\omega|_W=0$. Therefore

$$
\boxed{L\text{ is Lagrangian}\iff J(T_pL)=(T_pL)^\perp\text{ for every }p.}
$$

A positive-definite [inner product](../../../linear-algebra.md#inner-product) has $W\cap W^\perp=\{0\}$. Hence $W\cap JW=\{0\}$, proving that **every [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) is a [totally real submanifold](../../../complex-geometry.md#totally-real-submanifold) for a [compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure)**.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Use $\mathbb C^2$ with the [standard symplectic form](../../../symplectic-geometry.md#standard-symplectic-form) $\omega_0=dx_1\wedge dy_1+dx_2\wedge dy_2$ and the [compatible almost complex structure](../../../complex-geometry.md#compatible-almost-complex-structure) given by multiplication by $i$. Consider the [embedded submanifold](../../../differential-geometry.md#embedded-submanifold)

$$
\boxed{L=\{(s+it,t):s,t\in\mathbb R\}.}
$$

In coordinates $(x_1,y_1,x_2,y_2)$, its [tangent space](../../../differential-geometry.md#tangent-space) is $W=\{(a,b,b,0):a,b\in\mathbb R\}$. Applying $J$ gives $J(a,b,b,0)=(-b,a,0,b)$. If this is again in $W$, its fourth coordinate forces $b=0$, and its second and third coordinates then force $a=0$. Thus $W\cap JW=0$ and $\dim_\mathbb R L=2$: $L$ is a [totally real submanifold](../../../complex-geometry.md#totally-real-submanifold).

However, the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) under the parametrization is

$$
\boxed{\omega_0|_L=ds\wedge dt\ne0.}
$$

Thus **this [totally real submanifold](../../../complex-geometry.md#totally-real-submanifold) is not a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold)**.

## 6

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For $X\in\mathfrak h$, the [fundamental vector field](../../../lie-theory.md#fundamental-vector-field) of the restricted [Lie group action](../../../lie-theory.md#lie-group-action) is $(iX)_M$. If $\phi$ is the original [moment map](../../../symplectic-geometry.md#moment-map), then

$$
d\langle\pi\circ\phi,X\rangle_H
=d\langle\phi,iX\rangle_G
=\iota_{(iX)_M}\omega
=\iota_{X_M}\omega.
$$

This is the defining [Hamiltonian action](../../../symplectic-geometry.md#hamiltonian-group-action) identity, in the convention $\iota_{X_H}\omega=dH$.

If equivariance is included in the definition of a [moment map](../../../symplectic-geometry.md#moment-map), it is also preserved: the [dual map](../../../linear-algebra.md#transpose-of-a-linear-map) $\pi=i^*$ intertwines the [coadjoint actions](../../../lie-theory.md#coadjoint-representation) of $H$, since $i(\operatorname{Ad}_hX)=\operatorname{Ad}_h(iX)$. Thus

$$
\boxed{\phi_H=i^*\phi=\pi\circ\phi}
$$

is a [moment map](../../../symplectic-geometry.md#moment-map) for the restricted [Hamiltonian action](../../../symplectic-geometry.md#hamiltonian-group-action) of the [Lie subgroup](../../../lie-theory.md#lie-subgroup) $H$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The diagonal [Lie algebra](../../../lie-algebra.md) inclusion is $i(a)=(a,\ldots,a)$. Its [dual map](../../../linear-algebra.md#transpose-of-a-linear-map) is characterized by

$$
\langle\pi(\eta),a\rangle
=\langle\eta,i(a)\rangle
=a\sum_{j=1}^n\eta_j.
$$

Consequently

$$
\boxed{\pi(\eta_1,\ldots,\eta_n)=\eta_1+\cdots+\eta_n.}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Use the paper's [Fubini-Study form](../../../complex-geometry.md#fubini-study-form) normalization $\widetilde\omega_{FS}=\frac{i}{2}\partial\overline\partial\log(1+|z|^2)$, the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) convention $\iota_{X_H}\omega=dH$, and the [Lie algebra](../../../lie-algebra.md) generator whose [circle](../../../topology.md#circle) action is $e^{i\theta}$. Write $D=|z_0|^2+|z_1|^2+|z_2|^2$. The normalized [moment map](../../../symplectic-geometry.md#moment-map) for the [torus](../../../topology.md#torus) action is

$$
\boxed{\phi([z_0,z_1,z_2])=-\frac1{2D}\bigl(|z_1|^2,|z_2|^2\bigr).}
$$

The [moment map](../../../symplectic-geometry.md#moment-map) image is the filled triangle

$$
\boxed{\phi(\mathbb{CP}^2)=\{(u,v):u\leq0,\ v\leq0,\ u+v\geq-\tfrac12\}.}
$$

Indeed, the three quantities $|z_j|^2/D$ are nonnegative and add to one, and any such triple is realized by choosing their square roots as [homogeneous coordinates](../../../projective-space.md#homogeneous-coordinate).

For the diagonal [circle](../../../topology.md#circle) action, a point in the [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) satisfies $[z_0,tz_1,tz_2]=[z_0,z_1,z_2]$ for every $t\in S^1$. If $z_0\ne0$, the projective scaling must be one, forcing $z_1=z_2=0$. If $z_0=0$, all coordinates are scaled together. Therefore

$$
\boxed{\operatorname{Fix}(S^1)=\{[1,0,0]\}\ \sqcup\ \{[0,z_1,z_2]\}\cong\{\mathrm{point}\}\sqcup\mathbb{CP}^1.}
$$

By part (b), the diagonal [moment map](../../../symplectic-geometry.md#moment-map) is

$$
\boxed{\mu([z])=-\frac{|z_1|^2+|z_2|^2}{2D},\qquad\mu(\mathbb{CP}^2)=[-\tfrac12,0].}
$$

The factor $1/2$ follows from the specified [Fubini-Study form](../../../complex-geometry.md#fubini-study-form), not the integral normalization in the linked general article. For example, in one affine complex coordinate $w=re^{i\theta}$ the [symplectic form](../../../symplectic-geometry.md#symplectic-form) is $r(1+r^2)^{-2}dr\wedge d\theta$, whose [interior product of a differential form](../../../differential-form.md#interior-product) with $\partial_\theta$ is $-r(1+r^2)^{-2}dr=d[-r^2/(2(1+r^2))]$. Choosing the generator $e^{2\pi it}$ rescales all [moment maps](../../../symplectic-geometry.md#moment-map) by $2\pi$; reversing the defining sign reverses their signs. The negative level in parts (d) and (e) uses the convention displayed here.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

On $N=\mu^{-1}(-1/4)$, the diagonal [fundamental vector field](../../../lie-theory.md#fundamental-vector-field) $X$ is nonzero, since the [fixed-point set](../../../riemannian-geometry.md#fixed-point-set) lies at [moment map](../../../symplectic-geometry.md#moment-map) values $0$ and $-1/2$. The [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form) $\omega_p$ and $d\mu=\iota_X\omega$ imply $d\mu\ne0$, so $-1/4$ is a [regular value](../../../differential-geometry.md#regular-value). By the [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem), $N$ is a three-dimensional [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) of the four-dimensional [Complex projective plane](../../../algebraic-topology.md#complex-projective-plane).

At $p\in N$, set $W=T_pN=\ker d\mu_p$. Then $\omega(X,v)=0$ for every $v\in W$, so $X\in W^\omega$, the [symplectic orthogonal complement](../../../linear-algebra.md#symplectic-orthogonal-complement). This complement is one-dimensional and $d\mu(X)=\omega(X,X)=0$, giving

$$
\boxed{(T_pN)^\omega=\mathbb RX_p\subset T_pN.}
$$

Thus **the level set is a [coisotropic submanifold](../../../symplectic-geometry.md#coisotropic-submanifold), neither an [isotropic submanifold](../../../symplectic-geometry.md#isotropic-submanifold) nor a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold)**. Indeed an [isotropic subspace of a symplectic vector space](../../../linear-algebra.md#isotropic-subspace-of-a-symplectic-vector-space) in dimension four has dimension at most two, whereas $\dim N=3$. Its [characteristic line field](../../../symplectic-geometry.md#characteristic-line-field) is generated by the diagonal [circle](../../../topology.md#circle) action.

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

The level equation is $|z_1|^2+|z_2|^2=|z_0|^2$. In particular $z_0\ne0$, so the global affine coordinates on this level are $w_j=z_j/z_0$. They identify it with

$$
N=\{(w_1,w_2)\in\mathbb C^2:|w_1|^2+|w_2|^2=1\}=S^3.
$$

The diagonal [circle](../../../topology.md#circle) action becomes $(w_1,w_2)\mapsto(tw_1,tw_2)$ and is free: at least one coordinate is nonzero, so fixing a point forces $t=1$. Since the [circle](../../../topology.md#circle) is [compact](../../../topology.md#compact-space), the [Free proper Lie-group action theorem](../../../fiber-bundle.md#free-proper-lie-group-action-theorem) makes the quotient a smooth two-dimensional [smooth manifold](../../../differential-geometry.md#smooth-manifold).

The map $(w_1,w_2)\mapsto[w_1,w_2]$ is the [Hopf fibration](../../../algebraic-topology.md#hopf-fibration). It is onto the [complex projective line](../../../algebraic-topology.md#complex-projective-line), and two unit representatives determine the same complex line precisely when they differ by a scalar of modulus one, hence by a [circle](../../../topology.md#circle) orbit. Local sections, for example $[1,u]\mapsto(1,u)/\sqrt{1+|u|^2}$, show that the induced identification is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism). Therefore

$$
\boxed{M_{\mathrm{red}}=\mu^{-1}(-1/4)/S^1\cong\mathbb{CP}^1\cong S^2.}
$$

This identifies the [symplectic reduction](../../../symplectic-geometry.md#symplectic-reduction) as a [smooth manifold](../../../differential-geometry.md#smooth-manifold); no computation of its reduced [symplectic form](../../../symplectic-geometry.md#symplectic-form) is needed.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
