# Paper 17

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper17.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper17.pdf)

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
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
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

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Work with real [vector bundles](../../../fiber-bundle.md#vector-bundle); for complex bundles replace the [inner products](../../../linear-algebra.md#inner-product) below by [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) [Hermitian forms](../../../linear-algebra.md#hermitian-form). A smooth rank-$r$ [vector bundle](../../../fiber-bundle.md#vector-bundle) is a smooth total space $E$ with a smooth projection $\pi:E\to M$, a real [vector space](../../../vector-space.md) structure on each [fiber](../../../function.md#fiber-of-a-function) $E_p$, and an [open cover](../../../topology.md#open-cover) with [vector bundle trivializations](../../../fiber-bundle.md#vector-bundle-trivialization)

$$
\Phi_i:\pi^{-1}(U_i)\longrightarrow U_i\times\mathbb R^r.
$$

Each $\Phi_i$ is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) over $U_i$ and is linear on [fibers](../../../function.md#fiber-of-a-function). The overlap maps have the form $(p,v)\mapsto(p,A_{ji}(p)v)$, where $A_{ji}:U_i\cap U_j\to GL_r(\mathbb R)$ is smooth. The [rank of a vector bundle](../../../fiber-bundle.md#rank-of-a-vector-bundle) may be specified separately on each [connected component](../../../geometry-and-topology.md#connected-component).

A smooth [fiber metric](../../../fiber-bundle.md#fiber-metric) is a [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) $h_p$ on each [fiber](../../../function.md#fiber-of-a-function), with smoothly varying coefficients in every [local frame](../../../fiber-bundle.md#frame-of-a-vector-bundle). Equivalently it is a smooth section of $\operatorname{Sym}^2E^*$ which is positive definite at every point. Each trivialization supplies a local [fiber metric](../../../fiber-bundle.md#fiber-metric) $h_i$ by pulling back the Euclidean [inner product](../../../linear-algebra.md#inner-product).

A [smooth manifold](../../../differential-geometry.md#smooth-manifold) is Hausdorff and second-countable, hence [paracompact](../../../topology.md#paracompact-space). Choose a smooth, locally finite [partition of unity](../../../differential-geometry.md#partition-of-unity) $\{\phi_i\}$ subordinate to a trivializing cover, with $\phi_i\ge0$, $\operatorname{supp}\phi_i\subset U_i$, and $\sum_i\phi_i=1$. Define

$$
\boxed{h=\sum_i\phi_i h_i.}
$$

Extend each weighted term by zero outside its trivializing set; its support lies inside that set, so the extension is smooth. Local finiteness makes the sum smooth. At a point $p$ and for $0\ne v\in E_p$, every nonzero term $\phi_i(p)h_i(v,v)$ is positive and at least one such term occurs. Thus $h_p(v,v)>0$. This proves that **every smooth [vector bundle](../../../fiber-bundle.md#vector-bundle) admits a smooth [fiber metric](../../../fiber-bundle.md#fiber-metric)**.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $r=\operatorname{rank}F$ and $s=\operatorname{rank}E$. Around any $p$, choose a [local frame](../../../fiber-bundle.md#frame-of-a-vector-bundle) $f_1,\ldots,f_r$ of the [vector subbundle](../../../fiber-bundle.md#vector-subbundle) $F$. Choose additional smooth sections $e_{r+1},\ldots,e_s$ of $E$ which complement these vectors at $p$. They can be obtained by constant-coordinate sections in a [vector bundle trivialization](../../../fiber-bundle.md#vector-bundle-trivialization). The [determinant](../../../linear-algebra.md#determinant) of the resulting frame is nonzero at $p$, hence on a sufficiently small neighborhood. Thus

$$
f_1,\ldots,f_r,e_{r+1},\ldots,e_s
$$

is an adapted [local frame](../../../fiber-bundle.md#frame-of-a-vector-bundle) of $E$ near $p$.

On the fiberwise quotient, the classes $[e_{r+1}],\ldots,[e_s]$ form a [basis](../../../vector-space.md#basis). Give the [quotient vector bundle](../../../fiber-bundle.md#quotient-vector-bundle) its local coordinates by

$$
\sum_{j=r+1}^s a_j[e_j(p)]\longleftrightarrow(p,a_{r+1},\ldots,a_s).
$$

An overlap between adapted frames has a smooth [transition function of a vector bundle](../../../fiber-bundle.md#transition-function-of-a-vector-bundle) represented by an invertible block upper triangular [matrix](../../../vector-space.md#matrix),

$$
\begin{pmatrix}A&B\\0&D\end{pmatrix}.
$$

The zero lower-left block expresses that both sets of first $r$ frame vectors span $F$. Its lower-right block $D$ is smooth and invertible. Passing to quotient coordinates removes the upper block, leaving precisely the transition $D$. These lower-right blocks satisfy the cocycle identity because the original transition matrices do. Consequently they define a compatible smooth bundle atlas of rank $s-r$. This proves **$E/F$ is a smooth [vector bundle](../../../fiber-bundle.md#vector-bundle)**, and its fiberwise quotient map $q:E\to E/F$ is a smooth [vector bundle morphism](../../../fiber-bundle.md#vector-bundle-morphism). The construction is independent of the adapted frames: any two choices have the same type of compatible transition. The usual quotient topology agrees with this atlas, since in adapted coordinates $q$ is an open linear projection on each [fiber](../../../function.md#fiber-of-a-function).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Choose the smooth [fiber metric](../../../fiber-bundle.md#fiber-metric) supplied by part (a), and let $P_p:E_p\to F_p$ be [orthogonal projection](../../../hilbert-space.md#orthogonal-projection). These projections vary smoothly. Indeed, in a [local frame](../../../fiber-bundle.md#frame-of-a-vector-bundle) of $E$ write its metric as a [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) [matrix](../../../vector-space.md#matrix) $G(p)$, and let the columns of $A(p)$ be a frame of $F$. Then

$$
P=A(A^tGA)^{-1}A^tG.
$$

The [matrix](../../../vector-space.md#matrix) $A^tGA$ is positive definite, so its inverse is smooth. This formula proves smoothness of the intrinsic projections in every chart. It also gives $P^2=P$ and $\operatorname{im}P=F$.

The [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) $F^\perp=\ker P$ is a smooth [vector subbundle](../../../fiber-bundle.md#vector-subbundle): applying $I-P$ to a complement frame gives a frame of its [fibers](../../../function.md#fiber-of-a-function), of constant rank $s-r$, after shrinking the chart. Fiberwise,

$$
E=F\oplus F^\perp,
$$

and the restriction $q|_{F^\perp}:F^\perp\to E/F$ is a smooth fiberwise bijective [vector bundle morphism](../../../fiber-bundle.md#vector-bundle-morphism). In [local frames](../../../fiber-bundle.md#frame-of-a-vector-bundle) its [matrix](../../../vector-space.md#matrix) is invertible, with smooth inverse, so it is a [vector bundle isomorphism](../../../fiber-bundle.md#vector-bundle-isomorphism).

More explicitly, the desired [orthogonal splitting of a vector subbundle](../../../fiber-bundle.md#orthogonal-splitting-of-a-vector-subbundle) is

$$
\boxed{\Psi:E\longrightarrow F\oplus(E/F),\qquad \Psi(v)=(Pv,[v]).}
$$

Its inverse is $(f,[v])\mapsto f+(I-P)v$. Replacing $v$ by $v+w$ with $w\in F_p$ leaves $(I-P)v$ unchanged, so the inverse is well-defined. Both maps are smooth and linear on [fibers](../../../function.md#fiber-of-a-function), and their compositions are identities. The splitting exists globally but depends on the chosen [fiber metric](../../../fiber-bundle.md#fiber-metric).

## 2

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A smooth [differential form](../../../differential-form.md) of degree $p$ is a smooth section of $\Lambda^pT^*M$, so

$$
\Omega^p(M)=\Gamma(\Lambda^pT^*M).
$$

It is equivalently a smooth alternating covariant $p$-tensor field. In a [coordinate chart](../../../differential-geometry.md#manifold-chart) $x^1,\ldots,x^n$ it has a unique expression

$$
\omega=\sum_{i_1<\cdots<i_p}a_{i_1\cdots i_p}\,dx^{i_1}\wedge\cdots\wedge dx^{i_p}
$$

with smooth coefficients. At $p=0$ these are the [smooth functions](../../../analysis.md#smooth-function), and for $p>n$ the space is zero.

Define the [exterior derivative](../../../differential-form.md#exterior-derivative) in a chart by

$$
d\omega=\sum_{I,j}\frac{\partial a_I}{\partial x^j}\,dx^j\wedge dx^I.
$$

To check that it is well-defined, let $y^1,\ldots,y^n$ be other smooth coordinates. The expression $dy^a=\sum_i(\partial_i y^a)dx^i$ satisfies

$$
d_x(dy^a)=\sum_{i,j}(\partial_j\partial_i y^a)\,dx^j\wedge dx^i=0
$$

because the coefficients are symmetric and the wedge products antisymmetric. The coordinate formula also satisfies the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule), and for a function $b$ the [chain rule](../../../calculus.md#chain-rule) gives $d_xb=\sum_a(\partial b/\partial y^a)dy^a=d_yb$. Applying these two facts to $\omega=\sum_I b_I\,dy^I$ yields $d_x\omega=\sum_I d_yb_I\wedge dy^I=d_y\omega$. Thus the local operators agree on overlaps and define a global [linear map](../../../vector-space.md#linear-map) $d:\Omega^p(M)\to\Omega^{p+1}(M)$.

A second application in any chart gives

$$
d^2\omega=\sum_{I,j,k}(\partial_k\partial_j a_I)\,dx^k\wedge dx^j\wedge dx^I=0,
$$

again by symmetry of mixed derivatives and antisymmetry of the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms). Consequently every [exact differential form](../../../differential-form.md#exact-differential-form) is closed. Put $\Omega^{-1}(M)=0$ and define the [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) by

$$
\boxed{H^p_{\mathrm{dR}}(M)=\frac{\ker(d:\Omega^p\to\Omega^{p+1})}{\operatorname{im}(d:\Omega^{p-1}\to\Omega^p)}.}
$$

The identity $d^2=0$ is exactly what puts the denominator inside the numerator, making this quotient meaningful. Since $\Omega^p(M)=0$ for $p>\dim M$, **$H^p_{\mathrm{dR}}(M)=0$ in those degrees**.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The two components of a [disjoint union](../../../set-theory.md#disjoint-union) are open and closed. Restriction therefore gives an isomorphism

$$
\Omega^p(M)\longrightarrow\Omega^p(U)\oplus\Omega^p(V),\qquad \omega\longmapsto(\omega|_U,\omega|_V).
$$

Its inverse assigns the first form on $U$ and the second on $V$; it is smooth because there are no overlaps on which compatibility must be imposed. The [exterior derivative](../../../differential-form.md#exterior-derivative) is local, so this is an isomorphism of cochain complexes.

A form on $M$ is a [closed differential form](../../../differential-form.md#closed-differential-form) exactly when both restrictions are closed. It is an [exact differential form](../../../differential-form.md#exact-differential-form) exactly when both restrictions are exact: primitives on $U$ and $V$ join into a global primitive. Taking the quotient therefore yields the [de Rham cohomology of a finite disjoint union](../../../differential-form.md#de-rham-cohomology-of-a-finite-disjoint-union):

$$
\boxed{H^p_{\mathrm{dR}}(U\sqcup V)\cong H^p_{\mathrm{dR}}(U)\oplus H^p_{\mathrm{dR}}(V)\qquad(p\ge0).}
$$

The same argument covers degree zero, with the space of degree-minus-one forms taken to be zero.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**The direct-sum assertion fails in both degrees when the pieces overlap.** Take genuine [open covers](../../../topology.md#open-cover), so the failure does not depend on any subtle choice of smooth structures on subsets.

For degree zero, let $M=\mathbb R$, $U=(-\infty,1)$ and $V=(-1,\infty)$. By [degree-zero de Rham cohomology](../../../differential-form.md#degree-zero-de-rham-cohomology), $H^0_{\mathrm{dR}}$ consists of [locally constant functions](../../../calculus.md#locally-constant-function). Each of $M,U,V$ is connected and nonempty, so

$$
H^0_{\mathrm{dR}}(M)=\mathbb R,\qquad H^0_{\mathrm{dR}}(U)\oplus H^0_{\mathrm{dR}}(V)=\mathbb R^2.
$$

They are not isomorphic as real [vector spaces](../../../vector-space.md). The restriction map is $c\mapsto(c,c)$; the overlap forces equality instead of allowing two independent constants.

For degree one, let $M=S^1$, and remove distinct points $a,b$ to form $U=S^1\setminus\{a\}$ and $V=S^1\setminus\{b\}$. Each is diffeomorphic to an [open interval](../../../topology.md#open-interval). Every one-form $f(t)dt$ on an interval has the smooth primitive $\int_{t_0}^t f(s)ds$, so both pieces have zero first [de Rham cohomology](../../../differential-form.md#de-rham-cohomology). On the [circle](../../../topology.md#circle), the form $\eta=x\,dy-y\,dx$ is closed because all two-forms on a one-dimensional manifold vanish. The parameterization $(x,y)=(\cos t,\sin t)$ gives

$$
\int_{S^1}\eta=\int_0^{2\pi}dt=2\pi.
$$

An exact form has zero [integral](../../../calculus.md#integral) around this loop: the [integral](../../../calculus.md#integral) of $dF$ is the difference of the endpoint values of the periodic function $F$. Thus $[\eta]\ne0$, while the proposed right side is zero, disproving the isomorphism.

In fact $H^1_{\mathrm{dR}}(S^1)\cong\mathbb R$. For a periodic one-form $f(t)dt$, subtract $c\,dt$ where $c=(2\pi)^{-1}\int_0^{2\pi}f(t)dt$. The remainder has the periodic primitive $\int_0^t(f(s)-c)ds$, and hence is exact. This also explicitly identifies the nonzero class used above.

## 3

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field) $X$ on a [Lie group](../../../lie-theory.md#lie-group) satisfies

$$
(dL_g)_h X_h=X_{gh}\qquad(g,h\in G),
$$

or equivalently $(L_g)_*X=X$ for every $g$. For $\xi\in T_eG$, define

$$
X^\xi_g=(dL_g)_e\xi.
$$

This is smooth because multiplication is smooth and its differential depends smoothly on the base points. The identity $L_g\circ L_h=L_{gh}$ gives $(dL_g)_hX^\xi_h=X^\xi_{gh}$, so $X^\xi$ is a [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field). Conversely, left invariance forces any such field to have this form with $\xi=X_e$. Evaluation at $e$ and the construction above are inverse [linear maps](../../../vector-space.md#linear-map). Hence

$$
\boxed{T_eG\cong\{\text{left-invariant vector fields on }G\}.}
$$

The [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) is their [commutator](../../../lie-algebra.md#commutator) as [derivations](../../../associative-algebra.md#derivation-of-an-algebra) on [smooth functions](../../../analysis.md#smooth-function): $[X,Y]f=X(Yf)-Y(Xf)$. It is another vector field because the cross terms cancel in the Leibniz rule for its action on a product. The bracket is preserved by a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism): conjugating the [derivation](../../../associative-algebra.md#derivation-of-an-algebra) operators by [pullback of a smooth function](../../../differential-geometry.md#pullback-of-a-smooth-function) preserves their [commutator](../../../lie-algebra.md#commutator). Therefore

$$
(L_g)_*[X,Y]=[(L_g)_*X,(L_g)_*Y]=[X,Y]
$$

for left-invariant $X,Y$. These fields are consequently closed under the bracket.

Transport the bracket to the [tangent space](../../../differential-geometry.md#tangent-space) by

$$
\boxed{[\xi,\eta]_{\mathfrak g}=[X^\xi,X^\eta]_e.}
$$

Bilinearity and antisymmetry come from the [commutator](../../../lie-algebra.md#commutator). The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) follows by expanding the three nested [commutators](../../../lie-algebra.md#commutator) of [derivation](../../../associative-algebra.md#derivation-of-an-algebra) operators: their six terms cancel in pairs. Thus $T_eG$ is a [Lie algebra](../../../lie-algebra.md), and the displayed correspondence is a [Lie algebra isomorphism](../../../lie-algebra.md#lie-algebra-isomorphism) onto the algebra of [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $e$ be the identity. For a [left-invariant differential form](../../../lie-theory.md#left-invariant-differential-form) $\omega$ and a [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field) $X$, one has

$$
\omega_g(X_g)=\omega_g((dL_g)_eX_e)=(L_g^*\omega)_e(X_e)=\omega_e(X_e).
$$

The value is therefore independent of $g$, even if the [Lie group](../../../lie-theory.md#lie-group) is disconnected. The same calculation applies to another left-invariant field $Y$.

The standard [exterior derivative of a one-form evaluated on vector fields](../../../differential-form.md#exterior-derivative-of-a-one-form-evaluated-on-vector-fields) is

$$
d\omega(X,Y)=X(\omega(Y))-Y(\omega(X))-\omega([X,Y]).
$$

Both differentiated functions are constant in the present situation. Thus

$$
\boxed{d\omega(X,Y)=-\omega([X,Y]).}
$$

This identity is a direct consequence of left invariance and the stated general formula for the [exterior derivative](../../../differential-form.md#exterior-derivative).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The correspondence in part (a) respects [Lie brackets](../../../lie-algebra.md#lie-bracket). If the [Lie algebra](../../../lie-algebra.md) is abelian, any two [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) satisfy $[X,Y]=0$ everywhere, not just at the identity. Part (b) therefore gives $d\omega(X,Y)=0$ for every such pair.

At a point $g$, the map $(dL_g)_e:T_eG\to T_gG$ is an isomorphism. Thus every [tangent vector](../../../differential-geometry.md#tangent-vector) at $g$ is the value of a [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field). The two-form $d\omega$ consequently vanishes on every pair of [tangent vectors](../../../differential-geometry.md#tangent-vector) at every point, proving

$$
\boxed{d\omega=0.}
$$

No connectedness assumption on the [Lie group](../../../lie-theory.md#lie-group) is needed: the argument uses its left translations and its [abelian Lie algebra](../../../lie-algebra.md#abelian-lie-algebra).

## 4

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

A connection on $TM$ is a [metric connection](../../../fiber-bundle.md#metric-connection) for $g$ if for all smooth [vector fields](../../../calculus.md#vector-field) $X,Y,Z$,

$$
\boxed{X\bigl(g(Y,Z)\bigr)=g(\nabla_XY,Z)+g(Y,\nabla_XZ).}
$$

Equivalently, its induced [covariant derivative](../../../general-relativity.md#covariant-derivative) of the metric satisfies $\nabla g=0$. This is also called a [metric-compatible connection](../../../fiber-bundle.md#metric-connection).

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

The [torsion tensor](../../../fiber-bundle.md#torsion-tensor) of an [affine connection](../../../fiber-bundle.md#affine-connection) is

$$
T(X,Y)=\nabla_XY-\nabla_YX-[X,Y].
$$

The connection is symmetric, or a [torsion-free connection](../../../fiber-bundle.md#torsion-free-connection), exactly when

$$
\boxed{\nabla_XY-\nabla_YX=[X,Y]\quad\text{for all }X,Y.}
$$

In a coordinate frame, write $\nabla_{\partial_i}\partial_j=\sum_k\Gamma^k_{ij}\partial_k$. Since coordinate fields commute, the condition is $\Gamma^k_{ij}=\Gamma^k_{ji}$; this is the reason for the word symmetric.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

The [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) is the unique [affine connection](../../../fiber-bundle.md#affine-connection) which is both a [metric connection](../../../fiber-bundle.md#metric-connection) and a [torsion-free connection](../../../fiber-bundle.md#torsion-free-connection). Uniqueness is encoded by the Koszul formula

$$
\begin{aligned}
2g(\nabla_XY,Z)={}&Xg(Y,Z)+Yg(X,Z)-Zg(X,Y)\\
&+g([X,Y],Z)-g([Y,Z],X)+g([Z,X],Y).
\end{aligned}
$$

It follows by adding the metric-compatibility identities with derivative fields $X,Y$, subtracting the one with derivative field $Z$, and replacing differences of [covariant derivatives](../../../general-relativity.md#covariant-derivative) by [Lie brackets](../../../lie-algebra.md#lie-bracket). Nondegeneracy of $g$ determines $\nabla_XY$ uniquely from all its pairings with $Z$. The [existence and uniqueness of the Levi-Civita connection](../../../fiber-bundle.md#existence-and-uniqueness-of-the-levi-civita-connection) supplies existence; no existence proof is needed here.

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

In Cartesian coordinates on Euclidean space, define

$$
\boxed{\nabla_XY=\sum_{j=1}^n X(Y^j)\,\partial_j\qquad\text{when }Y=\sum_jY^j\partial_j.}
$$

This is an [affine connection](../../../fiber-bundle.md#affine-connection) by the ordinary product rule. Its [connection coefficients](../../../fiber-bundle.md#connection-components) in this coordinate frame are all zero. The component formula for the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) gives $\nabla_XY-\nabla_YX=[X,Y]$, so it is torsion-free. Also, since the Euclidean metric has constant coefficients,

$$
X\!\left(\sum_jY^jZ^j\right)=\sum_j X(Y^j)Z^j+\sum_jY^jX(Z^j).
$$

This is exactly metric compatibility. By uniqueness it is the Euclidean [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). In particular constant vector fields are parallel, while the derivative of a general field is given by the boxed formula.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In coordinates, write $\nabla_{\partial_i}\partial_\ell=\Gamma^k_{i\ell}\partial_k$. The [Riemannian curvature two-form](../../../fiber-bundle.md#riemannian-curvature-two-form) is defined by the matrices

$$
R^k{}_{\ell ij}=\partial_i\Gamma^k_{j\ell}-\partial_j\Gamma^k_{i\ell}+\Gamma^k_{im}\Gamma^m_{j\ell}-\Gamma^k_{jm}\Gamma^m_{i\ell},
$$

with repeated indices summed. It assigns to $X,Y$ the fiberwise [endomorphism](../../../algebra.md#endomorphism) $R(X,Y)$ whose entries are $R^k{}_{\ell ij}X^iY^j$. We can prove both coordinate independence and the required intrinsic identity as follows.

Define an operator on vector fields by $C(X,Y)=[\nabla_X,\nabla_Y]-\nabla_{[X,Y]}$. It is alternating in $X,Y$. For a [smooth function](../../../analysis.md#smooth-function) $f$, the identities $[fX,Y]=f[X,Y]-Y(f)X$ and $\nabla_Y(fZ)=Y(f)Z+f\nabla_YZ$ give

$$
C(fX,Y)Z=fC(X,Y)Z;
$$

the two terms involving $Y(f)\nabla_XZ$ cancel. Alternation gives linearity over [smooth functions](../../../analysis.md#smooth-function) in $Y$ as well. Expanding in the final argument yields

$$
C(X,Y)(fZ)=fC(X,Y)Z+\bigl(X(Yf)-Y(Xf)-[X,Y]f\bigr)Z=fC(X,Y)Z.
$$

Thus $C$ is tensorial in all three arguments, defining a global [endomorphism](../../../algebra.md#endomorphism)-valued two-form.

For coordinate fields $\partial_i,\partial_j$, their bracket is zero. Expand $[\nabla_{\partial_i},\nabla_{\partial_j}]Z$ using $Z=Z^\ell\partial_\ell$. The second derivatives of $Z^\ell$ cancel by equality of mixed partials. The terms containing first derivatives of $Z^\ell$ cancel in pairs, and the remaining coefficient of $Z^\ell\partial_k$ is exactly $R^k{}_{\ell ij}$ above. Hence the coordinate definition equals the global tensor $C$, establishing coordinate independence and proving

$$
\boxed{R(X,Y)=[\nabla_X,\nabla_Y]-\nabla_{[X,Y]}.}
$$

This convention for the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) is valid for any [affine connection](../../../fiber-bundle.md#affine-connection); in particular it applies to the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Take $\mathbf n$ to be the [unit normal](../../../differential-geometry.md#unit-normal), so $P(v)=v-\langle v,\mathbf n\rangle\mathbf n$ is [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto $TM$. With $D$ the Euclidean [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection), the proposed derivative is

$$
\nabla_XY=P(D_{\widetilde X}\widetilde Y)|_M.
$$

It is a smooth tangent field, and independence of the extensions is given. Linearity follows from linearity of $D$ and $P$. Moreover, for $f\in C^\infty(M)$, take local extensions of $f,X,Y$ to obtain

$$
\nabla_{fX}Y=f\nabla_XY,\qquad \nabla_X(fY)=X(f)Y+f\nabla_XY,
$$

since $PY=Y$. Thus it is an [affine connection](../../../fiber-bundle.md#affine-connection) on $M$.

For tangent fields $Y,Z$, the normal component of $DY$ pairs to zero with $Z$. Differentiating the ambient [inner product](../../../linear-algebra.md#inner-product) along $X$ gives

$$
Xg(Y,Z)=\langle D_XY,Z\rangle+\langle Y,D_XZ\rangle
=g(\nabla_XY,Z)+g(Y,\nabla_XZ).
$$

Hence it is a [metric connection](../../../fiber-bundle.md#metric-connection) for the induced [Riemannian metric](../../../differential-geometry.md#riemannian-metric). The ambient torsion vanishes, so

$$
\nabla_XY-\nabla_YX=P(D_XY-D_YX)=P[X,Y]=[X,Y].
$$

Here the restriction of the ambient bracket is the intrinsic bracket and is tangent to $M$: [derivations](../../../associative-algebra.md#derivation-of-an-algebra) of functions restricted to $M$ give the same bracket, or this follows in submanifold coordinates. Thus the projected derivative is also a [torsion-free connection](../../../fiber-bundle.md#torsion-free-connection). Uniqueness now proves

$$
\boxed{\nabla\text{ is the Levi-Civita connection of the induced metric.}}
$$

This is the [projected ambient connection](../../../fiber-bundle.md#projected-ambient-connection). The projection formula requires a [unit normal](../../../differential-geometry.md#unit-normal). If a nonunit normal is used, its normal term must instead be $\langle DY,\mathbf n\rangle\mathbf n/\langle\mathbf n,\mathbf n\rangle$. For example, on the unit [circle](../../../topology.md#circle), taking $\mathbf n=2p$ and differentiating its unit tangent along itself gives $DY=-p$; the unnormalized printed expression would be $3p$, which is not tangent. Normalizing the normal removes that ambiguity.

## 5

↑ **Parent:** [Paper 17](paper-17.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) is an $\mathbb R$-linear map

$$
\nabla:\Gamma(E)\longrightarrow\Omega^1(M;E)
$$

which satisfies $\nabla(fs)=df\otimes s+f\nabla s$ for every [smooth function](../../../analysis.md#smooth-function) $f$ and section $s$. Here $\Omega^1(M;E)=\Gamma(T^*M\otimes E)$. Equivalently, writing $\nabla_Xs=(\nabla s)(X)$, it is linear over [smooth functions](../../../analysis.md#smooth-function) in $X$, linear over $\mathbb R$ in $s$, and obeys

$$
\nabla_X(fs)=X(f)s+f\nabla_Xs.
$$

Choose a trivializing [open cover](../../../topology.md#open-cover) and a [local frame](../../../fiber-bundle.md#frame-of-a-vector-bundle) $e_{i1},\ldots,e_{ir}$ on each $U_i$. Differentiating the coefficient functions gives a local [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle):

$$
\nabla^i_X\left(\sum_a s^a e_{ia}\right)=\sum_a X(s^a)e_{ia}.
$$

No compatibility of these local connections is assumed. Choose a smooth locally finite [partition of unity](../../../differential-geometry.md#partition-of-unity) $\{\phi_i\}$ subordinate to the cover and define

$$
\boxed{\nabla_Xs=\sum_i\phi_i\nabla^i_X(s|_{U_i}),}
$$

extending each weighted term by zero outside $U_i$. Its support lies inside $U_i$, so each extension is smooth, and local finiteness makes the whole sum smooth. The operation is linear over [smooth functions](../../../analysis.md#smooth-function) in $X$. For the Leibniz rule,

$$
\nabla_X(fs)=\sum_i\phi_i\bigl(X(f)s+f\nabla^i_Xs\bigr)
=X(f)s+f\nabla_Xs,
$$

using $\sum_i\phi_i=1$. This proves **every smooth [vector bundle](../../../fiber-bundle.md#vector-bundle) admits a connection** by the [construction of a vector bundle connection by a partition of unity](../../../fiber-bundle.md#construction-of-a-vector-bundle-connection-by-a-partition-of-unity).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Fix the coefficient-column convention: write the [local frame](../../../fiber-bundle.md#frame-of-a-vector-bundle) as a row $e=(e_1,\ldots,e_r)$ and a section as $s=eu$ for a column $u$ of functions. Define the [connection matrix](../../../fiber-bundle.md#connection-one-form) $\theta=(\theta_{ij})$ by

$$
\nabla e_j=\sum_i e_i\theta_{ij},\qquad \nabla(eu)=e(du+\theta u).
$$

Each entry is a smooth one-form. Define the [curvature form of a connection](../../../fiber-bundle.md#curvature-form) by

$$
R^E(X,Y)s=\nabla_X\nabla_Ys-\nabla_Y\nabla_Xs-\nabla_{[X,Y]}s.
$$

The same Leibniz cancellations as for tangent-bundle curvature show that this is linear over [smooth functions](../../../analysis.md#smooth-function) in $X,Y,s$. Thus it is a two-form with values in the [endomorphisms](../../../algebra.md#endomorphism) of $E$. Its [curvature matrix](../../../fiber-bundle.md#curvature-form) $\Theta=(\Theta_{ij})$ is specified by $R^E(X,Y)e_j=\sum_i e_i\Theta_{ij}(X,Y)$.

The [covariant exterior derivative](../../../fiber-bundle.md#exterior-covariant-derivative) on coefficient forms is $d+\theta\wedge$. Squaring it on $u$ gives

$$
(d+\theta\wedge)^2u=d\theta\,u-\theta\wedge du+\theta\wedge du+\theta\wedge\theta\,u.
$$

Therefore the [Cartan curvature matrix equation](../../../fiber-bundle.md#cartan-curvature-matrix-equation) is

$$
\boxed{\Theta=d\theta+\theta\wedge\theta,\qquad\Theta_{ij}=d\theta_{ij}+\sum_k\theta_{ik}\wedge\theta_{kj}.}
$$

Matrix-valued wedge products here combine [matrix](../../../vector-space.md#matrix) multiplication with the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms), in the stated order.

Using $d^2=0$ and the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule),

$$
d\Theta=d\theta\wedge\theta-\theta\wedge d\theta.
$$

On the other hand, associativity of the [endomorphism-valued exterior product](../../../fiber-bundle.md#endomorphism-valued-exterior-product) gives

$$
\begin{aligned}
\Theta\wedge\theta-\theta\wedge\Theta
&=d\theta\wedge\theta+\theta\wedge\theta\wedge\theta
-\theta\wedge d\theta-\theta\wedge\theta\wedge\theta\\
&=d\theta\wedge\theta-\theta\wedge d\theta.
\end{aligned}
$$

The cubic terms cancel, proving the requested [Bianchi identity](../../../fiber-bundle.md#bianchi-identity)

$$
\boxed{d\Theta=\Theta\wedge\theta-\theta\wedge\Theta.}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let another [local frame](../../../fiber-bundle.md#frame-of-a-vector-bundle) be $e'=eA$ with $A:U\to GL_r(\mathbb R)$ smooth. Since the coefficient columns satisfy $u=Au'$, the Leibniz rule gives the [change of frame of a vector-bundle connection](../../../fiber-bundle.md#change-of-frame-of-a-vector-bundle-connection):

$$
\theta'=A^{-1}\theta A+A^{-1}dA.
$$

The [curvature form of a connection](../../../fiber-bundle.md#curvature-form) is linear over [smooth functions](../../../analysis.md#smooth-function) in its section argument, so its [matrix](../../../vector-space.md#matrix) transforms homogeneously:

$$
\Theta'=A^{-1}\Theta A.
$$

Consequently

$$
\operatorname{tr}\Theta'=\operatorname{tr}(A^{-1}\Theta A)=\operatorname{tr}\Theta.
$$

The entries of $A$ are functions, of degree zero, so ordinary cyclic invariance of [trace](../../../linear-algebra.md#matrix-trace) applies without a graded sign. The local forms therefore glue to a globally defined two-form $\alpha=\operatorname{tr}\Theta$, the [trace of vector-bundle curvature](../../../fiber-bundle.md#trace-of-vector-bundle-curvature).

Apply the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity) proved in part (b):

$$
d\alpha=\operatorname{tr}(\Theta\wedge\theta)-\operatorname{tr}(\theta\wedge\Theta).
$$

For the first term,

$$
\operatorname{tr}(\Theta\wedge\theta)=\sum_{i,j}\Theta_{ij}\wedge\theta_{ji}
=\sum_{i,j}\theta_{ji}\wedge\Theta_{ij}
=\sum_{i,j}\theta_{ij}\wedge\Theta_{ji}
=\operatorname{tr}(\theta\wedge\Theta).
$$

The middle interchange has sign $(-1)^{2\cdot1}=1$, and the next equality simply renames $i,j$. Thus

$$
\boxed{\alpha=\operatorname{tr}\Theta\text{ is frame-independent and }d\alpha=0.}
$$

One can also check closedness locally: the off-diagonal terms in $\operatorname{tr}(\theta\wedge\theta)=\sum_{i,j}\theta_{ij}\wedge\theta_{ji}$ cancel in pairs, while the diagonal terms vanish. Hence $\alpha=d(\operatorname{tr}\theta)$ in each frame, and $d^2=0$ gives the same conclusion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
