<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [sine](../../../../../sine.md) and [cosine](../../../../../cosine.md) functions are orthogonal over a complete period. For positive integers $m,n$,

$$
\int_0^T\cos(m\omega t)\cos(n\omega t)\,dt
=\int_0^T\sin(m\omega t)\sin(n\omega t)\,dt
=\frac T2\delta_{mn},
$$

while every mixed sine-cosine integral and every integral of a nonconstant single harmonic is zero. These identities follow from the product-to-sum formulas and the integer-period endpoint values.

Multiply the [Fourier series](../../../../../fourier-series-split.md) by $\cos(m\omega t)$ and integrate. All terms except $a_m\cos^2(m\omega t)$ vanish, giving $Ta_m/2$. Repeating with [sine](../../../../../sine.md) isolates $b_m$. Thus

$$
\boxed{a_n=\frac2T\int_0^T V_1(t)\cos(n\omega t)\,dt,\qquad
b_n=\frac2T\int_0^T V_1(t)\sin(n\omega t)\,dt},\quad n\geq1.
$$

Integrating without a harmonic also gives $a_0=(2/T)\int_0^T V_1(t)\,dt$. The factor $1/2$ on the constant term in the chosen convention is essential.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
