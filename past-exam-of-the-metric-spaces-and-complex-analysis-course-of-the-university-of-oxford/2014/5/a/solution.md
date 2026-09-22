<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [Laurent series](../../../../laurent-series.md) about $a$ as $\sum_{k\in\mathbb Z}c_k(z-a)^k$. The isolated singularity is:

- [removable singularity](../../../../removable-singularity.md) if every negative-index coefficient is zero;
- a [pole](../../../../pole.md) of order $m\geq1$ if $c_{-m}\ne0$ and $c_k=0$ for $k<-m$;
- an [essential singularity](../../../../essential-singularity.md) if infinitely many negative-index coefficients are nonzero.

These cases exhaust the possible principal parts. The [residue](../../../../residue.md) is

$$
\boxed{\operatorname{res}(f;a)=c_{-1}=\frac1{2\pi i}\int_{|z-a|=\rho}f(z)\,dz,\quad0<\rho<r.}
$$

For the first example, $\sin z=z+O(z^3)$ gives

$$
\frac1{\sin^2z}=\frac1{z^2}+\frac13+O(z^2).
$$

Thus zero is a **double [pole](../../../../pole.md)**, with [residue](../../../../residue.md) zero. For the other example,

$$
1-\cos z=\frac{z^2}2+O(z^4),\qquad1-e^z=-z+O(z^2),
$$

so the ratio is $-z/2+O(z^2)$. Its singularity is **removable**, with extended value zero and [residue](../../../../residue.md) zero. The numerator's zero has higher order than the denominator's, so there is no [pole](../../../../pole.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
