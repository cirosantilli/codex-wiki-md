<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [First Chern class](../../../../../first-chern-class.md) identity, use finite-dimensional classifying maps. A [complex line bundle](../../../../../complex-line-bundle.md) on a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) embeds in a finite-dimensional [trivial vector bundle](../../../../../trivial-vector-bundle.md), so it is a [pullback vector bundle](../../../../../pullback-vector-bundle.md) of the [tautological bundle](../../../../../tautological-bundle.md) on some [Complex projective space](../../../../../complex-projective-space.md). For the two [complex line bundles](../../../../../complex-line-bundle.md), the universal [tensor product of vector bundles](../../../../../tensor-product-of-vector-bundles.md) is classified by the map

$$
m:\mathbb{CP}^N\times\mathbb{CP}^M\longrightarrow\mathbb{CP}^{(N+1)(M+1)-1},\qquad ([v],[w])\longmapsto[v\otimes w].
$$

Its restriction to either factor pulls the [tautological bundle](../../../../../tautological-bundle.md) back to the [tautological bundle](../../../../../tautological-bundle.md) on that factor. The degree-two [cohomology](../../../../../cohomology-split.md) of the product is the [direct sum](../../../../../direct-sum.md) of the degree-two [cohomology](../../../../../cohomology-split.md) of its factors, so these two restrictions determine its [First Chern class](../../../../../first-chern-class.md). Pulling back to $X$ proves

$$
\boxed{c_1(L_1\otimes L_2)=c_1(L_1)+c_1(L_2).}
$$

This proves the integral identity, including possible [torsion elements](../../../../../torsion-element.md) in the [cohomology](../../../../../cohomology-split.md) of $X$; an argument using only curvature forms would not detect those [torsion elements](../../../../../torsion-element.md).

The [splitting principle for complex vector bundles](../../../../../splitting-principle-for-complex-vector-bundles.md) says that for a [vector bundle](../../../../../vector-bundle.md) $E\to X$ there is an iterated [projective bundle](../../../../../projective-bundle.md) $p:F(E)\to X$ for which $p^*$ is injective on integral [cohomology](../../../../../cohomology-split.md), and $p^*E$ is a [direct sum](../../../../../direct-sum.md) of [complex line bundles](../../../../../complex-line-bundle.md). The same assertion holds with rational coefficients, and a common such space can split any finite collection of [vector bundles](../../../../../vector-bundle.md). The injectivity follows at each stage from the [projective bundle formula for complex vector bundles](../../../../../projective-bundle-formula-for-complex-vector-bundles.md); a [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) splits the resulting filtration into a [direct sum](../../../../../direct-sum.md).

Write $x_i=c_1(L_i)$ for the [Chern roots](../../../../../chern-root.md) of the pulled-back [vector bundle](../../../../../vector-bundle.md). Define the degree-$2j$ component of its [Chern character](../../../../../chern-character.md) by

$$
\operatorname{ch}_0(E)=\operatorname{rank}E,\qquad
\operatorname{ch}_j(E)=\frac{1}{j!}\sum_i x_i^j,\qquad
\operatorname{ch}(E)=\sum_{j\geq0}\operatorname{ch}_j(E).
$$

The [Fundamental theorem of symmetric polynomials](../../../../../fundamental-theorem-of-symmetric-polynomials.md) expresses each [power-sum symmetric polynomial](../../../../../power-sum-symmetric-polynomial.md) $\sum_i x_i^j$ uniquely as an integral polynomial in the [elementary symmetric polynomials](../../../../../elementary-symmetric-polynomial.md), which are the [Chern classes](../../../../../chern-class.md) of $E$. Thus the definition makes sense on $X$ itself, without choosing actual [Chern roots](../../../../../chern-root.md) there. On a [compact Hausdorff space](../../../../../compact-hausdorff-space.md), each [vector bundle](../../../../../vector-bundle.md) is classified by a finite-dimensional [Grassmannian](../../../../../grassmannian.md); its high-degree [Chern character](../../../../../chern-character.md) components therefore vanish. Hence this defines a class in the direct sum $H^{2*}(X;\mathbb Q)$ even if $X$ has no finite dimension. On more general spaces an infinite [Chern character](../../../../../chern-character.md) is instead interpreted in the product of the even-degree [cohomology](../../../../../cohomology-split.md) groups.

