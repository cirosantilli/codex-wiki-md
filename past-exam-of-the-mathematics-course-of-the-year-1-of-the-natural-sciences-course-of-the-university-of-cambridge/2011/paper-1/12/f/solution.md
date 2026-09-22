<h1 id="12/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the lower limit $s=t+r_0$ for the inner integral:

$$
P(r>r_0)=\int_0^\infty\frac{e^{-t/\bar t}}{\bar t}
\left[\int_{t+r_0}^\infty\frac{e^{-s/\bar s}}{\bar s}ds\right]dt
=\frac{e^{-r_0/\bar s}}{\bar t}\int_0^\infty e^{-t(1/\bar s+1/\bar t)}dt.
$$

Hence

$$
\boxed{P(r>r_0)=\frac{\bar s}{\bar s+\bar t}e^{-r_0/\bar s},\qquad r_0>0.}
$$

The prefactor is the [probability](../../../../../probability.md) that interruption occurs; the remaining exponential is its conditional positive tail. This is the [positive difference of independent exponential waiting times](../../../../../positive-difference-of-independent-exponential-waiting-times.md). The exponent is dimensionless because both $r_0$ and $\bar s$ are measured in minutes.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
