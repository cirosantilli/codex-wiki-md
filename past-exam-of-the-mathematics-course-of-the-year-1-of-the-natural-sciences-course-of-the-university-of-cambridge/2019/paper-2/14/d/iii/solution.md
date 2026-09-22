<h1 id="14/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [probability density](../../../../../../probability-density.md) is an [even function](../../../../../../even-function.md). Its [derivative](../../../../../../derivative.md) simplifies to

$$
h'(z)=\frac1\pi\left[\frac1{1+(z+1/2)^2}-\frac1{1+(z-1/2)^2}\right]
=\frac{-2z}{\pi[1+(z+1/2)^2][1+(z-1/2)^2]}.
$$

It increases for $z<0$ and decreases for $z>0$, with maximum height $h(0)=2\arctan(1/2)/\pi$. Thus the most probable value, or [mode](../../../../../../mode-statistics.md), is $\boxed{z=0}$. The original sketch shows the symmetric, slightly flattened peak and long tails.

<a id="14/d/iii/image-density-of-a-standard-cauchy-variable-after-an-independent-uniform-displacement"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2-q14-cauchy-smoothing.png)

**[Figure 3](#14/d/iii/image-density-of-a-standard-cauchy-variable-after-an-independent-uniform-displacement). Density of a standard Cauchy variable after an independent uniform displacement**.

There is a genuine qualification to the request for a mean: **the mean does not exist**. The integral representation shows that $h(z)\sim1/(\pi z^2)$ as $|z|\to\infty$, so

$$
\int_0^\infty z h(z)\,dz=\infty,\qquad
\int_{-\infty}^0 z h(z)\,dz=-\infty.
$$

The two divergent integrals cannot be subtracted to define an [expected value](../../../../../../expected-value-split.md). Symmetry does give the [Cauchy principal value](../../../../../../cauchy-principal-value.md) $\lim_{A\to\infty}\int_{-A}^A zh(z)\,dz=0$, but that is not the mean. Equivalently, adding the bounded variable $Y$ cannot make the first absolute moment of a [Cauchy distribution](../../../../../../cauchy-distribution.md) finite.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [14](../../../14.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
