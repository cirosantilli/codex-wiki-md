<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With $K\ge2$ distinct knots $\kappa_1<\cdots<\kappa_K$, a [natural cubic spline](../../../../../../natural-cubic-spline.md) is a $C^2$ function on the real line, cubic on each interval between consecutive knots and affine outside the two outer knots. The latter condition gives $m''(\kappa_1)=m''(\kappa_K)=0$.

There are $4(K-1)$ coefficients for the interior cubic pieces. Matching values and the first two [derivatives](../../../../../../derivative.md) at the $K-2$ interior knots imposes $3(K-2)$ independent constraints, and the two natural endpoint conditions impose two more. The affine continuations are then determined by endpoint values and slopes. The [dimension of a vector space](../../../../../../dimension-vector-space.md) is therefore

$$
\boxed{4(K-1)-3(K-2)-2=K.}
$$

One explicit [basis](../../../../../../basis.md) uses $1,x$ and $d_j(x)-d_{K-1}(x)$ for $j=1,\ldots,K-2$, where

$$
d_j(x)=\frac{(x-\kappa_j)_+^3-(x-\kappa_K)_+^3}{\kappa_K-\kappa_j},\qquad u_+=\max(u,0).
$$

The cubic and quadratic terms cancel in each difference above $\kappa_K$, making it affine there; below $\kappa_1$ the truncated powers vanish. The changes in third derivative at individual knots show [independence](../../../../../../independent-random-variables.md) of these basis functions. This count uses the [linear independence](../../../../../../linear-independence.md) of the spline constraints and counts the listed outer knots as boundary knots. If a convention instead lists $K$ interior knots and two additional boundaries, the dimension is $K+2$. With only one listed knot and linearity on both sides, the $C^2$ condition forces a globally [affine function](../../../../../../affine-function.md), so the exceptional dimension is two.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
