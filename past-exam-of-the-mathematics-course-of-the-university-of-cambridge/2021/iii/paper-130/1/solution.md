<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Fix a number $k$ of colors. For a two-point set whose points are distance $d$ apart, take the vertices of a [regular simplex](../../../../../regular-simplex.md) with $k+1$ vertices and side length $d$. The [pigeonhole principle](../../../../../pigeonhole-principle.md) gives two vertices of one color, and they form the required congruent copy. Thus every two-point set, equivalently every [line segment](../../../../../line-segment.md), is a [Euclidean Ramsey set](../../../../../euclidean-ramsey-set.md).

For an [equilateral triangle](../../../../../equilateral-triangle.md) of side length $d$, take a [regular simplex](../../../../../regular-simplex.md) with $2k+1$ vertices and side length $d$. The [pigeonhole principle](../../../../../pigeonhole-principle.md) gives three vertices of one color, and every three vertices of a regular simplex form an equilateral triangle. Hence every equilateral triangle is Euclidean Ramsey.

To prove the [product theorem for Euclidean Ramsey sets](../../../../../product-theorem-for-euclidean-ramsey-sets.md), let $S_X$ be a finite Ramsey witness for $X$ under $k$ colors. There are at most $k^{|S_X|}$ possible color patterns on $S_X$. Choose a finite Ramsey witness $S_Y$ for $Y$ under that many colors. Given a $k$-coloring of $S_X\times S_Y$, color each $y\in S_Y$ by the complete pattern

$$
x\longmapsto c(x,y),\qquad x\in S_X.
$$

There is a copy $Y'\cong Y$ on which this pattern is constant. The common pattern on $S_X$ contains a monochromatic copy $X'\cong X$. Every point of $X'\times Y'$ then has the same original color, and the orthogonal product is congruent to $X\times Y$.

A rectangle is the [Cartesian product](../../../../../cartesian-product.md) of two line segments, so it is Euclidean Ramsey. Three suitable vertices of a rectangle form a [right triangle](../../../../../right-triangle.md); any subset of a monochromatic set is monochromatic. Thus every right triangle is Euclidean Ramsey.

It remains to show that the collinear set $\{0,1,2\}$ behaves differently. In every $\mathbb R^m$, use the [finite coloring](../../../../../finite-coloring.md)

$$
c(x)=\lfloor2\|x\|^2\rfloor\pmod {10}.
$$

A congruent copy has the form $a-v,a,a+v$ with $\|v\|=1$ for the [Euclidean norm](../../../../../euclidean-norm.md). The [parallelogram law](../../../../../parallelogram-law.md) gives

$$
2\|a+v\|^2+2\|a-v\|^2-4\|a\|^2=4.
$$

Put $n_+=\lfloor2\|a+v\|^2\rfloor$, $n_-=\lfloor2\|a-v\|^2\rfloor$, and $n_0=\lfloor2\|a\|^2\rfloor$. The errors introduced by the three [floor functions](../../../../../floor-function.md) show that

$$
2<n_++n_--2n_0<6.
$$

If all three points had one color, the integer in the middle would be divisible by ten, which is impossible. This proves the [three-term unit arithmetic progression is not Euclidean Ramsey](../../../../../three-term-unit-arithmetic-progression-is-not-euclidean-ramsey.md) assertion.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
