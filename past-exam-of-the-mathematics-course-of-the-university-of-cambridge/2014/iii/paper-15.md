# Paper 15

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_15.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_15.pdf)

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

The [exterior derivative](../../../differential-form.md#exterior-derivative) is an $\mathbb R$-linear map $d:\Omega^p(M)\to\Omega^{p+1}(M)$, agrees with the differential $df$ of a [smooth function](../../../analysis.md#smooth-function), satisfies the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) $d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^p\alpha\wedge d\beta$ for $\alpha\in\Omega^p(M)$, and has $d^2=0$. These properties determine it locally and hence globally. To see locality directly, if a [differential form](../../../differential-form.md) $\alpha$ vanishes near $x$, choose a [smooth bump function](../../../partial-differential-equation.md#smooth-bump-function) $\chi$ equal to one near $x$ and supported where $\alpha=0$. The identity $d(\chi\alpha)=d\chi\wedge\alpha+\chi d\alpha$ gives $(d\alpha)_x=0$. Thus global forms can be computed using local extensions in a [manifold chart](../../../differential-geometry.md#manifold-chart).

In coordinates write $\alpha=\sum_Ia_I\,dx^{i_1}\wedge\cdots\wedge dx^{i_p}$. Since $d(dx^i)=d^2x^i=0$, the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) forces

$$
d\alpha=\sum_{I,j}\partial_ja_I\,dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_p}.
$$

