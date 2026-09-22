# Paper 55

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_55.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_55.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
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
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the [Lie bracket](../../../lie-algebra.md#lie-bracket) convention $[X,Y]=XY-YX$. If $E_{ij}$ denotes a [matrix unit](../../../vector-space.md#matrix-unit), then $E_{ij}E_{kl}=\delta_{jk}E_{il}$. Here this gives

$$
[X_0,X_1]=X_1,\qquad [X_0,X_2]=X_2,\qquad [X_1,X_2]=0.
$$

Thus, writing $[X_j,X_k]=f^i{}_{jk}X_i$, **the nonzero [structure constants of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) are**

$$
\boxed{f^1{}_{01}=f^2{}_{02}=1,\qquad f^1{}_{10}=f^2{}_{20}=-1.}
$$

All other entries vanish. This is the [Lie algebra](../../../lie-algebra.md) of the [translation-dilation group of the plane](../../../lie-theory.md#translation-dilation-group-of-the-plane): its two-dimensional translation ideal is abelian, and $X_0$ acts on that ideal as the identity. In group coordinates the multiplication and inverse are

$$
(\rho,x)(\rho',x')=(\rho\rho',x+\rho x'),\qquad (\rho,x)^{-1}=(\rho^{-1},-\rho^{-1}x).
$$

These formulas also make the [semidirect product](../../../group-theory.md#semidirect-product) structure explicit.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Maurer-Cartan form](../../../lie-theory.md#maurer-cartan-form) is $g^{-1}dg=\lambda^jX_j$. Direct matrix multiplication gives

$$
g^{-1}dg=\begin{pmatrix}d\rho/\rho&dx^1/\rho&dx^2/\rho\\0&0&0\\0&0&0\end{pmatrix},\qquad
\boxed{\lambda^0=\frac{d\rho}{\rho},\quad\lambda^1=\frac{dx^1}{\rho},\quad\lambda^2=\frac{dx^2}{\rho}.}
$$

These are [left-invariant differential forms](../../../lie-theory.md#left-invariant-differential-form): for a constant group element $a$, $(ag)^{-1}d(ag)=g^{-1}dg$. Equivalently, left translation sends $(\rho,x)$ to $(a\rho,b+ax)$, so all three coordinate differentials and the denominator acquire the same factor $a>0$.

The [left-invariant coframe of the translation-dilation group](../../../lie-theory.md#left-invariant-coframe-of-the-translation-dilation-group) is pointwise linearly independent because $\rho>0$. Consequently

$$
h=\sum_{j=0}^2\lambda^j\otimes\lambda^j
$$

is positive definite and unchanged under every left translation. **It therefore defines the required [left-invariant metric](../../../lie-theory.md#left-invariant-metric)**, with precisely the coordinate expression obtained from this sum. The notation $d\rho^2$ in that metric means $d\rho\otimes d\rho$, not the differential of $\rho^2$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Taking the [exterior derivative](../../../differential-form.md#exterior-derivative) of the [left-invariant differential forms](../../../lie-theory.md#left-invariant-differential-form) yields

$$
d\lambda^0=0,\qquad d\lambda^1=-\lambda^0\wedge\lambda^1,\qquad d\lambda^2=-\lambda^0\wedge\lambda^2.
$$

For example, $d(\rho^{-1}dx^1)=-\rho^{-2}d\rho\wedge dx^1$. With the antisymmetric [structure constants of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) found above, the two terms with indices $(0,1)$ and $(1,0)$ combine as

$$
\tfrac12\left(f^1{}_{01}\lambda^0\wedge\lambda^1+f^1{}_{10}\lambda^1\wedge\lambda^0\right)=\lambda^0\wedge\lambda^1.
$$

The same computation holds for superscript $2$, and all superscript-$0$ terms vanish. **Hence the [Maurer-Cartan equation](../../../lie-theory.md#maurer-cartan-equation) is**

$$
\boxed{d\lambda^i+\tfrac12 f^i{}_{jk}\lambda^j\wedge\lambda^k=0.}
$$

The factor $1/2$ avoids counting each antisymmetric pair twice. If coefficients were not required to be antisymmetric in $j,k$, their symmetric parts would be invisible to the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms); the standard [structure constants of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) fix this ambiguity.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Take the frame dual to the [left-invariant coframe of the translation-dilation group](../../../lie-theory.md#left-invariant-coframe-of-the-translation-dilation-group). It is

$$
\boxed{L_0=\rho\partial_\rho,\qquad L_1=\rho\partial_{x^1},\qquad L_2=\rho\partial_{x^2}.}
$$

Indeed $\lambda^i(L_j)=\delta^i_j$. These are [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field), either because they are dual to invariant forms or because $L_j(g)=(dL_g)_eX_j$. For instance, the curve $g\exp(tX_0)$ differentiates to $\rho\partial_\rho$, while $g\exp(tX_1)$ differentiates to $\rho\partial_{x^1}$.

The coordinate [Lie brackets](../../../lie-algebra.md#lie-bracket) satisfy

$$
[L_0,L_1]=\rho\partial_{x^1}=L_1,\qquad [L_0,L_2]=L_2,\qquad [L_1,L_2]=0.
$$

For the first identity only the derivative of the coefficient $\rho$ contributes. **The linear map $\boxed{X_j\longmapsto L_j}$ is a [Lie algebra isomorphism](../../../lie-algebra.md#lie-algebra-isomorphism)**: it preserves all basis brackets, is injective by independence of the frame, and is onto the three-dimensional space of [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field).

## 2

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [topological degree](../../../geometry-and-topology.md#topological-degree) measures an oriented net number of sheets of a map. Its simplest integer-valued setting is a map $f:M\to N$ between connected oriented [closed manifolds](../../../differential-geometry.md#closed-manifold) of the same positive dimension $n$. The hypotheses matter: an integer sign count needs orientations; compactness prevents preimages from escaping; and the same dimension makes a regular fiber discrete. A [fundamental class](../../../cohomology.md#fundamental-class) gives the definition for continuous maps:

$$
\boxed{f_*[M]=(\deg f)[N],\qquad \deg f\in\mathbb Z.}
$$

Here $H_n(M;\mathbb Z)$ and $H_n(N;\mathbb Z)$ are generated by their chosen [fundamental classes](../../../cohomology.md#fundamental-class). Reversing either orientation changes the sign of the [degree of a map between oriented manifolds](../../../homology.md#degree-of-a-map-between-oriented-manifolds). Disconnected sources contribute a sum over components; disconnected targets require a degree for each target component rather than one universal integer.

For a smooth map, choose a [regular value](../../../differential-geometry.md#regular-value) $y$. The [Sard theorem](../../../differential-geometry.md#sard-s-theorem) guarantees plentiful choices. Each point of $f^{-1}(y)$ has an invertible derivative, so the [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes it an isolated point. The fiber is finite by compactness of $M$. An oriented coordinate chart defines $\operatorname{sgn}\det df_x$, and the [degree as a sum of local degrees](../../../homology.md#degree-as-a-sum-of-local-degrees) becomes

$$
\boxed{\deg f=\sum_{x\in f^{-1}(y)}\operatorname{sgn}\det df_x.}
$$

An empty fiber contributes zero. The sign is independent of the chosen oriented charts. Thus the [mapping degree](../../../homology.md#degree-of-a-continuous-mapping) counts sheets with signs, not simply the number of preimages: orientation-preserving and orientation-reversing sheets cancel.

A differential-form argument both proves that this count is independent of $y$ and relates it to the topological definition. Around a [regular value](../../../differential-geometry.md#regular-value), take a small neighborhood $V$ whose full preimage is a disjoint union of neighborhoods mapped diffeomorphically onto $V$. Compactness rules out additional preimages approaching $V$ from elsewhere. Choose a smooth top-degree form $\eta$ supported in $V$, with $\int_N\eta=1$. The [change of variables formula](../../../calculus.md#change-of-variables-formula) gives

$$
\int_M f^*\eta=\sum_{x\in f^{-1}(y)}\operatorname{sgn}\det df_x.
$$

Although $\eta$ need not be everywhere positive, it represents the same normalized top cohomology class as any normalized [volume form](../../../differential-form.md#volume-form). The [top de Rham cohomology of a compact connected oriented manifold](../../../differential-form.md#top-de-rham-cohomology-of-a-compact-connected-oriented-manifold) says that two top forms with equal integrals differ by $d\beta$. Their pullback integrals agree, because the [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem) gives $\int_Md(f^*\beta)=0$. Therefore **the [degree by integration of a pullback volume form](../../../homology.md#degree-by-integration-of-a-pullback-volume-form) is**

$$
\boxed{\int_Mf^*\eta=(\deg f)\int_N\eta}
$$

for every smooth top form $\eta$. Pairing [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) with [fundamental classes](../../../cohomology.md#fundamental-class) identifies this integer with the homological definition. This proof also shows that every [regular value](../../../differential-geometry.md#regular-value) gives the same signed sum.

The [homotopy invariance of mapping degree](../../../homology.md#homotopy-invariance-of-mapping-degree) makes it stable under continuous deformation. Homologically this follows from homotopic maps inducing the same map on [homology](../../../homology.md). For a smooth homotopy $F:M\times[0,1]\to N$, a direct proof uses $d\eta=0$ and the [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem) on the cylinder to get

$$
\int_M f_1^*\eta-\int_M f_0^*\eta=\int_{M\times[0,1]}d(F^*\eta)=0,
$$

with the cylinder orientation chosen to give the indicated boundary signs. Smooth approximation extends the geometric description to continuous maps, while the [fundamental class](../../../cohomology.md#fundamental-class) definition already applies without differentiability. The [multiplicativity of mapping degree](../../../homology.md#multiplicativity-of-mapping-degree) follows from functoriality and gives

$$
\deg(g\circ f)=\deg g\,\deg f,\qquad \deg\operatorname{id}=1.
$$

A constant map has degree zero when $n>0$. If the [mapping degree](../../../homology.md#degree-of-a-continuous-mapping) is nonzero, the map is onto: a point outside its image is a [regular value](../../../differential-geometry.md#regular-value) with empty preimage. An orientation-preserving [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) has degree $1$, and an orientation-reversing one has degree $-1$. An orientation-preserving $k$-sheeted [covering map](../../../algebraic-topology.md#covering-space) has degree $k$; the signs of sheets must be included for other orientation conventions.

Examples show both the strength and the limits of the invariant. On the [circle](../../../topology.md#circle), $e^{i\theta}\mapsto e^{ik\theta}$ has degree $k$, including negative integers and zero; it is the [winding number](../../../complex-analysis.md#winding-number). On the [sphere](../../../geometry-and-topology.md#sphere) $S^n$, an ambient reflection has degree $-1$, and the [antipodal map](../../../homology.md#antipodal-map) has degree $(-1)^{n+1}$, because the determinant of $-I$ on the ambient $\mathbb R^{n+1}$ is $(-1)^{n+1}$. On the [torus](../../../topology.md#torus), an integer matrix $A$ induces a map of degree $\det A$, obtained by pulling back the constant top form. However, degree does not classify general manifold maps: the identity and an integer shear on the two-torus both have degree one but induce different maps on $H_1$, so are not homotopic.

The [mapping degree](../../../homology.md#degree-of-a-continuous-mapping) gives useful obstruction and existence arguments. There is no [retraction](../../../topology.md#retraction) of a closed ball onto its boundary sphere: such a retraction would make the degree-one identity of the boundary null-homotopic, since it would extend across a contractible ball, contradicting homotopy invariance and the degree-zero constant map. This is the degree obstruction underlying the [Brouwer fixed-point theorem](../../../topological-analysis.md#brouwer-fixed-point-theorem). Also an everywhere nonzero tangent [vector field](../../../calculus.md#vector-field) on an even-dimensional sphere would, after normalization, produce the homotopy $\cos(\pi t)x+\sin(\pi t)v(x)$ from the identity to the antipodal map. Orthogonality makes every value a unit vector, but the endpoint degrees are $1$ and $-1$, impossible. This proves the corresponding [Hairy ball theorem](../../../fiber-bundle.md#hairy-ball-theorem) obstruction.

There are appropriate extensions rather than an unrestricted integer degree for every pair of manifolds. For a [proper map](../../../cohomology.md#proper-map) between connected oriented manifolds without boundary of equal dimension, the regular-value count remains finite and is invariant; compactly supported top forms or locally finite [homology](../../../homology.md) replace the compact fundamental-class description. Without orientations, [degree modulo two](../../../differential-geometry.md#degree-modulo-two) counts preimages modulo two and uses mod-two fundamental classes. For manifolds with boundary one uses [relative mapping degree](../../../homology.md#relative-mapping-degree) for maps of pairs, keeping the boundary away from the chosen target value. Maps of unequal dimensions, or nonproper maps where preimages can escape to infinity, do not in general admit this same signed sheet-count invariant. **The central principle is an integer signed count stable under homotopy, with its hypotheses explicitly preserved.**

## 3

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [principal bundle](../../../fiber-bundle.md#principal-bundle) consists of smooth manifolds $P,B$, a [Lie group](../../../lie-theory.md#lie-group) $G$, a smooth surjection $\pi:P\to B$, and a smooth free right action of $G$ on $P$, whose orbits are the fibers. Every $b\in B$ has an open neighborhood $U$ with a $G$-equivariant [local trivialization](../../../fiber-bundle.md#local-trivialization) $\pi^{-1}(U)\cong U\times G$, under which $\pi$ is projection and the action is $(x,\gamma)h=(x,\gamma h)$. Equivalently a local section $s:U\to P$ writes every fiber point uniquely as $p=s(x)\gamma$. On overlaps, sections differ by smooth transition functions $s_\beta=s_\alpha u_{\alpha\beta}$ satisfying the cocycle identity.

A [principal connection](../../../fiber-bundle.md#connection-principal-bundle) is a Lie-algebra-valued one-form $\omega$ on $P$ satisfying $R_h^*\omega=\operatorname{Ad}_{h^{-1}}\omega$ and $\omega(\xi^\#)=\xi$ for the [fundamental vector field](../../../lie-theory.md#fundamental-vector-field) $\xi^\#(p)=\left.\frac d{dt}\right|_0p\exp(t\xi)$. Its [horizontal distribution of a principal connection](../../../fiber-bundle.md#horizontal-distribution-of-a-principal-connection) is the complement $\ker\omega$ to the vertical tangent spaces. **The local [gauge potential of a principal connection](../../../fiber-bundle.md#local-principal-connection-form) is Lie-algebra-valued**, specifically $A=s^*\omega$; matrix notation identifies the adjoint action with conjugation. The displayed connection expression is understood on each coordinate trivialization, not as a choice of a global section.

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Choose local sections related by $s'=su$, where $u:U\to G$. Keeping the same point of the [principal bundle](../../../fiber-bundle.md#principal-bundle) requires $s\gamma=s'\gamma'$, so $\gamma'=u^{-1}\gamma$. For [reconstruction of a principal connection from local gauge potentials](../../../fiber-bundle.md#reconstruction-of-a-principal-connection-from-local-gauge-potentials), the [local principal connection form](../../../fiber-bundle.md#local-principal-connection-form) transforms as

$$
A'=u^{-1}Au+u^{-1}du.
$$

Using $d(u^{-1})=-u^{-1}(du)u^{-1}$, compute

$$
(\gamma')^{-1}A'\gamma'=\gamma^{-1}A\gamma+\gamma^{-1}(du)u^{-1}\gamma,
$$

and

$$
(\gamma')^{-1}d\gamma'=\gamma^{-1}d\gamma-\gamma^{-1}(du)u^{-1}\gamma.
$$

The inhomogeneous terms cancel. **Thus $\boxed{\omega'=\omega}$**: both local expressions define the same one-form on the total space. This is compatibility across trivializations, whereas $R_h^*\omega=\operatorname{Ad}_{h^{-1}}\omega$ describes the separate right-action equivariance of a [principal connection](../../../fiber-bundle.md#connection-principal-bundle). In particular a change of trivialization is not an assertion that the local [gauge potential of a principal connection](../../../fiber-bundle.md#local-principal-connection-form) $A$ itself is unchanged.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Work over a coordinate neighborhood $U\subset B$ with coordinates $x^i$, and choose a basis $T_a$ of the [Lie algebra](../../../lie-algebra.md), with $[T_a,T_b]=c^c{}_{ab}T_c$. Put $A=A_i^aT_a\,dx^i$. For each $T_a$ let $R_a$ be its [right-invariant vector field](../../../lie-theory.md#right-invariant-vector-field) on the fiber group. In matrix notation $R_a(\gamma)=T_a\gamma$, and

$$
[R_a,R_b]=-c^c{}_{ab}R_c.
$$

This minus sign is the [right-invariant vector fields realize the opposite Lie algebra](../../../lie-theory.md#right-invariant-vector-fields-realize-the-opposite-lie-algebra) rule. It is essential here. Define the [coordinate horizontal lifts of a principal connection](../../../fiber-bundle.md#coordinate-horizontal-lifts-of-a-principal-connection) by

$$
\boxed{H_i=\partial_i-A_i^aR_a.}
$$

Their projections are $\pi_*H_i=\partial_i$, so they are linearly independent and there are exactly $\dim B$ of them. Also $d\gamma(H_i)=-A_i\gamma$, whence

$$
\omega(H_i)=\gamma^{-1}A_i\gamma+\gamma^{-1}(-A_i\gamma)=0.
$$

They therefore span the [horizontal distribution of a principal connection](../../../fiber-bundle.md#horizontal-distribution-of-a-principal-connection) on this trivialization.

The coefficients $A_i^a$ depend only on the base variables, so taking [Lie brackets](../../../lie-algebra.md#lie-bracket) gives

$$
[H_i,H_j]=-\left(\partial_iA_j^c-\partial_jA_i^c+c^c{}_{ab}A_i^aA_j^b\right)R_c=-F_{ij}^cR_c,
$$

where $F_{ij}=\partial_iA_j-\partial_jA_i+[A_i,A_j]$ and $F=\tfrac12F_{ij}\,dx^i\wedge dx^j=dA+A\wedge A$. Since the [right-invariant vector fields](../../../lie-theory.md#right-invariant-vector-field) form a basis on each fiber, **$\boxed{[H_i,H_j]=0\text{ for all }i,j\iff F=0}$**. This is the local coordinate version of vanishing [curvature of a principal connection](../../../fiber-bundle.md#curvature-of-a-principal-connection) and, by the [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem), integrability of the horizontal distribution.

The coordinate qualification is necessary: horizontal lifts of arbitrary noncommuting base fields need not commute even for a [flat principal connection](../../../fiber-bundle.md#flat-principal-connection). Nor does flatness guarantee a globally defined coordinate frame or a global horizontal section; [holonomy of a connection](../../../fiber-bundle.md#holonomy) can obstruct the latter. If the requested frame were read globally, the trivial flat bundle $S^2\times G$ would already be a counterexample: restricting a global horizontal frame to the identity-fiber section would trivialize $TS^2$, contrary to the [Hairy ball theorem](../../../fiber-bundle.md#hairy-ball-theorem). The construction on each coordinate trivialization supplies the intended result without that global claim.

## 4

↑ **Parent:** [Paper 55](paper-55.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Fix the convention $\iota_{X_f}\omega=-df$ for a [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field). Nondegeneracy of the [symplectic form](../../../symplectic-geometry.md#symplectic-form) gives one unique smooth $X_f$ for each smooth real-valued function $f$. Define the [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) by

$$
\{f,g\}=\omega(X_f,X_g)=X_f(g).
$$

In coordinates with $\omega=\sum dq^i\wedge dp_i$, this is $\sum(f_{q^i}g_{p_i}-f_{p_i}g_{q^i})$. Thus the sign convention is explicit and agrees with the usual coordinate [Poisson bracket](../../../classical-mechanics.md#poisson-bracket). By [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula), $\mathcal L_{X_f}\omega=d\iota_{X_f}\omega+\iota_{X_f}d\omega=0$. The contraction–[Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form) commutator identity now gives

$$
\iota_{[X_f,X_g]}\omega=\mathcal L_{X_f}(\iota_{X_g}\omega)-\iota_{X_g}(\mathcal L_{X_f}\omega)=-d(X_f g)=-d\{f,g\}.
$$

Hence **the [Hamiltonian Lie algebra homomorphism](../../../symplectic-geometry.md#hamiltonian-lie-algebra-homomorphism) is $\boxed{\Phi(f)=X_f,\quad[X_f,X_g]=X_{\{f,g\}}}$**. It is linear and onto the space of [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field) by definition. For completeness, the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) for the bracket on functions follows from closure of $\omega$: evaluating $d\omega=0$ on $X_f,X_g,X_h$ and using the displayed commutator relation gives the cyclic Jacobi sum zero. Thus this really is a map of [Lie algebras](../../../lie-algebra.md), not just a bracket-preserving notation.

Its kernel is determined by nondegeneracy:

$$
\boxed{\ker\Phi=\{f:df=0\}=\{\text{locally constant smooth functions}\}.}
$$

On a connected manifold these are precisely the real constants; on a disconnected manifold the constant may differ on each component. Therefore the quotient by these functions is isomorphic to the [Lie algebra](../../../lie-algebra.md) of [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field). The printed “homeomorphis” is interpreted as homomorphism: the map before taking this quotient is not an isomorphism because of its nontrivial kernel. The alternative convention $\iota_{X_f}\omega=df$ requires a corresponding bracket sign change to retain this homomorphism.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Differentiate the [circle group](../../../lie-theory.md#circle-group) action at angle zero. The resulting real [vector field](../../../calculus.md#vector-field) is

$$
\boxed{K=iz\partial_z-i\bar z\partial_{\bar z}.}
$$

In real coordinates $z=x+iy$, this is $K=-y\partial_x+x\partial_y$; the complex coefficients are conjugates, so it is indeed real. Its integral curves satisfy $\dot z=iz$ and hence $z(t)=e^{it}z(0)$, with period $2\pi$ away from the fixed points.

The affine coordinate does not cover the whole [complex projective line](../../../algebraic-topology.md#complex-projective-line), so check the other chart. With $w=1/z$, the same [vector field](../../../calculus.md#vector-field) is $K=-iw\partial_w+i\bar w\partial_{\bar w}$, smooth at $w=0$. It vanishes at $z=0$ and $w=0$, the two fixed poles. **It therefore generates the stated global rotation of $S^2$, not merely a flow in one chart.**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Set $s=|z|^2$. Contraction of the [symplectic form](../../../symplectic-geometry.md#symplectic-form) with the rotation [vector field](../../../calculus.md#vector-field) gives

$$
\iota_K\omega=\frac{i}{(1+s)^2}\left(iz\,d\bar z+i\bar z\,dz\right)=-\frac{ds}{(1+s)^2}.
$$

With the convention fixed in the unheaded solution, $\iota_K\omega=-dH$, so **the [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function) is**

$$
\boxed{H(z)=\frac{|z|^2}{1+|z|^2}+C.}
$$

Its derivative is $dH=ds/(1+s)^2$. In the chart $w=1/z$, $H=1/(1+|w|^2)+C$, so it extends smoothly across infinity; the additive constant is the kernel freedom already identified. Thus $K=X_H$ globally, proving that the action is a [Hamiltonian group action](../../../symplectic-geometry.md#hamiltonian-group-action). With $C=0$, the [moment map for rotation of the complex projective line](../../../symplectic-geometry.md#moment-map-for-rotation-of-the-complex-projective-line) takes values in $[0,1]$, reaching its endpoints at the two fixed poles.

One can check the normalization in polar coordinates: $\omega=2r(1+r^2)^{-2}dr\wedge d\phi$ has total [symplectic area](../../../symplectic-geometry.md#symplectic-area) $2\pi$, not $4\pi$, and $H=r^2/(1+r^2)$. Equivalently, in a polar angle with $r=\tan(\vartheta/2)$, $H=(1-\cos\vartheta)/2$. This explains the half-height factor that would be lost by replacing the printed form with the unscaled round-sphere area form. Under the opposite convention $\iota_{X_H}\omega=dH$, the Hamiltonian is the negative of this function, up to a constant.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
