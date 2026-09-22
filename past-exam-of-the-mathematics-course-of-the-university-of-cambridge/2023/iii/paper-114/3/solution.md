<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a singular $(k+l)$-simplex $\sigma:[v_0,\ldots,v_{k+l}]\to X$, define the cochain-level [cup product](../../../../../cup-product.md) by

$$
(\alpha\smile\beta)(\sigma)
=\alpha(\sigma|[v_0,\ldots,v_k])\,
\beta(\sigma|[v_k,\ldots,v_{k+l}]).
$$

If $\alpha\in C^k(X,A;R)$ and $\sigma$ lies in $A$, its front $k$-face also lies in $A$, so the first factor vanishes. Thus $\alpha\smile\beta\in C^{k+l}(X,A;R)$.

For the projections from $X\times Y$, the [exterior product in cohomology](../../../../../exterior-product-in-cohomology.md) is

$$
a\times b=p_X^*a\smile p_Y^*b.
$$

For CW pairs over a field $R$, subject to the usual finite-type condition that makes the graded tensor product commute with the relevant direct products, the [Künneth theorem](../../../../../kunneth-theorem.md) says that

$$
\Phi:H^*(X,A;R)\otimes_RH^*(Y;R)
\xrightarrow{\sim}H^*(X\times Y,A\times Y;R).
$$

More generally the conclusion holds over a principal ideal domain when one factor has degreewise finitely generated free cohomology. It fails over $\mathbb Z$ in general: $H^*(\mathbb{RP}^2;\mathbb Z)$ is $\mathbb Z$ in degree zero and $\mathbb Z/2$ in degree two, but the integral Künneth and [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) calculations give

$$
H^3(\mathbb{RP}^2\times\mathbb{RP}^2;\mathbb Z)\cong\mathbb Z/2.
$$

The tensor product of the two cohomology groups has no degree-three term, so $\Phi$ is not surjective.

Use the homeomorphism

$$
T^2\times T^2\longrightarrow T^2\times T^2,
\qquad(x,y)\longmapsto(x,y-x),
$$

which carries the diagonal $\Delta$ to $T^2\times\{0\}$. Hence

$$
T^4\setminus\Delta\cong T^2\times(T^2\setminus\{0\}).
$$

The punctured torus deformation retracts onto a wedge of two circles. Let $a,b$ be the degree-one generators from the first torus and $c,d$ those from the punctured torus. Since all cohomology groups are free, the Künneth theorem identifies the integral cohomology ring as

$$
H^*(T^4\setminus\Delta;\mathbb Z)
\cong\Lambda_{\mathbb Z}(a,b)\otimes
\frac{\Lambda_{\mathbb Z}(c,d)}{(cd)},
\qquad |a|=|b|=|c|=|d|=1.
$$

**Thus $ab$, $ac$, $ad$, $bc$, and $bd$ form a basis in degree two; $abc$ and $abd$ form a basis in degree three; and all higher positive degrees vanish.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