On a common splitting space, the [Chern roots](../../../../../chern-root.md) of a [direct sum](../../../../../direct-sum.md) are the combined root lists, whereas the [First Chern class](../../../../../first-chern-class.md) identity makes the [Chern roots](../../../../../chern-root.md) of a [tensor product of vector bundles](../../../../../tensor-product-of-vector-bundles.md) the pairwise sums $x_i+y_j$. Consequently

$$
\begin{aligned}
\operatorname{ch}(E\oplus F)&=\sum_i e^{x_i}+\sum_j e^{y_j},\\
\operatorname{ch}(E\otimes F)&=\sum_{i,j}e^{x_i+y_j}
=\left(\sum_i e^{x_i}\right)\left(\sum_j e^{y_j}\right).
\end{aligned}
$$

The injectivity in the [splitting principle for complex vector bundles](../../../../../splitting-principle-for-complex-vector-bundles.md) descends both identities to $X$. Additivity extends the [Chern character](../../../../../chern-character.md) to the [Grothendieck group](../../../../../grothendieck-group.md) by $\operatorname{ch}([E]-[F])=\operatorname{ch}(E)-\operatorname{ch}(F)$. Multiplicativity and $\operatorname{ch}(1)=1$ then show that **the [Chern character](../../../../../chern-character.md) is a unital [ring homomorphism](../../../../../ring-homomorphism.md)**.

For [Complex K-theory of complex projective space](../../../../../complex-k-theory-of-complex-projective-space.md), let $\gamma$ be the [tautological bundle](../../../../../tautological-bundle.md), put $t=1-[\gamma]$, and set $h=-c_1(\gamma)$. The [cohomology ring of complex projective space](../../../../../cohomology-ring-of-complex-projective-space.md) is $\mathbb Z[h]/(h^{n+1})$. The [CW filtration](../../../../../cw-filtration.md) gives a [cofibration](../../../../../cofibration.md)

$$
\mathbb{CP}^{n-1}\longrightarrow\mathbb{CP}^n\longrightarrow S^{2n}.
$$

The [K-theory six-term exact sequence](../../../../../k-theory-six-term-exact-sequence.md) and [Complex K-theory of a sphere](../../../../../complex-k-theory-of-a-sphere.md) give, inductively,

$$
K^{-1}(\mathbb{CP}^n)=0,\qquad
0\longrightarrow\mathbb Z\{b_n\}\longrightarrow K^0(\mathbb{CP}^n)
\longrightarrow K^0(\mathbb{CP}^{n-1})\longrightarrow0.
$$

Here $b_n$ is the image of a [Bott element](../../../../../bott-element.md) from $S^{2n}$, normalized so that $\operatorname{ch}(b_n)=h^n$. This normalization follows from the multiplicative form of [Bott periodicity](../../../../../bott-isomorphism.md): the [Chern character](../../../../../chern-character.md) of the degree-two [Bott element](../../../../../bott-element.md) is an integral generator, and multiplication yields the top-degree generator on $S^{2n}$. In particular, the [abelian group](../../../../../abelian-group.md) $K^0(\mathbb{CP}^n)$ is a [free abelian group](../../../../../free-abelian-group.md) of rank $n+1$.

Assume inductively that $1,t,\ldots,t^{n-1}$ form an integral basis on $\mathbb{CP}^{n-1}$. Their lifts, together with $b_n$, form an integral basis on $\mathbb{CP}^n$. Since

$$
\operatorname{ch}(t)=1-e^{-h}=h-\frac{h^2}{2!}+\frac{h^3}{3!}-\cdots,
$$

the [Chern characters](../../../../../chern-character.md) of this basis are [linearly independent](../../../../../linear-independence.md) over $\mathbb Q$: their first nonzero degrees are $0,2,\ldots,2n$. Thus the [Chern character](../../../../../chern-character.md) is injective on $K^0(\mathbb{CP}^n)$. By induction $t^n$ restricts to zero on $\mathbb{CP}^{n-1}$, so $t^n=a b_n$ for an integer $a$. Comparing [Chern characters](../../../../../chern-character.md) gives $a=1$. Also $\operatorname{ch}(t^{n+1})=0$, so $t^{n+1}=0$. This proves the integral answer, rather than merely its rationalization:

$$
\boxed{K^0(\mathbb{CP}^n)\cong\mathbb Z[t]/(t^{n+1}),\qquad t=1-[\gamma].}
$$

The induction begins with $\mathbb{CP}^0$ a point and $t=0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 142](../../paper-142-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
