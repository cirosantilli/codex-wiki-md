<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For finite-dimensional [Complex projective space](../../../../../complex-projective-space.md) $\mathbb{CP}^r$, use the filtration by its linear projective subspaces. The difference $\mathbb{CP}^j\setminus\mathbb{CP}^{j-1}$ is $\mathbb C^j$, so there is one [topological cell](../../../../../topological-cell.md) in every even dimension $0,2,\ldots,2r$, and none in odd dimensions. Every cellular boundary vanishes for degree reasons. The integral [cohomology](../../../../../cohomology-split.md) is therefore $\mathbb Z$ in those even degrees and zero elsewhere.

For the [cohomology ring](../../../../../cohomology-ring.md), let $x\in H^2(\mathbb{CP}^r;\mathbb Z)$ be the [Poincare dual](../../../../../poincare-dual.md) of a [projective hyperplane](../../../../../projective-hyperplane.md), using the complex [orientation](../../../../../orientation-of-a-simplex.md). Generic hyperplanes meet transversely, and a collection of $j$ of them intersects in $\mathbb{CP}^{r-j}$. The geometric interpretation of the [cup product](../../../../../cup-product.md) identifies $x^j$ with the dual of that intersection. Restricting to a linear $\mathbb{CP}^j$, the $j$ hyperplanes meet in one point, with positive sign because the transverse normal directions are complex lines. Hence

$$
\left\langle x^j,[\mathbb{CP}^j]\right\rangle=1.
$$

Thus $x^j$ is a primitive generator in degree $2j$, not merely a nonzero multiple. There are no classes beyond degree $2r$, so

$$
\boxed{H^*(\mathbb{CP}^r;\mathbb Z)\cong\mathbb Z[x]/(x^{r+1}),\qquad |x|=2.}
$$

The point case $r=0$ has ring $\mathbb Z$. Taking the union of the finite projective spaces gives $H^*(\mathbb{CP}^{\infty};\mathbb Z)=\mathbb Z[x]$, since each fixed cohomological degree stabilizes. This proves the [cohomology ring of complex projective space](../../../../../cohomology-ring-of-complex-projective-space.md) computation.

For the [rank bound for a nonsingular complex bilinear map](../../../../../rank-bound-for-a-nonsingular-complex-bilinear-map.md), write $a=\dim_{\mathbb C}U$, $b=\dim_{\mathbb C}V$, $R=\operatorname{im}\phi$, and $s=\dim_{\mathbb C}R$. Assume $a,b\geq1$. Injectivity with either nonzero factor fixed implies $\phi(u\otimes v)\ne0$ whenever $u,v\ne0$. Therefore

$$
F:\mathbb{CP}^{a-1}\times\mathbb{CP}^{b-1}\longrightarrow\mathbb{CP}^{s-1},\qquad ([u],[v])\longmapsto[\phi(u\otimes v)]
$$

is well defined and continuous. Scaling either vector only scales the output, and in local projective charts the formula is given by bilinear coordinates with no simultaneous zero. Let $h$ be the target's degree-two generator and $x,y$ the pullbacks of the two factor generators. The [Künneth theorem](../../../../../kunneth-theorem.md) gives

$$
H^*(\mathbb{CP}^{a-1}\times\mathbb{CP}^{b-1};\mathbb Z)=\mathbb Z[x,y]/(x^a,y^b).
$$

Fixing $[v]$ or $[u]$ makes $F$ a projective linear embedding induced by an injective [linear map](../../../../../linear-map.md). Such an embedding pulls back the hyperplane class to the factor's hyperplane class. Since the two restrictions determine $H^2$ of the product, $F^*h=x+y$, with the generator of a point factor interpreted as zero.

Put $d=a+b-2$. In the source [cohomology ring](../../../../../cohomology-ring.md), every term in $(x+y)^d$ vanishes except the one with exponents $a-1,b-1$, and

$$
F^*(h^d)=(x+y)^d=\binom{a+b-2}{a-1}x^{a-1}y^{b-1}\ne0.
$$

The binomial coefficient is a positive integer and the final monomial generates the top integral [cohomology](../../../../../cohomology-split.md). If $s\leq d$, the class $h^d$ in $\mathbb{CP}^{s-1}$ would be zero. This contradiction proves

$$
\boxed{\operatorname{rank}\phi\geq\dim_{\mathbb C}U+\dim_{\mathbb C}V-1.}
$$

When $a=b=1$, the nonzero pure-tensor image already gives $s\geq1$. A positivity convention is genuinely necessary: if $U=0$, $V=\mathbb C^2$, and $W=0$, all restrictions to the zero tensor subspaces are injective, but the literal bound would read $0\geq1$. The displayed theorem is therefore the nonzero-factor version. If a nonzero factor is infinite-dimensional, either factor restriction already bounds the image dimension below by that factor dimension; the sum of two positive cardinal dimensions, with at least one infinite, is their maximum, giving the corresponding cardinal bound.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
