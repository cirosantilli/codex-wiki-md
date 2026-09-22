<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Here is an intrinsic definition that also proves well-definedness. For a [complex line bundle](../../../../../complex-line-bundle.md) $L$, define its [First Chern class](../../../../../first-chern-class.md) to be the [Euler class](../../../../../euler-class-of-a-vector-bundle.md) of its canonically oriented underlying real rank-two bundle: pull its integral [Thom class](../../../../../thom-class.md) back along the zero section after forgetting relative support. The complex orientation fixes the sign, so this construction makes no arbitrary choice of generator.

For a rank-$r>0$ [complex vector bundle](../../../../../complex-vector-bundle.md) $E$, let $\pi:\mathbb P(E)\to X$ be its [projective bundle](../../../../../projective-bundle.md) of lines, let $S\subset\pi^*E$ be the [tautological bundle](../../../../../tautological-bundle.md), and put $h=-c_1(S)=c_1(S^*)$. On every fiber $\mathbb{CP}^{r-1}$, $h$ is the positive degree-two generator. The [Leray-Hirsch theorem](../../../../../leray-hirsch-theorem.md) says that if globally defined [cohomology](../../../../../cohomology-split.md) classes restrict to a free basis of the [cohomology](../../../../../cohomology-split.md) of every fiber, then multiplication by those classes identifies the [cohomology](../../../../../cohomology-split.md) of the total space with a [free module](../../../../../free-module.md) over the base. Applied here, it gives

$$
\bigoplus_{j=0}^{r-1}H^{*-2j}(X;\mathbb Z)\xrightarrow{\ \cong\ }H^*(\mathbb P(E);\mathbb Z),\qquad(a_j)_j\longmapsto\sum_j\pi^*a_j\smile h^j.
$$

The finite trivializing cover in the question is sufficient for this application: the assertion holds on each trivializing open set by the [Künneth theorem](../../../../../kunneth-theorem.md), since the fiber has finite free [cohomology](../../../../../cohomology-split.md), and the [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) and the [Five lemma](../../../../../five-lemma.md) glue it over the finite cover. The same local argument constructs the oriented [Thom class](../../../../../thom-class.md) used for line bundles. It does not require a choice of classifying map.

There are therefore unique classes $c_i(E)\in H^{2i}(X;\mathbb Z)$ such that

$$
\boxed{h^r+\pi^*c_1(E)h^{r-1}+\cdots+\pi^*c_r(E)=0.}
$$

Define $c_0(E)=1$ and $c_i(E)=0$ for $i>r$. For rank zero the [Total Chern class](../../../../../total-chern-class.md) is $1$. This is the [projective bundle definition of Chern classes](../../../../../projective-bundle-definition-of-chern-classes.md). Existence and uniqueness follow by expressing $h^r$ in the displayed [free module](../../../../../free-module.md) basis, with degrees determining each coefficient. The [projective bundle](../../../../../projective-bundle.md) and [tautological bundle](../../../../../tautological-bundle.md) are intrinsic to $E$, and the line [Thom class](../../../../../thom-class.md) is uniquely fixed by orientation. Hence the resulting [Chern classes](../../../../../chern-class.md) do not depend on trivializations or other auxiliary choices. For a line bundle the relation is $h+c_1(E)=0$, agreeing with the original normalization. Pulling back this unique relation also proves naturality. This standard construction and the sum theorem are treated in [Vector Bundles and K-Theory, Section 3.1](https://pi.math.cornell.edu/~hatcher/VBKT/VB.pdf).

The requested result is the [Whitney sum formula for Chern classes](../../../../../whitney-sum-formula-for-chern-classes.md):

$$
\boxed{c(E\oplus E')=c(E)c(E'),\qquad c_k(E\oplus E')=\sum_{i+j=k}c_i(E)\smile c_j(E').}
$$

Here $c(E)=1+c_1(E)+\cdots+c_r(E)$, and the formula holds for complex vector bundles over a common base. In particular, a trivial bundle has total Chern class $1$.

Now take $B=\mathbb{CP}^{n-1}$ and let $L\subset B\times\mathbb C^n$ be its [tautological bundle](../../../../../tautological-bundle.md). The standard [Hermitian inner product](../../../../../hermitian-form.md) gives the rank-$(n-1)$ complex bundle $Q=L^\perp$, with $L\oplus Q\cong\underline{\mathbb C}^{\,n}$. The [orthogonal complex line flag manifold](../../../../../orthogonal-complex-line-flag-manifold.md) in the question is precisely $\mathbb P(Q)$: over a first line $\ell$, the second line is any line in $\ell^\perp$. Local orthonormal frames give this identification as a [fiber bundle](../../../../../fiber-bundle-split.md), with fiber $\mathbb{CP}^{n-2}$.

Let $x=c_1(L^*)$ on $B$, also writing $x$ for its pullback to $\mathbb P(Q)$. By part 3(a), $H^*(B;\mathbb Z)=\mathbb Z[x]/(x^n)$. The [Whitney sum formula for Chern classes](../../../../../whitney-sum-formula-for-chern-classes.md) gives

$$
(1-x)c(Q)=1,\qquad c(Q)=1+x+x^2+\cdots+x^{n-1},\qquad c_i(Q)=x^i.
$$

Let $S_2$ be the second tautological line on $\mathbb P(Q)$, and set $y=c_1(S_2^*)$. Thus $x,y$ are exactly the pullbacks of the positive hyperplane classes from the two projective factors. The [projective bundle definition of Chern classes](../../../../../projective-bundle-definition-of-chern-classes.md) for $Q$ gives

$$
y^{n-1}+xy^{n-2}+x^2y^{n-3}+\cdots+x^{n-1}=0.
$$

Together with $x^n=0$, this gives a surjective graded ring map

$$
\mathbb Z[x,y]\big/(x^n,\,x^{n-1}+x^{n-2}y+\cdots+xy^{n-2}+y^{n-1})\longrightarrow H^*(X;\mathbb Z).
$$

There are **no additional relations**. Indeed the second relation is monic of degree $n-1$ in $y$, so [polynomial division](../../../../../polynomial-division.md) makes its source free over $\mathbb Z[x]/(x^n)$ on $1,y,\ldots,y^{n-2}$. The [projective bundle formula for complex vector bundles](../../../../../projective-bundle-formula-for-complex-vector-bundles.md) gives exactly the same free basis on the target. The map sends each basis element to its corresponding basis element, and is therefore an isomorphism. Consequently

$$
\boxed{H^*(X;\mathbb Z)=\mathbb Z[x,y]/\left(x^n,\ \sum_{j=0}^{n-1}x^{n-1-j}y^j\right),\qquad |x|=|y|=2.}
$$

This is the [cohomology ring of the orthogonal complex line flag manifold](../../../../../cohomology-ring-of-the-orthogonal-complex-line-flag-manifold.md). Its additive basis is $x^iy^j$ with $0\leq i<n$, $0\leq j<n-1$. As a symmetry check, multiplying the second relation by $y-x$ gives $y^n-x^n=0$, so $y^n=0$ as expected from the second projection. For $n=2$, every line has a unique orthogonal line, and the relations become $x^2=0$, $x+y=0$, giving the ring of $\mathbb{CP}^1$. If $n=1$, the space is empty and the second relation is $1=0$, so the printed formula still gives the zero [cohomology ring](../../../../../cohomology-ring.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
