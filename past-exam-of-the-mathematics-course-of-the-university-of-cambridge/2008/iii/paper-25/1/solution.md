<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $A=E\times\{p\}$, $B=\{p\}\times E$ and $D=\Delta_E$. Their [self-intersection numbers](../../../../../self-intersection-number.md) vanish: each factor curve has trivial [normal bundle](../../../../../normal-bundle.md), and the [self-intersection of the diagonal of a curve](../../../../../self-intersection-of-the-diagonal-of-a-curve.md) is $2-2g(E)=0$. Each pair meets transversely once. Their [intersection pairing](../../../../../intersection-pairing.md) is therefore

$$
\begin{pmatrix}A^2&A\cdot B&A\cdot D\\B\cdot A&B^2&B\cdot D\\D\cdot A&D\cdot B&D^2\end{pmatrix}
=\begin{pmatrix}0&1&1\\1&0&1\\1&1&0\end{pmatrix},\qquad\det=2.
$$

If a rational [linear combination](../../../../../linear-combination.md) of their [cycle classes](../../../../../cycle-class.md) vanished in $H^2(E\times E,\mathbb Q)$, intersecting it with $A,B,D$ would multiply its coefficients by this invertible matrix and give zero. All coefficients must vanish, proving **the three classes are [linearly independent](../../../../../linear-independence.md)**.

The [cycle class map](../../../../../cycle-class-map.md) detects the [Chow Künneth failure for an elliptic self-product](../../../../../chow-kunneth-failure-for-an-elliptic-self-product.md). The codimension-one image of the [external product of Chow classes](../../../../../external-product-of-chow-classes.md) consists of sums from $\operatorname{CH}^1(E)\otimes\operatorname{CH}^0(E)$ and $\operatorname{CH}^0(E)\otimes\operatorname{CH}^1(E)$. Here $\operatorname{CH}^0(E)=\mathbb Z[E]$, and every divisor's [cohomology class](../../../../../cohomology-class.md) is its [degree of a divisor](../../../../../degree-of-a-divisor.md) times the class of a point. Thus the image's cohomology is contained in the span of $[A],[B]$. The diagonal's independent class lies outside that span, so its [Chow class](../../../../../chow-class.md) lies outside the external-product image. Therefore **the natural map of Chow groups is not surjective**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
