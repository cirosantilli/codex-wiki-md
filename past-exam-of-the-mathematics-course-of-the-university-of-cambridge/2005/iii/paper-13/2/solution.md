<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For integral [singular cochains](../../../../../singular-cochain.md) $a\in C^p(X)$ and $b\in C^q(X)$, define the [cup product](../../../../../cup-product.md) on an ordered simplex by

$$
(a\smile b)(\sigma)=a(\sigma[0,\ldots,p])\,b(\sigma[p,\ldots,p+q]).
$$

The same construction works over any commutative coefficient ring. Expanding the [coboundary](../../../../../coboundary.md) as the alternating sum of faces gives the Leibniz identity

$$
\delta(a\smile b)=\delta a\smile b+(-1)^p a\smile\delta b.
$$

Indeed faces deleting vertices before the split occur in the first sum, faces after the split occur in the second, and the two terms at the common vertex cancel with opposite signs. Thus the product of [cocycles](../../../../../cocycle.md) is a [cocycle](../../../../../cocycle.md). Replacing $a$ by $a+\delta c$ changes the product with a [cocycle](../../../../../cocycle.md) $b$ by $\delta(c\smile b)$; replacing $b$ by $b+\delta d$ changes the product with a [cocycle](../../../../../cocycle.md) $a$ by $(-1)^p\delta(a\smile d)$. Hence the product is independent of representatives and defines a **well-defined product on [cohomology classes](../../../../../cohomology-class.md)**.

With $\mathbb F_2=\mathbb Z_2$ coefficients, the real-projective-space [cohomology ring](../../../../../cohomology-ring.md) is

$$
H^*(\mathbb{RP}^r;\mathbb F_2)=\mathbb F_2[t]/(t^{r+1}),\qquad |t|=1.
$$

For $n>m\geq1$, the pullback of the degree-one generator is either zero or $t$. The second choice would send the zero class $t^{m+1}$ to the nonzero class $t^{m+1}\in H^{m+1}(\mathbb{RP}^n;\mathbb F_2)$, contradicting the naturality of the [cup product](../../../../../cup-product.md). Thus the generator pulls back to zero, and so do all its positive powers. For $m=0$ the target's reduced [cohomology](../../../../../cohomology-split.md) is already zero. Therefore **every such map induces zero on reduced mod-two [cohomology](../../../../../cohomology-split.md)**.

Suppose a continuous $f:S^n\to\mathbb R^n$ had $f(x)\ne f(-x)$ everywhere. Then

$$
h(x)=\frac{f(x)-f(-x)}{|f(x)-f(-x)|}
$$

is a continuous odd map to $S^{n-1}$ and descends to $\bar h:\mathbb{RP}^n\to\mathbb{RP}^{n-1}$. For $n\geq2$, a path from $x$ to $-x$ projects to a loop detected by the degree-one generator of the double cover. Its image lifts to a path from $h(x)$ to $-h(x)$, so is detected by the target's double cover as well. Thus $\bar h^*$ is nonzero in degree one, contradicting the preceding calculation. For $n=1$, an odd continuous map from the connected circle to $S^0$ is already impossible. The case $n=0$ is immediate. Hence

$$
\boxed{\text{There exists }x\in S^n\text{ with }f(x)=f(-x).}
$$

This proves the [Borsuk-Ulam theorem](../../../../../borsuk-ulam-theorem.md) rather than assuming it.

For a closed cover $A_1,\ldots,A_{n+1}$, assume no member contains an [antipodal pair](../../../../../antipodal-pair.md). Apply the just-proved theorem to $F(x)=(d(x,A_1),\ldots,d(x,A_n))$, using any metric on the sphere. Empty sets can be assigned a constant positive coordinate. It gives equal distances at $x,-x$. If either point belongs to an $A_i$ with $i\leq n$, zero distance and closedness place both points in it, a contradiction. Hence neither lies in any of the first $n$ sets, and both must lie in $A_{n+1}$, another contradiction. This proves the [Lusternik-Schnirelmann-Borsuk theorem](../../../../../lusternik-schnirelmann-theorem.md) for [closed sets](../../../../../closed-set.md).

**Four [closed sets](../../../../../closed-set.md) on $S^2$ need not contain an [antipodal pair](../../../../../antipodal-pair.md).** Take the four unit vertices $v_i$ of a regular tetrahedron centered at zero and define $C_i=\{x:x\cdot v_i\geq x\cdot v_j\text{ for every }j\}$. These [closed sets](../../../../../closed-set.md) cover the sphere by maximizing the four scalar products. If $x$ and $-x$ belonged to $C_i$, both inequalities would force all four scalar products to be equal. Since $\sum v_i=0$, they would all be zero, and because the vertices span $\mathbb R^3$, $x$ would be zero. This is impossible on the sphere. Thus these four sets give the [antipodal-free closed cover from simplex Voronoi cells](../../../../../antipodal-free-closed-cover-from-simplex-voronoi-cells.md) counterexample.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
