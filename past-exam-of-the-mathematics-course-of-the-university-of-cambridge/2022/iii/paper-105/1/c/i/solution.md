<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Sobolev fundamental theorem of calculus on lines](../../../../../../../sobolev-fundamental-theorem-of-calculus-on-lines.md) gives, for almost every $x$,

$$
\Delta_i^hu(x)=\int_0^1D_i u(x+the_i)\,dt.
$$

Apply the [Minkowski integral inequality](../../../../../../../minkowski-integral-inequality.md) and translation invariance of [Lebesgue measure](../../../../../../../lebesgue-measure.md):

$$
\lVert\Delta_i^hu\rVert_{L^2(V)}
\leq\int_0^1\lVert D_i u(\,cdot+the_i)\rVert_{L^2(V)}dt
\leq\lVert D_i u\rVert_{L^2(U)}.
$$

The restriction on $h$ ensures that every translated copy used above lies in $U$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
