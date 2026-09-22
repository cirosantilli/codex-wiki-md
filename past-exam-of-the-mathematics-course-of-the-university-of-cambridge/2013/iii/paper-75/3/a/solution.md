<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Euclidean configuration-space transition kernel](../../../../../../euclidean-configuration-space-transition-kernel.md) is obtained by slicing $\tau$ into $M$ steps $\delta=\tau/M$, inserting position resolutions and using the free Gaussian kernel. With initial $q_i=\pm a$ and final $q_f=a$,

$$
\boxed{\langle q_f|e^{-H\tau/\hbar}|q_i\rangle=\int_{q(0)=q_i}^{q(\tau)=q_f}\!\mathcal Dq\,
\exp\left[-\frac1\hbar\int_0^\tau\left(\frac m2\dot q^2+V(q)\right)dt\right].}
$$

The normalization means the limit of $(m/(2\pi\hbar\delta))^{M/2}\int\prod_{j=1}^{M-1}dq_j$ with exponent $-\sum_j[m(q_{j+1}-q_j)^2/(2\delta)+\delta V(q_j)]/\hbar$, in a consistent time-slice prescription. This fixes the endpoint normalization that an informal continuum symbol alone leaves unspecified. The [Wick rotation](../../../../../../wick-rotation.md) converts oscillatory real-time weight into the positive-potential Euclidean weight; classical extrema of this action organize the semiclassical approximation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
