# Paper 115

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_115.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_115.pdf)

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

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [exterior derivative](../../../differential-form.md#exterior-derivative) is the real-linear degree-one map $d:\Omega^r(M)\to\Omega^{r+1}(M)$ characterized by $df(X)=Xf$ on [smooth functions](../../../analysis.md#smooth-function), the graded [Leibniz rule](../../../calculus.md#leibniz-rule)

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^r\alpha\wedge d\beta
\qquad(\alpha\in\Omega^r(M)),
$$

and $d^2=0$. In [local coordinates](../../../complex-analysis.md#local-coordinate) $(x^1,\ldots,x^m)$, write $\alpha=\sum_I\alpha_I dx^{i_1}\wedge\cdots\wedge dx^{i_r}$ using [multi-index notation](../../../distribution-theory.md#multi-index-notation). Since $dx^i=d(x^i)$ and hence $d(dx^i)=0$, the defining rules force

$$
\boxed{d\alpha=\sum_{I,j}\frac{\partial\alpha_I}{\partial x^j}dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_r}.}
$$

This proves local uniqueness, and the coordinate formulas agree on overlaps because the same rules are preserved by the [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form). They also directly define an operator satisfying all three rules, proving existence.

An [exact differential form](../../../differential-form.md#exact-differential-form) is a form $\omega=d\eta$. Let $\pi:S^{2n}\to\mathbb{RP}^{2n}$ be the antipodal double [covering map](../../../algebraic-topology.md#covering-space) and let $a(x)=-x$. For a $2n$-form $\omega$ on real projective space, $a^*\pi^*\omega=\pi^*\omega$, while the [mapping degree](../../../homology.md#degree-of-a-continuous-mapping) of the [antipodal map](../../../homology.md#antipodal-map) is $-1$. Therefore

$$
\int_{S^{2n}}\pi^*\omega
=\int_{S^{2n}}a^*\pi^*\omega
=-\int_{S^{2n}}\pi^*\omega=0.
$$

By the stated criterion, $\pi^*\omega=d\eta$. The [invariant primitive under a finite group action](../../../homology.md#invariant-primitive-under-a-finite-group-action)

$$
\bar\eta=\frac12(\eta+a^*\eta)
$$

still satisfies $d\bar\eta=\pi^*\omega$ and descends to a form $\beta$ on $\mathbb{RP}^{2n}$. Since pullback through a covering is injective on differential forms, $\pi^*(d\beta-\omega)=0$ implies $d\beta=\omega$. Thus **every $2n$-form on $\mathbb{RP}^{2n}$ is exact**; this is the [top-degree differential forms on even-dimensional real projective space are exact](../../../homology.md#top-degree-differential-forms-on-even-dimensional-real-projective-space-are-exact) result.

The $k$th [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) is

$$
H^k_{\mathrm{dR}}(M)=\frac{\ker(d:\Omega^k(M)\to\Omega^{k+1}(M))}{\operatorname{im}(d:\Omega^{k-1}(M)\to\Omega^k(M))},
$$

the [closed differential forms](../../../differential-form.md#closed-differential-form) modulo the exact ones. For the product, let $p:M\times S^1\to M$ be projection and choose a closed one-form $\nu$ on the circle with $\int_{S^1}\nu=1$. [Averaging differential forms over the circle](../../../differential-form.md#averaging-differential-forms-over-the-circle) is cochain-homotopic to the identity, so every class has a rotation-invariant representative; if such a representative is exact, averaging a primitive gives an invariant primitive. Every invariant $k$-form has a unique decomposition $p^*\alpha+p^*\beta\wedge\nu$, and

$$
d(p^*\alpha+p^*\beta\wedge\nu)=p^*(d\alpha)+p^*(d\beta)\wedge\nu.
$$

Closedness and exactness are therefore componentwise. Hence the map

$$
\boxed{([\alpha],[\beta])\longmapsto[p^*\alpha+p^*\beta\wedge\nu]}
$$

is a well-defined bijection $H^k_{\mathrm{dR}}(M)\oplus H^{k-1}_{\mathrm{dR}}(M)\to H^k_{\mathrm{dR}}(M\times S^1)$, proving the [de Rham cohomology of a product with a circle](../../../differential-form.md#de-rham-cohomology-of-a-product-with-a-circle) formula.

## 2

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

An [immersed submanifold](../../../differential-geometry.md#immersed-submanifold) of $M$ is a manifold $Y$ equipped with an injective [immersion](../../../differential-geometry.md#immersion) $\psi:Y\to M$. It is an [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) when $\psi$ is also a homeomorphism onto its image with the subspace topology, equivalently when it is a [smooth embedding](../../../differential-geometry.md#smooth-embedding). For irrational $\alpha$, the [irrational winding of the torus](../../../differential-geometry.md#irrational-winding-of-the-torus)

$$
t\longmapsto(e^{it},e^{i\alpha t})
$$

is an injective immersion $\mathbb R\to T^2$ with dense image, and therefore is not an embedding. If $Y$ is compact, however, an injective immersion is a continuous bijection from a [compact](../../../topology.md#compact-space) space to its image in the [Hausdorff](../../../topology.md#hausdorff-space) manifold $M$; its inverse is continuous. Thus the [compact injective immersion is an embedding](../../../differential-geometry.md#compact-injective-immersion-is-an-embedding) theorem makes $\psi(Y)$ embedded.

Now let $X\subset M$ be embedded, with $\dim M=m$, $\dim X=m-k$, and $p\in X$. Apply the [constant rank theorem](../../../calculus.md#constant-rank-theorem) to its inclusion. After choosing coordinates and reordering them, there is a neighborhood $U$ of $p$ with coordinates $(x^1,\ldots,x^m)$ for which

$$
\boxed{U\cap X=\{x^1=\cdots=x^k=0\}.}
$$

This is the [slice chart for an embedded submanifold](../../../differential-geometry.md#slice-chart-for-an-embedded-submanifold).

It is **false** that every embedded submanifold is the inverse image of a regular value of a map to a [Euclidean space](../../../functional-analysis.md#euclidean-norm). If a codimension-$k$ submanifold is $f^{-1}(y)$ for a [regular value](../../../differential-geometry.md#regular-value) of $f:M\to\mathbb R^k$, the differentials of the component functions give a global frame of its conormal bundle, so its [normal bundle](../../../algebraic-geometry.md#normal-bundle) is trivial. The core circle of the [Möbius band](../../../topology.md#mobius-band) is embedded but has the nontrivial Möbius normal line bundle. This is the [normal-bundle obstruction to being a regular level set](../../../differential-geometry.md#normal-bundle-obstruction-to-being-a-regular-level-set).

Finally, an inductive spinning construction gives the requested torus. Place an embedding $F:N^m\hookrightarrow\mathbb R^{m+1}$ in the half-space $F_{m+1}>0$ and define

$$
\widetilde F(x,e^{i\theta})=
\bigl(F_1(x),\ldots,F_m(x),F_{m+1}(x)\cos\theta,F_{m+1}(x)\sin\theta\bigr).
$$

The positive radius makes this map injective, and its differential is injective in both the $N$ and circle directions; compactness then makes it an embedding. Starting with $S^1\hookrightarrow\mathbb R^2$ and iterating proves the [embedding of the n-dimensional torus in codimension one](../../../topology.md#embedding-of-the-n-dimensional-torus-in-codimension-one):

$$
\boxed{T^n\hookrightarrow\mathbb R^{n+1}.}
$$

## 3

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [Lie group](../../../lie-theory.md#lie-group) is a [group](../../../group.md) and [smooth manifold](../../../differential-geometry.md#smooth-manifold) whose multiplication and inversion are smooth. A [Lie algebra](../../../lie-algebra.md) is a [vector space](../../../vector-space.md) with a bilinear alternating bracket satisfying the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). For a [Matrix Lie group](../../../lie-theory.md#matrix-lie-group) $G\subset GL(m,\mathbb C)$, a [logarithmic chart of a matrix Lie group](../../../lie-theory.md#logarithmic-chart-of-a-matrix-lie-group) near $g$ sends $h$ to $\log(g^{-1}h)\in\mathfrak g=T_I G$; the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) is its local inverse, and the [Baker--Campbell--Hausdorff formula](../../../linear-operator-theory.md#baker-campbell-hausdorff-formula) makes the local group operations smooth.

For $B_1,B_2\in\mathfrak g$, consider the group commutator

$$
C(s,t)=e^{sB_1}e^{tB_2}e^{-sB_1}e^{-tB_2}\in G.
$$

Its logarithm takes values in the vector space $\mathfrak g$, and expansion at $(0,0)$ gives

$$
\frac{\partial^2}{\partial s\,\partial t}\bigg|_{(0,0)}\log C(s,t)
=B_1B_2-B_2B_1.
$$

Thus $\mathfrak g$ is closed under the [commutator](../../../lie-algebra.md#commutator). Bilinearity, alternation, and the Jacobi identity follow from matrix multiplication, so this proves that the [Lie algebra of a matrix Lie group](../../../lie-algebra.md#lie-algebra-of-a-matrix-lie-group) has

$$
\boxed{[B_1,B_2]=B_1B_2-B_2B_1.}
$$

A [principal bundle](../../../fiber-bundle.md#principal-bundle) $\pi:P\to M$ with structure group $G$ is a smooth [fiber bundle](../../../fiber-bundle.md) with a free right $G$-action, each fiber a single orbit, and equivariant local trivializations $\pi^{-1}(U)\cong U\times G$.

For the right action of the [unitary group](../../../topological-group.md#unitary-group) on $GL(n,\mathbb C)$, define

$$
q(g)=\frac12\log(gg^*)\in H(n).
$$

The matrix $gg^*$ is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) and a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator), and $q(gu)=q(g)$ for $u\in U(n)$. The [polar decomposition of an invertible complex matrix](../../../linear-algebra.md#polar-decomposition-of-an-invertible-complex-matrix) gives the unique factorization

$$
g=e^{q(g)}u(g),
\qquad u(g)=e^{-q(g)}g\in U(n).
$$

Consequently

$$
\Phi:H(n)\times U(n)\longrightarrow GL(n,\mathbb C),
\qquad(B,u)\longmapsto e^Bu
$$

is a diffeomorphism. If $W\subset H(n)$ is a neighborhood of zero and $N=q^{-1}(W)$, then $N$ is an open neighborhood of $I$, it is a union of complete orbits, and

$$
V=\bigcup_{h\in N}R(h)=N\cong W\times U(n).
$$

Moreover, two matrices have the same value of $q$ exactly when they differ by right multiplication by a unitary matrix. Thus $q$ induces the smooth identification

$$
\boxed{M=GL(n,\mathbb C)/U(n)\cong H(n),}
$$

under which $\pi$ is projection $H(n)\times U(n)\to H(n)$. This is the [general linear group modulo the unitary group](../../../fiber-bundle.md#general-linear-group-modulo-the-unitary-group), and $\pi$ is in fact a globally trivial principal $U(n)$-bundle.

## 4

↑ **Parent:** [Paper 115](paper-115.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) of a [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) $(M,g)$ is the unique [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) on $TM$ that is [torsion-free](../../../fiber-bundle.md#torsion-free-connection) and compatible with the [Riemannian metric](../../../differential-geometry.md#riemannian-metric). Any such connection must satisfy the [Koszul formula](../../../fiber-bundle.md#koszul-formula)

$$
\begin{aligned}
2g(\nabla_XY,Z)={}&Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)\\
&-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
\end{aligned}
$$

Nondegeneracy of $g$ determines $\nabla_XY$ uniquely from the right-hand side. Conversely, define $\nabla$ by this formula. Direct substitution shows that it is $C^\infty$-linear in $X$, satisfies the [Leibniz rule](../../../calculus.md#leibniz-rule) in $Y$, preserves $g$, and obeys $\nabla_XY-\nabla_YX=[X,Y]$. It is therefore a torsion-free metric connection. This proves the [existence and uniqueness of the Levi-Civita connection](../../../fiber-bundle.md#existence-and-uniqueness-of-the-levi-civita-connection).

For the metric vector bundle $E$, choose the stated orthonormal local frame $(e_1,\ldots,e_m)$ and write $d_Ae_j=A^i{}_j e_i$. Since $\langle e_i,e_j\rangle=\delta_{ij}$, metric compatibility gives

$$
0=d\langle e_i,e_j\rangle
=\langle d_Ae_i,e_j\rangle+\langle e_i,d_Ae_j\rangle
=A^j{}_i+A^i{}_j.
$$

Hence the [connection matrix in an orthonormal frame is skew-symmetric](../../../fiber-bundle.md#connection-matrix-in-an-orthonormal-frame-is-skew-symmetric):

$$
\boxed{A^i{}_j=-A^j{}_i.}
$$

On an oriented Riemannian $d$-manifold, the [Hodge star operator](../../../differential-form.md#hodge-star-operator) is defined by

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle\,d\operatorname{vol}_g.
$$

It is an orthogonal map $*:\Lambda^rT_x^*M\to\Lambda^{d-r}T_x^*M$ and satisfies $*^2=(-1)^{r(d-r)}$. In dimension $d=2n$ on middle-degree forms, the [Adjoint of the Hodge star on middle-degree forms](../../../differential-form.md#adjoint-of-the-hodge-star-on-middle-degree-forms) is

$$
*^\dagger=*^{-1}=(-1)^{n^2}*.
$$

Thus it is self-adjoint when $n$ is even, but **it is not always self-adjoint**. For $n=1$ on the oriented Euclidean plane,

$$
*dx=dy,
\qquad *dy=-dx,
$$

so its matrix in the orthonormal basis $(dx,dy)$ is skew-adjoint.

The [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator) on differential forms is the [Hodge Laplacian](../../../differential-form.md#hodge-laplacian)

$$
\Delta=d\delta+\delta d,
$$

where the [codifferential](../../../differential-form.md#codifferential) $\delta$ is the formal $L^2$ adjoint of the [exterior derivative](../../../differential-form.md#exterior-derivative). On a compact manifold without boundary, if $\Delta\omega=\lambda\omega$ for a nonzero differential form $\omega$, then [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\lambda\lVert\omega\rVert_{L^2}^2
=\langle\Delta\omega,\omega\rangle_{L^2}
=\lVert d\omega\rVert_{L^2}^2+\lVert\delta\omega\rVert_{L^2}^2\geq0.
$$

Therefore the [nonnegativity of the Hodge Laplacian](../../../differential-form.md#nonnegativity-of-the-hodge-laplacian) yields

$$
\boxed{\lambda\geq0.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
