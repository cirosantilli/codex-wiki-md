# Paper 14

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper14.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper14.pdf)

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
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [Lie group](../../../lie-theory.md#lie-group) is a group which is a finite-dimensional smooth Hausdorff second-countable manifold, with smooth multiplication and inversion. For the [special unitary group](../../../topological-group.md#special-unitary-group), consider the real [vector space](../../../vector-space.md)

$$
\mathfrak{su}(n)=\{X\in M_n(\mathbb C):X^*=-X,\ \operatorname{tr}X=0\}.
$$

The diagonal entries of a skew-Hermitian [matrix](../../../vector-space.md#matrix) supply $n$ real parameters, and the entries above the diagonal supply $2\binom n2$; the trace-zero condition removes one real parameter. Thus $\dim_{\mathbb R}\mathfrak{su}(n)=n^2-1$.

The [matrix](../../../vector-space.md#matrix) facts used to construct charts are these: the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) is analytic, its derivative at zero is the identity, and it has an analytic inverse [matrix logarithm](../../../vector-space.md#matrix-logarithm) on a sufficiently small neighborhood of the identity. On those neighborhoods $\log(e^X)=X$, $e^{\log U}=U$, and $\det(e^X)=e^{\operatorname{tr}X}$. For a unitary [matrix](../../../vector-space.md#matrix) in that neighborhood, the [spectral theorem](../../../hilbert-space.md#spectral-theorem) writes $U=W\operatorname{diag}(e^{i\theta_j})W^*$ with principal angles close to zero, and $\log U=W\operatorname{diag}(i\theta_j)W^*$ is skew-Hermitian.

Choose a norm ball of radius $\varepsilon<\pi/n$ small enough to lie in the exponential's inverse domain. If $U$ is unitary, $\det U=1$ and $\|\log U\|<\varepsilon$ in operator norm, then

$$
\operatorname{tr}\log U\in2\pi i\mathbb Z,\qquad
|\operatorname{tr}\log U|\le n\|\log U\|<\pi,
$$

so its trace is zero. Conversely $X\in\mathfrak{su}(n)$ gives $(e^X)^*e^X=I$ and $\det(e^X)=1$. Thus the logarithm identifies an open neighborhood $V$ of $I$ in $SU(n)$, with its [matrix](../../../vector-space.md#matrix) subspace topology, with the open ball $B_\varepsilon\subset\mathfrak{su}(n)$. Choosing a real linear identification $\mathfrak{su}(n)\cong\mathbb R^{n^2-1}$ turns this into a chart.

For every $A\in SU(n)$ take the translated chart

$$
\boxed{\phi_A:AV\longrightarrow B_\varepsilon,\qquad \phi_A(U)=\log(A^{-1}U)}.
$$

Their overlap maps are $X\mapsto\log(B^{-1}A e^X)$ wherever both charts are defined, so they are real analytic. They cover the group; the [matrix](../../../vector-space.md#matrix) topology is Hausdorff and second-countable. This constructs the real manifold directly, rather than merely counting equations. [Matrix](../../../vector-space.md#matrix) multiplication is polynomial in real/imaginary entries and inversion here is $U\mapsto U^*$; in the logarithm charts both are smooth. The [logarithm charts for the special unitary group](../../../topological-group.md#logarithm-charts-for-the-special-unitary-group) therefore prove

$$
\boxed{SU(n)\text{ is a Lie group of real dimension }n^2-1}.
$$

For $n=1$ it is the one-point group of dimension zero.

For $n=2$, let the first column be $(a,b)$, of unit norm. Every unit vector orthogonal to it is a scalar of modulus one times $(-\bar b,\bar a)$. The [determinant](../../../linear-algebra.md#determinant) of the resulting [matrix](../../../vector-space.md#matrix) is that scalar, so [determinant](../../../linear-algebra.md#determinant) one fixes it to $1$. Hence

$$
\boxed{\Phi:S^3\subset\mathbb C^2\longrightarrow SU(2),\qquad
(a,b)\longmapsto\begin{pmatrix}a&-\bar b\\b&\bar a\end{pmatrix}}
$$

is bijective, with inverse given by taking the first column. The forward map is real polynomial in the four coordinates; composing with the local logarithm charts verifies smoothness into the constructed manifold. The inverse is a smooth [matrix](../../../vector-space.md#matrix)-coordinate projection and, in the usual embedded sphere charts, is smooth into $S^3$. Thus $\boxed{SU(2)\cong S^3\text{ by a diffeomorphism}}$, the explicit realization of [SU(2) as the three-sphere](../../../topological-group.md#su-2-as-the-three-sphere).

## 2

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a positive-dimensional smooth connected manifold, three [equivalent formulations of orientability of a smooth manifold](../../../differential-geometry.md#equivalent-formulations-of-orientability-of-a-smooth-manifold) are an [oriented atlas](../../../differential-geometry.md#oriented-atlas), a continuously varying orientation of each [tangent space](../../../differential-geometry.md#tangent-space), and a nowhere-vanishing smooth top-degree [differential form](../../../differential-form.md). An orientation of a [tangent space](../../../differential-geometry.md#tangent-space) means a choice of one class of ordered bases, where two bases agree when their change-of-basis [determinant](../../../linear-algebra.md#determinant) is positive. The second formulation chooses these classes locally continuously; it does not require a global frame.

An [oriented atlas](../../../differential-geometry.md#oriented-atlas) has positive Jacobian [determinant](../../../linear-algebra.md#determinant) on every overlap. Its coordinate bases then give a consistent orientation of all [tangent spaces](../../../differential-geometry.md#tangent-space). Conversely, a continuous choice of tangent-space orientations makes the sign of a coordinate basis locally constant. Shrink to connected charts and reverse one coordinate when necessary; the resulting positively positively oriented coordinate charts have positive transition [determinants](../../../linear-algebra.md#determinant). An orientation in atlas language is the maximal collection of charts compatible with that positive sign convention.

We use the [partition of unity](../../../differential-geometry.md#partition-of-unity) theorem: every open cover of a Hausdorff second-countable [smooth manifold](../../../differential-geometry.md#smooth-manifold) has a smooth locally finite subordinate partition. From the oriented atlas, choose such a [partition of unity](../../../differential-geometry.md#partition-of-unity) $\rho_i$. Extend each $\rho_i\,dx_i^1\wedge\cdots\wedge dx_i^n$ by zero outside its chart and sum the locally finite family. At every point, the nonzero summands are positive multiples of one another and at least one coefficient is positive. Their sum is a smooth nowhere-zero form $\omega$. Conversely, a nowhere-zero form declares a basis positive exactly when $\omega(v_1,\ldots,v_n)>0$, giving a continuously varying orientation and hence an [oriented atlas](../../../differential-geometry.md#oriented-atlas). Two top forms define the same orientation precisely when $\omega'=h\omega$ for a smooth positive function $h$. Since a nonvanishing coefficient cannot change sign on a connected manifold, these definitions give exactly two opposite orientations.

For the unit sphere in $\mathbb R^{n+1}$, define

$$
\boxed{\omega_x(v_1,\ldots,v_n)=\det(x,v_1,\ldots,v_n)}.
$$

The radial vector $x$ is a unit normal, so appending any tangent basis gives an ambient basis and the [determinant](../../../linear-algebra.md#determinant) never vanishes. The form is smooth and provides the outward-normal-first orientation. Therefore $\boxed{S^n\text{ is orientable for every }n}$. For $n=0$, this is the nonzero zero-form taking opposite signs on the two sphere points; zero-dimensional manifolds admit orientations by assigning generator signs at their points.

For $n\ge1$, the quotient map $\pi:S^n\to\mathbb{RP}^n$ is a twofold smooth covering with [deck transformation](../../../algebraic-topology.md#deck-transformation) $A(x)=-x$. Its action on the sphere form is

$$
(A^*\omega)_x(v_1,\ldots,v_n)=\det(-x,-v_1,\ldots,-v_n)
=(-1)^{n+1}\omega_x(v_1,\ldots,v_n).
$$

If $n$ is odd, the form is invariant and descends using the local covering inverses to a nowhere-vanishing form on the quotient. If $n$ is even, suppose the quotient had a nonvanishing top form $\eta$. Its pullback would be $h\omega$ for a smooth nonzero function $h$ on the connected sphere and would be invariant under $A$. Invariance would require $h(-x)=-h(x)$, impossible because $h$ has constant sign. This proves the [orientability of real projective space](../../../algebraic-topology.md#orientability-of-real-projective-space) criterion

$$
\boxed{\mathbb{RP}^n\text{ is orientable exactly when }n\text{ is odd, for }n\ge1}.
$$

The separate endpoint $\mathbb{RP}^0$ is one point and is orientable, so the full nonnegative-dimensional answer is $n=0$ or $n$ odd.

## 3

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A subset $X\subset M^m$ is a $d$-dimensional [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) if, with the subspace topology, every point has a smooth ambient chart in which $X$ is the intersection of the coordinate domain with $\mathbb R^d\times\{0\}$. These slice charts give its smooth structure, and its inclusion is an [embedding](../../../geometry-and-topology.md#embedding).

The [inverse function theorem](../../../calculus.md#inverse-function-theorem) says that a smooth map $F:U\subset\mathbb R^m\to\mathbb R^m$ with invertible derivative at $a$ restricts to a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) between open neighborhoods of $a$ and $F(a)$. A point $q\in N$ is a [regular value](../../../differential-geometry.md#regular-value) of a smooth map $f:M^m\to N^n$ when $df_x:T_xM\to T_qN$ is surjective at every $x\in f^{-1}(q)$.

Choose local coordinates centered at $x$ and $q$. At a fiber point, rank $n$ means that, after relabeling coordinates, the first $n$ columns of the coordinate derivative form an invertible [matrix](../../../vector-space.md#matrix). Define

$$
F(u_1,\ldots,u_m)=\bigl(f_1(u),\ldots,f_n(u),u_{n+1},\ldots,u_m\bigr).
$$

Its derivative is block upper triangular with that invertible block and an identity block, hence invertible. The inverse function theorem makes $F$ a new ambient coordinate chart in which $f^{-1}(q)$ is exactly $v_1=\cdots=v_n=0$. Therefore the [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem) gives

$$
\boxed{f^{-1}(q)\text{ is an embedded submanifold of dimension }m-n}
$$

when the fiber is nonempty. An empty fiber is regular vacuously; if $m<n$, it is the only possible regular fiber. The construction does not assign a negative dimension to a nonempty manifold.

For the projective hyperplane, the map

$$
\iota:\mathbb{RP}^1\longrightarrow\mathbb{RP}^2,\qquad[a:b]\longmapsto[a:b:0]
$$

is injective with inverse $[x_0:x_1:0]\mapsto[x_0:x_1]$ on its image. At every image point, either $x_0$ or $x_1$ is nonzero; the corresponding standard projective chart uses $x_2/x_i$ as one coordinate and cuts the image out by setting it to zero. The map and inverse are smooth in these charts, and the slice condition proves

$$
\boxed{X\text{ is embedded and }X\cong\mathbb{RP}^1}.
$$

Nevertheless, $\mathbb{RP}^2\setminus X$ is the single affine chart $x_2\ne0$, diffeomorphic to $\mathbb R^2$, so it is connected. If a smooth real function had exactly this zero set with zero regular, the inverse function theorem near any point of $X$ would give both positive and negative values off $X$. On the connected complement it never vanishes, so continuity requires its sign to be constant. This contradiction is the obstruction that [regular zero hypersurfaces have disconnected complements](../../../differential-geometry.md#regular-zero-hypersurfaces-have-disconnected-complements). Thus

$$
\boxed{X\text{ cannot be a global regular zero set of a smooth real function}}.
$$

It illustrates why local defining equations for an embedded hypersurface need not glue to a global real defining function, as in [real projective hyperplane is not a global regular zero set](../../../differential-geometry.md#real-projective-hyperplane-is-not-a-global-regular-zero-set).

## 4

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A rank-$k$ [complex vector bundle](../../../fiber-bundle.md#complex-vector-bundle) is a smooth map $\pi:E\to B$ whose fibers are $k$-dimensional complex [vector spaces](../../../vector-space.md), with local [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism) $\Phi_i:\pi^{-1}(U_i)\to U_i\times\mathbb C^k$ commuting with projection and linear on every fiber. Define [transition functions of a vector bundle](../../../fiber-bundle.md#transition-function-of-a-vector-bundle) by

$$
\Phi_i\Phi_j^{-1}(b,v)=(b,g_{ij}(b)v),\qquad g_{ij}:U_i\cap U_j\to GL(k,\mathbb C).
$$

They are smooth and obey

$$
\boxed{g_{ii}=I,\qquad g_{ij}=g_{ji}^{-1},\qquad g_{ij}g_{jk}=g_{ik}}
$$

on the appropriate double/triple overlaps. The [structure group of a vector bundle](../../../fiber-bundle.md#structure-group-of-a-vector-bundle) is a Lie subgroup $G\subset GL(k,\mathbb C)$ in which a chosen set of transitions takes values. It records allowed changes of fiber frame; different trivializations may exhibit different reductions of that group.

Using the same cocycle, glue the disjoint union of $U_i\times G$ by

$$
(b,h)_j\sim(b,g_{ij}(b)h)_i.
$$

The cocycle makes this an equivalence relation and makes its local charts compatible. Right multiplication $(b,h)_i\cdot a=(b,ha)_i$ is well-defined because it commutes with the left gluing [matrices](../../../vector-space.md#matrix). It is free and transitive on each fiber. These charts therefore construct the associated right [principal bundle](../../../fiber-bundle.md#principal-bundle) $P\to B$ with group $G$.

For the natural line realization, take the [complex tautological line bundle](../../../fiber-bundle.md#complex-tautological-line-bundle) $L=\{(\ell,v):\ell\in\mathbb{CP}^1,\ v\in\ell\subset\mathbb C^2\}$. Its nonzero vectors identify with $\mathbb C^2\setminus\{0\}$ by $(\ell,v)\mapsto v$, with projection $v\mapsto[v]$. On the two standard charts, use $\zeta=z_2/z_1$ and $\eta=z_1/z_2=1/\zeta$. The local frames are $e_0=(1,\zeta)$ and $e_1=(\eta,1)$, so $e_1=e_0/\zeta$. Normalize them using the ambient Hermitian norm:

$$
u_0=\frac{(1,\zeta)}{\sqrt{1+|\zeta|^2}},\qquad
u_1=\frac{(\eta,1)}{\sqrt{1+|\eta|^2}}
=\frac{|\zeta|}{\zeta}u_0.
$$

If $v=t_0u_0=t_1u_1$, then $t_0=(|\zeta|/\zeta)t_1$. Thus the [unitary transitions of the tautological line over the projective line](../../../fiber-bundle.md#unitary-transitions-of-the-tautological-line-over-the-projective-line) are

$$
\boxed{g_{01}(\zeta)=\frac{|\zeta|}{\zeta}\in S^1,\qquad
g_{10}=g_{01}^{-1},\qquad g_{00}=g_{11}=1}.
$$

These are smooth on the overlap $\zeta\ne0$. A [Hermitian metric on a smooth complex vector bundle](../../../fiber-bundle.md#hermitian-metric-on-a-smooth-complex-vector-bundle) generally permits precisely this unitary reduction; here the ambient norm supplies it explicitly.

The corresponding principal circle bundle consists of unit vectors in the tautological line. Sending $(\ell,v)$ to $v$ identifies its total space with $S^3\subset\mathbb C^2$, and the right circle action is $v\cdot e^{i\theta}=e^{i\theta}v$. Identify $\mathbb{CP}^1$ with $S^2$ using

$$
[z_1:z_2]\longmapsto
\frac{(2\operatorname{Re}(z_1\bar z_2),\ 2\operatorname{Im}(z_1\bar z_2),\ |z_1|^2-|z_2|^2)}{|z_1|^2+|z_2|^2}.
$$

Its affine-coordinate inverse on the chart $Z\ne-1$ is $\zeta=(X-iY)/(1+Z)$; the other chart handles the missing pole. This gives a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), and the projection becomes the [Hopf fibration](../../../algebraic-topology.md#hopf-fibration)

$$
\boxed{S^3\longrightarrow S^2,\qquad
(z_1,z_2)\longmapsto(2\operatorname{Re}(z_1\bar z_2),2\operatorname{Im}(z_1\bar z_2),|z_1|^2-|z_2|^2)}.
$$

There is a distinction if the stated punctured-bundle identification is interpreted only as a projection-preserving [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism), rather than a fiber-linear identification. It does not determine whether the complex line is tautological or dual: for a nonzero $\phi\in L_\ell^*$, the unique $v\in\ell$ with $\phi(v)=1$ gives a smooth map $L^*\setminus0\to L\setminus0$. Locally it is inversion of a nonzero complex number. Thus [punctured line bundles do not determine their duality sign](../../../fiber-bundle.md#punctured-line-bundles-do-not-determine-their-duality-sign).

For completeness, these are the only possible signs here. Complex line bundles over $S^2$ are described by the [clutching construction](../../../fiber-bundle.md#clutching-construction) with a loop in $\mathbb C^*$, reducible to $S^1$, and its integer [winding number](../../../complex-analysis.md#winding-number) determines the bundle: a zero-degree ratio has a logarithm and can be removed by changes of trivializations extending over the two disks. For [winding number](../../../complex-analysis.md#winding-number) $d$, the unit circle bundle has [fundamental group](../../../algebraic-topology.md#fundamental-group) $\mathbb Z/d\mathbb Z$, as the two solid-torus trivializations identify the common fiber generator and impose its $d$th power as the equatorial gluing relation. There is a fiberwise radial [deformation retraction](../../../algebraic-topology.md#deformation-retraction) from the punctured [line bundle](../../../ringed-space.md#line-bundle) onto its unit circle bundle. Since $\mathbb C^2\setminus0$ retracts to [simply connected](../../../algebraic-topology.md#simply-connected-space) $S^3$, the hypothesis forces $|d|=1$.

Consequently the allowed unitary transitions are the displayed $g_{01}$ or its reciprocal, according to the bundle's sign. For the dual, the same underlying Hopf projection has the inverse principal action $v\cdot e^{i\theta}=e^{-i\theta}v$. **In either case the principal total space and projection are $S^3\to S^2$; the purely diffeomorphic hypothesis alone leaves the circle-action sign unspecified**.

## 5

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [Riemannian metric](../../../differential-geometry.md#riemannian-metric) is a smooth positive-definite symmetric [inner product](../../../linear-algebra.md#inner-product) $g_x$ on every [tangent space](../../../differential-geometry.md#tangent-space). A [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) is a connection on the [tangent bundle](../../../fiber-bundle.md#tangent-bundle) which is torsion-free, $\nabla_XY-\nabla_YX=[X,Y]$, and metric-compatible,

$$
Xg(Y,Z)=g(\nabla_XY,Z)+g(Y,\nabla_XZ).
$$

Apply this identity with the cyclic triples $(X,Y,Z)$, $(Y,Z,X)$ and $(Z,X,Y)$, add the first two and subtract the third, and replace differences of covariant derivatives by [Lie brackets](../../../lie-algebra.md#lie-bracket). The result is the [Koszul formula](../../../fiber-bundle.md#koszul-formula)

$$
\boxed{\begin{aligned}
2g(\nabla_XY,Z)={}&Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)\\
&-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
\end{aligned}}
$$

Its right side depends only on $g$ and the [vector fields](../../../calculus.md#vector-field); nondegeneracy of $g$ determines $\nabla_XY$ uniquely. This proves uniqueness.

For existence, in a coordinate chart define

$$
\Gamma^k_{ij}=\frac12g^{k\ell}(\partial_i g_{j\ell}+\partial_jg_{i\ell}-\partial_\ell g_{ij}),\qquad
(\nabla_XY)^k=X^i\partial_iY^k+\Gamma^k_{ij}X^iY^j.
$$

This is linear over smooth functions in $X$ and obeys the Leibniz rule in $Y$. Symmetry $\Gamma^k_{ij}=\Gamma^k_{ji}$ proves zero torsion, and direct substitution gives

$$
\partial_i g_{jk}=g_{\ell k}\Gamma^\ell_{ij}+g_{j\ell}\Gamma^\ell_{ik},
$$

which proves [metric compatibility](../../../fiber-bundle.md#metric-compatibility). On chart overlaps the two resulting connections satisfy the same intrinsic Koszul identity and therefore agree by uniqueness. They glue globally. Thus the [existence and uniqueness of the Levi-Civita connection](../../../fiber-bundle.md#existence-and-uniqueness-of-the-levi-civita-connection) holds on every [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold).

Fix the curvature convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z.
$$

For coordinate vectors $e_i$, define the [Riemann curvature tensor](../../../general-relativity.md#riemann-curvature-tensor) components by $R_{ij,kl}=g(R(e_i,e_j)e_l,e_k)$. In these indices the Ricci and scalar contractions are

$$
\boxed{\operatorname{Ric}_{jl}=g^{ik}R_{ij,kl},\qquad
s=g^{jl}\operatorname{Ric}_{jl}=g^{ik}g^{jl}R_{ij,kl}}.
$$

Explicitly, $R_{ij,kl}=g_{ka}R^a{}_{l ij}$, where

$$
R^a{}_{l ij}=\partial_i\Gamma^a_{jl}-\partial_j\Gamma^a_{il}
+\Gamma^a_{ip}\Gamma^p_{jl}-\Gamma^a_{jp}\Gamma^p_{il}.
$$

These expressions define [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature) and [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) without ambiguity about which indices are contracted. With this convention a round unit $m$-sphere has $\operatorname{Ric}=(m-1)g$ and $s=m(m-1)$.

If $\operatorname{Ric}=\lambda g$ with a constant real $\lambda$, tracing gives $\boxed{s=m\lambda}$, so every [Einstein metric](../../../second-fundamental-form.md#einstein-metric) has constant [scalar curvature](../../../second-fundamental-form.md#scalar-curvature). The converse is not valid in arbitrary dimension. On $S^2\times S^1$ with the [product Riemannian metric](../../../differential-geometry.md#product-riemannian-metric) of the unit round sphere and a circle, the connection splits between factors. The mixed curvatures and circle curvature vanish, while the sphere has curvature one. Hence

$$
\boxed{\operatorname{Ric}=g_{S^2}\oplus0,\qquad s=2\text{ everywhere}}.
$$

A scalar multiple of the whole metric would require $\lambda=1$ on the sphere directions and $\lambda=0$ on the circle direction, which is impossible. This proves that [constant scalar curvature does not imply an Einstein metric](../../../second-fundamental-form.md#constant-scalar-curvature-does-not-imply-an-einstein-metric), and supplies a counterexample to the unrestricted requested equivalence.

In dimension two, the curvature tensor is determined by the [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) $K$:

$$
R_{ij,kl}=K(g_{ik}g_{jl}-g_{il}g_{jk}),\qquad
\operatorname{Ric}=Kg,\qquad s=2K.
$$

There the valid equivalence is

$$
\boxed{s\text{ constant}\iff\operatorname{Ric}=\lambda g\text{ with constant }\lambda=s/2}.
$$

In dimension one both curvature and [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) vanish identically. Without a two-dimensional restriction or another added geometric hypothesis, the general converse cannot be proved.

## 6

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

On an oriented Riemannian $n$-manifold, the [metric volume form](../../../differential-form.md#metric-volume-form) is the unique top form taking value one on every positively oriented orthonormal tangent basis. In a positive coordinate chart it is

$$
\boxed{\operatorname{vol}_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n}.
$$

For another positive coordinate chart $y$, write $A=\partial x/\partial y$. Then $g_y=A^{\mathsf T}g_xA$, so $\sqrt{\det g_y}=\det A\sqrt{\det g_x}$, since $\det A>0$. The wedge of coordinate differentials acquires the same [determinant](../../../linear-algebra.md#determinant) factor. The two local expressions agree, proving coordinate independence and smooth global existence. Positivity of the chosen charts is what fixes the sign of the [volume form](../../../differential-form.md#volume-form).

The metric induces the [inner product on exterior powers of a cotangent space](../../../differential-geometry.md#inner-product-on-exterior-powers-of-a-cotangent-space). Define the [Hodge star operator](../../../differential-form.md#hodge-star-operator) $*:\Lambda^pT^*M\to\Lambda^{n-p}T^*M$ by

$$
\boxed{\alpha\wedge*\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g}
$$

for forms of the same degree, and apply it fiberwise to smooth forms. In an oriented orthonormal coframe, if $I$ is an increasing $p$-index and $I^c$ its ordered complement, $*e^I=\epsilon(I,I^c)e^{I^c}$. Exchanging the two blocks has sign $(-1)^{p(n-p)}$, so

$$
\boxed{*^2|_{\Omega^p}=(-1)^{p(n-p)}I}.
$$

Use the real $L^2$ [inner product](../../../linear-algebra.md#inner-product) $(\alpha,\beta)=\int_M\alpha\wedge*\beta$. For a $p$-form $\alpha$ and a $(p+1)$-form $\beta$, the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) and the given boundaryless Stokes identity give

$$
0=\int_M d(\alpha\wedge*\beta)
=\int_M d\alpha\wedge*\beta+(-1)^p\int_M\alpha\wedge d*\beta.
$$

The [codifferential](../../../differential-form.md#codifferential) acting on $\beta$ has sign $(-1)^{n(p+2)+1}$. Applying the star once more and using its square on the $(n-p)$-form $d*\beta$ gives

$$
*\delta\beta=(-1)^{n(p+2)+1+p(n-p)}d*\beta=(-1)^{p+1}d*\beta.
$$

The exponent reduction uses parity, since $p^2\equiv p\pmod2$. Combining the two displayed identities proves $(d\alpha,\beta)=(\alpha,\delta\beta)$. Symmetry of the real [inner product](../../../linear-algebra.md#inner-product) supplies precisely

$$
\boxed{\int_M\beta\wedge*d\alpha=\int_M\delta\beta\wedge*\alpha}.
$$

Thus [Hodge integration by parts in arbitrary degree](../../../differential-form.md#hodge-integration-by-parts-in-arbitrary-degree) identifies $\delta$ as the formal adjoint of $d$. The displayed bilinear identity extends to complex [differential forms](../../../differential-form.md) by complex linearity. For positive norm identities on complex forms, use the Hermitian [inner product](../../../linear-algebra.md#inner-product) with conjugation instead.

With the nonnegative convention, the [Hodge Laplacian](../../../differential-form.md#hodge-laplacian) is

$$
\boxed{\Delta=d\delta+\delta d}.
$$

It is the form-valued extension of the [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator), whose action on functions is $-\operatorname{div}\operatorname{grad}$. A [harmonic differential form](../../../differential-form.md#harmonic-differential-form) is a smooth form in $\ker\Delta$. The adjoint identity gives

$$
(\Delta\alpha,\alpha)=\|d\alpha\|_{L^2}^2+\|\delta\alpha\|_{L^2}^2.
$$

If $\Delta\alpha=0$, both norms vanish, and smoothness implies

$$
\boxed{d\alpha=0,\qquad\delta\alpha=0}.
$$

The closed compact hypotheses are essential for the absence of boundary terms and this global energy conclusion.

The [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem) states that on a closed oriented [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold)

$$
\boxed{\Omega^p(M)=\mathcal H^p(M)\oplus d\Omega^{p-1}(M)\oplus\delta\Omega^{p+1}(M)}
$$

is an $L^2$-orthogonal direct sum, with finite-dimensional harmonic space $\mathcal H^p$. Every smooth form has unique harmonic, exact and coexact components, although primitives of the latter two need not be unique. Equivalently every [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class has a unique harmonic representative. An exact harmonic form belongs to both the harmonic and exact summands; their orthogonality makes its squared norm zero. Therefore $\boxed{\alpha\text{ exact and harmonic}\Longrightarrow\alpha=0}$. The same conclusion follows directly from $\alpha=d\eta$ and $\|\alpha\|^2=(\delta\alpha,\eta)=0$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
