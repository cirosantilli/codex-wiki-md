# Paper 115

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_115.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_115.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
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
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An $m$ by $n$ matrix has [matrix rank](../../../vector-space.md#matrix-rank) $m$ exactly when at least one of its $m$ by $m$ minors has nonzero [determinant](../../../linear-algebra.md#determinant). For each multi-index $I$, the set

$$
U_I=\{M:\det M_I\ne0\}
$$

is [open](../../../topology.md#open-set) in the [vector space](../../../vector-space.md) of all real $m$ by $n$ matrices, because the determinant is [continuous](../../../calculus.md#continuous-function). Their union is $X_{m,n}$, so $X_{m,n}$ is itself open in $\mathbb R^{mn}$. It therefore inherits the standard [smooth manifold](../../../differential-geometry.md#smooth-manifold) structure and has [dimension](../../../vector-space.md#dimension-vector-space) $mn$. This is the [full-row-rank matrix manifold](../../../differential-geometry.md#full-row-rank-matrix-manifold).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Define the [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds)

$$
\Phi:X_{m,n}\times\mathbb R^n\longrightarrow\mathbb R^m,
\qquad \Phi(M,v)=Mv.
$$

At $(M,v)$ its [derivative](../../../calculus.md#derivative) in the direction $(A,w)$ is

$$
D\Phi_{(M,v)}(A,w)=Av+Mw.
$$

The restriction to variations $(0,w)$ is the [surjective linear map](../../../vector-space.md#surjective-linear-map) $M:\mathbb R^n\to\mathbb R^m$, since $M$ has full row rank. Thus $0$ is a [regular value](../../../differential-geometry.md#regular-value) of $\Phi$. The [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem) now shows that

$$
E_{m,n}=\Phi^{-1}(0)
$$

is an [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) of $X_{m,n}\times\mathbb R^n$, of dimension $mn+n-m$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Fix $I$ and write $I'$ for the complementary column indices. Over $U_I$, decompose $M=(M_I,M_{I'})$ and $v=(v_I,v_{I'})$. The equation $Mv=0$ is equivalent to

$$
v_I=-M_I^{-1}M_{I'}v_{I'}.
$$

Matrix inversion is [smooth](../../../analysis.md#smooth-function) on the [invertible matrices](../../../linear-algebra.md#invertible-matrix), so

$$
(M,u)\longmapsto\left(M,\bigl(-M_I^{-1}M_{I'}u,u\bigr)\right)
$$

is a smooth, fiberwise-linear trivialization $U_I\times\mathbb R^{n-m}\to\pi^{-1}(U_I)$. The sets $U_I$ cover the base, proving that $\pi:E_{m,n}\to X_{m,n}$ is a [vector bundle](../../../fiber-bundle.md#vector-bundle) of rank $n-m$. It is the [kernel bundle of a constant-rank family of linear maps](../../../fiber-bundle.md#kernel-bundle-of-a-constant-rank-family-of-linear-maps), and its rank also follows from the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $x\in S^2\subset\mathbb R^3$, let $F(x)=x^T$, viewed as a nonzero $1$ by $3$ matrix. This defines a [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds) $F:S^2\to X_{1,3}$. Its pulled-back fiber is

$$
(F^*E_{1,3})_x=\ker x^T=x^\perp=T_xS^2,
$$

so the evident fiberwise identity gives an isomorphism of [vector bundles](../../../fiber-bundle.md#vector-bundle) $F^*E_{1,3}\cong TS^2$.

If $E_{1,3}$ were a [trivial vector bundle](../../../fiber-bundle.md#trivial-vector-bundle), its [pullback](../../../fiber-bundle.md#pullback-vector-bundle) would be trivial. A trivial rank-two bundle has a [nowhere-zero section](../../../fiber-bundle.md#nowhere-zero-section), whereas the assumed form of the [Hairy ball theorem](../../../fiber-bundle.md#hairy-ball-theorem) says that the [tangent bundle](../../../fiber-bundle.md#tangent-bundle) $TS^2$ does not. Hence $E_{1,3}$ is nontrivial.

## 2

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Give $\partial X$ the [outward-normal-first boundary orientation](../../../differential-geometry.md#outward-normal-first-boundary-orientation). The [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem) states that, for every compactly supported $(n-1)$-form $\omega$,

$$
\int_Xd\omega=\int_{\partial X}F^*\omega.
$$

Choose an oriented coordinate cover by charts into $\mathbb R^n$ or the half-space $\mathbb H^n=\{x^1\geq0\}$, and choose a [partition of unity](../../../differential-geometry.md#partition-of-unity) $(\rho_i)$ subordinate to it. Since the family is locally finite and $\omega$ has [compact support](../../../function.md#compact-support), only finitely many $\rho_i\omega$ are nonzero. It is therefore legitimate to write both integrals as finite sums and prove the identity for a form supported in one chart.

In an interior chart the integral of an exact compactly supported top form is zero by the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus). In a boundary chart write

$$
\omega=\sum_{j=1}^n(-1)^{j-1}a_j\,dx^1\wedge\cdots\wedge\widehat{dx^j}\wedge\cdots\wedge dx^n.
$$

Integrating $d\omega=(\sum_j\partial_ja_j)dx^1\wedge\cdots\wedge dx^n$ coordinate by coordinate kills every tangential derivative. The normal derivative leaves precisely the restriction to $x^1=0$, with the sign selected by the outward-normal-first convention. This is $\int_{\partial X}F^*\omega$, proving the theorem.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $(\theta^1,\ldots,\theta^n)$ be the [dual basis](../../../linear-algebra.md#dual-basis) of the positively oriented [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $(v_1,\ldots,v_n)$. By the definition of the [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form),

$$
\omega_X=\theta^1\wedge\cdots\wedge\theta^n.
$$

The [interior product of a differential form](../../../differential-form.md#interior-product) with the outward unit normal is

$$
\iota_{v_1}\omega_X=\theta^2\wedge\cdots\wedge\theta^n.
$$

The vectors $(v_2,\ldots,v_n)$ form a positive orthonormal frame of $T\partial X$ by the [outward-normal-first boundary orientation](../../../differential-geometry.md#outward-normal-first-boundary-orientation). Consequently the pullback of the last display is the positive unit boundary volume form:

$$
\boxed{\omega_{\partial X}=F^*(\iota_{v_1}\omega_X).}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

On the Euclidean [unit ball](../../../functional-analysis.md#unit-ball) $D^n$,

$$
\omega_X=dx^1\wedge\cdots\wedge dx^n.
$$

The outward [unit normal](../../../differential-geometry.md#unit-normal) along $S^{n-1}$ is the radial vector field $N=\sum_i x^i\partial_i$, so part b gives

$$
\omega_{\partial X}
=\sum_{i=1}^n(-1)^{i-1}x^i\,dx^1\wedge\cdots\wedge\widehat{dx^i}\wedge\cdots\wedge dx^n.
$$

Let $R=\sum_i x^i\partial_i$ on the ball and put $\beta=\iota_R\omega_X$. Direct use of the [exterior derivative](../../../differential-form.md#exterior-derivative) gives $d\beta=n\omega_X$. Therefore the [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem) yields

$$
\int_{\partial X}\omega_{\partial X}
=\int_{\partial X}F^*\beta
=\int_Xd\beta
=n\int_X\omega_X.
$$

This proves the [volume of a Euclidean unit sphere](../../../differential-geometry.md#volume-of-a-euclidean-unit-sphere) formula.

## 3

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [local flow](../../../differential-geometry.md#local-flow) of $v$ is a smooth family $\Phi^t$ defined near $\{0\}\times X$ such that $\Phi^0=\operatorname{id}$, $\partial_t\Phi^t(x)=v(\Phi^t(x))$, and $\Phi^{s+t}=\Phi^s\circ\Phi^t$ whenever defined. The [Lie derivative of a differential form](../../../differential-form.md#lie-derivative-of-a-differential-form) is

$$
\mathcal L_v\alpha=\left.\frac d{dt}\right|_{t=0}(\Phi^t)^*\alpha.
$$

[Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) is

$$
\boxed{\mathcal L_v\alpha=d(\iota_v\alpha)+\iota_v(d\alpha).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For $\xi$ in the [Lie algebra](../../../lie-algebra.md) $\mathfrak g$, set $\Phi^t=R_{\exp(t\xi)}$. The [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) law gives the flow law, and

$$
\left.\frac d{dt}\right|_{0}g\exp(t\xi)=(dL_g)_e\xi=l_\xi(g),
$$

so this is the global flow of the [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field) $l_\xi$.

For $f(g)=R_g^*\alpha$, every tangent vector at $g$ is the initial velocity of $g\exp(t\xi)$ for some $\xi$. Since $R_{g\exp(t\xi)}=R_{\exp(t\xi)}\circ R_g$,

$$
\left.\frac d{dt}\right|_0f(g\exp(t\xi))
=R_g^*(\mathcal L_{l_\xi}\alpha).
$$

**Thus all $\mathcal L_{l_\xi}\alpha$ vanish exactly when every derivative of $f$ vanishes. This is equivalent to $f$ being a [locally constant function](../../../calculus.md#locally-constant-function).**

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Suppose first that the [left-invariant 1-form](../../../lie-theory.md#left-invariant-differential-form) $\alpha$ is [closed](../../../differential-form.md#closed-differential-form). The scalar function $\alpha(l_\xi)$ is constant for every $\xi$, because both the form and vector field are left-invariant. [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) therefore gives

$$
\mathcal L_{l_\xi}\alpha=d(\alpha(l_\xi))+\iota_{l_\xi}d\alpha=0.
$$

Part b says that $g\mapsto R_g^*\alpha$ is locally constant. Since $G$ is [connected](../../../geometry-and-topology.md#connected-space), it is constant, and its value at the identity is $\alpha$. Hence $R_g^*\alpha=\alpha$ for every $g$, so $\alpha$ is [bi-invariant](../../../lie-theory.md#bi-invariant-differential-form).

Conversely, if $\alpha$ is bi-invariant, then all these [Lie derivatives](../../../differential-form.md#lie-derivative-of-a-differential-form) vanish. Cartan's formula and the constancy of $\alpha(l_\xi)$ give $\iota_{l_\xi}d\alpha=0$. The left-invariant vector fields span every tangent space, so $d\alpha=0$.

Connectedness cannot be omitted. The [orthogonal group](../../../linear-algebra.md#orthogonal-group) $O(2)$ has an [abelian Lie algebra](../../../lie-algebra.md#abelian-lie-algebra), so every left-invariant 1-form is closed by the [Maurer-Cartan equation in a Lie-algebra basis](../../../lie-theory.md#maurer-cartan-equation-in-a-lie-algebra-basis). Conjugation by a reflection acts as $-1$ on its one-dimensional Lie algebra, so a nonzero left-invariant 1-form is not right-invariant. This is the standard obstruction recorded by the [closed left-invariant 1-form](../../../lie-theory.md#closed-left-invariant-1-form) criterion.

## 4

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The differential-forms version of the [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem) says that a constant-rank [distribution](../../../differential-geometry.md#distribution-differential-geometry) $D=\bigcap_i\ker\alpha^i$ is [integrable](../../../differential-geometry.md#integrable-distribution) exactly when

$$
d\alpha^i=\sum_j\beta^i{}_j\wedge\alpha^j
$$

for suitable 1-forms $\beta^i{}_j$. For a [plane distribution](../../../differential-geometry.md#plane-distribution) $D=\ker\alpha$ on $\mathbb R^3$, this reduces to the [integrability criterion for a plane distribution](../../../differential-geometry.md#integrability-criterion-for-a-plane-distribution) $\alpha\wedge d\alpha=0$.

For example, $\ker dz$ is integrable: its integral surfaces are the horizontal planes $z=\text{constant}$. In contrast, for $\alpha=dz-x\,dy$,

$$
\alpha\wedge d\alpha=(dz-x\,dy)\wedge(-dx\wedge dy)=-dz\wedge dx\wedge dy\ne0.
$$

**Thus $\ker(dz-x\,dy)$ is not integrable; it is the standard [contact structure](../../../differential-geometry.md#contact-structure) on $\mathbb R^3$.**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For a [principal connection](../../../fiber-bundle.md#connection-principal-bundle) with connection form $\mathcal A$, the [horizontal distribution of a principal connection](../../../fiber-bundle.md#horizontal-distribution-of-a-principal-connection) is $H=\ker\mathcal A$, the complement of the tangent spaces to the $G$-orbits. Its [curvature of a principal connection](../../../fiber-bundle.md#curvature-of-a-principal-connection) is

$$
\mathcal F=d\mathcal A+\frac12[\mathcal A\wedge\mathcal A].
$$

If $X,Y$ are horizontal vector fields, then $\mathcal A(X)=\mathcal A(Y)=0$, and hence

$$
\mathcal F(X,Y)=d\mathcal A(X,Y)=-\mathcal A([X,Y]).
$$

The [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem) says that $H$ is integrable exactly when $[X,Y]$ is horizontal for all horizontal $X,Y$. The displayed identity makes this equivalent to the vanishing of the horizontal two-form $\mathcal F$, hence to $\mathcal F=0$. Thus the horizontal distribution is integrable exactly for a [flat principal connection](../../../fiber-bundle.md#flat-principal-connection).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The vertical tangent space of the trivial principal $\mathbb R$-bundle is spanned by $\partial_z$. Since

$$
D=\operatorname{span}\{\partial_\theta+f\partial_z,\ \partial_t+g\partial_z\}
$$

projects isomorphically onto the tangent space of $S^1\times\mathbb R$, it is always complementary to the vertical direction. It is the [horizontal distribution of a principal connection](../../../fiber-bundle.md#horizontal-distribution-of-a-principal-connection) precisely when it is invariant under the principal translations $z\mapsto z+a$. The horizontal lifts of $\partial_\theta$ and $\partial_t$ are unique, so this invariance is equivalent to

$$
\partial_zf=\partial_zg=0.
$$

The functions must also be smooth and [periodic](../../../function.md#periodic-function) in $\theta$, as is already required for them to be functions on the cylinder.

Under these conditions the connection form is

$$
\mathcal A=dz-f\,d\theta-g\,dt.
$$

It sends $\partial_z$ to $1$, is translation-invariant, and has kernel $D$, proving sufficiency as well. Since the structure group $\mathbb R$ is [abelian](../../../group.md#abelian-group), the bracket term vanishes and

$$
\boxed{\mathcal F=d\mathcal A=(\partial_tf-\partial_\theta g)\,d\theta\wedge dt.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For $f=t\cos\theta+1$ and $g=\sin\theta$,

$$
\partial_tf-\partial_\theta g=\cos\theta-\cos\theta=0.
$$

The connection is therefore [flat](../../../fiber-bundle.md#flat-principal-connection), so the [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem) gives [horizontal sections](../../../fiber-bundle.md#horizontal-section-of-a-principal-bundle) locally.

A global section has the form $z=h(\theta,t)$ and is horizontal exactly when

$$
\partial_\theta h=t\cos\theta+1,
\qquad
\partial_th=\sin\theta.
$$

The second equation gives $h=t\sin\theta+k(\theta)$, and the first then forces $k'(\theta)=1$. No such $k$ is periodic on $S^1$, so no global horizontal section exists. Equivalently, the horizontal lift of one positive circuit in the $\theta$ direction changes $z$ by

$$
\int_0^{2\pi}(t\cos\theta+1)\,d\theta=2\pi,
$$

which is nontrivial [holonomy](../../../fiber-bundle.md#holonomy).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
