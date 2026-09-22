<h1 id="11f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Another [convolution of probability densities](../../../../../../convolution-of-independent-random-variables.md) gives, for $0\le s\le1$,

$$
\boxed{f_{X+Y+Z}(s)=\int_0^s f_{X+Y}(u)\,du=\int_0^s u\,du=\frac{s^2}{2}.}
$$

Only this part of the density is needed because the fourth length is at most one.

Four positive lengths $a,b,c,d$ can form a nondegenerate [quadrilateral](../../../../../../quadrilateral.md) if and only if every length is less than the sum of the other three. Necessity follows by following the other three sides between the endpoints of the longest side and applying the [triangle inequality](../../../../../../triangle-inequality.md). For sufficiency, select a diagonal length $r$ in the intersection

$$
(|a-b|,a+b)\cap(|c-d|,c+d).
$$

Both intervals are nonempty, and their intersection is nonempty exactly when $|a-b|<c+d$ and $|c-d|<a+b$. These are precisely the four strict length inequalities. Construct [triangles](../../../../../../triangle.md) with sides $(a,b,r)$ and $(c,d,r)$ on opposite sides of their common diagonal. Their union has the required simple, nondegenerate [quadrilateral](../../../../../../quadrilateral.md) as boundary.

The failure events, in which one length is at least the sum of the others, are disjoint except on sets of [probability](../../../../../../probability.md) zero. For the specified length $W$, [independence](../../../../../../independent-random-variables.md) and the density above give

$$
\mathbb P(W\ge X+Y+Z)=\int_0^1(1-s)\frac{s^2}{2}\,ds=\frac1{24}.
$$

There are four symmetric choices of the overly long side, so **the probability is**

$$
\boxed{1-4\cdot\frac1{24}=\frac56.}
$$

This is the four-sided case of the [polygon probability for independent uniform rods](../../../../../../polygon-probability-for-independent-uniform-rods.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
