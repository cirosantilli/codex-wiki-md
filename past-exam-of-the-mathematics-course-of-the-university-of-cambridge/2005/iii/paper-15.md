# Paper 15

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper15.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper15.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [exterior derivative](../../../differential-form.md#exterior-derivative) is an $\mathbb R$-linear operator $d:\Omega^r(M)\to\Omega^{r+1}(M)$ which agrees with the [differential of a smooth function](../../../differential-geometry.md#differential-of-a-smooth-function) on degree zero, satisfies $d^2=0$, and obeys the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule)

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^r\alpha\wedge d\beta,
\qquad \alpha\in\Omega^r(M).
$$

For the [uniqueness of the exterior derivative from its axioms](../../../differential-form.md#uniqueness-of-the-exterior-derivative-from-its-axioms), first note that these axioms force locality. If $\alpha$ vanishes near $p$, choose a [smooth bump function](../../../partial-differential-equation.md#smooth-bump-function) $\chi$ equal to one near $p$ and supported where $\alpha=0$. Then $0=d(\chi\alpha)=d\chi\wedge\alpha+\chi d\alpha$ gives $d\alpha(p)=0$. Thus $d\alpha(p)$ depends only on the form near $p$.

In a coordinate chart write $\alpha=\sum_I a_I\,dx^{i_1}\wedge\cdots\wedge dx^{i_r}$. Since $d(dx^i)=d^2x^i=0$, the axioms force

$$
d\alpha=\sum_{I,j}\partial_j a_I\,dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_r}.
$$

This also proves existence. Define $d$ by that formula in each chart. The product rule for [partial derivatives](../../../calculus.md#partial-derivative) gives the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule), and symmetry of mixed [partial derivatives](../../../calculus.md#partial-derivative) against antisymmetry of the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms) gives $d^2=0$. On overlaps it still agrees with the differential of every function, by the [chain rule](../../../calculus.md#chain-rule), so the preceding uniqueness argument in the second coordinate system makes the formulas agree. They therefore glue to a global [exterior derivative](../../../differential-form.md#exterior-derivative).

For a [differential one-form](../../../differential-form.md#one-form) $\omega=\sum_i a_i dx^i$, the [exterior derivative of a one-form evaluated on vector fields](../../../differential-form.md#exterior-derivative-of-a-one-form-evaluated-on-vector-fields) follows directly:

$$
d\omega(X,Y)=\sum_i\bigl(X(a_i)Y^i-Y(a_i)X^i\bigr).
$$

In $X(\omega(Y))-Y(\omega(X))$, the additional terms are $\sum_i a_i[X(Y^i)-Y(X^i)]=\omega([X,Y])$, where the bracket is the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields). Hence

$$
\boxed{d\omega(X,Y)=X\bigl(\omega(Y)\bigr)-Y\bigl(\omega(X)\bigr)-\omega([X,Y])}.
$$

The [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) is

$$
H^r_{\mathrm{dR}}(M)=
\frac{\ker(d:\Omega^r(M)\to\Omega^{r+1}(M))}
{\operatorname{im}(d:\Omega^{r-1}(M)\to\Omega^r(M))},
$$

with zero denominator in degree zero. The [Poincaré lemma](../../../differential-form.md#poincare-lemma) states that a [closed differential form](../../../differential-form.md#closed-differential-form) of positive degree on a star-shaped open subset of Euclidean space is an [exact differential form](../../../differential-form.md#exact-differential-form); consequently every closed positive-degree form is locally exact on a [smooth manifold](../../../differential-geometry.md#smooth-manifold).

For the [suspension isomorphism for top de Rham cohomology of spheres](../../../differential-form.md#suspension-isomorphism-for-top-de-rham-cohomology-of-spheres), put $U=S^n\setminus\{\text{south pole}\}$ and $V=S^n\setminus\{\text{north pole}\}$. Both are diffeomorphic to $\mathbb R^n$, while $W=U\cap V$ deformation retracts onto the equatorial $S^{n-1}$. The [Mayer--Vietoris sequence for de Rham cohomology](../../../differential-form.md#mayer-vietoris-sequence-for-de-rham-cohomology) comes from the [short exact sequence](../../../module-theory.md#short-exact-sequence) of [cochain complexes](../../../algebra.md#cochain-complex)

$$
0\longrightarrow\Omega^*(S^n)
\longrightarrow\Omega^*(U)\oplus\Omega^*(V)
\xrightarrow{(\alpha,\beta)\mapsto\alpha|_W-\beta|_W}
\Omega^*(W)\longrightarrow0.
$$

The final map is surjective: a [partition of unity](../../../differential-geometry.md#partition-of-unity) $\chi_U+\chi_V=1$ lets a form $\eta$ on $W$ be lifted by extending $\chi_V\eta$ to $U$ and $-\chi_U\eta$ to $V$ by zero. The [Poincaré lemma](../../../differential-form.md#poincare-lemma) makes $H^{n-1}(U),H^{n-1}(V),H^n(U),H^n(V)$ vanish when $n>1$. Exactness gives

$$
0\longrightarrow H^{n-1}_{\mathrm{dR}}(W)
\xrightarrow{\delta}H^n_{\mathrm{dR}}(S^n)\longrightarrow0.
$$

If $j:S^{n-1}\hookrightarrow W$ is the equatorial inclusion, [homotopy invariance of de Rham cohomology](../../../differential-form.md#homotopy-invariance-of-de-rham-cohomology) makes $j^*$ an [isomorphism](../../../algebra.md#isomorphism). Therefore

$$
\boxed{j^*\delta^{-1}:H^n_{\mathrm{dR}}(S^n)\longrightarrow H^{n-1}_{\mathrm{dR}}(S^{n-1})}
$$

is injective, indeed an [isomorphism](../../../algebra.md#isomorphism). Concretely, choose local primitives $d\alpha_U=\omega|_U$, $d\alpha_V=\omega|_V$, and send $[\omega]$ to $[j^*(\alpha_U-\alpha_V)]$. Their difference is closed; changing either primitive changes it by an exact form, so this agrees with the cohomological construction.

## 2

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A $d$-dimensional [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) $F\subseteq M^m$ has the subspace topology and, near each of its points, a [manifold chart](../../../differential-geometry.md#manifold-chart) identifying it with a coordinate slice $\mathbb R^d\times\{0\}$. These [slice charts for an embedded submanifold](../../../differential-geometry.md#slice-chart-for-an-embedded-submanifold) give its smooth structure, and its inclusion is a [smooth embedding](../../../differential-geometry.md#smooth-embedding).

A [regular value](../../../differential-geometry.md#regular-value) $q\in N^n$ of a [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds) $f:M^m\to N^n$ is one for which $df_p:T_pM\to T_qN$ is [surjective](../../../algebra.md#surjective-function) at every $p\in f^{-1}(q)$. If the preimage is nonempty this forces $m\geq n$.

The [inverse function theorem](../../../calculus.md#inverse-function-theorem) used here says that if $G:U\subseteq\mathbb R^m\to\mathbb R^m$ is smooth and $DG_p$ is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), then its restriction to a suitable neighbourhood of $p$ is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) onto an open neighbourhood of $G(p)$, with smooth inverse.

To prove the [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem), fix $p\in f^{-1}(q)$ and choose coordinates centred at $p,q$. The coordinate representative $\widetilde f$ has a rank-$n$ [Jacobian matrix](../../../calculus.md#jacobian-matrix). After permuting domain coordinates, its first $n$ columns form an [invertible matrix](../../../linear-algebra.md#invertible-matrix). Define

$$
G(x)=\bigl(\widetilde f^1(x),\ldots,\widetilde f^n(x),x^{n+1},\ldots,x^m\bigr).
$$

Its [Jacobian matrix](../../../calculus.md#jacobian-matrix) is block triangular with invertible diagonal blocks, so the [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes $G$ a local coordinate change. In these coordinates, $f^{-1}(q)$ is precisely the slice with first $n$ coordinates zero. Thus it is an [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) of dimension $m-n$, with

$$
\boxed{T_p f^{-1}(q)=\ker df_p}.
$$

An empty preimage is harmless; the local assertion is then vacuous.

Three [equivalent formulations of orientability of a smooth manifold](../../../differential-geometry.md#equivalent-formulations-of-orientability-of-a-smooth-manifold) are: an [oriented atlas](../../../differential-geometry.md#oriented-atlas) whose transition [Jacobian determinants](../../../calculus.md#jacobian-determinant) are positive; a smoothly varying [orientation of a vector space](../../../linear-algebra.md#orientation-of-a-vector-space) on each [tangent space](../../../differential-geometry.md#tangent-space); and a nowhere-vanishing smooth top-degree [differential form](../../../differential-form.md). An oriented atlas gives compatible oriented coordinate frames. A [partition of unity](../../../differential-geometry.md#partition-of-unity) glues their positive local top forms, and a nonzero top form declares a frame positive precisely when it evaluates positively on that frame. These constructions prove the equivalence.

For the [orientability of a regular fibre](../../../differential-geometry.md#orientability-of-a-regular-fibre), write $F=f^{-1}(q)$. The derivative gives a [short exact sequence](../../../module-theory.md#short-exact-sequence) of [vector bundles](../../../fiber-bundle.md#vector-bundle)

$$
0\longrightarrow TF\longrightarrow TM|_F
\xrightarrow{df}F\times T_qN\longrightarrow0.
$$

This is the reason the [normal bundle of a regular fibre is trivial](../../../differential-geometry.md#normal-bundle-of-a-regular-fibre-is-trivial). Choose any fixed positive basis $b_1,\ldots,b_n$ of $T_qN$ and an ambient orientation on $M$. Declare a frame $v_1,\ldots,v_{m-n}$ of $T_pF$ positive when

$$
\widetilde b_1,\ldots,\widetilde b_n,v_1,\ldots,v_{m-n}
$$

is positive in $T_pM$, where $df_p(\widetilde b_i)=b_i$. Changing a lift adds a tangent vector and leaves the [determinant](../../../linear-algebra.md#determinant) sign unchanged. Local smooth lifts exist because $df$ is surjective, so this rule varies smoothly and agrees on overlaps. It gives a global orientation on $F$. Only an orientation of the single vector space $T_qN$ was chosen; $N$ itself need not be orientable.

## 3

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An [orthogonal structure on a real vector bundle](../../../fiber-bundle.md#orthogonal-structure-on-a-real-vector-bundle) $E$ of rank $r$ is a choice of local frames whose transition matrices lie in the [orthogonal group](../../../linear-algebra.md#orthogonal-group) $O(r)$. In such frames declare

$$
h\left(\sum_i a_ie_i,\sum_i b_ie_i\right)=\sum_i a_ib_i.
$$

Orthogonal transitions preserve this expression, so it defines a smooth positive-definite [fiber metric](../../../fiber-bundle.md#fiber-metric). Conversely, a [fiber metric](../../../fiber-bundle.md#fiber-metric) turns any local frame into a smooth orthonormal frame by the [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process); the resulting transition matrices are orthogonal. The two constructions are inverse, giving the required equivalence.

An [orthogonal local trivialization](../../../fiber-bundle.md#orthogonal-local-trivialization) $E|_U\cong U\times\mathbb R^r$ identifies each fiber isometrically with standard Euclidean space. Equivalently, its coordinate frame satisfies $h(e_i,e_j)=\delta_{ij}$. This is local and does not assert the existence of a global frame.

Every real [vector bundle](../../../fiber-bundle.md#vector-bundle) over a [smooth manifold](../../../differential-geometry.md#smooth-manifold) admits a [fiber metric](../../../fiber-bundle.md#fiber-metric). Choose a trivializing open cover and local Euclidean metrics $h_i$. The [partition of unity](../../../differential-geometry.md#partition-of-unity) theorem for a Hausdorff second-countable smooth manifold supplies nonnegative smooth functions $\rho_i$, with locally finite supports contained in the respective cover members, such that $\sum_i\rho_i=1$. Set

$$
h=\sum_i\rho_i h_i,
$$

extending each weighted metric by zero off its chart. Local finiteness makes this smooth. For every nonzero fiber vector $v$, at least one positive weight gives $h(v,v)=\sum_i\rho_i h_i(v,v)>0$. Thus $h$ is a [fiber metric](../../../fiber-bundle.md#fiber-metric) and provides an [orthogonal structure](../../../fiber-bundle.md#orthogonal-structure-on-a-real-vector-bundle).

One definition of an [orthogonal connection](../../../fiber-bundle.md#metric-connection) is that its [covariant derivative](../../../general-relativity.md#covariant-derivative) preserves the [fiber metric](../../../fiber-bundle.md#fiber-metric):

$$
X\bigl(h(s,t)\bigr)=h(\nabla_Xs,t)+h(s,\nabla_Xt)
$$

for all [vector fields](../../../calculus.md#vector-field) $X$ and smooth [sections of a vector bundle](../../../fiber-bundle.md#section-of-a-vector-bundle) $s,t$. Another is that its [parallel transport](../../../fiber-bundle.md#parallel-transport) along every smooth curve is an [isometry](../../../riemannian-geometry.md#isometry) between the endpoint fibers.

For the first implication, take parallel sections $s,t$ along a curve. Their covariant derivatives vanish, so the displayed identity makes $h(s,t)$ constant: [parallel transport preserves a fibre metric](../../../fiber-bundle.md#parallel-transport-preserves-a-fibre-metric). Conversely, if parallel transport preserves the [inner product](../../../linear-algebra.md#inner-product), choose parallel extensions of arbitrary initial fiber vectors along a curve with prescribed initial tangent $X$. Differentiating their constant inner product gives $(\nabla_Xh)(s,t)=0$ at the initial point. Since $X,s,t$ were arbitrary, the connection is [metric-compatible](../../../fiber-bundle.md#metric-connection).

The equivalent local description is that the [connection matrix in an orthonormal frame is skew-symmetric](../../../fiber-bundle.md#connection-matrix-in-an-orthonormal-frame-is-skew-symmetric). Writing $\nabla e_j=\sum_i A^i{}_j e_i$ in an [orthogonal trivialization](../../../fiber-bundle.md#orthogonal-local-trivialization), differentiate $h(e_i,e_j)=\delta_{ij}$ to obtain

$$
\boxed{A^i{}_j+A^j{}_i=0,\qquad A^T=-A}.
$$

Conversely this matrix identity gives the metric-preservation formula by expanding arbitrary sections. It is the [orthogonal group](../../../linear-algebra.md#orthogonal-group) connection description of the same condition.

## 4

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $D$ be the ambient [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) and $\nabla$ the one for the [induced metric](../../../riemannian-geometry.md#induced-metric) on $M$. The [Gauss formula](../../../second-fundamental-form.md#gauss-formula) is

$$
D_XY=\nabla_XY+II(X,Y),
$$

where the [second fundamental form](../../../second-fundamental-form.md) $II(X,Y)=(D_XY)^\perp$ is normal. The tangential part of $D$ is [metric-compatible](../../../fiber-bundle.md#metric-connection) and [torsion-free](../../../fiber-bundle.md#torsion-free-connection), so the [existence and uniqueness of the Levi-Civita connection](../../../fiber-bundle.md#existence-and-uniqueness-of-the-levi-civita-connection) identifies it with $\nabla$.

For a normal field $\xi$, the [Weingarten formula](../../../second-fundamental-form.md#weingarten-formula) defines the [shape operator in a normal direction](../../../second-fundamental-form.md#shape-operator-in-a-normal-direction) $A_\xi$ and the [normal connection](../../../fiber-bundle.md#normal-connection) by

$$
D_X\xi=-A_\xi X+\nabla_X^\perp\xi.
$$

Differentiate $\langle\xi,Y\rangle=0$ using metric compatibility to get

$$
\langle A_\xi X,Y\rangle=\langle II(X,Y),\xi\rangle.
$$

The [symmetry of the second fundamental form](../../../second-fundamental-form.md#symmetry-of-the-second-fundamental-form) follows from the ambient torsion-free condition:

$$
II(X,Y)-II(Y,X)=\bigl(D_XY-D_YX-[X,Y]\bigr)^\perp=0,
$$

since the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) tangent to $M$ is tangent. Therefore

$$
\boxed{\langle A_\xi X,Y\rangle=\langle X,A_\xi Y\rangle},
$$

so every normal-direction [shape operator](../../../second-fundamental-form.md#shape-operator) is [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator).

The paper uses $R(X,Y)=D_{[X,Y]}-[D_X,D_Y]$, so use the [Gauss equation with reversed curvature convention](../../../second-fundamental-form.md#gauss-equation-with-reversed-curvature-convention). Applying the [Gauss formula](../../../second-fundamental-form.md#gauss-formula) and [Weingarten formula](../../../second-fundamental-form.md#weingarten-formula) twice gives

$$
(D_XD_YZ)^\top=\nabla_X\nabla_YZ-A_{II(Y,Z)}X.
$$

Subtracting in the stated curvature order yields

$$
(R^V(X,Y)Z)^\top=R^M(X,Y)Z+A_{II(Y,Z)}X-A_{II(X,Z)}Y.
$$

Pair with a tangent field $W$ and use the defining relation for the [shape operator in a normal direction](../../../second-fundamental-form.md#shape-operator-in-a-normal-direction):

$$
\boxed{\langle R^M(X,Y)Z,W\rangle
=\langle R^V(X,Y)Z,W\rangle
-\langle II(X,W),II(Y,Z)\rangle
+\langle II(Y,W),II(X,Z)\rangle}.
$$

This is the [Gauss equation](../../../second-fundamental-form.md#gauss-equation) in the supplied sign convention. If one defines curvature by $[D_X,D_Y]-D_{[X,Y]}$ instead, the two quadratic terms have the opposite signs.

For an [orthonormal frame](../../../general-relativity.md#orthonormal-frame-in-spacetime) $X,Y$ on a surface, positive [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) with the convention here is $K=\langle R^M(X,Y)X,Y\rangle$. If the ambient space is Euclidean and $\xi$ is a unit normal, the equation becomes

$$
K=\langle II(X,X),II(Y,Y)\rangle-\|II(X,Y)\|^2
=\boxed{\det A_\xi}.
$$

The [Koszul formula](../../../fiber-bundle.md#koszul-formula) determines $\nabla$ from the [induced metric](../../../riemannian-geometry.md#induced-metric), and hence determines its [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) and $K$. Therefore the [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) depends only on that metric, even though its expression as a product of [principal curvatures](../../../second-fundamental-form.md#principal-curvature) appears extrinsic. This is [Theorema Egregium](../../../differential-geometry.md#theorema-egregium).

## 5

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use the standard boundaryless-manifold convention, so $M$ is a [closed manifold](../../../differential-geometry.md#closed-manifold). Its orientation and [Riemannian metric](../../../differential-geometry.md#riemannian-metric) determine a unique positive [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form) $\mu_g$ taking value one on every positively oriented [orthonormal frame](../../../general-relativity.md#orthonormal-frame-in-spacetime). In an [oriented atlas](../../../differential-geometry.md#oriented-atlas) it is

$$
\mu_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n.
$$

For the [coordinate invariance of the Riemannian volume form](../../../differential-geometry.md#coordinate-invariance-of-the-riemannian-volume-form), on an overlap put $J=\partial y/\partial x$. Then $g_x=J^Tg_yJ$ and $dy^1\wedge\cdots\wedge dy^n=(\det J)dx^1\wedge\cdots\wedge dx^n$. The oriented transition has $\det J>0$, so the square root of the metric determinant and the coordinate volume transform together. The local forms therefore agree and define $\mu_g$ globally.

For real $r$-forms the [Hodge star operator](../../../differential-form.md#hodge-star-operator) is defined by

$$
\alpha\wedge*\beta=\langle\alpha,\beta\rangle_g\mu_g.
$$

The pointwise wedge pairing is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form), so this uniquely defines a smooth map $*:\Omega^r(M)\to\Omega^{n-r}(M)$. On an oriented orthonormal coframe, it sends a basis wedge to the signed complementary wedge. Applying it twice gives

$$
*^2\alpha=(-1)^{r(n-r)}\alpha.
$$

For [Hodge star eigenvalues on graded differential forms](../../../differential-form.md#hodge-star-eigenvalues-on-graded-differential-forms), extend $*$ complex-linearly to the direct sum of all form degrees. This interpretation matters: on a fixed degree it is an [endomorphism](../../../algebra.md#endomorphism) only in middle degree. In positive odd dimension, $r(n-r)$ is even for every $r$, so $*^2=I$ and only $\pm1$ can occur. Both occur, with eigenforms $1+\mu_g$ and $1-\mu_g$.

In positive even dimension, $*^2$ is $+I$ on even-degree forms and $-I$ on odd-degree forms. Hence $*^4=I$ and the only possible [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\pm1,\pm i$. The first two occur as above. For the latter, choose a smooth local [orthonormal frame](../../../general-relativity.md#orthonormal-frame-in-spacetime) and multiply its first dual [differential one-form](../../../differential-form.md#one-form) by a nonzero [smooth bump function](../../../partial-differential-equation.md#smooth-bump-function) supported in the chart. This gives a form $\eta$ for which $\eta$ and $*\eta$ are independent. For $\lambda=\pm i$,

$$
*\bigl(\eta+\lambda^{-1}*\eta\bigr)
=\lambda\bigl(\eta+\lambda^{-1}*\eta\bigr).
$$

Thus all four occur. Consequently, for $n\geq1$,

$$
\boxed{\operatorname{Spec}(*)=
\begin{cases}
\{1,-1\},&n\text{ odd},\\
\{1,-1,i,-i\},&n\text{ even}.
\end{cases}}
$$

On degree $m$ in dimension $2m$, the [Hodge star](../../../differential-form.md#hodge-star-operator) has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\pm1$ for even $m$ and $\pm i$ for odd $m$; signed complementary middle-degree wedges show both occur for $m\geq1$. In zero dimensions it is multiplication by the signed unit volume at each point, so only the signs actually present occur.

For [Hodge integration by parts in arbitrary degree](../../../differential-form.md#hodge-integration-by-parts-in-arbitrary-degree), let $\alpha\in\Omega^{r-1}(M)$ and $\beta\in\Omega^r(M)$. The [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) and [Stokes theorem](../../../calculus.md#stokes-theorem) on the closed manifold give

$$
0=\int_M d(\alpha\wedge*\beta)
=\int_Md\alpha\wedge*\beta+(-1)^{r-1}\int_M\alpha\wedge d*\beta.
$$

Using the given [codifferential](../../../differential-form.md#codifferential) and the square of the [Hodge star](../../../differential-form.md#hodge-star-operator),

$$
*\delta\beta
=(-1)^{n(r+1)+1+(n-r+1)(r-1)}d*\beta
=(-1)^r d*\beta.
$$

Therefore

$$
\boxed{\langle d\alpha,\beta\rangle_{L^2}
=\int_Md\alpha\wedge*\beta
=\int_M\alpha\wedge*\delta\beta
=\langle\alpha,\delta\beta\rangle_{L^2}},
$$

which proves that $\delta$ is the [formal adjoint](../../../hilbert-space.md#formal-adjoint) of $d$. The complex version inserts conjugation in the usual [Hermitian inner product](../../../linear-algebra.md#hermitian-form).

The [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem) gives an $L^2$-orthogonal decomposition

$$
\Omega^k(M)=\mathcal H^k(M)\oplus d\Omega^{k-1}(M)\oplus\delta\Omega^{k+1}(M),
$$

where $\mathcal H^k(M)=\ker\Delta$ is finite dimensional and consists of the [harmonic differential forms](../../../differential-form.md#harmonic-differential-form). Each [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class has a unique harmonic representative. Equivalently, with harmonic projection $P_{\mathcal H}$ there is a smooth [Green operator of the Hodge Laplacian](../../../differential-form.md#green-operator-of-the-hodge-laplacian) $G$ satisfying $\Delta G=G\Delta=I-P_{\mathcal H}$.

The [solvability condition for the Hodge Poisson equation](../../../differential-form.md#solvability-condition-for-the-hodge-poisson-equation) is

$$
\boxed{\Delta\alpha=\beta\text{ is solvable}\quad\Longleftrightarrow\quad
\langle\beta,h\rangle_{L^2}=0\text{ for every }h\in\mathcal H^k(M)}.
$$

Necessity follows from $\langle\Delta\alpha,h\rangle=\langle\alpha,\Delta h\rangle=0$. Conversely the orthogonality condition gives $P_{\mathcal H}\beta=0$, so $\alpha_0=G\beta$ solves the [Poisson equation for differential forms](../../../differential-form.md#poisson-equation-for-differential-forms).

The [nonnegativity of the Hodge Laplacian](../../../differential-form.md#nonnegativity-of-the-hodge-laplacian) identity

$$
\langle\Delta\eta,\eta\rangle_{L^2}=\|d\eta\|_{L^2}^2+\|\delta\eta\|_{L^2}^2
$$

identifies its kernel with closed and coclosed forms. Thus the [affine space of solutions of the Hodge Poisson equation](../../../differential-form.md#affine-space-of-solutions-of-the-hodge-poisson-equation) is

$$
\boxed{\alpha_0+\mathcal H^k(M)}.
$$

For completeness, if a closed form is decomposed as $\omega=h+d\xi+\delta\zeta$, then $d\delta\zeta=0$, and $\|\delta\zeta\|^2=\langle\zeta,d\delta\zeta\rangle=0$. Hence its cohomology class is represented by $h$. An exact harmonic form $h=d\xi$ must vanish, since $\|h\|^2=\langle\delta h,\xi\rangle=0$. This proves the canonical [isomorphism](../../../algebra.md#isomorphism) $\mathcal H^k(M)\cong H^k_{\mathrm{dR}}(M)$, so the solution set is an [affine space](../../../geometry-and-topology.md#affine-space) whose translation [vector space](../../../vector-space.md) is isomorphic to the requested [de Rham cohomology](../../../differential-form.md#de-rham-cohomology).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