This is the [uniqueness of the exterior derivative from its axioms](../../../differential-form.md#uniqueness-of-the-exterior-derivative-from-its-axioms). The coordinate formula also establishes existence: it has the stated properties, and the [chain rule](../../../calculus.md#chain-rule) shows that coordinate changes give the same operator.

The [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) is the real [quotient vector space](../../../vector-space.md#quotient-vector-space)

$$
H^p_{\mathrm{dR}}(M)=\frac{\ker(d:\Omega^p(M)\to\Omega^{p+1}(M))}{\operatorname{im}(d:\Omega^{p-1}(M)\to\Omega^p(M))}.
$$

Thus a [cohomology class](../../../cohomology.md#cohomology-class) records a [closed differential form](../../../differential-form.md#closed-differential-form) modulo an [exact differential form](../../../differential-form.md#exact-differential-form). In degree zero there are no exact forms; closed functions are locally constant. The [Poincaré lemma](../../../differential-form.md#poincare-lemma) says that every closed form of positive degree on a star-shaped open subset of $\mathbb R^n$ is exact, and hence that positive-degree closed forms are locally exact on a [smooth manifold](../../../differential-geometry.md#smooth-manifold).

For the [first de Rham cohomology of the two-sphere](../../../differential-form.md#first-de-rham-cohomology-of-the-two-sphere), let $U=S^2\setminus\{N\}$ and $V=S^2\setminus\{S\}$. [Stereographic projection](../../../complex-analysis.md#stereographic-projection) identifies each with $\mathbb R^2$, so a closed one-form $\alpha$ has primitives $f_U,f_V$. On the connected overlap $U\cap V$, the [derivative](../../../calculus.md#derivative) of $f_U-f_V$ is zero, so this difference is a constant. Subtracting that constant from $f_U$ makes the primitives agree. They glue to a global smooth primitive. Therefore **$H^1_{\mathrm{dR}}(S^2)=0$.**

Let $q:S^2\to\mathbb{RP}^2$ be the double [covering map](../../../algebraic-topology.md#covering-space) and $a$ the [antipodal map](../../../homology.md#antipodal-map). The [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) identifies forms downstairs with $a$-invariant forms upstairs. Averaging $(\eta+a^*\eta)/2$ commutes with $d$. If an invariant form is exact upstairs, averaging its primitive proves it exact downstairs. Conversely an invariant [cohomology class](../../../cohomology.md#cohomology-class) has an invariant representative by the same averaging. This proves the [de Rham cohomology of a finite quotient](../../../differential-form.md#de-rham-cohomology-of-a-finite-quotient) identification $H^p_{\mathrm{dR}}(\mathbb{RP}^2)\cong H^p_{\mathrm{dR}}(S^2)^{a^*}$. In degree zero the sphere is connected and $a^*$ fixes constants; degree one is zero; in degree two the granted action is multiplication by $-1$, whose invariant real subspace is zero. Forms of degree greater than two vanish. Hence

$$
\boxed{H^p_{\mathrm{dR}}(\mathbb{RP}^2)=\begin{cases}\mathbb R,&p=0,\\0,&p>0.\end{cases}}
$$

This is real [de Rham cohomology](../../../differential-form.md#de-rham-cohomology); it does not detect the integral two-torsion of the [real projective plane](../../../differential-geometry.md#real-projective-plane).

## 2

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [Lie group](../../../lie-theory.md#lie-group) is a finite-dimensional [smooth manifold](../../../differential-geometry.md#smooth-manifold) with a group structure for which multiplication and inversion are smooth. The group defined here is the [compact symplectic group](../../../topological-group.md#compact-symplectic-group) $Sp(n)=U(2n)\cap Sp(2n,\mathbb C)$, rather than the full complex symplectic group. Also, the displayed matrix expression requires $B$ to be $2n\times2n$; the printed $n\times n$ size is incompatible with $J$.

Since $J^2=-I$, we have $J^{-1}=-J$. The [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) commutes with conjugation, as follows term by term from its absolutely convergent [power series](../../../real-analysis.md#power-series). Consequently

$$
e^{-JBJ}=e^{JBJ^{-1}}=Je^BJ^{-1}=-Je^BJ.
$$

To construct [logarithm charts for the compact symplectic group](../../../topological-group.md#logarithm-charts-for-the-compact-symplectic-group), consider the real [vector space](../../../vector-space.md)

$$
\mathfrak k=\{X:X^*=-X,\quad XJ+JX^t=0\}.
$$

Differentiating the defining identities at $I$ gives precisely these conditions. Conversely if $X\in\mathfrak k$, $e^X$ is unitary and

$$
\frac d{dt}(e^{tX}Je^{tX^t})=e^{tX}(XJ+JX^t)e^{tX^t}=0,
$$

so $e^X\in Sp(n)$. These are the infinitesimal conditions of the [compact symplectic Lie algebra](../../../semisimple-lie-algebra.md#compact-symplectic-lie-algebra).

Near $I$, the convergent [matrix logarithm](../../../vector-space.md#matrix-logarithm) series $\log(I+C)=\sum_{m\ge1}(-1)^{m+1}C^m/m$ is smooth and inverse to the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) near zero. These local inverses respect transpose, conjugate transpose, and conjugation; also $\log(A^{-1})=-\log A$ when both matrices are sufficiently close to $I$. Shrink their neighborhoods accordingly. If $A\in Sp(n)$ there, unitarity gives

$$
(\log A)^*=\log(A^*)=\log(A^{-1})=-\log A.
$$

The symplectic identity is equivalent to $A^t=J^{-1}A^{-1}J$, so, putting $X=\log A$, it gives $X^t=-J^{-1}XJ=JXJ$, equivalently $XJ+JX^t=0$. Thus this local logarithm restricts to a bijection between a neighborhood of $I$ in $Sp(n)$ and an open neighborhood of zero in $\mathfrak k$. Its inverse is the restricted [matrix exponential](../../../linear-operator-theory.md#matrix-exponential). These restrictions are [manifold charts](../../../differential-geometry.md#manifold-chart); left multiplication translates them to every $A_0\in Sp(n)$ via $A\mapsto\log(A_0^{-1}A)$. The chart overlaps are smooth compositions of multiplication, exponential and logarithm. The subspace topology is Hausdorff and second countable, inherited from the finite-dimensional matrix space, so these charts give a [smooth manifold](../../../differential-geometry.md#smooth-manifold).

Closure under products and inverses follows from $AJ A^t=J$ and unitarity. Matrix multiplication is polynomial in real and imaginary entries, and inversion on the unitary group is $A\mapsto A^*$, a real linear operation. Their restrictions are smooth in the charts just constructed. Hence $Sp(n)$ is a [Lie group](../../../lie-theory.md#lie-group) without needing a closed-subgroup theorem.

Write $X$ in $n\times n$ blocks. The two infinitesimal conditions give

$$
X=\begin{pmatrix}P&Q\\-\overline Q&\overline P\end{pmatrix},\qquad P^*=-P,\quad Q^t=Q.
$$

The [skew-Hermitian matrix](../../../linear-operator-theory.md#skew-hermitian-matrix) $P$ has $n^2$ real parameters; the complex symmetric matrix $Q$ has $n(n+1)/2$ complex parameters, hence $n(n+1)$ real parameters. Therefore

$$
\boxed{\dim_{\mathbb R}Sp(n)=n(2n+1).}
$$

For $n=1$, any two-by-two matrix satisfies $AJA^t=(\det A)J$, so the group is $SU(2)$. Explicitly,

$$
(a,b)\longmapsto\begin{pmatrix}a&b\\-\overline b&\overline a\end{pmatrix},\qquad |a|^2+|b|^2=1.
$$

The rows are orthonormal and the determinant is one; conversely unitarity and determinant one force this form. This is the [SU(2) as the three-sphere](../../../topological-group.md#su-2-as-the-three-sphere) parametrization. The map and its inverse, extraction of the first row, are smooth. Thus **$Sp(1)$ is diffeomorphic to $S^3$.**

## 3

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [fiber metric](../../../fiber-bundle.md#fiber-metric) on a real [vector bundle](../../../fiber-bundle.md#vector-bundle) $E\to M$ is a smoothly varying positive-definite [inner product](../../../linear-algebra.md#inner-product) on each fiber. Choose a trivializing open cover $\{U_i\}$ and a smooth [partition of unity](../../../differential-geometry.md#partition-of-unity) $\{\rho_i\}$ subordinate to it. The partition theorem gives nonnegative functions summing to one, a [locally finite family of subsets](../../../topology.md#locally-finite-family-of-subsets) of supports, and $\operatorname{supp}\rho_i\subset U_i$; the usual Hausdorff second-countable [smooth manifold](../../../differential-geometry.md#smooth-manifold) hypotheses ensure this theorem applies. Transfer the Euclidean [inner product](../../../linear-algebra.md#inner-product) to each local [vector bundle trivialization](../../../fiber-bundle.md#vector-bundle-trivialization), obtaining $h_i$, and set

$$
h_x(v,w)=\sum_i\rho_i(x)(h_i)_x(v,w).
$$

Each weighted term extends smoothly by zero outside $U_i$, and local finiteness makes the sum smooth in every [vector bundle trivialization](../../../fiber-bundle.md#vector-bundle-trivialization). At each $x$ some weight is positive, so $h_x(v,v)>0$ for every nonzero $v$. This proves existence of a [fiber metric](../../../fiber-bundle.md#fiber-metric), with no orientability or triviality assumption.

A [vector bundle morphism](../../../fiber-bundle.md#vector-bundle-morphism) covering the identity is a smooth map $F:E'\to E''$ that preserves base points and is a [linear map](../../../vector-space.md#linear-map) on each fiber. Its induced map on the [module of smooth sections](../../../fiber-bundle.md#module-of-smooth-sections) is $s\mapsto F\circ s$, and is $C^\infty(M)$-linear. We prove the converse by constructing [bundle morphisms from maps of smooth sections](../../../fiber-bundle.md#bundle-morphisms-from-maps-of-smooth-sections).

First the given map $\alpha$ is local. If a global section $s$ vanishes on a neighborhood of $x$, take a [smooth bump function](../../../partial-differential-equation.md#smooth-bump-function) $\chi$ supported there with $\chi=1$ near $x$. Then $\chi s=0$, so $\chi\alpha(s)=\alpha(\chi s)=0$, and hence $\alpha(s)(x)=0$. Thus sections agreeing near $x$ have images agreeing at $x$.

Choose a local frame $e_1,\ldots,e_r$ on $U$, and a bump function equal to one on a smaller neighborhood $V$ of $x$ and supported in $U$. Multiplying the frame by that bump and extending by zero gives global smooth sections $t_j$ whose restrictions to $V$ are the frame. If $s(x)=0$, write $s=\sum a_j e_j$ on $V$. A second bump extends each $a_j$ to a global smooth function $\widetilde a_j$ agreeing near $x$. By locality and $C^\infty(M)$-linearity,

$$
\alpha(s)(x)=\sum_j\widetilde a_j(x)\alpha(t_j)(x)=0.
$$

Every fiber vector $v\in E'_x$ is the value of a global smooth section, by the same bumped-frame construction. Define $F_x(v)=\alpha(s)(x)$ for any such section. The just-proved vanishing statement makes this well-defined. The maps $F_x$ are [linear maps](../../../vector-space.md#linear-map), and locally their matrix columns are the smooth sections $\alpha(t_j)$ in a frame of $E''$. Thus $F$ is smooth, is a [vector bundle morphism](../../../fiber-bundle.md#vector-bundle-morphism), and satisfies $\alpha(s)=F\circ s$. Fiberwise evaluation also proves uniqueness.

Finally apply the [fiber metric](../../../fiber-bundle.md#fiber-metric) construction to the [tangent bundle](../../../fiber-bundle.md#tangent-bundle). A [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $g$ defines the [musical isomorphism](../../../differential-geometry.md#musical-isomorphism)

$$
\boxed{\flat_g:TM\longrightarrow T^*M,\qquad v\longmapsto g(v,\cdot).}
$$

Positive definiteness makes it a fiberwise bijection; its inverse is smooth because inverse metric matrices vary smoothly. Hence **$TM$ and $T^*M$ are isomorphic as real smooth vector bundles on every such manifold.** The isomorphism depends on the chosen metric and is not canonical.

## 4

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) on a [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) is a [covariant derivative](../../../general-relativity.md#covariant-derivative) $D$ that is a [torsion-free connection](../../../fiber-bundle.md#torsion-free-connection), $D_XY-D_YX=[X,Y]$, and a [metric connection](../../../fiber-bundle.md#metric-connection), $Xg(Y,Z)=g(D_XY,Z)+g(Y,D_XZ)$. A [covariant derivative](../../../general-relativity.md#covariant-derivative) is $C^\infty(M)$-linear in $X$, real linear in $Y$, and obeys $D_X(fY)=X(f)Y+fD_XY$.

Combining metric compatibility for the cyclic triples and eliminating reversed derivatives with the torsion identity gives the [Koszul formula](../../../fiber-bundle.md#koszul-formula)

$$
2g(D_XY,Z)=Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
$$

Since $g$ is nondegenerate, this determines $D_XY$ uniquely. For existence, use the right-hand side to define $D_XY$: expansion of the [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) shows it is $C^\infty(M)$-linear in $Z$, hence defines a smooth one-form, which the [musical isomorphism](../../../differential-geometry.md#musical-isomorphism) converts to a smooth [vector field](../../../calculus.md#vector-field). The same expansion shows $D_{fX}Y=fD_XY$ and $D_X(fY)=X(f)Y+fD_XY$. Subtracting the formula with $X,Y$ exchanged gives torsion zero; adding its versions for $Y,Z$ exchanged gives metric compatibility. Thus it is a [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). Equivalently its coefficients in a [manifold chart](../../../differential-geometry.md#manifold-chart) are the [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol)

$$
\Gamma^k_{ij}=\frac12 g^{k\ell}(\partial_i g_{j\ell}+\partial_j g_{i\ell}-\partial_\ell g_{ij}).
$$

The intrinsically defined [Koszul formula](../../../fiber-bundle.md#koszul-formula) ensures these local expressions fit together. This proves the [fundamental theorem of Riemannian geometry](../../../general-relativity.md#fundamental-theorem-of-riemannian-geometry).

The [product Riemannian metric](../../../differential-geometry.md#product-riemannian-metric) on $M\times N$ is

$$
g_{(m,n)}((u,v),(u',v'))=(g_M)_m(u,u')+(g_N)_n(v,v').
$$

The two factor tangent spaces are orthogonal, and the sum is positive definite. Lift $X$ from $M$ and $Y$ from $N$. We check $D_XY$ against lifted local frame fields from both factors, which together span each product tangent space.

If $Z$ is lifted from $M$, then $g(Y,Z)=g(X,Y)=0$, while $g(Z,X)$ depends only on $m$, so $Yg(Z,X)=0$. Also $[Y,Z]=[X,Y]=0$ and $[Z,X]$ is horizontal, hence orthogonal to $Y$. Every term in the [Koszul formula](../../../fiber-bundle.md#koszul-formula) is zero. If $W$ is lifted from $N$, $g(W,X)=g(X,Y)=0$ and $g(Y,W)$ depends only on $n$, so $Xg(Y,W)=0$. Now $[W,X]=[X,Y]=0$ and $[Y,W]$ is vertical, hence orthogonal to $X$. Again every term is zero. Thus $D_XY$ is orthogonal to both spanning frame families, and positive definiteness yields

$$
\boxed{D_XY=0.}
$$

This calculation uses the lifts' independence of the other factor coordinates; a vector field with varying coefficients in those coordinates can have a nonzero mixed derivative.

## 5

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use the given orientation throughout, and the usual convention that the manifold has no boundary. In an oriented [manifold chart](../../../differential-geometry.md#manifold-chart) the [metric volume form](../../../differential-form.md#metric-volume-form) is

$$
\omega_g=\sqrt{\det(g_{ij})}\,dx^1\wedge\cdots\wedge dx^n.
$$

If $y$ is another oriented chart and $A=\partial x/\partial y$, then $g_y=A^tg_xA$, so $\sqrt{\det g_y}=(\det A)\sqrt{\det g_x}$ because $\det A>0$. This is exactly the transformation of the top [exterior product](../../../linear-algebra.md#exterior-product). The formulas therefore agree on overlaps and define a smooth positive [volume form](../../../differential-form.md#volume-form). Equivalently it takes value one on any positively oriented orthonormal tangent frame.

The metric induces an [inner product](../../../linear-algebra.md#inner-product) on $p$-forms by making the increasing exterior products of an orthonormal coframe orthonormal. The [Hodge star operator](../../../differential-form.md#hodge-star-operator) is the unique pointwise linear map $*:\Lambda^pT^*M\to\Lambda^{n-p}T^*M$ satisfying

$$
\eta\wedge *\theta=\langle\eta,\theta\rangle_g\omega_g.
$$

For an increasing multi-index $I$, $*e^I$ is the complementary wedge with the sign making $e^I\wedge *e^I=\omega_g$. Swapping the blocks of $p$ and $n-p$ factors introduces $(-1)^{p(n-p)}$. Therefore

$$
\boxed{*^2=(-1)^{p(n-p)}\operatorname{id}\quad\text{on }\Omega^p(M).}
$$

In particular $*1=\omega_g$ and $*\omega_g=1$.

For compactly supported smooth $f$, the $(n-1)$-form $f*\alpha$ has compact support. [Stokes theorem](../../../calculus.md#stokes-theorem) and the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) give

$$
0=\int_Md(f*\alpha)=\int_Mdf\wedge *\alpha+\int_Mf\,d*\alpha.
$$

A top form $\tau$ equals $(*\tau)\omega_g$. Consequently this [Hodge integration by parts for one-forms](../../../differential-form.md#hodge-integration-by-parts-for-one-forms) becomes exactly

$$
\int_M(-f*d*\alpha)\omega_g=\int_M\langle df,\alpha\rangle_g\omega_g.
$$

Compact support of $f$ is enough; $\alpha$ need not itself have compact support.

Define the [codifferential](../../../differential-form.md#codifferential) on $p$-forms by $\delta=(-1)^{n(p+1)+1}*d*$ and the [Hodge Laplacian](../../../differential-form.md#hodge-laplacian) by $\Delta=d\delta+\delta d$. A [harmonic differential form](../../../differential-form.md#harmonic-differential-form) is a smooth form in $\ker\Delta$. On functions this is the [positive Laplace-Beltrami operator](../../../differential-geometry.md#positive-laplace-beltrami-operator), $\Delta f=\delta df=-\operatorname{div}_g\operatorname{grad}_gf$. This sign convention is required by the product identity; it is the negative of the $\operatorname{div}\operatorname{grad}$ convention also commonly used for the [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator).

For a $p$-form $\beta$, the square of the [Hodge star operator](../../../differential-form.md#hodge-star-operator) and the [codifferential](../../../differential-form.md#codifferential) formula give

$$
\delta(*\beta)=(-1)^{p+1}*d\beta,\qquad d(*\beta)=(-1)^p*\delta\beta.
$$

Applying the second formula to $d\beta$ and the first to $\delta\beta$ gives

$$
\Delta(*\beta)=(-1)^{p+1}d(*d\beta)+(-1)^p\delta(*\delta\beta)=*\delta d\beta+*d\delta\beta=*\Delta\beta.
$$

Thus [Hodge star commutes with the Hodge Laplacian](../../../differential-form.md#hodge-star-commutes-with-the-hodge-laplacian). Since $*$ is invertible, **$\beta$ is harmonic if and only if $*\beta$ is harmonic.** This holds without compactness; we have not used the generally false noncompact implication that a harmonic form must be closed and coclosed.

For a smooth function $h$ and one-form $\alpha$, the same [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) gives $\delta(h\alpha)=h\delta\alpha-*\,(dh\wedge *\alpha)=h\delta\alpha-\langle dh,\alpha\rangle_g$. Apply this to $d(f_1f_2)=f_2df_1+f_1df_2$ to obtain the [product rule for the positive Laplace-Beltrami operator](../../../differential-geometry.md#product-rule-for-the-positive-laplace-beltrami-operator)

$$
\boxed{\Delta(f_1f_2)=f_2\Delta f_1+f_1\Delta f_2-2\langle df_1,df_2\rangle_g.}
$$

The [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem) states that on a compact oriented boundaryless [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold), smooth forms have the $L^2$-orthogonal decomposition

$$
\Omega^p(M)=\mathcal H^p(M)\oplus d\Omega^{p-1}(M)\oplus\delta\Omega^{p+1}(M),\qquad\mathcal H^p(M)=\ker\Delta,
$$

and each [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class has a unique [harmonic differential form](../../../differential-form.md#harmonic-differential-form) representative. To spell out the last conclusion, a harmonic form is closed and coclosed because $\langle\Delta\eta,\eta\rangle=\|d\eta\|^2+\|\delta\eta\|^2$. If a closed form decomposes as $h+du+\delta v$, then $d\delta v=0$; integration by parts gives $\|\delta v\|^2=\langle v,d\delta v\rangle=0$. Thus it represents $h$. A harmonic exact form has zero norm by adjointness, proving uniqueness. The analytic existence of the decomposition is the stated [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem).

Now let $M$ be compact, connected and oriented. A harmonic function satisfies $0=\langle f,\Delta f\rangle=\|df\|^2$, so it is constant. The [Hodge star operator](../../../differential-form.md#hodge-star-operator) identifies $\mathcal H^0(M)$ with $\mathcal H^n(M)$, hence $\mathcal H^n(M)=\mathbb R\omega_g$. A [Riemannian metric](../../../differential-geometry.md#riemannian-metric) exists by Question 3 even if none was initially chosen. Using the harmonic representative of each class, we obtain the [top de Rham cohomology of a compact connected oriented manifold](../../../differential-form.md#top-de-rham-cohomology-of-a-compact-connected-oriented-manifold)

$$
\boxed{H^n_{\mathrm{dR}}(M)\cong\mathbb R,\qquad[\omega_g]\text{ spans it}.}
$$

The class is nonzero also directly from [Stokes theorem](../../../calculus.md#stokes-theorem), since $\int_M\omega_g>0$ while every exact top form has zero integral. Boundarylessness matters: a compact interval has zero first [de Rham cohomology](../../../differential-form.md#de-rham-cohomology).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
