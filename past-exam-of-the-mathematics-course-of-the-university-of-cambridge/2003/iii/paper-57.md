# Paper 57

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper57.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper57.pdf)

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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
    - [iii](#6/a/iii)
      - [Solution](#6/a/iii/solution)
    - [iv](#6/a/iv)
      - [Solution](#6/a/iv/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
- [7](#7)
  - [Solution](#7/solution)

## 1

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $M$ be an oriented smooth $m$-dimensional [manifold with boundary](../../../differential-geometry.md#manifold-with-boundary) and $\alpha$ a smooth compactly supported $(m-1)$-[differential form](../../../differential-form.md). Give $\partial M$ the outward-normal-first [orientation](../../../algebraic-topology.md#orientation-of-a-simplex). A [partition of unity](../../../differential-geometry.md#partition-of-unity) subordinate to oriented interior and boundary charts reduces the proof to a compactly supported form on $\mathbb R^m$ or on a half-space. Indeed $\alpha=\sum_j\chi_j\alpha$, so $d\alpha=\sum_jd(\chi_j\alpha)$; the sum of terms involving $d\chi_j$ is zero. [Exterior derivative](../../../differential-form.md#exterior-derivative) commutes with chart [pullbacks](../../../category.md#pullback-category-theory), so each summand can be calculated in coordinates.

Write the local form as

$$
\alpha=\sum_{j=1}^m(-1)^{j-1}f_j\,dx^1\wedge\cdots\wedge\widehat{dx^j}\wedge\cdots\wedge dx^m,
\qquad d\alpha=\left(\sum_j\partial_jf_j\right)dx^1\wedge\cdots\wedge dx^m.
$$

For an interior chart, integrate each derivative using the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus): its integral is zero because $f_j$ has compact support. For a boundary chart modeled on $x^m\geq0$, all tangential derivatives again integrate to zero, while $\int_0^\infty\partial_mf_m\,dx^m=-f_m(x',0)$. The outward normal is $-\partial_m$; its contraction with the volume form gives exactly this sign in the induced boundary integral of $\alpha$. Summing the chart identities proves the [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem):

$$
\boxed{\int_Md\alpha=\int_{\partial M}\alpha.}
$$

Compact support can be replaced by compactness of $M$; on a noncompact [manifold](../../../topology.md#topological-manifold), sufficient support or convergence conditions are necessary.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Keep the metric and hence the [Hodge star](../../../differential-form.md#hodge-star-operator) fixed. Write $\alpha=\delta A$, so $\delta F=d\alpha$, and use the [Bianchi identity for an Abelian p-form](../../../relativistic-quantum-field.md#bianchi-identity-for-an-abelian-p-form) $dF=d^2A=0$. The bilinear pairing $U\wedge\star V$ on real four-forms is symmetric even for a fixed indefinite metric. Consequently the variation of the kinetic term is $d\alpha\wedge\star F$.

The two differentiated four-form factors in the cubic term have the same sign, since moving a four-form through another four-form or through a three-form contributes an even exponent. Thus

$$
\delta(F\wedge F\wedge A)=2d\alpha\wedge F\wedge A+\alpha\wedge F\wedge F.
$$

The [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) gives

$$
d(\alpha\wedge\star F)=d\alpha\wedge\star F-\alpha\wedge d\star F,
\qquad
d(\alpha\wedge F\wedge A)=d\alpha\wedge F\wedge A-\alpha\wedge F\wedge F.
$$

Using the [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem), the complete [first variation](../../../calculus-of-variations.md#first-variation) is therefore

$$
\delta S=\int_M\alpha\wedge(d\star F+3F\wedge F)
+\int_{\partial M}(\alpha\wedge\star F+2\alpha\wedge F\wedge A).
$$

For compactly supported variations, a closed $M$, or boundary conditions removing this last term, the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) and the [Bianchi identity for an Abelian p-form](../../../relativistic-quantum-field.md#bianchi-identity-for-an-abelian-p-form) are

$$
\boxed{d\star F+3F\wedge F=0,\qquad dF=0.}
$$

The coefficient three follows from the normalization actually present in the action; inserting a differently normalized supergravity coupling would change it. This is the [eleven-dimensional three-form action variation](../../../differential-form.md#eleven-dimensional-three-form-action-variation).

Under the [gauge transformation](../../../electromagnetism.md#gauge-transformation) $A\mapsto A+d\Lambda$, the four-form $F$ is unchanged because $d^2\Lambda=0$. The kinetic density is unchanged, and the cubic density changes by

$$
F\wedge F\wedge d\Lambda=d(F\wedge F\wedge\Lambda).
$$

It is an exact eleven-form, so the action changes only by a boundary integral. The [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) depend only on $F$ and are invariant even when this boundary integral is nonzero. Invariance of the action itself additionally requires suitable boundary or support conditions.

## 2

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Choose a basis $T_a$ of the [Lie algebra](../../../lie-algebra.md), with $[T_b,T_c]=c^a{}_{bc}T_a$. On the [Matrix Lie group](../../../lie-theory.md#matrix-lie-group) set

$$
\lambda=g^{-1}dg=T_a\lambda^a,\qquad \rho=dg\,g^{-1}=T_a\rho^a.
$$

Left multiplication by a constant matrix preserves $\lambda$, while right multiplication preserves $\rho$. Differentiating $g^{-1}g=I$ gives $d(g^{-1})=-g^{-1}(dg)g^{-1}$. Apply the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) to obtain

$$
d\lambda=-\lambda\wedge\lambda,
\qquad d\rho=+\rho\wedge\rho.
$$

Because the [wedge product](../../../linear-algebra.md#exterior-product) antisymmetrizes the matrix products, these [Maurer-Cartan equations](../../../lie-theory.md#maurer-cartan-equation) become

$$
\boxed{d\lambda^a=-\tfrac12c^a{}_{bc}\lambda^b\wedge\lambda^c,
\qquad d\rho^a=+\tfrac12c^a{}_{bc}\rho^b\wedge\rho^c.}
$$

Follow the vector-field naming used in the question: $L_a(g)=T_ag$ is right-invariant and generates left multiplication, whereas $R_a(g)=gT_a$ is left-invariant and generates right multiplication. They are dual to $\rho^a$ and $\lambda^a$, respectively. For any [one-form](../../../differential-form.md#one-form) $\eta$, $d\eta(X,Y)=X(\eta(Y))-Y(\eta(X))-\eta([X,Y])$. Evaluating the two [Maurer-Cartan equations](../../../lie-theory.md#maurer-cartan-equation) on the corresponding invariant fields yields

$$
\boxed{[L_a,L_b]=-c^c{}_{ab}L_c,\qquad[R_a,R_b]=c^c{}_{ab}R_c,\qquad[L_a,R_b]=0.}
$$

For the last identity, the left and right multiplication flows commute. The opposite sign for the [right-invariant vector fields](../../../lie-theory.md#right-invariant-vector-field) is therefore intrinsic; the letters attached to the two families are only a convention.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $B(X,Y)=\operatorname{tr}(\operatorname{ad}X\operatorname{ad}Y)$ be the [Killing form](../../../lie-algebra.md#killing-form). A real [semisimple Lie algebra](../../../semisimple-lie-algebra.md) has nondegenerate $B$, and its invariance gives $B([X,Y],Z)=B(X,[Y,Z])$. Translating $B$ defines a [bi-invariant pseudo-Riemannian metric](../../../lie-theory.md#bi-invariant-pseudo-riemannian-metric) $g=B$ on the [Lie group](../../../lie-theory.md#lie-group).

For [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field), all derivatives of their pairwise inner products vanish. The [Koszul formula](../../../fiber-bundle.md#koszul-formula) reduces to

$$
2B(\nabla_XY,Z)=B([X,Y],Z)-B([Y,Z],X)+B([Z,X],Y)=B([X,Y],Z).
$$

Nondegeneracy gives $\nabla_XY=[X,Y]/2$. With $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$, the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) now gives

$$
R(X,Y)Z=-\tfrac14[[X,Y],Z].
$$

Taking the trace of $X\mapsto R(X,Y)Z=-\tfrac14\operatorname{ad}Z\operatorname{ad}Y(X)$ yields the [Ricci tensor](../../../general-relativity.md#ricci-tensor)

$$
\boxed{\operatorname{Ric}(Y,Z)=-\tfrac14 B(Y,Z)=-\tfrac14 g(Y,Z).}
$$

Thus the [Killing-form Einstein metric](../../../lie-theory.md#killing-form-einstein-metric) makes the group an [Einstein manifold](../../../second-fundamental-form.md#einstein-manifold), allowing an indefinite metric. Its [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) in this convention is $-\dim G/4$.

For a connected compact [semisimple Lie group](../../../lie-theory.md#semisimple-lie-group), $B$ is negative definite: the adjoint operators are skew-adjoint for an invariant positive inner product, so $B(X,X)=\operatorname{tr}((\operatorname{ad}X)^2)<0$ for $X\ne0$. The conventional positive [Riemannian metric](../../../differential-geometry.md#riemannian-metric) is instead $g_+=-B$. Its [Ricci tensor](../../../general-relativity.md#ricci-tensor) is $g_+/4$, and its [sectional curvature](../../../second-fundamental-form.md#sectional-curvature) is

$$
K_{g_+}(X,Y)=\frac{\|[X,Y]\|_{g_+}^2}{4(\|X\|_{g_+}^2\|Y\|_{g_+}^2-\langle X,Y\rangle_{g_+}^2)}\geq0.
$$

It can vanish on commuting two-planes; positivity is not automatic in every direction. With the literal negative metric $B$, the corresponding sectional-curvature signs are reversed.

For a noncompact real semisimple group, a Cartan decomposition $\mathfrak g=\mathfrak k\oplus\mathfrak p$ has $B$ negative on $\mathfrak k$ and positive on $\mathfrak p$. The [Killing metric](../../../lie-theory.md#killing-form-einstein-metric) is indefinite and cannot be made positive by an overall sign. Its Einstein constant remains $-1/4$ for $g=B$, but that does not assert a uniform sign for sectional curvature of all nondegenerate planes. For connected semisimple groups, negative-definite $B$ characterizes the compact case. Disconnected groups require a separate condition on the number of components before compactness follows.

## 3

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [Poisson manifold](../../../symplectic-geometry.md#poisson-manifold) is a smooth [manifold](../../../topology.md#topological-manifold) $P$ with a bilinear bracket on $C^\infty(P)$ that is antisymmetric, satisfies the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) and obeys $\{f,gh\}=\{f,g\}h+g\{f,h\}$. Equivalently it has a [bivector](../../../linear-algebra.md#bivector) $\Pi$ defining $\{f,g\}=\Pi(df,dg)$ with vanishing Schouten bracket $[\Pi,\Pi]$; nondegeneracy is not required.

For a [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold), define the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) by $\iota_{X_f}\omega=df$ and put $\{f,g\}=\omega(X_f,X_g)$. Nondegeneracy gives a unique $X_f$, antisymmetry is inherited from $\omega$, and $d(gh)=g\,dh+h\,dg$ proves the [Leibniz rule](../../../calculus.md#leibniz-rule). Moreover $\mathcal L_{X_f}\omega=d\iota_{X_f}\omega+\iota_{X_f}d\omega=0$ by [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula). Since $X_fg=-\{f,g\}$,

$$
\iota_{[X_f,X_g]}\omega=\mathcal L_{X_f}(\iota_{X_g}\omega)=d(X_fg)=-d\{f,g\},
\qquad [X_f,X_g]=-X_{\{f,g\}}.
$$

For completeness, evaluate $d\omega=0$ on $X_f,X_g,X_h$. Its three derivative terms sum to minus the cyclic sum of $\{f,\{g,h\}\}$, and its three bracket terms sum to minus the same cyclic sum, using the displayed identity. Hence that sum is zero. This proves the [Jacobi identity for the Poisson bracket](../../../classical-mechanics.md#jacobi-identity-for-the-poisson-bracket), not merely the Jacobi identity modulo constants. The inverse of a closed nondegenerate two-form therefore defines a [Poisson manifold](../../../symplectic-geometry.md#poisson-manifold).

The [Symplectic Darboux theorem](../../../symplectic-geometry.md#darboux-theorem-symplectic-geometry) says that near every point of a $2n$-dimensional [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) there are coordinates $(q^1,\ldots,q^n,p_1,\ldots,p_n)$ with

$$
\boxed{\omega=\sum_{i=1}^n dq^i\wedge dp_i,\qquad
\{f,g\}=\sum_i\left(\frac{\partial f}{\partial q^i}\frac{\partial g}{\partial p_i}-\frac{\partial f}{\partial p_i}\frac{\partial g}{\partial q^i}\right).}
$$

Thus every symplectic structure has the same local normal form, despite possible global topological differences.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For the graph embedding $\iota(q)=(q,p(q))$, pull back the [symplectic form](../../../symplectic-geometry.md#symplectic-form) in [Darboux coordinates](../../../symplectic-geometry.md#darboux-chart):

$$
\iota^*\omega=\sum_{i,j}\frac{\partial p_i}{\partial q^j}\,dq^i\wedge dq^j
=\sum_{i<j}\left(\frac{\partial p_i}{\partial q^j}-\frac{\partial p_j}{\partial q^i}\right)dq^i\wedge dq^j.
$$

The coordinate two-forms are linearly independent. The graph has dimension $n$, so it is a [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) exactly when this [pullback](../../../category.md#pullback-category-theory) vanishes, equivalently when its displayed coefficient matrix is symmetric.

Let $\theta_L=\sum_i p_i(q)dq^i$. Then $d\theta_L=-\iota^*\omega$, so the same condition says that $\theta_L$ is a [closed differential form](../../../differential-form.md#closed-differential-form). On a sufficiently small contractible coordinate neighborhood the [Poincaré lemma](../../../differential-form.md#poincare-lemma) supplies $S$ with $\theta_L=dS$. Consequently

$$
\boxed{p_i=\partial_iS.}
$$

One explicit primitive on a star-shaped neighborhood of $q_0$ is $S(q)=S(q_0)+\int_0^1p_i(q_0+t(q-q_0))(q^i-q_0^i)\,dt$. Differentiate it and use $\partial_jp_i=\partial_ip_j$ to recognize the derivative of $t p_j(q_0+t(q-q_0))$; the result is $\partial_jS=p_j(q)$. Conversely $p=dS$ has symmetric mixed derivatives and gives a [Lagrangian graph](../../../symplectic-geometry.md#lagrangian-graph). This construction requires the local projection to the $q$ coordinates to be nonsingular. A general [Lagrangian submanifold](../../../symplectic-geometry.md#lagrangian-submanifold) need not be such a graph in a preassigned chart, and a closed one-form on a larger domain need not be globally exact.

## 4

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A smooth [principal bundle](../../../fiber-bundle.md#principal-bundle) with structure [Lie group](../../../lie-theory.md#lie-group) $G$ can be specified by a locally trivial map $\pi:E\to B$ whose fiber coordinate changes have the form $(x,g)_i\mapsto(x,h_{ji}(x)g)_j$, with the usual [transition functions of a principal bundle](../../../fiber-bundle.md#transition-function-of-a-principal-bundle) cocycle on triple overlaps. In each chart define $(x,g)\cdot k=(x,gk)$. On overlaps, $h_{ji}(x)(gk)=(h_{ji}(x)g)k$, so these local right actions agree. They therefore give a global smooth right [group action](../../../group-theory.md#group-action), free and transitive on every fiber. Equivalently, this action together with equivariant local triviality is the definition of a [principal bundle](../../../fiber-bundle.md#principal-bundle).

Use five-dimensional [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) with ambient metric $\eta=\operatorname{diag}(-1,1,1,1,1)$ and realize unit-radius [de Sitter spacetime](../../../general-relativity.md#de-sitter-spacetime) as $\eta(x,x)=1$. Its [tangent space](../../../differential-geometry.md#tangent-space) is $x^\perp$, of Lorentzian signature $(3,1)$. An oriented [pseudo-orthonormal frame](../../../fiber-bundle.md#pseudo-orthonormal-frame) $(e_0,e_1,e_2,e_3)$ of $x^\perp$, together with the last column $x$, is precisely a matrix

$$
g=(e_0,e_1,e_2,e_3,x)\in SO(4,1).
$$

Conversely the last column of such a matrix lies on the hyperboloid, and its other columns give that frame. Thus

$$
\boxed{SO(4,1)\longrightarrow\mathrm{dS}_4,
\qquad g\longmapsto ge_4,\qquad G=SO(3,1).}
$$

Right multiplication by $\operatorname{diag}(h,1)$ fixes $x$ and changes the tangent frame by $h$. It is free and transitive on frames over $x$, proving the [principal bundle](../../../fiber-bundle.md#principal-bundle) description. Smooth local choices of frames provide its local trivializations. The dimensions are $10=4+6$.

This is the [oriented frame bundle of de Sitter spacetime](../../../fiber-bundle.md#oriented-frame-bundle-of-de-sitter-spacetime). Allowing orientation reversal gives $O(4,1)$ and structure group $O(3,1)$; imposing a time orientation as well selects $SO_0(4,1)$ and $SO_0(3,1)$. For radius $a$, take the last column $x/a$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For a [principal bundle](../../../fiber-bundle.md#principal-bundle) $\pi:E\to B$, the vertical space is $V_e=\ker d\pi_e$. A [principal connection](../../../fiber-bundle.md#connection-principal-bundle) specifies smooth complements $T_eE=H_e\oplus V_e$ with $(R_g)_*H_e=H_{eg}$. Equivalently its Lie-algebra-valued connection one-form $\mathcal A$ satisfies $\mathcal A(\xi_E)=\xi$ and $R_g^*\mathcal A=\operatorname{Ad}_{g^{-1}}\mathcal A$. Every base vector has a unique [horizontal lift](../../../fiber-bundle.md#horizontal-lift) because $d\pi:H_e\to T_{\pi(e)}B$ is an isomorphism. A base curve lifts from a chosen initial fiber point by solving $\mathcal A(\dot e)=0$; this defines [parallel transport](../../../fiber-bundle.md#parallel-transport). Closed curves can give nontrivial [holonomy](../../../fiber-bundle.md#holonomy), and failure of horizontal fields to close under brackets is measured by the [curvature of a principal connection](../../../fiber-bundle.md#curvature-of-a-principal-connection).

For a smooth strictly convex [rigid body](../../../classical-mechanics.md#rigid-body-dynamics), assume contact with the plane is unique and varies smoothly with orientation. Write a configuration as $(R,c_{\parallel})\in SO(3)\times\mathbb R^2$. Contact determines the reference point's height $h(R)$, so the full reference position is $c=(c_{\parallel},h(R))$. Let $r(R)$ be the spatial vector from that point to the contacting material point and let $\widehat\Omega=\dot R R^{-1}$ encode the spatial [angular velocity](../../../classical-mechanics.md#angular-velocity). The instantaneous contact velocity is

$$
v_{\mathrm{contact}}=\dot c+\Omega\times r(R).
$$

The no-slip condition is its vanishing. Its vertical component follows already from differentiating contact: the normal component of the changing contact point along the body surface is zero, giving $\dot h=-(\Omega\times r)_z$. The two remaining equations are

$$
\dot c_{\parallel}=-(\Omega\times r(R))_{\parallel}.
$$

Translations of $c_{\parallel}$ define a free right $\mathbb R^2$ action, with quotient $SO(3)$. The [translational connection for a convex body rolling on a plane](../../../fiber-bundle.md#translational-connection-for-a-convex-body-rolling-on-a-plane) is

$$
\boxed{\mathcal A=dc_{\parallel}+(\Omega\times r(R))_{\parallel}.}
$$

Here $\Omega$ denotes the vector-valued right [Maurer-Cartan form](../../../lie-theory.md#maurer-cartan-form) on $SO(3)$. This one-form is invariant under translations and returns a translation vector on a vertical translation, so it satisfies both [principal connection](../../../fiber-bundle.md#connection-principal-bundle) axioms. A prescribed orientation path has the unique rolling [horizontal lift](../../../fiber-bundle.md#horizontal-lift)

$$
c_{\parallel}(t)=c_{\parallel}(0)-\int_0^t(\Omega(s)\times r(R(s)))_{\parallel}\,ds.
$$

This is a kinematic connection; inertia and gravity determine which of the allowed paths is dynamically realized.

For a sphere of radius $a$, $r=-a n$, where $n$ is the upward unit normal. The same no-slip condition gives $\dot c_{\parallel}=a\Omega\times n$. It leaves the component $\Omega\cdot n$ arbitrary. If one additionally forbids twisting about $n$, then $\Omega=n\times\dot c_{\parallel}/a$ and a plane path uniquely lifts to an orientation path by $\dot R=\widehat\Omega R$. This is the familiar $SO(3)$ [principal connection](../../../fiber-bundle.md#connection-principal-bundle) over the plane; its horizontal lifts have noncommuting rotation generators and hence nonzero [curvature](../../../differential-geometry.md#curvature). No-slip alone does not supply that latter two-dimensional horizontal distribution. Corners or nonsmooth changes of contact require piecewise treatment rather than the smooth bundle construction.

## 5

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Write $\xi_P(p)=\left.\frac d{dt}\right|_0\exp(t\xi)\cdot p$ for the [fundamental vector field](../../../lie-theory.md#fundamental-vector-field) of a left [Lie group action](../../../lie-theory.md#lie-group-action), and use $\iota_{X_f}\omega=df$ throughout. Such fundamental fields satisfy $[\xi_P,\eta_P]=-[\xi,\eta]_P$. A [moment map](../../../symplectic-geometry.md#moment-map) has linear components $\mu_\xi=\langle\mu,\xi\rangle$ satisfying

$$
d\mu_\xi=\iota_{\xi_P}\omega.
$$

For the action to be [Hamiltonian](../../../classical-mechanics.md#hamiltonian), these components can be chosen equivariantly, or, infinitesimally,

$$
\boxed{\{\mu_\xi,\mu_\eta\}=\mu_{[\xi,\eta]}.}
$$

This identifies the span of the component Hamiltonians with the Lie algebra image, rather than identifying the entire infinite-dimensional [Poisson algebra](../../../algebra.md#poisson-algebra) $C^\infty(P)$ with $\mathfrak g$. For an actual isomorphism with $\mathfrak g$, injectivity is also needed; a faithful infinitesimal action supplies it.

Preservation of $\omega$ alone gives $d\iota_{\xi_P}\omega=0$, not necessarily exactness. For example, translation generated by $\partial_q$ on the symplectic two-torus has contraction $dp$, whose period is nonzero. That action has no globally defined component Hamiltonian. Once the contractions are exact, choose Hamiltonians linearly in $\xi$. On each connected component of $P$, the discrepancy

$$
\kappa(\xi,\eta)=\{\mu_\xi,\mu_\eta\}-\mu_{[\xi,\eta]}
$$

is constant: apply $[X_f,X_g]=-X_{\{f,g\}}$ and the fundamental-field bracket. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) makes $\kappa$ a [Lie algebra two-cocycle](../../../lie-algebra.md#lie-algebra-two-cocycle). Replacing $\mu_\xi$ by $\mu_\xi+b(\xi)$ changes it to $\kappa(\xi,\eta)-b([\xi,\eta])$. Thus the exactness condition and vanishing of this [moment-map equivariance obstruction](../../../symplectic-geometry.md#moment-map-equivariance-obstruction) are precisely the required infinitesimal conditions.

For a [semisimple Lie algebra](../../../semisimple-lie-algebra.md), both hold. First [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) gives

$$
\iota_{[\xi_P,\eta_P]}\omega=d(\iota_{\xi_P}\iota_{\eta_P}\omega)
=-d[\omega(\xi_P,\eta_P)],
\qquad \iota_{[\xi,\eta]_P}\omega=d[\omega(\xi_P,\eta_P)].
$$

Semisimplicity implies $[\mathfrak g,\mathfrak g]=\mathfrak g$, so every generator is a sum of commutators and has a globally exact contraction. This proves [Hamiltonian existence for a semisimple symplectic action](../../../symplectic-geometry.md#hamiltonian-existence-for-a-semisimple-symplectic-action).

Next use the nondegenerate [Killing form](../../../lie-algebra.md#killing-form) to define $D$ by $B(D\xi,\eta)=\kappa(\xi,\eta)$. Antisymmetry makes $D$ skew for $B$. The cocycle identity and invariance of $B$ imply $D[\xi,\eta]=[D\xi,\eta]+[\xi,D\eta]$, so $D$ is a derivation. Choose $Z$ by

$$
B(Z,\xi)=\operatorname{tr}(D\operatorname{ad}\xi).
$$

Then, using cyclicity of trace and $[D,\operatorname{ad}\xi]=\operatorname{ad}(D\xi)$,

$$
B([Z,\xi],\eta)=\operatorname{tr}(D[\operatorname{ad}\xi,\operatorname{ad}\eta])
=\operatorname{tr}([D,\operatorname{ad}\xi]\operatorname{ad}\eta)=B(D\xi,\eta).
$$

Hence $D=\operatorname{ad}Z$ and $\kappa(\xi,\eta)=B(Z,[\xi,\eta])$. Taking $b(\xi)=B(Z,\xi)$ removes the cocycle and proves [semisimple moment-map equivariance](../../../symplectic-geometry.md#semisimple-moment-map-equivariance) without merely invoking a cohomology theorem. For a connected group, integrate the infinitesimal equivariance along its one-parameter subgroups to obtain group equivariance. A disconnected group can require an additional discrete-equivariance check.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $\mu:P\to\mathbb R$ be the [moment map](../../../symplectic-geometry.md#moment-map) for the [circle group](../../../lie-theory.md#circle-group), assume $c$ is a [regular value](../../../differential-geometry.md#regular-value), and assume the circle action on $N=\mu^{-1}(c)$ is free. The action is proper because the circle is compact. Then $N$ has dimension $2n-1$ and $P_c=N/SO(2)$ is a smooth [manifold](../../../topology.md#topological-manifold) of dimension $2n-2$.

If $\xi_P$ generates the action, $\omega(\xi_P,v)=d\mu(v)=0$ for every $v\in TN$. In fact $(TN)^\omega$ is exactly the line spanned by $\xi_P$, since $TN=\ker d\mu$ is a hyperplane and $\omega$ is nondegenerate. Therefore the kernel of the restricted two-form is precisely the orbit direction. The restriction is invariant and horizontal, so it descends to a unique nondegenerate closed two-form $\omega_c$ with

$$
\boxed{\pi^*\omega_c=\iota^*\omega.}
$$

This proves the [Marsden-Weinstein theorem](../../../symplectic-geometry.md#marsden-weinstein-theorem) in the circle case. If the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) $H$ is invariant, then $\{\mu,H\}=0$: its [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) stays on $N$, projects to the quotient and is generated there by the descended function $H_c$. This is a reduced [Hamiltonian system](../../../classical-mechanics.md#hamiltonian-system) in $2n-2$ local variables. At a critical level or a nonfree orbit the quotient can be singular, so the smooth dimension assertion needs the stated hypotheses.

For a mass-$m$ particle in the plane with [central force](../../../physics.md#central-force) potential $V(r)$, work on $r>0$ and write

$$
p_xdx+p_ydy=p_rdr+\ell d\theta,\quad
p_r=\frac{xp_x+yp_y}{r},\quad \ell=xp_y-yp_x.
$$

Exterior differentiation gives $\omega=dr\wedge dp_r+d\theta\wedge d\ell$. Rotation translates $\theta$ and has [moment map](../../../symplectic-geometry.md#moment-map) $\ell$. Fix $\ell=\ell_0$ and quotient out $\theta$ to obtain the [planar rotational symplectic reduction](../../../symplectic-geometry.md#planar-rotational-symplectic-reduction)

$$
\boxed{\omega_{\mathrm{red}}=dr\wedge dp_r,\qquad
H_{\mathrm{red}}=\frac{p_r^2}{2m}+\frac{\ell_0^2}{2mr^2}+V(r).}
$$

The reduced equations are $\dot r=p_r/m$ and $\dot p_r=\ell_0^2/(mr^3)-V'(r)$. The centrifugal term arises from the conserved angular momentum; it is not an extra force imposed by hand. Reconstruct the angle from $\dot\theta=\ell_0/(mr^2)$. For $\ell_0\ne0$ the origin cannot lie on the level; for $\ell_0=0$ the same local reduction holds away from the origin, while the full phase-space origin is a singular fixed orbit.

## 6

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

Identify $\mathbb R^3$ with the traceless [Hermitian matrices](../../../hilbert-space.md#hermitian-operator) $X=x\cdot\sigma$, where $\sigma_i$ are the [Pauli matrices](../../../algebra.md#pauli-matrices). Then $\det X=-|x|^2$. For $U\in SU(2)$ the action $X\mapsto UXU^\dagger$ preserves trace, Hermiticity and determinant, so gives an orthogonal transformation of $\mathbb R^3$. Since $SU(2)$ is connected, the determinant of this transformation is $+1$.

An element in the kernel commutes with every $\sigma_i$, hence is scalar. Unitarity and determinant one restrict it to $\pm I$. Every three-dimensional rotation is a rotation through some angle $\theta$ around a unit axis $n$. It is obtained by

$$
U=\exp(-i\theta\,n\cdot\sigma/2)=\cos(\theta/2)I-i\sin(\theta/2)n\cdot\sigma.
$$

Indeed multiplication with $\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k$ gives the [Rodrigues rotation formula](../../../mathematics.md#rodrigues-rotation-formula) for $UXU^\dagger$. This proves surjectivity, not just equality of Lie-algebra dimensions. Therefore

$$
\boxed{SU(2)/\{\pm I\}\cong SO(3).}
$$

A full $2\pi$ rotation lifts from $I$ to $-I$, explaining the double cover and the [Spin group](../../../semisimple-lie-algebra.md#spin-group) interpretation.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

On the three-dimensional vector space of real symmetric matrices, write

$$
X=\begin{pmatrix}t+x&y\\y&t-x\end{pmatrix},\qquad -\det X=x^2+y^2-t^2.
$$

The [special linear group](../../../group-theory.md#special-linear-group) acts by $X\mapsto AXA^T$, preserving this [quadratic form](../../../linear-algebra.md#quadratic-form) when $\det A=1$. A kernel element satisfies $AA^T=I$ and commutes with every symmetric matrix, so it is scalar and equals $\pm I$. Its derivative is injective: if $aX+Xa^T=0$ for every symmetric $X$, taking $X=I$ makes $a$ skew-symmetric, and commuting with diagonal matrices then makes $a=0$.

Both real [Lie group](../../../lie-theory.md#lie-group) dimensions are three. The derivative is consequently an isomorphism, so the image is an open subgroup. The source $SL(2,\mathbb R)$ is connected: polar decomposition deforms it onto $SO(2)$, with the positive symmetric determinant-one factor contractible. Its image is thus the full identity component $SO_0(2,1)$, since a connected group has no proper open subgroup. This is the [symmetric-matrix double cover of SO0(2,1)](../../../semisimple-lie-algebra.md#symmetric-matrix-double-cover-of-so0-2-1).

For $J=\left(\begin{smallmatrix}0&1\\-1&0\end{smallmatrix}\right)$, direct multiplication gives $A^TJA=(\det A)J$. Hence preserving the two-dimensional [symplectic form](../../../symplectic-geometry.md#symplectic-form) is exactly the determinant-one condition, so

$$
\boxed{SO_0(2,1)\cong SL(2,\mathbb R)/\{\pm I\}\cong Sp(2,\mathbb R)/\{\pm I\}.}
$$

The subscript zero is necessary. The full $SO(2,1)$ also contains a component reversing time orientation, which cannot be the image of the connected source.

<h4 id="6/a/iii">iii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/a/iii)

Use the four-dimensional real vector space of [Hermitian matrices](../../../hilbert-space.md#hermitian-operator)

$$
X=tI+x\cdot\sigma=\begin{pmatrix}t+x_3&x_1-ix_2\\x_1+ix_2&t-x_3\end{pmatrix},
\qquad \det X=t^2-|x|^2.
$$

For $A\in SL(2,\mathbb C)$, $X\mapsto AXA^\dagger$ preserves determinant, hence defines a [Lorentz transformation](../../../special-relativity.md#lorentz-transformation). Positive definite $X$ stays positive definite, so future timelike vectors remain future timelike. Connectedness also fixes the orientation, giving an image in $SO_0(3,1)$.

If the action is trivial, $X=I$ makes $A$ unitary. The remaining condition says it commutes with every Hermitian matrix, forcing $A=\lambda I$ with $\lambda^2=1$. Infinitesimally $aX+Xa^\dagger=0$ first makes $a$ anti-Hermitian and then scalar; tracelessness forces $a=0$. Both real Lie-algebra dimensions are six, so the image is open. Polar decomposition shows $SL(2,\mathbb C)$ is connected, with connected unitary factor $SU(2)$ and a contractible positive Hermitian determinant-one factor. The image is therefore the full proper orthochronous [Lorentz group](../../../special-relativity.md#lorentz-group).

$$
\boxed{SL(2,\mathbb C)/\{\pm I\}\cong SO_0(3,1).}
$$

This is the [Hermitian-matrix double cover of SO0(3,1)](../../../semisimple-lie-algebra.md#hermitian-matrix-double-cover-of-so0-3-1). The full determinant-one [Lorentz group](../../../special-relativity.md#lorentz-group) also contains transformations reversing time orientation, so the identity-component qualification cannot be omitted.

<h4 id="6/a/iv">iv</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/a/iv)

Let $V=\mathbb R^4$ have [symplectic basis](../../../linear-algebra.md#symplectic-basis) $(e_1,f_1,e_2,f_2)$. Fix $\mathrm{vol}=e_1\wedge f_1\wedge e_2\wedge f_2$ and define a symmetric [bilinear form](../../../linear-algebra.md#bilinear-form) $Q$ on $\Lambda^2V$ by $u\wedge v=Q(u,v)\mathrm{vol}$. The pairings between complementary basis bivectors split this six-dimensional space into three hyperbolic planes, so $Q$ has signature $(3,3)$.

The [symplectic group](../../../symplectic-geometry.md#symplectic-group) preserves volume and the bivector $\Omega=e_1\wedge f_1+e_2\wedge f_2$, obtained from the inverse symplectic form, up to its fixed sign convention. Since $Q(\Omega,\Omega)=2$, its orthogonal complement $W=\Omega^\perp$ has dimension five and signature $(2,3)$. On $W$ use $-Q$, which has signature $(3,2)$. This constructs the [exterior-square double cover of SO0(3,2)](../../../semisimple-lie-algebra.md#exterior-square-double-cover-of-so0-3-2).

If an element acts trivially on $W$, it also fixes $\Omega$, so its action on the entire [exterior square](../../../linear-algebra.md#exterior-square) is the identity. Every decomposable bivector then shows that its two-plane is preserved. A line is the intersection of two such planes; hence every line is preserved, and the matrix is scalar. Its exterior-square action forces its scalar square to equal one, giving precisely $\pm I$.

The derivative is injective by the same infinitesimal argument: zero action on $\Lambda^2V$ forces an infinitesimal scalar, whose induced scalar there is twice its value and therefore zero. The [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra) has dimension $2^2+2(2\cdot3/2)=10$, from blocks $\left(\begin{smallmatrix}A&B\\C&-A^T\end{smallmatrix}\right)$ with symmetric $B,C$. The orthogonal Lie algebra in five dimensions also has dimension ten. Thus the image is open. Real symplectic polar decomposition has connected compact factor $U(2)$ and a contractible positive symplectic factor, so $Sp(4,\mathbb R)$ is connected and its image is exactly the identity component:

$$
\boxed{Sp(4,\mathbb R)/\{\pm I\}\cong SO_0(3,2).}
$$

As in the preceding noncompact cases, this does not identify the quotient with the disconnected full $SO(3,2)$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Every matrix in $SU(2)$ has the unique form

$$
U=\begin{pmatrix}\alpha&\beta\\-\overline\beta&\overline\alpha\end{pmatrix},\qquad |\alpha|^2+|\beta|^2=1.
$$

The four real coordinates of $(\alpha,\beta)$ give a smooth bijection with smooth inverse onto the unit [three-sphere](../../../geometry-and-topology.md#three-sphere). Matrix multiplication identifies this model with the [unit quaternions](../../../algebra.md#unit-quaternion). Its round metric is invariant under left and right multiplication by unit quaternions. The action

$$
(a,b):q\longmapsto aqb^{-1}
$$

has kernel $\{(1,1),(-1,-1)\}$: a kernel pair must have $a=b$ from $q=1$ and must commute with all quaternions. Its derivative is injective, and both dimensions are six, giving

$$
\boxed{\operatorname{Isom}_0(S^3)=SO(4)\cong(SU(2)\times SU(2))/\{\pm(I,I)\}.}
$$

The full [isometry group](../../../riemannian-geometry.md#isometry-group) is $O(4)$. Quaternion conjugation reverses orientation and supplies the additional component. Thus an arbitrary isometry has either the displayed left-right form or that form composed with conjugation.

For the [Anti-de Sitter spacetime](../../../general-relativity.md#anti-de-sitter-spacetime) model, write

$$
M=\begin{pmatrix}x_0+x_1&x_2+x_3\\x_2-x_3&x_0-x_1\end{pmatrix},\qquad
-\det M=-x_0^2-x_3^2+x_1^2+x_2^2.
$$

The hyperboloid with this quadratic form equal to $-1$ is exactly $SL(2,\mathbb R)$. Its induced Lorentzian metric is preserved by $M\mapsto AMB^{-1}$ for $A,B\in SL(2,\mathbb R)$. At the identity the metric is $g(U,V)=\tfrac12\operatorname{tr}(UV)$ on traceless matrices, so it is the [Killing metric](../../../lie-theory.md#killing-form-einstein-metric) divided by eight. This proves the geometric identification, including the metric rather than only the underlying manifold.

A trivial left-right action again forces $A=B$ to be a scalar commuting with all determinant-one matrices, hence $A=B=\pm I$. The differential is injective and both dimensions are six, so

$$
\boxed{\operatorname{Isom}_0(\mathrm{AdS}_3)=SO_0(2,2)
\cong(SL(2,\mathbb R)\times SL(2,\mathbb R))/\{\pm(I,I)\}.}
$$

This is the existing [left-right double cover of SO0(2,2)](../../../general-relativity.md#left-right-double-cover-of-so0-2-2). The full hyperboloid [isometry group](../../../riemannian-geometry.md#isometry-group) is $O(2,2)$. Its other components can be obtained by also using $M\mapsto M^T$ and $M\mapsto CMC^{-1}$, $C=\operatorname{diag}(1,-1)$. Transposition reverses one timelike coordinate; conjugation by $C$ reverses one timelike and one spacelike coordinate, so these generate the four component classes. All isometries of these constant-curvature quadrics come from ambient orthogonal transformations: a value and an orthonormal derivative at one point determine an isometry, and the ambient group realizes every such choice.

Here $\mathrm{AdS}_3$ means the hyperboloid with periodic time. The physically common causally unwrapped spacetime is its [universal cover](../../../algebraic-topology.md#universal-cover), modeled by the [universal covering Lie group](../../../lie-theory.md#universal-covering-lie-group) of $SL(2,\mathbb R)$, and is not itself $SL(2,\mathbb R)$. Its isometries lift the above local symmetries, with the global covering and central identifications changed accordingly.

## 7

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

[Geometric quantization](../../../symplectic-geometry.md#geometric-quantization) constructs quantum state spaces from the geometry of a classical [symplectic manifold](../../../symplectic-geometry.md#symplectic-manifold) $(P,\omega)$. Its first task is to represent classical [observables](../../../quantum-mechanics.md#observable) and their [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) by operators; its second is to reduce the excessive phase-space dependence of the resulting states. These are different steps, called [prequantization](../../../symplectic-geometry.md#prequantization) and choice of a [polarization in geometric quantization](../../../symplectic-geometry.md#polarization-in-geometric-quantization).

Use $\iota_{X_f}\omega=df$ and $\{f,g\}=\omega(X_f,X_g)$, so $[X_f,X_g]=-X_{\{f,g\}}$. A [prequantum line bundle](../../../symplectic-geometry.md#prequantum-line-bundle) is a Hermitian complex [line bundle](../../../ringed-space.md#line-bundle) $L\to P$ with unitary [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) of curvature

$$
F_\nabla=\frac{i}{\hbar}\omega.
$$

Its existence requires the integrality of all symplectic periods:

$$
\boxed{\frac1{2\pi\hbar}\int_\Sigma\omega\in\mathbb Z\quad\text{for every integral closed two-cycle }\Sigma.}
$$

One way to see the obstruction is to choose local primitives $\omega=-d\theta_i$ on contractible charts. The local connections are $d-i\theta_i/\hbar$. On overlaps the differences of $\theta_i$ are exact and determine unitary transition phases. On triple overlaps their exponentials obey the cocycle condition exactly when the periods have the stated integral values. Conversely that integral class is realized by a line bundle; adjusting a connection by a global one-form makes its curvature equal to the prescribed representative. Connections with this curvature can still differ by a flat connection, so integrality need not specify unique quantum data.

On smooth sections define the [Kostant-Souriau prequantum operator](../../../symplectic-geometry.md#kostant-souriau-prequantum-operator)

$$
\widehat f=-i\hbar\nabla_{X_f}+f.
$$

Its defining algebraic property follows directly from the curvature commutator:

$$
[\nabla_{X_f},\nabla_{X_g}]=-\nabla_{X_{\{f,g\}}}+\frac{i}{\hbar}\{f,g\}.
$$

The multiplication terms contribute $-i\hbar(X_fg-X_gf)=2i\hbar\{f,g\}$, so

$$
\boxed{[\widehat f,\widehat g]=i\hbar\widehat{\{f,g\}},\qquad\widehat1=I.}
$$

The preliminary inner product integrates the Hermitian pairing against the [symplectic volume](../../../symplectic-geometry.md#symplectic-volume) $\omega^n/n!$, where $\dim P=2n$. Hamiltonian flows preserve this measure, so real observables give formally symmetric operators on suitable compactly supported sections. Actual self-adjoint realizations and their domains require analysis, especially on a noncompact phase space.

The prequantum representation is generally reducible and depends on all $2n$ variables, whereas a configuration-space wave function should depend on $n$. A [polarization in geometric quantization](../../../symplectic-geometry.md#polarization-in-geometric-quantization) is an involutive complex rank-$n$ distribution $\mathcal F\subset T_\mathbb CP$ that is isotropic for $\omega$. A real polarization is tangent to a [Lagrangian foliation](../../../symplectic-geometry.md#lagrangian-foliation); a compatible complex polarization is supplied by a [Kähler manifold](../../../complex-geometry.md#kahler-manifold). Polarized sections satisfy

$$
\nabla_Xs=0\quad(X\in\mathcal F).
$$

This condition is locally consistent because the connection curvature vanishes on pairs of polarization vectors, and involutivity closes the differential constraints. Globally, leaf holonomy can obstruct nonzero polarized sections. To construct the quantum [Hilbert space](../../../hilbert-space.md), one must also choose the appropriate quotient measure or density data and complete the polarized sections; it need not be a literal closed subspace of the original phase-space $L^2$ space.

For $P=T^*\mathbb R^n$, set $\theta=\sum_jp_jdq^j$, so $\omega=-d\theta$ and the line bundle is trivial with $\nabla=d-i\theta/\hbar$. The vertical polarization is spanned by $\partial_{p_j}$. Its equations say $\partial_{p_j}\psi=0$, hence $\psi=\psi(q)$. Before this restriction,

$$
\widehat f=-i\hbar X_f+f-\theta(X_f),\quad
\widehat q^j=i\hbar\partial_{p_j}+q^j,\quad
\widehat p_j=-i\hbar\partial_{q^j}.
$$

After restricting and using the configuration-space measure, the [Schrödinger representation](../../../lie-algebra.md#schrodinger-representation-of-the-heisenberg-group) is

$$
\boxed{\mathcal H=L^2(\mathbb R^n,dq),\qquad
\widehat q^j\psi=q^j\psi,\quad \widehat p_j\psi=-i\hbar\partial_{q^j}\psi.}
$$

Their commutator is $i\hbar\delta^j{}_k$ on a common smooth test-function domain. Functions of $q$ act by multiplication. Observables affine in momenta have flows preserving this polarization and can act directly, with density terms when required for symmetry. An arbitrary observable does not: already $p^2/(2m)$ has a flow taking a vertical fiber to a slanted one. Thus merely restricting its prequantum operator does not produce the free Schrödinger Hamiltonian.

The [Blattner-Kostant-Sternberg pairing](../../../symplectic-geometry.md#blattner-kostant-sternberg-pairing) compares different polarizations. One can transport a state by a Hamiltonian flow to its transported polarization, pair back with the chosen state space and differentiate to obtain additional operators when the pairing is well defined. The [metaplectic correction](../../../symplectic-geometry.md#metaplectic-correction) tensors polarized sections with a suitable square root of the polarization's canonical bundle. Half-forms improve the invariant state pairing and contribute to operator transport; their global existence is additional data.

A closed real-polarization leaf illustrates the topological restriction. Since $\omega$ vanishes along a [Lagrangian leaf](../../../symplectic-geometry.md#lagrangian-leaf), the restricted prequantum connection is flat. A nonzero parallel section exists around a closed loop only if its holonomy is trivial. In cotangent coordinates this is

$$
\exp\left(\frac i\hbar\oint p\,dq\right)=1,
\qquad \oint p\,dq=2\pi\hbar N.
$$

This is the [Bohr-Sommerfeld quantization condition](../../../quantum-mechanics.md#bohr-sommerfeld-quantization) before the half-form correction. With the standard Maslov correction it becomes $\oint p\,dq=2\pi\hbar(N+\nu/4)$, where $\nu$ is the [Maslov index](../../../symplectic-geometry.md#maslov-index). For an oscillator ellipse, the enclosed phase-space area is $2\pi E/\omega_0$ and the index is two; the corrected rule gives $E_N=\hbar\omega_0(N+1/2)$ for $N\geq0$, exhibiting the zero-point shift. Singular real polarizations can require distributional sections rather than ordinary smooth polarized sections.

The construction thus separates local operator algebra from global integrality, polarization and holonomy. It recovers familiar quantum representations while exposing their geometric choices. A polarization also limits which observables preserve the state space, and exact Poisson-to-commutator correspondence cannot in general be extended to every classical polynomial in an irreducible canonical quantization. Changes of polarization, operator domains, half-form existence and singular reductions are substantive issues, so geometric quantization is a framework with specified additional data rather than a unique automatic procedure for every classical system.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
