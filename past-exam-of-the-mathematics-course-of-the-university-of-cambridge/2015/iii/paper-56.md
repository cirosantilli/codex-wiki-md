# Paper 56

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_56.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_56.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Rescale the ambient coordinates by $q_i=a_i r_i$. For each $i\in\{1,\ldots,n+1\}$ and $\varepsilon\in\{1,-1\}$, take the relatively open set $U_i^\varepsilon$ where $\varepsilon q_i>0$. Define a [manifold chart](../../../differential-geometry.md#manifold-chart) by retaining all the $q_j$ except $q_i$:

$$
\phi_i^\varepsilon(r)=(q_1,\ldots,\widehat{q_i},\ldots,q_{n+1})\in B^n.
$$

Here $B^n$ is the open unit [open unit ball](../../../functional-analysis.md#open-unit-ball). The inverse of this [manifold chart](../../../differential-geometry.md#manifold-chart) is explicit:

$$
r_j=\frac{x_j}{a_j}\quad(j\ne i),\qquad r_i=\frac{\varepsilon}{a_i}\sqrt{1-\sum_{j\ne i}x_j^2}.
$$

The coordinate labels in $x$ retain their original indices. All the $a_i$ are nonzero, so this inverse exists; the strictly positive radicand makes it smooth on the whole open [open unit ball](../../../functional-analysis.md#open-unit-ball). Projection and this inverse are continuous, so each [manifold chart](../../../differential-geometry.md#manifold-chart) is a [homeomorphism](../../../topology.md#homeomorphism) onto an open subset of $\mathbb R^n$.

These $2(n+1)$ [manifold charts](../../../differential-geometry.md#manifold-chart) cover the [ellipsoid](../../../geometry-and-topology.md#ellipsoid), because at every point at least one $q_i$ is nonzero. On an overlap with a different chart $U_j^\eta$, the coordinates of $\phi_j^\eta\circ(\phi_i^\varepsilon)^{-1}$ are the retained $x_k$ for $k\ne i,j$ together with

$$
q_i=\varepsilon\sqrt{1-\sum_{k\ne i}x_k^2}.
$$

Its domain is the open subset $\eta x_j>0$ of $B^n$. The displayed functions, and the reverse transition functions obtained by exchanging $i,j$, are smooth. Transitions between identical charts are the identity; opposite-sign charts with the same omitted coordinate do not overlap. The ambient subspace topology is [Hausdorff](../../../topology.md#hausdorff-space) and [second countable](../../../topology.md#second-countable-space), as it is inherited from Euclidean space. Thus this [coordinate-projection atlas of an ellipsoid](../../../geometry-and-topology.md#coordinate-projection-atlas-of-an-ellipsoid) is a [smooth atlas](../../../differential-geometry.md#smooth-atlas), proving **the ellipsoid is a smooth manifold of dimension $n$**. The rescaling $r\mapsto q$ also gives a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) with the unit [sphere](../../../geometry-and-topology.md#sphere) $S^n$.

For the [three-sphere](../../../geometry-and-topology.md#three-sphere), use its identification with [SU(2)](../../../topological-group.md#su-2-group) rather than separate local constructions. With the [Pauli matrices](../../../algebra.md#pauli-matrices) $\tau_i$, put $T_i=-i\tau_i$. These form a real basis of the [SU(2) Lie algebra](../../../semisimple-lie-algebra.md#su-2-lie-algebra) and satisfy

$$
T_iT_j=-\delta_{ij}I+\epsilon_{ijk}T_k.
$$

For $q_0^2+q_1^2+q_2^2+q_3^2=1$, the identification [SU(2) as the three-sphere](../../../topological-group.md#su-2-as-the-three-sphere) is

$$
U(q)=q_0I+q_iT_i=\begin{pmatrix}q_0-iq_3&-q_2-iq_1\\q_2-iq_1&q_0+iq_3\end{pmatrix}.
$$

The matrix is unitary with determinant one. Conversely, every [SU(2) matrix](../../../topological-group.md#su-2-matrix) has this form, and both the correspondence and its inverse are smooth.

The left translations $L_g(h)=gh$ are [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism). Define three [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) by

$$
\boxed{X_i(g)=(dL_g)_eT_i=gT_i,\qquad i=1,2,3.}
$$

Matrix multiplication makes these [vector fields](../../../calculus.md#vector-field) smooth globally. Since $(dL_g)_e$ is an isomorphism from the [SU(2) Lie algebra](../../../semisimple-lie-algebra.md#su-2-lie-algebra) to $T_g\mathrm{SU}(2)$, the three vectors are linearly independent at every point, and each is nowhere zero. This is the [parallelization of a Lie group by left translations](../../../lie-theory.md#parallelization-of-a-lie-group-by-left-translations).

Transporting the [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) to the [three-sphere](../../../geometry-and-topology.md#three-sphere) gives the [quaternionic left-invariant frame on the three-sphere](../../../differential-geometry.md#quaternionic-left-invariant-frame-on-the-three-sphere):

$$
\begin{aligned}
X_1(q)&=(-q_1,q_0,q_3,-q_2),\\
X_2(q)&=(-q_2,-q_3,q_0,q_1),\\
X_3(q)&=(-q_3,q_2,-q_1,q_0).
\end{aligned}
$$

Directly, $q\cdot X_i=0$ and $X_i\cdot X_j=\delta_{ij}$ on the unit [three-sphere](../../../geometry-and-topology.md#three-sphere). Thus the vectors are tangent and form a global orthonormal [frame of a vector bundle](../../../fiber-bundle.md#frame-of-a-vector-bundle). **The three-sphere is a parallelizable manifold**, with [tangent bundle](../../../fiber-bundle.md#tangent-bundle) $TS^3\cong S^3\times\mathbb R^3$.

## 2

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a [Matrix Lie group](../../../lie-theory.md#matrix-lie-group) $G$, the left [Maurer-Cartan form](../../../lie-theory.md#maurer-cartan-form) identifies tangent vectors with the [Lie algebra](../../../lie-algebra.md) by translating them to the identity:

$$
\boxed{\rho_g(v)=(dL_{g^{-1}})_g v=g^{-1}v,\qquad \rho=g^{-1}dg.}
$$

It is a [Lie algebra](../../../lie-algebra.md)-valued [differential form](../../../differential-form.md) of degree one. For a fixed $h\in G$, replacing $g$ by $hg$ gives $(hg)^{-1}d(hg)=g^{-1}dg$, so it is a [left-invariant differential form](../../../lie-theory.md#left-invariant-differential-form).

Differentiate $g^{-1}g=I$ to get $d(g^{-1})=-g^{-1}(dg)g^{-1}$. The [exterior derivative](../../../differential-form.md#exterior-derivative) then gives

$$
d\rho=d(g^{-1})\wedge dg+g^{-1}d^2g=-g^{-1}dg\wedge g^{-1}dg=-\rho\wedge\rho.
$$

Here the [exterior product](../../../linear-algebra.md#exterior-product) of matrix-valued [differential forms](../../../differential-form.md) includes matrix multiplication; the order of the matrices matters. Hence **the Maurer-Cartan equation is**

$$
\boxed{d\rho+\rho\wedge\rho=0.}
$$

Write $\rho=\sigma^\alpha T_\alpha$. Antisymmetry of the [exterior product](../../../linear-algebra.md#exterior-product) implies

$$
\rho\wedge\rho=\frac12\sum_{\alpha,\beta}\sigma^\alpha\wedge\sigma^\beta[T_\alpha,T_\beta]
=\frac12\sum_{\alpha,\beta,\gamma}c^\gamma{}_{\alpha\beta}\sigma^\alpha\wedge\sigma^\beta T_\gamma.
$$

Comparison of the [Lie algebra](../../../lie-algebra.md) components yields the [Maurer-Cartan equation in a Lie-algebra basis](../../../lie-theory.md#maurer-cartan-equation-in-a-lie-algebra-basis):

$$
\boxed{d\sigma^\gamma=-\frac12\sum_{\alpha,\beta}c^\gamma{}_{\alpha\beta}\sigma^\alpha\wedge\sigma^\beta.}
$$

Thus **the canonical antisymmetric choice is $f^\gamma{}_{\alpha\beta}=-\tfrac12c^\gamma{}_{\alpha\beta}$**. The factor one half is required because the sum includes both ordered pairs $(\alpha,\beta)$ and $(\beta,\alpha)$. If only $\alpha<\beta$ is summed, its coefficient is $-c^\gamma{}_{\alpha\beta}$. Strictly, the equality of [differential forms](../../../differential-form.md) determines only the antisymmetric part of $f$: one may add any tensor symmetric in $\alpha,\beta$ without changing it. This is the [symmetric-part ambiguity in Maurer-Cartan coefficients](../../../lie-theory.md#symmetric-part-ambiguity-in-maurer-cartan-coefficients).

A faithful [matrix representation](../../../representation-theory.md#matrix-representation) of the orientation-preserving [real affine group](../../../lie-theory.md#orientation-preserving-affine-group-of-the-real-line) is

$$
\boxed{g(a,b)=\begin{pmatrix}a&b\\0&1\end{pmatrix},\qquad a>0,\ b\in\mathbb R.}
$$

Its action on $(x,1)^T$ has first component $ax+b$. The [group operation](../../../group.md#group-operation) and inverse are

$$
g(a,b)g(a',b')=g(aa',b+ab'),\qquad g(a,b)^{-1}=g(a^{-1},-b/a).
$$

Different transformations have different matrix entries, proving faithfulness. With the [Lie algebra](../../../lie-algebra.md) basis

$$
D=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad T=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad [D,T]=T,
$$

the left [Maurer-Cartan form](../../../lie-theory.md#maurer-cartan-form) is

$$
g^{-1}dg=\begin{pmatrix}da/a&db/a\\0&0\end{pmatrix}=\sigma^D D+\sigma^T T.
$$

The requested [left-invariant differential forms](../../../lie-theory.md#left-invariant-differential-form) therefore form the [Maurer-Cartan coframe of the real affine group](../../../lie-theory.md#maurer-cartan-coframe-of-the-real-affine-group):

$$
\boxed{\sigma^D=\frac{da}{a},\qquad\sigma^T=\frac{db}{a},\qquad d\sigma^D=0,\quad d\sigma^T=-\sigma^D\wedge\sigma^T.}
$$

For a direct invariance check, left translation by $(a_0,b_0)$ sends $(a,b)$ to $(a_0a,b_0+a_0b)$, and the pullbacks of the two displayed [differential forms](../../../differential-form.md) are unchanged. Their dual [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) are $a\partial_a$ and $a\partial_b$, whose bracket is $a\partial_b$, in agreement with $[D,T]=T$.

## 3

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The product of the magnetic field with the velocity in this question is the three-dimensional [cross product](../../../vector-space.md#cross-product). Fix $\epsilon_{123}=1$ and write $K^i{}_j=\epsilon^i{}_{kj}B^k$, so $K\mathbf v=\mathbf B\times\mathbf v$. In coordinates $y^0=t$, $y^i=x^i$ on $\mathbb R^3\times\mathbb R$, prescribe an [affine connection](../../../fiber-bundle.md#affine-connection) by the following [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol):

$$
\boxed{\Gamma^i{}_{00}=-E^i,\qquad\Gamma^i{}_{0j}=\Gamma^i{}_{j0}=-K^i{}_j=\epsilon^i{}_{jk}B^k,}
$$

with all other [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) zero. These are smooth globally in the given Cartesian coordinates. The lower-index symmetry makes this a [torsion-free connection](../../../fiber-bundle.md#torsion-free-connection). It is the [geometrization of the Lorentz force by an affine connection](../../../electromagnetism.md#geometrization-of-the-lorentz-force-by-an-affine-connection); no condition on the [curl](../../../calculus.md#curl) of $\mathbf E$ or the [divergence](../../../calculus.md#divergence) of $\mathbf B$ is required for this construction.

An affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic), with primes denoting differentiation with respect to $\lambda$, satisfies

$$
t''=0,\qquad \mathbf x''-\mathbf E(t')^2-2t'\mathbf B\times\mathbf x'=0.
$$

On the branch $t'=c\ne0$, use $t$ itself as an [affine parameter](../../../riemannian-geometry.md#affine-parameter). Dividing the spatial equation by $c^2$ gives

$$
\boxed{\frac{d^2\mathbf x}{dt^2}=\mathbf E+2\mathbf B\times\frac{d\mathbf x}{dt}.}
$$

Conversely, each solution of this equation makes $\lambda=t$, $y(t)=(t,\mathbf x(t))$ an affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic) of the constructed [affine connection](../../../fiber-bundle.md#affine-connection). Therefore its image is also an unparametrized [geodesic](../../../riemannian-geometry.md#geodesic). A general change of parameter adds a term proportional to the tangent in the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation), leaving the curve unchanged. The branch $t'=0$ is not a trajectory with time as parameter.

For the metric realization, assume $\mathbf E=-\nabla U$ and $\nabla\cdot\mathbf B=0$. Introduce the [differential form](../../../differential-form.md)

$$
F=\iota_{\mathbf B}(dx^1\wedge dx^2\wedge dx^3)=\frac12F_{ij}\,dx^i\wedge dx^j,\qquad F_{ij}=\epsilon_{ijk}B^k.
$$

Then $dF=(\nabla\cdot\mathbf B)\,dx^1\wedge dx^2\wedge dx^3=0$. The global [Poincaré lemma](../../../differential-form.md#poincare-lemma) on the contractible space $\mathbb R^3$ supplies a one-form $A=A_i dx^i$ with $dA=F$, equivalently a [magnetic vector potential](../../../electromagnetism.md#magnetic-vector-potential) with $\nabla\times\mathbf A=\mathbf B$. An explicit [radial-gauge potential for a divergence-free magnetic field](../../../electromagnetism.md#radial-gauge-potential-for-a-divergence-free-magnetic-field) is

$$
\boxed{A_i(\mathbf x)=\int_0^1 s x^jF_{ji}(s\mathbf x)\,ds,\qquad\mathbf A(\mathbf x)=\int_0^1s\,\mathbf B(s\mathbf x)\times\mathbf x\,ds.}
$$

This is the radial homotopy formula for a closed two-form and is smooth even at the origin. For a constant magnetic field it gives $\mathbf A=\tfrac12\mathbf B\times\mathbf x$.

Consider the [Eisenhart-Duval lift](../../../classical-mechanics.md#eisenhart-duval-lift) with the [Lorentzian metric](../../../general-relativity.md#lorentzian-metric)

$$
g=d\mathbf x^2+2dt\bigl(du-2A_i dx^i-Udt\bigr).
$$

The independent one-forms $dx^1,dx^2,dx^3,dt,du-2A_i dx^i-Udt$ exhibit three positive directions and a two-dimensional block with one positive and one negative direction. Thus the metric is nondegenerate, of signature $(4,1)$. Its coefficients do not depend on $u$, and $g_{uu}=0$, so $\xi=\partial_u$ is a null [Killing vector field](../../../general-relativity.md#killing-vector-field). Indeed $g_{Au}$ are constant, so $\Gamma^A{}_{Bu}=0$ for the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) and $\xi$ is parallel.

The [geodesic](../../../riemannian-geometry.md#geodesic) Lagrangian for an [affine parameter](../../../riemannian-geometry.md#affine-parameter) $\lambda$ is

$$
L=\frac12|\mathbf x'|^2-U(t')^2-2A_i x'^i t'+t'u'.
$$

The cyclic coordinate $u$ gives the [conserved quantity](../../../classical-mechanics.md#conserved-quantity) $p_u=\partial L/\partial u'=t'$. Work at a nonzero value of $p_u$ and rescale the [affine parameter](../../../riemannian-geometry.md#affine-parameter) to set $t'=1$. This is the essential step in the [null Kaluza-Klein reduction of a stationary force](../../../classical-mechanics.md#null-kaluza-klein-reduction-of-a-stationary-force): one fixes the momentum along the null isometry and projects its [geodesics](../../../riemannian-geometry.md#geodesic), rather than dividing by $g_{uu}$.

The spatial [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation), before setting $t'=1$, are

$$
x''_i+\partial_iU(t')^2+2(\partial_iA_j-\partial_jA_i)x'^j t'-2A_i t''=0.
$$

Since $t''=0$ and $F_{ij}v^j=-(\mathbf B\times\mathbf v)_i$, their reduction is

$$
\boxed{\ddot{\mathbf x}=-\nabla U+2\mathbf B\times\dot{\mathbf x}.}
$$

Equivalently, after taking $t$ as the [affine parameter](../../../riemannian-geometry.md#affine-parameter), the term $\dot u$ is a total derivative and the reduced Lagrangian is $L_{\mathrm{red}}=\tfrac12|\dot{\mathbf x}|^2-2\mathbf A\cdot\dot{\mathbf x}-U$. Its [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) give the same sign and factor two.

There is also an explicit converse using null [geodesics](../../../riemannian-geometry.md#geodesic). For any physical trajectory, set

$$
\boxed{\dot u=U+2\mathbf A\cdot\dot{\mathbf x}-\frac12|\dot{\mathbf x}|^2.}
$$

This makes its five-dimensional tangent null. The conserved momentum of the cyclic coordinate $t$ becomes

$$
p_t=-2U-2\mathbf A\cdot\dot{\mathbf x}+\dot u=-\left(U+\frac12|\dot{\mathbf x}|^2\right).
$$

The quantity in parentheses is conserved, because its derivative is $\dot{\mathbf x}\cdot(2\mathbf B\times\dot{\mathbf x})=0$. Hence the $t$ equation, as well as the spatial and $u$ [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation), is satisfied. **Every trajectory admits a null geodesic lift with $p_u=1$, and every such lift projects to the required trajectory.**

Finally, a time-independent [gauge transformation](../../../electromagnetism.md#gauge-transformation) $\mathbf A\mapsto\mathbf A+\nabla\chi$ is absorbed by $u\mapsto u+2\chi$. The one-form $du-2A_i dx^i-Udt$ and the five-dimensional metric are unchanged. These [gauge transformations of an Eisenhart-Duval lift](../../../classical-mechanics.md#gauge-transformations-of-an-eisenhart-duval-lift) alter the reduced Lagrangian only by the total derivative $-2d\chi/dt$.

## 4

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [degree of a map between oriented manifolds](../../../homology.md#degree-of-a-map-between-oriented-manifolds) measures how many times the domain covers the target, with signs recording the local [local orientation of a manifold](../../../cohomology.md#local-orientation-of-a-manifold). Let $M,N$ be connected, oriented [closed manifolds](../../../differential-geometry.md#closed-manifold) of the same dimension $n>0$. A continuous map $f:M\to N$ acts on top-dimensional [homology](../../../homology.md) by

$$
\boxed{f_*[M]=\deg(f)[N],\qquad\deg(f)\in\mathbb Z,}
$$

where $[M],[N]$ are their [fundamental classes](../../../cohomology.md#fundamental-class). Connectedness and the choices of [local orientation of a manifold](../../../cohomology.md#local-orientation-of-a-manifold) identify $H_n(N;\mathbb Z)$ with $\mathbb Z$. Reversing the orientation of either manifold changes the sign; reversing both does not.

For a smooth map, [Sard theorem](../../../differential-geometry.md#sard-s-theorem) supplies a [regular value](../../../differential-geometry.md#regular-value) $y$. Its inverse image is discrete and, by compactness, finite. At each $x\in f^{-1}(y)$ the differential is an isomorphism; let its sign be $+1$ or $-1$ according to whether it preserves or reverses the chosen local orientations. The [degree as a sum of local degrees](../../../homology.md#degree-as-a-sum-of-local-degrees) is

$$
\boxed{\deg(f)=\sum_{x\in f^{-1}(y)}\operatorname{sgn}\det(df_x).}
$$

The sign is computed in oriented [manifold charts](../../../differential-geometry.md#manifold-chart). The value is independent of the chosen [regular value](../../../differential-geometry.md#regular-value), even when inverse images appear or disappear: the signed count is the coefficient of $[N]$ in $f_*[M]$.

There is a useful local-density expression for the same [topological degree](../../../geometry-and-topology.md#topological-degree). If $\omega$ is a [volume form](../../../differential-form.md#volume-form) with $\int_N\omega=1$, then

$$
\boxed{\deg(f)=\int_M f^*\omega.}
$$

This [degree by integration of a pullback volume form](../../../homology.md#degree-by-integration-of-a-pullback-volume-form) follows first by choosing a smooth top-form supported in a small neighborhood of a [regular value](../../../differential-geometry.md#regular-value), where the inverse branches contribute their orientation signs. Any other normalized top-form differs from it by an exact form: integration identifies $H^n_{\mathrm{dR}}(N)$ with $\mathbb R$. The integral of its pullback difference vanishes by [Stokes theorem](../../../calculus.md#stokes-theorem). In particular, for any top-form $\eta$, $\int_M f^*\eta=\deg(f)\int_N\eta$.

A [homotopy](../../../algebraic-topology.md#homotopy) $H:M\times[0,1]\to N$ preserves this integral, since $d\omega=0$ and [Stokes theorem](../../../calculus.md#stokes-theorem) gives

$$
\int_M f_1^*\omega-\int_M f_0^*\omega=\int_{M\times[0,1]}d(H^*\omega)=0.
$$

Thus [topological degree](../../../geometry-and-topology.md#topological-degree) is a [homotopy](../../../algebraic-topology.md#homotopy) invariant. It is multiplicative under composition, because the induced maps on [homology](../../../homology.md) compose: $\deg(g\circ f)=\deg(g)\deg(f)$. The identity has degree one, a constant map has degree zero for $n>0$, and an orientation-reversing [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) has degree minus one. An orientation-preserving finite [covering map](../../../algebraic-topology.md#covering-space) has degree equal to its number of sheets. Nonzero [topological degree](../../../geometry-and-topology.md#topological-degree) forces surjectivity, since an omitted point would be a [regular value](../../../differential-geometry.md#regular-value) with an empty inverse image.

For the [circle](../../../topology.md#circle), $e^{i\theta}\mapsto e^{ik\theta}$ has degree $k$, positive or negative. This is its [winding number](../../../complex-analysis.md#winding-number), computable as $(2\pi i)^{-1}\int f^{-1}df$. The antipodal map of $S^n$ has degree $(-1)^{n+1}$: its extension $-I$ on the ambient $(n+1)$-dimensional vector space has that determinant sign and respects the outward-normal convention. A holomorphic map $z\mapsto z^k$, $k\geq1$, on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere) has degree $k$, whereas its complex conjugate has degree $-k$. These examples show how orientation, rather than simply the number of inverse images, determines the integer.

For maps $S^n\to S^n$, [topological degree](../../../geometry-and-topology.md#topological-degree) gives the complete [homotopy](../../../algebraic-topology.md#homotopy) classification $\pi_n(S^n)\cong\mathbb Z$. The [degree does not classify general manifold maps](../../../homology.md#degree-does-not-classify-general-manifold-maps): the identity of the [torus](../../../topology.md#torus) and the map induced by the integer matrix $\begin{pmatrix}1&1\\0&1\end{pmatrix}$ both have degree one, but have different induced maps on $H_1(T^2;\mathbb Z)$ and so are not homotopic. A nonzero-degree map $S^n\to S^n$ cannot extend continuously to $B^{n+1}$, because such an extension would make the boundary map null-homotopic. In the smooth setting, [Stokes theorem](../../../calculus.md#stokes-theorem) gives the same obstruction by applying it to the pulled-back normalized [volume form](../../../differential-form.md#volume-form).

The hypotheses can be adjusted, but must be stated. For connected oriented noncompact manifolds, a [proper map](../../../cohomology.md#proper-map) has a degree defined using compactly supported top-forms, and it is invariant under proper [homotopies](../../../algebraic-topology.md#homotopy). For [manifolds with boundary](../../../differential-geometry.md#manifold-with-boundary) one uses relative [fundamental classes](../../../cohomology.md#fundamental-class) and maps of pairs, or fixes appropriate boundary conditions. Without an integral orientation one can still count inverse images modulo two, obtaining a mod-two degree. The integer integral formula used below assumes the oriented setting.

In [classical field theory](../../../quantum-field-theory.md#classical-field-theory), these ideas turn continuous fields into quantized [topological charges](../../../classical-field-theory-soliton.md#topological-charge). Suppose a field on $\mathbb R^d$ approaches one fixed target value at spatial infinity. The [one-point compactification](../../../topology.md#alexandroff-extension) makes it a map $\phi:S^d\to\mathcal V$. When the target $\mathcal V$ is an oriented closed $d$-manifold, its [topological degree](../../../geometry-and-topology.md#topological-degree) labels [topological sectors](../../../classical-field-theory-soliton.md#topological-sector). More generally the sectors are described by [homotopy groups](../../../algebraic-topology.md#homotopy-group); an integer degree is available only when the domain and target have the appropriate dimensions and orientations. Smooth time evolution preserving the boundary condition is a [homotopy](../../../algebraic-topology.md#homotopy), so it cannot change the integer. A change requires a singular field, escape from the allowed target, or a change at the boundary.

A normalized closed target $d$-form gives the [pullback-volume representation of a topological current](../../../classical-field-theory-soliton.md#pullback-volume-representation-of-a-topological-current). On spacetime, put $\alpha=\phi^*\omega$. Since $d\alpha=\phi^*(d\omega)=0$, its dual current is identically conserved, and

$$
Q=\int_{\text{space}}\alpha=\deg(\phi)
$$

is independent of time when there is no flux at infinity. This conservation law follows from geometry without using the field equations; it need not arise from a continuous symmetry through [Noether theorem](../../../calculus-of-variations.md#noether-theorem).

A concrete example is the [O3 nonlinear sigma model](../../../quantum-field-theory.md#o3-nonlinear-sigma-model) in two spatial dimensions. Its unit-vector field $\mathbf n$ approaches a constant at infinity, defining $S^2\to S^2$. The normalized area form of the target gives the [degree charge of an O3 sigma-model lump](../../../quantum-field-theory.md#degree-charge-of-an-o3-sigma-model-lump):

$$
\boxed{Q=\frac1{4\pi}\int_{\mathbb R^2}\mathbf n\cdot(\partial_1\mathbf n\times\partial_2\mathbf n)\,dx^1dx^2\in\mathbb Z.}
$$

For the energy normalization $E=\tfrac12\int(|\partial_1\mathbf n|^2+|\partial_2\mathbf n|^2)$, the identities $\mathbf n\cdot\partial_i\mathbf n=0$ give

$$
E=\frac12\int|\partial_1\mathbf n\pm\mathbf n\times\partial_2\mathbf n|^2\,d^2x\ \pm4\pi Q,\qquad\boxed{E\geq4\pi|Q|.}
$$

This is the [Bogomolny degree bound for the O3 sigma model](../../../quantum-field-theory.md#bogomolny-degree-bound-for-the-o3-sigma-model). Choosing the sign appropriate to $Q$ makes the square nonnegative; vanishing of the square gives first-order [Bogomolny equations](../../../quantum-field-theory.md#bogomolny-equations) and a [sigma-model lump](../../../quantum-field-theory.md#sigma-model-lump) saturating the bound. With the oriented [stereographic projection](../../../complex-analysis.md#stereographic-projection)

$$
\mathbf n=\frac{(2\operatorname{Re}w,2\operatorname{Im}w,1-|w|^2)}{1+|w|^2},\qquad z=x^1+ix^2,
$$

the maps $w=z^k$ have $Q=k$ and $E=4\pi k$. Their conjugates have $Q=-k$ with the same energy. Holomorphic rational maps have positive degree equal to their degree as rational maps; taking a reciprocal does not reverse the orientation. Antiholomorphic dependence reverses it.

The [Skyrme model](../../../classical-field-theory-soliton.md#skyrme-model) supplies a three-dimensional example. A field $U:\mathbb R^3\to\mathrm{SU}(2)$ with $U\to I$ at infinity is a map $S^3\to\mathrm{SU}(2)\cong S^3$. Take $T_i=-i\tau_i$ and $U^{-1}dU=\theta^iT_i$, with $\theta^1\wedge\theta^2\wedge\theta^3$ positive. Since $\operatorname{tr}(T_iT_jT_k)=-2\epsilon_{ijk}$, the normalized target [volume form](../../../differential-form.md#volume-form) is

$$
\omega_3=-\frac1{24\pi^2}\operatorname{tr}(U^{-1}dU)^3=\frac1{2\pi^2}\theta^1\wedge\theta^2\wedge\theta^3.
$$

The integral is one on the unit [three-sphere](../../../geometry-and-topology.md#three-sphere). Consequently the [Skyrme baryon number as a mapping degree](../../../classical-field-theory-soliton.md#skyrme-baryon-number-as-a-mapping-degree) is

$$
\boxed{B=-\frac1{24\pi^2}\int_{\mathbb R^3}\operatorname{tr}(U^{-1}dU)^3=\deg(U).}
$$

This is the [topological baryon number in the Skyrme model](../../../classical-field-theory-soliton.md#topological-baryon-number-in-the-skyrme-model); the sign has been fixed by the stated orientation and anti-Hermitian generator convention.

A [topological charge](../../../classical-field-theory-soliton.md#topological-charge) alone does not guarantee a stable finite-size solution. The [degree and energetic stability of a field configuration](../../../classical-field-theory-soliton.md#degree-and-energetic-stability-of-a-field-configuration) concern different properties. For a three-dimensional configuration of size $R$, the two-derivative energy scales as $R$, so it can decrease by shrinking while the [topological degree](../../../geometry-and-topology.md#topological-degree) remains fixed for every $R>0$. The limit can be singular. The [Skyrme term](../../../classical-field-theory-soliton.md#skyrme-term), with four derivatives, scales as $R^{-1}$ and can balance the shrinking tendency. This is the role of [Derrick theorem](../../../classical-field-theory-soliton.md#derrick-s-theorem) in distinguishing topological obstruction from energetic stability.

For defects, the relevant boundary map can instead be the sphere surrounding a core. A [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) equal to $S^1$ gives the integer [winding number](../../../complex-analysis.md#winding-number) of a [vortex](../../../critical-phenomenon.md#phase-vortex); a vacuum manifold $S^2$ gives the degree of a surrounding $S^2$ for a [magnetic monopole](../../../physics.md#magnetic-monopole). This [vacuum-boundary degree as a defect charge](../../../classical-field-theory-soliton.md#vacuum-boundary-degree-as-a-defect-charge) obstructs extending the normalized vacuum field through the enclosed ball. A nonzero integer therefore forces the field to leave the [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) somewhere in the core. This construction does not require the field to take one constant value in every direction at infinity.

Degree also appears in four-dimensional gauge theory through a boundary transition function. For an anti-Hermitian [SU(2)](../../../topological-group.md#su-2-group) gauge connection on $\mathbb R^4$, write $F=dA+A\wedge A$ and assume finite-action boundary behavior $A\to g^{-1}dg$ on the large bounding [three-sphere](../../../geometry-and-topology.md#three-sphere). In the second-Chern convention

$$
k=\frac1{8\pi^2}\int_{\mathbb R^4}\operatorname{tr}(F\wedge F),
$$

the identity $d\operatorname{tr}(A\wedge dA+\tfrac23A^3)=\operatorname{tr}(F\wedge F)$ and the [Maurer-Cartan equation](../../../lie-theory.md#maurer-cartan-equation) give

$$
\boxed{k=-\frac1{24\pi^2}\int_{S^3}\operatorname{tr}(g^{-1}dg)^3=\deg(g).}
$$

This [boundary winding representation of Yang-Mills topological charge](../../../classical-field-theory-soliton.md#boundary-winding-representation-of-yang-mills-topological-charge) relates the [Second Chern number](../../../geometry-and-topology.md#second-chern-number) to the degree of $g:S^3\to\mathrm{SU}(2)$. The [Chern-Simons 3-form](../../../geometry-and-topology.md#chern-simons-3-form) turns the bulk integral into the boundary winding integral. Conventions which define the instanton number with the opposite trace sign reverse $k$; the integer quantization is unchanged. A [Yang-Mills theta term](../../../relativistic-quantum-field.md#yang-mills-theta-term) weights a sector by $e^{i\vartheta k}$, giving periodicity $\vartheta\mapsto\vartheta+2\pi$. Thus the same [topological degree](../../../geometry-and-topology.md#topological-degree) that counts oriented inverse images also labels field sectors and expresses their quantized charges as integrals of local densities.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
