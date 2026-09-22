<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $m=\dim M$ and $q=m-\dim Y$. Here a closed submanifold means compact and without boundary, which is the condition needed for a compactly supported dual class. The orientations of $M$ and $Y$ orient the [normal bundle](../../../../../normal-bundle.md) $\nu_Y$. Its [Thom class](../../../../../thom-class.md) is the unique relative class of degree $q$ restricting to the chosen orientation generator on every normal fiber. A [tubular neighborhood](../../../../../tubular-neighborhood.md) identifies this class with one near $Y$ in $M$. Choose a compact normal disc neighborhood and extend the relative class to [compactly supported cohomology](../../../../../compactly-supported-cohomology.md) of $M$. Equivalently, apply [Poincare duality](../../../../../poincare-duality.md) $H_c^q(M;\mathbb Q)\cong H_{m-q}(M;\mathbb Q)$ to the pushed-forward [fundamental class](../../../../../fundamental-class.md) of $Y$:

$$
\boxed{\varepsilon_Y=\operatorname{PD}_M(i_*[Y])\in H_c^q(M;\mathbb Q).}
$$

This [compactly supported dual of a compact submanifold](../../../../../compactly-supported-dual-of-a-compact-submanifold.md) is independent of the tubular neighborhood and represents intersection with $Y$. Fix the convention $\langle\varepsilon_Y\smile a,[M]\rangle=\langle i^*a,[Y]\rangle$ in complementary degree. Its image in ordinary [cohomology](../../../../../cohomology-split.md) restricts to zero on $M\setminus Y$, because it comes from relative [cohomology](../../../../../cohomology-split.md) supported near $Y$. If a submanifold is only closed as a subset but is noncompact, its usual dual lies in ordinary [cohomology](../../../../../cohomology-split.md) instead; compact support is not asserted in that situation.

Now let $\Delta\subset N\times N$ be the diagonal, with the orientation inherited from $N$, and let $\delta=\varepsilon_\Delta\in H^n(N\times N;\mathbb Q)$. For each $i$, choose a basis $a_{i,j}$ of $H^i(N;\mathbb Q)$ and its dual basis $b_{i,j}$ of $H^{n-i}(N;\mathbb Q)$ satisfying $\langle a_{i,j}\smile b_{i,k},[N]\rangle=\delta_{jk}$. The [Poincare duality pairing](../../../../../poincare-duality-pairing.md) and the [Künneth theorem](../../../../../kunneth-theorem.md) give the [cohomology class of the diagonal](../../../../../cohomology-class-of-the-diagonal.md)

$$
\delta=\sum_{i,j}(-1)^{i(n-i+1)}p_1^*b_{i,j}\smile p_2^*a_{i,j}.
$$

The sign can be checked from the defining identity

$$
\left\langle\delta\smile(p_1^*u\smile p_2^*v),[N\times N]\right\rangle=\langle u\smile v,[N]\rangle.
$$

For $|u|=i$, moving the degree-$i$ class in the second factor past $u$ contributes $(-1)^i$, and interchanging $b_{i,j}$ and $u$ contributes $(-1)^{i(n-i)}$; the displayed coefficient cancels their product. Equivalently its exponent is $ni$ modulo two.

The [cohomological pushforward between closed oriented manifolds](../../../../../cohomological-pushforward-between-closed-oriented-manifolds.md) is characterized by

$$
\langle f^!c\smile b,[N]\rangle=\langle c\smile f^*b,[M]\rangle,
$$

for complementary degrees. This follows immediately from its definition by [Poincare duality](../../../../../poincare-duality.md) and naturality of evaluation on pushed-forward homology. In degree $i$, the [matrix trace](../../../../../matrix-trace.md) of $f^!g^*$ on $H^i(N;\mathbb Q)$ is consequently

$$
\operatorname{tr}(f^!g^*)=\sum_j\langle g^*a_{i,j}\smile f^*b_{i,j},[M]\rangle.
$$

For finite-dimensional maps between two possibly different vector spaces, $\operatorname{tr}(AB)=\operatorname{tr}(BA)$. Thus this [matrix trace](../../../../../matrix-trace.md) equals that of $g^*f^!$ on $H^i(M;\mathbb Q)$. Pulling back the diagonal formula by $F=(f,g)$ and applying [graded commutativity of the cup product](../../../../../graded-commutativity-of-the-cup-product.md) now yields

$$
\boxed{\left\langle(f,g)^*\delta,[M]\right\rangle=\sum_i(-1)^i\operatorname{tr}(g^*f^!)=L(f,g).}
$$

This establishes the [Lefschetz coincidence number](../../../../../lefschetz-coincidence-number.md) with the requested sign convention.

If $f(m)\ne g(m)$ for every $m$, the map $(f,g)$ factors through $(N\times N)\setminus\Delta$. The diagonal class restricts to zero there, so its pullback is zero and $L(f,g)=0$. Taking the contrapositive proves the [Lefschetz coincidence theorem](../../../../../lefschetz-coincidence-theorem.md):

$$
\boxed{L(f,g)\ne0\quad\Longrightarrow\quad f(m)=g(m)\text{ for some }m\in M.}
$$

No transversality or isolated-coincidence assumption is needed. This cohomological argument also applies to continuous maps, which covers the last request.

For a map $f:M\to N$ of degree $d$, the adjoint identity above gives, for all complementary classes $a,b$ on $N$,

$$
\langle f^!f^*a\smile b,[N]\rangle=\langle f^*(a\smile b),[M]\rangle=d\langle a\smile b,[N]\rangle.
$$

Nondegeneracy therefore gives $f^!f^*=d\,\mathrm{id}$. Cyclic invariance of [matrix trace](../../../../../matrix-trace.md) proves the [self-coincidence number of a map of nonzero degree](../../../../../self-coincidence-number-of-a-map-of-nonzero-degree.md) formula

$$
L(f,f)=d\,\chi(N).
$$

In particular, $\mathbb{CP}^{2k}$ has one even-dimensional [cohomology](../../../../../cohomology-split.md) generator in each degree $0,2,\ldots,4k$, so $\chi(\mathbb{CP}^{2k})=2k+1$. Hence

$$
\boxed{L(f,f)=(2k+1)d\ne0.}
$$

If $g$ is homotopic to $f$, [homotopy invariance of cohomology](../../../../../homotopy-invariance-of-cohomology.md) gives $g^*=f^*$ and thus $L(f,g)=L(f,f)$. The [Lefschetz coincidence theorem](../../../../../lefschetz-coincidence-theorem.md) supplies a point at which $f$ and $g$ agree.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
