# Paper 16

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper16.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper16.pdf)

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

## 1

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $T=\dot\gamma$ along an affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic) and $D_t=\nabla_T$ for the [covariant derivative](../../../general-relativity.md#covariant-derivative) from the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). We use the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) convention $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$, for which positive [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) means $\langle R(X,Y)Y,X\rangle>0$ on an orthonormal pair. A [Jacobi field](../../../general-relativity.md#jacobi-field) is a smooth [vector field](../../../calculus.md#vector-field) along $\gamma$ satisfying

$$
\boxed{D_t^2J+R(J,T)T=0.}
$$

Such a field describes the first-order separation of nearby [geodesics](../../../riemannian-geometry.md#geodesic), as the [geodesic variation](../../../riemannian-geometry.md#geodesic-variation) construction in part (c) shows.

For $t_0>0$, $\gamma(t_0)$ is a [conjugate point](../../../calculus-of-variations.md#conjugate-point) of $\gamma(0)$ along this [geodesic](../../../riemannian-geometry.md#geodesic) if a nonzero [Jacobi field](../../../general-relativity.md#jacobi-field) satisfies $J(0)=J(t_0)=0$. The [multiplicity of a conjugate point](../../../calculus-of-variations.md#multiplicity-of-a-conjugate-point) is

$$
\boxed{\dim\{J:D_t^2J+R(J,T)T=0,\ J(0)=J(t_0)=0\}.}
$$

It is equivalently the dimension of the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of the [differential](../../../differential-geometry.md#differential-of-a-smooth-map) of the [Riemannian exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry) at $t_0\dot\gamma(0)$, by [Jacobi fields vanishing at their initial point](../../../general-relativity.md#jacobi-fields-vanishing-at-their-initial-point). Conjugacy concerns the specified [geodesic](../../../riemannian-geometry.md#geodesic) and its two parameter values, even when its endpoints represent the same point of the [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Suppose $J$ is a [Jacobi field](../../../general-relativity.md#jacobi-field) vanishing at both endpoints of a nonconstant [geodesic](../../../riemannian-geometry.md#geodesic) segment $[0,t_0]$. Its tangential component $h(t)=\langle J(t),T(t)\rangle$ satisfies

$$
h''(t)=\langle D_t^2J,T\rangle=-\langle R(J,T)T,T\rangle=0,
$$

because $D_tT=0$ and the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) has the usual skew-adjoint symmetry. The two zero endpoint values imply $h\equiv0$. Both $J$ and $D_tJ$ are therefore perpendicular to $T$.

The [linear map](../../../vector-space.md#linear-map) from these [Jacobi fields](../../../general-relativity.md#jacobi-field) to $T(0)^\perp$ given by $J\mapsto D_tJ(0)$ is injective: $J(0)=0$ together with $D_tJ(0)=0$ forces $J\equiv0$ by uniqueness for the linear [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) defining a [Jacobi field](../../../general-relativity.md#jacobi-field). Its target has dimension $n-1$, so

$$
\boxed{\text{multiplicity}\leq n-1.}
$$

This proves the [endpoint-vanishing normal Jacobi fields have dimension at most n-1](../../../general-relativity.md#endpoint-vanishing-normal-jacobi-fields-have-dimension-at-most-n-1) bound. For a constant [geodesic](../../../riemannian-geometry.md#geodesic) the equation is $J''=0$, and two zero values instead force $J=0$, so there is no [conjugate point](../../../calculus-of-variations.md#conjugate-point).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put $p=\gamma(0)$, $v=\dot\gamma(0)$, $a=J(0)$ and $b=D_tJ(0)$. Choose the short curve $c(s)=\exp_p(sa)$ and let $P_s:T_pM\to T_{c(s)}M$ be [parallel transport](../../../fiber-bundle.md#parallel-transport) along $c$. The tangent vectors

$$
V(s)=P_s(v+sb)
$$

satisfy $V(0)=v$ and $\nabla_sV(0)=b$. Define a [geodesic variation](../../../riemannian-geometry.md#geodesic-variation) by

$$
\boxed{F(s,t)=\exp_{c(s)}\bigl(tV(s)\bigr).}
$$

For each fixed $s$ this is an affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic) with initial point $c(s)$ and initial velocity $V(s)$. Although the [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) need not be complete, smooth dependence for the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) on a neighborhood of the compact reference segment provides a single $\varepsilon>0$ on which $F$ exists for all $|s|<\varepsilon$ and $0\leq t\leq1$. Thus completeness is unnecessary.

Set $X(t)=\partial_sF(0,t)$. The torsion-free [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) gives $\nabla_s\partial_tF=\nabla_t\partial_sF$. Differentiating $\nabla_t\partial_tF=0$ with respect to $s$, and commuting the two [covariant derivatives](../../../general-relativity.md#covariant-derivative), yields

$$
D_t^2X+R(X,T)T=0.
$$

Also $X(0)=c'(0)=a$ and $D_tX(0)=\nabla_sV(0)=b$. Uniqueness for the [Jacobi field](../../../general-relativity.md#jacobi-field) equation now gives **$X(t)=J(t)$** on the whole segment. This is [realization of Jacobi fields by geodesic variations](../../../riemannian-geometry.md#realization-of-jacobi-fields-by-geodesic-variations).

The printed formula switches the order of its two variables. The consistent notation here is $F(0,t)=\gamma(t)$ and $J(t)=\partial_sF(0,t)$. A parametrized surface here means a smooth variation map; it cannot be required to be an [immersion](../../../differential-geometry.md#immersion), since the allowed [Jacobi field](../../../general-relativity.md#jacobi-field) $J=0$ would already violate that condition along the reference curve.

## 2

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Consider the subset

$$
A=\{x\in M:f_1(x)=f_2(x),\ (df_1)_x=(df_2)_x\}.
$$

It is nonempty by the given initial data. A [local isometry](../../../differential-geometry.md#local-isometry) preserves the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) and therefore affinely parametrized [geodesics](../../../riemannian-geometry.md#geodesic). On a sufficiently small [normal neighborhood](../../../riemannian-geometry.md#normal-neighbourhood) of $x\in A$, this gives

$$
f_i(\exp_xv)=\exp_{f_i(x)}((df_i)_xv).
$$

The right sides agree, so $f_1=f_2$ on that neighborhood and their [differentials](../../../differential-geometry.md#differential-of-a-smooth-map) agree there as well. Consequently $A$ is [open](../../../topology.md#open-set).

It is also [closed](../../../topology.md#closed-set). If $x_j\in A$ converges to $x$, continuity first gives $f_1(x)=f_2(x)$. Choose coordinate charts around $x$ and this common image. The coordinate matrices of the two [differentials](../../../differential-geometry.md#differential-of-a-smooth-map) depend continuously on the base point; their equalities at $x_j$ therefore pass to $x$. Thus $x\in A$. Since $M$ is [connected](../../../geometry-and-topology.md#connected-space), the nonempty subset $A$ that is both open and closed equals $M$. Hence **$f_1=f_2$ everywhere**. This proves [local isometries are determined by first-order data](../../../differential-geometry.md#local-isometries-are-determined-by-first-order-data) without requiring completeness.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $\pi:\widetilde M\to M$ be the [universal cover](../../../algebraic-topology.md#universal-cover) and equip it with the pullback [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $\widetilde g=\pi^*g$. The [covering map](../../../algebraic-topology.md#covering-space) is a [local isometry](../../../differential-geometry.md#local-isometry), so $\widetilde M$ has constant [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) one.

We must check completeness of the lifted [Riemannian metric](../../../differential-geometry.md#riemannian-metric). A [geodesic](../../../riemannian-geometry.md#geodesic) on $\widetilde M$ projects to a [geodesic](../../../riemannian-geometry.md#geodesic) on $M$. By [geodesic completeness](../../../riemannian-geometry.md#geodesic-completeness) of $M$, the projected [geodesic](../../../riemannian-geometry.md#geodesic) extends for all real time. Its unique lift with a specified initial point extends the original lifted [geodesic](../../../riemannian-geometry.md#geodesic), because $\pi$ is a [local isometry](../../../differential-geometry.md#local-isometry). Hence $\widetilde M$ is geodesically complete, and the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem) also gives metric completeness.

The allowed constant-curvature form of [Cartan-Ambrose-Hicks theorem](../../../riemannian-geometry.md#cartan-ambrose-hicks-theorem) says that a linear tangent-space [isometry](../../../riemannian-geometry.md#isometry) between complete simply connected [Riemannian manifolds](../../../riemannian-geometry.md#riemannian-manifold) of the same constant [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) extends to a global [isometry](../../../riemannian-geometry.md#isometry). The unit round [sphere](../../../geometry-and-topology.md#sphere) $S^n$ is complete, simply connected for $n\geq2$, and has [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) one. Comparing it with $\widetilde M$ therefore yields

$$
\boxed{(\widetilde M,\widetilde g)\cong S^n.}
$$

This is the covering step in the [classification of complete positive constant-curvature manifolds](../../../riemannian-geometry.md#classification-of-complete-positive-constant-curvature-manifolds). As usual for this assertion, $n\geq2$ is understood: in dimension one there are no sectional two-planes, and the [universal cover](../../../algebraic-topology.md#universal-cover) of the circle is the line, not the circle.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

By part (b), $M=S^n/\Gamma$, where the group of [deck transformations](../../../algebraic-topology.md#deck-transformation) acts freely by round [isometries](../../../riemannian-geometry.md#isometry). Every round [isometry](../../../riemannian-geometry.md#isometry) is the restriction of an [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation) of $\mathbb R^{n+1}$: it preserves the inner product $\langle x,y\rangle=\cos d(x,y)$, so its images of an orthonormal basis determine its linear extension.

Suppose $n$ is even. Every $A\in SO(n+1)$ has eigenvalue one. Indeed, the nonreal [eigenvalues](../../../linear-operator-theory.md#eigenvalue) come in conjugate pairs with product one, while the remaining real eigenvalues are $\pm1$. Their number is odd and their product is one, forcing at least one $+1$. Such a transformation fixes a unit vector. Freeness of the [deck transformation](../../../algebraic-topology.md#deck-transformation) action consequently implies that the [determinant](../../../linear-algebra.md#determinant) map $\Gamma\to\{\pm1\}$ has trivial kernel. Thus $|\Gamma|\leq2$.

If $\Gamma$ is nontrivial with generator $A$, then $A^2=I$. Its eigenvalues are $\pm1$, and freeness excludes the eigenvalue $+1$. Hence $A=-I$, the antipodal [involution](../../../group-theory.md#involution). We obtain

$$
\boxed{M\cong S^n\quad\text{or}\quad M\cong\mathbb{RP}^n.}
$$

This proves the even-dimensional part of the [classification of complete positive constant-curvature manifolds](../../../riemannian-geometry.md#classification-of-complete-positive-constant-curvature-manifolds).

**The conclusion fails in odd dimensions.** For $n=2m-1\geq3$, identify $S^{2m-1}$ with the unit sphere in $\mathbb C^m$. Scalar multiplication by $\zeta=e^{2\pi i/r}$, with $r\geq3$, generates a freely acting [cyclic group](../../../group.md#cyclic-group) of [isometries](../../../riemannian-geometry.md#isometry): $\zeta^jz=z$ for nonzero $z$ forces $\zeta^j=1$. The quotient is complete with constant [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) one and has [fundamental group](../../../algebraic-topology.md#fundamental-group) $C_r$, so it is neither the simply connected [sphere](../../../geometry-and-topology.md#sphere) nor [Real projective space](../../../algebraic-topology.md#real-projective-space) with fundamental group $C_2$. In particular $S^3/C_3$ is a [lens space](../../../knot-theory.md#lens-space) counterexample.

## 3

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $\tau>0$ be the first conjugate time and choose a nonzero [Jacobi field](../../../general-relativity.md#jacobi-field) $J$ with $J(0)=J(\tau)=0$. It is normal by part 1(b), and $D_tJ(\tau)\ne0$, since zero value and derivative there would force $J=0$. Fix any $T>\tau$ and extend $J$ by zero to a continuous piecewise smooth [vector field](../../../calculus.md#vector-field) $V$ on $[0,T]$.

For endpoint-vanishing fields, the [Riemannian index form](../../../riemannian-geometry.md#riemannian-index-form) is

$$
I(X,Y)=\int_0^T\bigl(\langle D_tX,D_tY\rangle-\langle R(X,\dot\gamma)\dot\gamma,Y\rangle\bigr)\,dt.
$$

Integration by parts on $[0,\tau]$ and the [Jacobi field](../../../general-relativity.md#jacobi-field) equation give $I(V,V)=0$ and

$$
I(V,W)=\langle D_tJ(\tau),W(\tau)\rangle.
$$

Choose a smooth normal field $W$, zero at $0,T$, with $W(\tau)=-D_tJ(\tau)$. Then

$$
I(V+\varepsilon W,V+\varepsilon W)=-2\varepsilon|D_tJ(\tau)|^2+\varepsilon^2I(W,W)<0
$$

for sufficiently small positive $\varepsilon$. The corner in $V$ causes no difficulty: smooth endpoint-vanishing fields approximate $V+\varepsilon W$ in the [Sobolev space](../../../sobolev-space.md) $H^1$, and the [Riemannian index form](../../../riemannian-geometry.md#riemannian-index-form) is continuous in this norm on the compact segment. A smooth approximant therefore still has negative index form.

Realize this smooth field as a fixed-endpoint curve variation using the [Riemannian exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry). The allowed [second variation of geodesic energy](../../../riemannian-geometry.md#second-variation-of-geodesic-energy) gives $E'(0)=0$ and $E''(0)<0$, so some nearby curve has energy less than $T/2$, the energy of the unit-speed reference [geodesic](../../../riemannian-geometry.md#geodesic). The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) bounds its length by

$$
L^2\leq T\int_0^T|\dot c|^2\,dt=2TE<T^2.
$$

It is shorter than the reference segment. Thus **a geodesic cannot minimize beyond its first conjugate time**. This argument deliberately uses $T>\tau$; it does not rule out minimization up to the [conjugate point](../../../calculus-of-variations.md#conjugate-point) itself.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $t_0$ be the finite cut time and put $q=\gamma(t_0)$. Continuity of [Riemannian distance](../../../riemannian-geometry.md#riemannian-distance) shows that the segment to $q$ still minimizes and $d(p,q)=t_0$. Choose $t_j\downarrow t_0$ with $t_j>t_0$. By the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem), there is a minimizing [geodesic](../../../riemannian-geometry.md#geodesic) from $p$ to $q_j=\gamma(t_j)$ with length $\ell_j=d(p,q_j)<t_j$ and initial unit vector $v_j$. Continuity gives $\ell_j\to t_0$.

The unit tangent sphere is compact, so after a subsequence $v_j\to v$. Smooth dependence of the [Riemannian exponential map](../../../riemannian-geometry.md#exponential-map-riemannian-geometry) gives $\exp_p(t_0v)=q$. The [geodesic](../../../riemannian-geometry.md#geodesic) with initial vector $v$ has length $t_0=d(p,q)$ up to $q$, hence minimizes. If $v\ne\dot\gamma(0)$, this is the required second minimizing [geodesic](../../../riemannian-geometry.md#geodesic).

Suppose instead $v=\dot\gamma(0)$ and $q$ is not a [conjugate point](../../../calculus-of-variations.md#conjugate-point). Then the [differential](../../../differential-geometry.md#differential-of-a-smooth-map) of $\exp_p$ at $t_0\dot\gamma(0)$ is nonsingular. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes $\exp_p$ injective on a neighborhood of this vector. For large $j$, both $\ell_jv_j$ and $t_j\dot\gamma(0)$ belong to that neighborhood and exponentiate to $q_j$. They must be equal, implying $\ell_j=t_j$, a contradiction. Thus either a distinct minimizing [geodesic](../../../riemannian-geometry.md#geodesic) exists or $q$ is conjugate. In the latter case it is the first [conjugate point](../../../calculus-of-variations.md#conjugate-point), since part (a) excludes any earlier one on a minimizing segment. We have proved the **cut-point dichotomy for complete Riemannian manifolds**.

Here the relevant concept is a [Riemannian cut point](../../../riemannian-geometry.md#riemannian-cut-point), not the topological [cut point](../../../geometry-and-topology.md#cut-point) obtained by disconnecting a space through removal of a point.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Take unit-curvature [Real projective space](../../../algebraic-topology.md#real-projective-space) $\mathbb{RP}^n=S^n/\{\pm1\}$ with $n\geq2$, and any point $p=[v]$. It is complete with positive [sectional curvature](../../../second-fundamental-form.md#sectional-curvature). A unit-speed [geodesic](../../../riemannian-geometry.md#geodesic) through $p$ lifts to

$$
\widetilde\gamma(t)=\cos t\,v+\sin t\,w,\qquad |v|=|w|=1,\quad\langle v,w\rangle=0.
$$

Since the two representatives of an endpoint are antipodal, [Riemannian distance](../../../riemannian-geometry.md#riemannian-distance) in the quotient is the smaller of the two spherical distances:

$$
d([v],[u])=\arccos|\langle v,u\rangle|,\qquad d(p,\gamma(t))=\arccos|\cos t|.
$$

This equals $t$ for $0\leq t\leq\pi/2$ and is strictly smaller just afterwards. Thus the [Riemannian cut point](../../../riemannian-geometry.md#riemannian-cut-point) occurs at time $\pi/2$ in every direction.

Along a curvature-one [geodesic](../../../riemannian-geometry.md#geodesic), every normal [Jacobi field](../../../general-relativity.md#jacobi-field) with initial value zero is $J(t)=\sin t\,P_ta$, where $P_t$ is [parallel transport](../../../fiber-bundle.md#parallel-transport) and $a\perp\dot\gamma(0)$. Its first further zero is $t=\pi$. The quotient map is a [local isometry](../../../differential-geometry.md#local-isometry), so the [Jacobi field](../../../general-relativity.md#jacobi-field) equation and conjugacy times are unchanged. Hence

$$
\boxed{t_{\mathrm{cut}}=\pi/2<\pi=t_{\mathrm{conj}}\quad\text{in every direction}.}
$$

This is [cut and conjugate times in round real projective space](../../../riemannian-geometry.md#cut-and-conjugate-times-in-round-real-projective-space).

## 4

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a connected complete $n$-dimensional [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold), $n\geq2$, the [Bonnet-Myers theorem](../../../second-fundamental-form.md#myers-s-theorem) states that

$$
\operatorname{Ric}\geq(n-1)kg,\quad k>0\quad\Longrightarrow\quad\boxed{\operatorname{diam}M\leq\frac{\pi}{\sqrt k},\quad M\text{ compact},\quad|\pi_1(M)|<\infty.}
$$

The [fundamental group](../../../algebraic-topology.md#fundamental-group) conclusion follows by applying the same diameter and compactness result to the complete [universal cover](../../../algebraic-topology.md#universal-cover): its covering fiber is closed and discrete in a compact space, hence finite.

There is an important [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) convention in the printed question. With the standard trace convention used in this wiki, the literal hypothesis $\operatorname{Ric}\geq kg$ yields instead $\operatorname{diam}M\leq\pi\sqrt{(n-1)/k}$. The sphere constants in parts (b) and (c) require [normalized Ricci curvature](../../../second-fundamental-form.md#normalized-ricci-curvature) $\overline{\operatorname{Ric}}=\operatorname{Ric}/(n-1)\geq kg$, equivalently the stronger trace bound $\operatorname{Ric}\geq(n-1)kg$. We prove those conclusions with this intended normalization below and exhibit counterexamples to the literal trace interpretation. Thus no factor of $n-1$ is silently discarded.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use the intended trace bound $\operatorname{Ric}\geq(n-1)kg$ and write $D=\pi/\sqrt k$. We state precisely the allowed [Bishop volume comparison with a positive-curvature model](../../../second-fundamental-form.md#bishop-volume-comparison-with-a-positive-curvature-model). Set

$$
s_k(r)=\frac{\sin(\sqrt k\,r)}{\sqrt k},\qquad v_k(r)=\omega_{n-1}\int_0^r s_k(t)^{n-1}\,dt,
$$

where $\omega_{n-1}$ is the area of the unit $(n-1)$-sphere. For $V_p(r)=\operatorname{Vol}B(p,r)$, the ratio $V_p(r)/v_k(r)$ is nonincreasing on $0<r<D$, tends to one at zero, and is at most one. Before the cut time, the radial volume density $J(r,\theta)$ in [geodesic polar coordinates](../../../riemannian-geometry.md#geodesic-polar-coordinates) is at most $s_k(r)^{n-1}$.

By the [Bonnet-Myers theorem](../../../second-fundamental-form.md#myers-s-theorem), $\operatorname{diam}M\leq D$. Therefore $V_p(D)=\operatorname{Vol}M$. If distance-$D$ endpoints exist, they do not affect this volume equality: the distance sphere is contained in the smooth image $\exp_p(D S_p^{n-1})$, which has zero $n$-dimensional [Riemannian volume](../../../differential-geometry.md#riemannian-volume). Taking limits in the comparison ratio at $D$ is legitimate. The assumed equality of total volume gives $V_p(D)/v_k(D)=1$, so monotonicity forces

$$
V_p(r)=v_k(r)\qquad(0<r<D)
$$

for every $p$.

We now extract the equality geometry, rather than merely naming a rigidity theorem. On a small [normal neighborhood](../../../riemannian-geometry.md#normal-neighbourhood) of $p$, the continuous nonnegative difference $s_k(r)^{n-1}-J(r,\theta)$ has integral zero. It is therefore identically zero. Let $A(X)=\nabla_X\partial_r$ on a distance sphere and $h=\operatorname{tr}A=\partial_r\log J$. Equality of the density gives $h=(n-1)s_k'/s_k$. The traced [radial Riccati equation for distance spheres](../../../riemannian-geometry.md#radial-riccati-equation-for-distance-spheres) reads

$$
h'+\operatorname{tr}(A^2)+\operatorname{Ric}(\partial_r,\partial_r)=0.
$$

Since $s_k''=-ks_k$, substituting $h$ makes the sum of the following two nonnegative quantities zero:

$$
\left(\operatorname{tr}(A^2)-\frac{h^2}{n-1}\right)+\left(\operatorname{Ric}(\partial_r,\partial_r)-(n-1)k\right)=0.
$$

Equality in the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) for the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of the self-adjoint operator $A$ forces $A=(s_k'/s_k)I$. The angular metric $g_r$ in [geodesic polar coordinates](../../../riemannian-geometry.md#geodesic-polar-coordinates) consequently satisfies $\partial_rg_r=2(s_k'/s_k)g_r$. Smoothness at the center fixes its integration constant, since $r^{-2}g_r\to g_{S^{n-1}}$. Hence

$$
g=dr^2+s_k(r)^2g_{S^{n-1}}
$$

on the normal ball: the [Riemannian metric](../../../differential-geometry.md#riemannian-metric) is locally the round curvature-$k$ metric. As $p$ was arbitrary, $M$ has constant [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) $k$.

The [classification of complete positive constant-curvature manifolds](../../../riemannian-geometry.md#classification-of-complete-positive-constant-curvature-manifolds) now gives $M=S_k^n/\Gamma$ with $\Gamma$ a finite freely acting group of [isometries](../../../riemannian-geometry.md#isometry). Covering degree gives $\operatorname{Vol}M=\operatorname{Vol}S_k^n/|\Gamma|$. Volume equality forces $|\Gamma|=1$, proving

$$
\boxed{M\cong S_k^n.}
$$

This establishes [spherical rigidity of maximal total volume](../../../second-fundamental-form.md#spherical-rigidity-of-maximal-total-volume) under the correct normalization.

**Under the literal trace bound, the assertion is false in dimension four.** Take the [Riemannian product](../../../riemannian-geometry.md#riemannian-product) $M=S^2(r)\times S^2(r)$ with $r^2=1/(\sqrt6\,k)$. Its [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) is $r^{-2}g=\sqrt6\,kg\geq kg$, and

$$
\operatorname{Vol}M=(4\pi r^2)^2=\frac{8\pi^2}{3k^2}=\operatorname{Vol}S_k^4.
$$

But a mixed tangent two-plane has [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) zero, whereas a factor plane has curvature $\sqrt6\,k$. Thus this manifold is not the round sphere despite having the literal hypotheses.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Again assume the intended trace [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) bound $\operatorname{Ric}\geq(n-1)kg$, and put $D=\pi/\sqrt k$. Compactness from the [Bonnet-Myers theorem](../../../second-fundamental-form.md#myers-s-theorem) ensures that the diameter is attained: choose $p,q$ with $d(p,q)=D$. For $0<r<D$, the open balls $B(p,r)$ and $B(q,D-r)$ are disjoint, because a point in both would violate the [triangle inequality](../../../topological-analysis.md#triangle-inequality).

The clearly stated [Bishop volume comparison with a positive-curvature model](../../../second-fundamental-form.md#bishop-volume-comparison-with-a-positive-curvature-model) from part (b), applied between radius $r$ and radius $D$, gives

$$
V_p(r)\geq\frac{v_k(r)}{v_k(D)}\operatorname{Vol}M,\qquad V_q(D-r)\geq\frac{v_k(D-r)}{v_k(D)}\operatorname{Vol}M.
$$

Here both radius-$D$ ball volumes equal the total volume, as shown in part (b). The symmetry $s_k(D-t)=s_k(t)$ gives

$$
v_k(r)+v_k(D-r)=v_k(D).
$$

The two lower bounds therefore sum to $\operatorname{Vol}M$, while disjointness bounds that same sum above by $\operatorname{Vol}M$. Both inequalities must be equalities. In particular

$$
\frac{V_p(r)}{v_k(r)}=\frac{\operatorname{Vol}M}{v_k(D)}\qquad(0<r<D).
$$

Letting $r\downarrow0$, the local Euclidean volume asymptotic gives one on the left. Thus $\operatorname{Vol}M=v_k(D)$, and the detailed equality proof in part (b) applies. We obtain

$$
\boxed{\operatorname{diam}M=\pi/\sqrt k\quad\Longrightarrow\quad M\cong S_k^n.}
$$

This proves [maximal diameter rigidity from disjoint comparison balls](../../../second-fundamental-form.md#maximal-diameter-rigidity-from-disjoint-comparison-balls) directly, including the required equality argument.

**The literal trace interpretation again has a counterexample.** On $M=S^2(r)\times S^2(r)$ with $r^2=1/(2k)$, the [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) equals $2kg\geq kg$. For the [product Riemannian metric](../../../differential-geometry.md#product-riemannian-metric), distances satisfy $d^2=d_1^2+d_2^2$: every product curve has length at least $\sqrt{d_1^2+d_2^2}$ by the integral [triangle inequality](../../../topological-analysis.md#triangle-inequality), and a pair of constant-speed minimizing factor [geodesics](../../../riemannian-geometry.md#geodesic) attains it. Consequently

$$
\operatorname{diam}M=\sqrt{(\pi r)^2+(\pi r)^2}=\frac{\pi}{\sqrt k}.
$$

The mixed [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) is zero, so this manifold is not $S_k^4$. The stronger bound, or [normalized Ricci curvature](../../../second-fundamental-form.md#normalized-ricci-curvature) convention, is essential.

## 5

↑ **Parent:** [Paper 16](paper-16.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Choose a finite symmetric generating set $S$ for $\Gamma$, a base point $p$, and put $L=\max_{s\in S}d(p,sp)$. If the [word length](../../../geometric-group-theory.md#word-length) of $\gamma$ is at most $m$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) and invariance of [Riemannian distance](../../../riemannian-geometry.md#riemannian-distance) under [isometries](../../../riemannian-geometry.md#isometry) give $d(p,\gamma p)\leq Lm$.

A [properly discontinuous group action](../../../geometric-group-theory.md#properly-discontinuous-group-action) has finite point stabilizer $F=\Gamma_p$ and a discrete orbit. More explicitly, properness on compact sets shows that only finitely many elements move $p$ into any bounded ball, since closed bounded balls are compact by the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem). Thus there is $\rho>0$ such that distinct orbit points have distance more than $2\rho$: choose it using the finitely many orbit points within a fixed small ball of $p$, and translate the resulting separation by [isometries](../../../riemannian-geometry.md#isometry). If the whole orbit is one point, the group itself is finite and the conclusion is immediate.

Let $N_m$ be the number of distinct orbit points represented by the [word metric](../../../geometric-group-theory.md#word-metric) ball of radius $m$. Their radius-$\rho$ balls are disjoint, have equal positive volume $v_0=\operatorname{Vol}B(p,\rho)$, and lie inside $B(p,Lm+\rho)$. The allowed [Bishop-Gromov inequality](../../../second-fundamental-form.md#bishop-gromov-inequality) for nonnegative [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) states that $\operatorname{Vol}B(p,R)/R^n$ is nonincreasing for $R>0$. Therefore

$$
N_mv_0\leq\operatorname{Vol}B(p,Lm+\rho)\leq v_0\left(\frac{Lm+\rho}{\rho}\right)^n.
$$

Each orbit point has at most $|F|$ preimages inside the word ball, since its full fiber is a coset of $F$. For the [growth function of a finitely generated group](../../../geometric-group-theory.md#growth-function-of-a-finitely-generated-group), this gives

$$
\boxed{\beta_\Gamma(m)\leq |F|\left(1+\frac{Lm}{\rho}\right)^n=O(m^n).}
$$

Hence $\Gamma$ has [polynomial growth of a group](../../../geometric-group-theory.md#polynomial-growth-of-a-group) of degree at most $n$. The finite stabilizer factor makes the proof valid even when the properly discontinuous action is not free. This is [polynomial growth of properly discontinuous isometry groups](../../../geometric-group-theory.md#polynomial-growth-of-properly-discontinuous-isometry-groups).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $\Gamma=\pi_1(M)$. A compact connected smooth [manifold](../../../topology.md#topological-manifold) has finite [CW complex](../../../algebraic-topology.md#cw-complex) homotopy type, hence a finitely generated [fundamental group](../../../algebraic-topology.md#fundamental-group). Its [universal cover](../../../algebraic-topology.md#universal-cover) with the lifted [Riemannian metric](../../../differential-geometry.md#riemannian-metric) is complete by the lifted-geodesic argument in part 2(b) and has nonnegative [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature). The [deck transformations](../../../algebraic-topology.md#deck-transformation) act freely and [properly discontinuously](../../../geometric-group-theory.md#properly-discontinuous-group-action) by [isometries](../../../riemannian-geometry.md#isometry). Part (a) gives

$$
\beta_\Gamma(m)\leq C(1+m)^n.
$$

The degree-one [Hurewicz theorem](../../../algebraic-topology.md#hurewicz-theorem) identifies $H_1(M;\mathbb Z)$ with the [abelianization](../../../group-theory.md#abelianization) of $\Gamma$. This finitely generated abelian group has free rank $b=b_1(M)$, so there is a surjection $\Gamma\to\mathbb Z^b$. Choose lifts $\gamma_1,\ldots,\gamma_b$ of a basis and let $A\geq1$ bound their [word lengths](../../../geometric-group-theory.md#word-length). For every $(z_1,\ldots,z_b)$ with $\sum|z_i|\leq m$, the product $\gamma_1^{z_1}\cdots\gamma_b^{z_b}$ has word length at most $Am$ and maps to that vector. Distinct vectors therefore give distinct group elements. The integer cube $|z_i|\leq\lfloor m/b\rfloor$ shows, for $b>0$, that

$$
\beta_\Gamma(Am)\geq c m^b
$$

for some $c>0$ and all sufficiently large $m$. Comparing with the degree-$n$ upper bound forces $b\leq n$; the case $b=0$ is immediate. Thus

$$
\boxed{b_1(M)\leq n.}
$$

This is the [first Betti-number bound from polynomial fundamental-group growth](../../../geometric-group-theory.md#first-betti-number-bound-from-polynomial-fundamental-group-growth).

The standard connectedness convention for a [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) is needed here. If disconnected manifolds are allowed, the bound applies to each connected component; a disjoint union of two flat $n$-tori has first [Betti number](../../../homology.md#betti-number) $2n$ and contradicts a global bound by $n$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Consider the [orientation-preserving affine group of the real line](../../../lie-theory.md#orientation-preserving-affine-group-of-the-real-line), realized as

$$
G=\left\{\begin{pmatrix}a&b\\0&1\end{pmatrix}:a>0,\ b\in\mathbb R\right\}.
$$

The coordinates $(\log a,b)$ identify it smoothly with $\mathbb R^2$, so this [Lie group](../../../lie-theory.md#lie-group) is connected. Choose the [Lie algebra](../../../lie-algebra.md) element $E$ and the group element $D$:

$$
E=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad D=\begin{pmatrix}2&0\\0&1\end{pmatrix}\in G.
$$

Direct [matrix multiplication](../../../vector-space.md#matrix-multiplication) gives $\operatorname{Ad}_D E=DED^{-1}=2E$.

If a [bi-invariant Riemannian metric](../../../lie-theory.md#bi-invariant-riemannian-metric) existed, every conjugation map $x\mapsto D xD^{-1}$ would be an [isometry](../../../riemannian-geometry.md#isometry) fixing the identity. Its [differential](../../../differential-geometry.md#differential-of-a-smooth-map) there, the [Adjoint representation of a Lie group](../../../lie-theory.md#adjoint-representation-of-a-lie-group), would preserve the [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) [inner product](../../../linear-algebra.md#inner-product) at the identity. Thus

$$
\|E\|^2=\|\operatorname{Ad}_D E\|^2=\|2E\|^2=4\|E\|^2,
$$

a contradiction since $E\ne0$. Therefore **this connected Lie group admits no bi-invariant Riemannian metric**. This is the [adjoint dilation obstruction to a bi-invariant Riemannian metric](../../../lie-theory.md#adjoint-dilation-obstruction-to-a-bi-invariant-riemannian-metric), an elementary alternative permitted by the question. The positive definite [Riemannian metric](../../../differential-geometry.md#riemannian-metric) interpretation matters; no claim about indefinite metrics is needed.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
