<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A two-dimensional [box spline](../../../../../../box-spline.md) built from $m$ spanning directions is piecewise polynomial of total degree at most $m-2$. Here there are eight directions, counting multiplicities, so the regular pieces have **total degree six**. This is total degree, not separate degree six in each parameter.

For the [box spline](../../../../../../box-spline.md) smoothness criterion, let $r$ be the smallest number of directions whose removal leaves a set that does not span the plane. In this direction multiset, a line can contain at most two of the eight vectors, since each of the four distinct directions appears twice. At least six vectors must therefore be removed, and removing the six outside one chosen direction does achieve loss of rank. Hence $r=6$, giving

$$
\boxed{C^{r-2}=C^4\quad\text{between polynomial pieces of total degree }6.}
$$

In particular all fourth partial derivatives are continuous across the piece boundaries; generic fifth derivatives need not be. The [box spline](../../../../../../box-spline.md) criterion and this degree-six four-direction example are documented in the primary paper [4–8 Subdivision](https://cims.nyu.edu/gcl/papers/velho20014s.pdf). The factor count also explains the large support: the extra smoothing comes from repeating all four directional averaging factors. This regular-grid calculation does not establish $C^4$ at an [extraordinary subdivision vertex](../../../../../../extraordinary-subdivision-vertex.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
