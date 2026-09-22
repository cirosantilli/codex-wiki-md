<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $k=2$ on an equidistant [spline knot sequence](../../../../../../spline-knot-sequence.md), $N_i$ is the triangular hat with value one at $t_{i+1}$ and [support](../../../../../../support.md) $[t_i,t_{i+2}]$. Its slopes on the two pieces are $1/h$ and $-1/h$, and $M_i=N_i/h$. Direct integration gives

$$
\int N_i^2=2\int_0^h(u/h)^2\,du=\frac{2h}{3},\qquad
\int N_iN_{i+1}=\int_0^h(u/h)(1-u/h)\,du=\frac h6.
$$

Nonadjacent hats have disjoint interiors of their supports, so their [inner product](../../../../../../inner-product.md) vanishes. Dividing by $h$ therefore gives

$$
\boxed{g_{ij}=\begin{cases}2/3,&i=j,\\1/6,&|i-j|=1,\\0,&|i-j|\ge2.\end{cases}}
$$

This [linear-spline mixed Gram matrix](../../../../../../linear-spline-mixed-gram-matrix.md) is [tridiagonal](../../../../../../tridiagonal-matrix.md). Every diagonal entry is $2/3$, including the first and last: the distinct-knot hats have their full supports inside $[0,1]$. End rows simply lack one off-diagonal neighbor; there are no repeated endpoint [spline knots](../../../../../../spline-knot.md) here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
