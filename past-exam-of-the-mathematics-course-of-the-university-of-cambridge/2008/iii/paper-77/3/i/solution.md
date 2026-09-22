<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write a degree-$p$ [B-spline](../../../../../../b-spline.md) as $C(t)=\sum_iP_iN_{i,p}(t)$ and locate its [spline knot](../../../../../../spline-knot.md) span. There are several equivalent exact evaluation methods.

Evaluate the at most $p+1$ nonzero basis functions by the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md), then form their weighted sum of control points. Alternatively apply [De Boor's algorithm](../../../../../../de-boor-s-algorithm.md) directly to the $p+1$ active control points. In a span $[t_k,t_{k+1})$, initialize $d_j^{(0)}=P_{k-p+j}$ and repeatedly interpolate:

$$
d_j^{(r)}=(1-\alpha_{j,r})d_{j-1}^{(r-1)}+\alpha_{j,r}d_j^{(r-1)},\qquad \alpha_{j,r}=\frac{t-t_{k-p+j}}{t_{k+1+j-r}-t_{k-p+j}},
$$

for $r=1,\ldots,p$ and $j=p,p-1,\ldots,r$. The last point $d_p^{(p)}$ is $C(t)$; zero knot intervals are handled by the standard limiting convention or an appropriate neighboring nonempty span.

A third method precomputes the local polynomial coefficients on each span and evaluates them by [Horner's method](../../../../../../horner-s-method.md). For a uniform cubic [B-spline](../../../../../../b-spline.md), a fixed four-by-four basis matrix gives these coefficients. A fourth method uses [knot insertion](../../../../../../knot-insertion.md) to express the relevant span as a [Bézier curve](../../../../../../bezier-curve.md), followed by [De Casteljau's algorithm](../../../../../../de-casteljau-s-algorithm.md). Both interpolation algorithms also split the curve at the requested parameter. Repeated subdivision supplies arbitrarily accurate polygonal evaluation, although a finite subdivision mesh is generally an approximation rather than the exact requested point. **Basis summation, de Boor interpolation, local polynomial evaluation and Bézier extraction are equivalent exact representations.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
