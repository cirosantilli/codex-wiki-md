<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $E$ have rank $r\geq1$, let $p:\mathbb P(E)\to X$ be its [projectivization of a real vector bundle](../../../../../projectivization-of-a-real-vector-bundle.md), and let $\lambda\subset p^*E$ be its [tautological bundle](../../../../../tautological-bundle.md). Put $u=w_1(\lambda)\in H^1(\mathbb P(E);\mathbb F_2)$. The [Projective bundle definition of Stiefel–Whitney classes](../../../../../projective-bundle-definition-of-stiefel-whitney-classes.md) starts from the isomorphism

$$
\bigoplus_{j=0}^{r-1}H^{*-j}(X;\mathbb F_2)
\xrightarrow{\ \cong\ }H^*(\mathbb P(E);\mathbb F_2),\qquad
(a_0,\ldots,a_{r-1})\longmapsto\sum_{j=0}^{r-1}p^*a_j\smile u^j.
$$

In particular, $p^*$ is injective. Expand $u^r$ uniquely in this basis. The coefficients define the [Stiefel–Whitney classes](../../../../../stiefel-whitney-class.md) through the relation

$$
\boxed{u^r+p^*w_1(E)u^{r-1}+\cdots+p^*w_r(E)=0.}
$$

Set $w_0(E)=1$ and $w_i(E)=0$ for $i>r$; for a rank-zero [vector bundle](../../../../../vector-bundle.md) set $w(E)=1$. Uniqueness also proves naturality of the [Stiefel–Whitney classes](../../../../../stiefel-whitney-class.md) under a [pullback vector bundle](../../../../../pullback-vector-bundle.md).

To prove the [Whitney product formula for Stiefel–Whitney classes](../../../../../whitney-product-formula-for-stiefel-whitney-classes.md), apply the [splitting principle for real vector bundles](../../../../../splitting-principle-for-real-vector-bundles.md) simultaneously to $E$ and $E'$. Its injective pullback on mod-two [cohomology](../../../../../cohomology-split.md) follows by iterating the [Projective bundle definition of Stiefel–Whitney classes](../../../../../projective-bundle-definition-of-stiefel-whitney-classes.md). It suffices to compute for a split [vector bundle](../../../../../vector-bundle.md) $E=\bigoplus_{i=1}^r L_i$. Put $x_i=w_1(L_i)$.

On $\mathbb P(E)$, the coordinate projections of the tautological inclusion $\lambda\hookrightarrow p^*E$ give sections of the [real line bundles](../../../../../real-line-bundle.md) $\lambda^*\otimes p^*L_i$ with no common zero. The [mod-two Euler class of a real line bundle](../../../../../mod-two-euler-class-of-a-real-line-bundle.md) is its first [Stiefel–Whitney class](../../../../../stiefel-whitney-class.md), and the [First Stiefel–Whitney class of a tensor product of real line bundles](../../../../../first-stiefel-whitney-class-of-a-tensor-product-of-real-line-bundles.md) gives $u+p^*x_i$. Multiplication of [Euler classes](../../../../../euler-class-of-a-vector-bundle.md) under a [direct sum](../../../../../direct-sum.md), and vanishing of the [Euler class of a vector bundle](../../../../../euler-class-of-a-vector-bundle.md) with a nowhere-zero section, therefore give

$$
\prod_{i=1}^r(u+p^*x_i)=0.
$$

Comparing with the unique monic relation defining the [Stiefel–Whitney classes](../../../../../stiefel-whitney-class.md) shows that $w_j(E)$ is the $j$th [elementary symmetric polynomial](../../../../../elementary-symmetric-polynomial.md) in the $x_i$. Thus $w(E)=\prod_i(1+x_i)$. A [direct sum](../../../../../direct-sum.md) joins the two lists, so injectivity of the splitting pullback gives

$$
\boxed{w(E\oplus E')=w(E)w(E'),\qquad
w_k(E\oplus E')=\sum_{i+j=k}w_i(E)\smile w_j(E').}
$$

For the [immersion](../../../../../immersion.md) obstruction, use the notation $g=(f,f)$: the printed $f\times f$ here means the map from one copy of [Real projective space](../../../../../real-projective-space.md) into the product. Write $x=w_1(\gamma_{\mathbb R})$ and let $z$ be the mod-two reduction of $c_1(\gamma_{\mathbb C}^*)$. The [mod-two cohomology ring of real projective space](../../../../../mod-two-cohomology-ring-of-real-projective-space.md) and the [cohomology ring of complex projective space](../../../../../cohomology-ring-of-complex-projective-space.md) give

$$
H^*(\mathbb{RP}^{2k+1};\mathbb F_2)=\mathbb F_2[x]/(x^{2k+2}),\qquad
H^*(\mathbb{CP}^k;\mathbb F_2)=\mathbb F_2[z]/(z^{k+1}),\qquad
|x|=1,\quad |z|=2.
$$

Nontriviality in degree two forces $f^*z=x^2$. Necessarily $k\geq1$, since the degree-two [cohomology](../../../../../cohomology-split.md) of $\mathbb{CP}^0$ vanishes.

The standard [tangent bundle](../../../../../tangent-bundle.md) identities for [Real projective space](../../../../../real-projective-space.md) and [Complex projective space](../../../../../complex-projective-space.md) are

$$
T\mathbb{RP}^{2k+1}\oplus\mathbb R\cong(2k+2)\gamma_{\mathbb R},\qquad
T\mathbb{CP}^k\oplus\mathbb C\cong(k+1)\gamma_{\mathbb C}^*.
$$

For the underlying real [vector bundle](../../../../../vector-bundle.md) of a [complex line bundle](../../../../../complex-line-bundle.md), its total [Stiefel–Whitney class](../../../../../stiefel-whitney-class.md) is $1+c_1\bmod2$. Hence

$$
w(T\mathbb{RP}^{2k+1})=(1+x)^{2k+2},\qquad
w(T\mathbb{CP}^k)=(1+z)^{k+1}.
$$

If $g$ is [homotopic](../../../../../homotopy.md) to an [immersion](../../../../../immersion.md) $j$, its [normal bundle](../../../../../normal-bundle.md) $\nu$ has rank $4k-(2k+1)=2k-1$, and

$$
T\mathbb{RP}^{2k+1}\oplus\nu\cong j^*T(\mathbb{CP}^k\times\mathbb{CP}^k).
$$

The [Whitney product formula for Stiefel–Whitney classes](../../../../../whitney-product-formula-for-stiefel-whitney-classes.md) and [homotopy invariance of cohomology](../../../../../homotopy-invariance-of-cohomology.md) yield

$$
w(\nu)=\frac{(1+x^2)^{2k+2}}{(1+x)^{2k+2}}
=(1+x)^{2k+2}.
$$

The division is legitimate in the truncated [cohomology ring](../../../../../cohomology-ring.md), since $1+x$ is a unit. The degree-$2k$ component is

$$
w_{2k}(\nu)=\binom{2k+2}{2k}x^{2k}
=(k+1)(2k+1)x^{2k}=(k+1)x^{2k}.
$$

It must vanish because $2k>\operatorname{rank}\nu$, while $x^{2k}\ne0$. Therefore **$k$ must be odd**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 142](../../paper-142-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
