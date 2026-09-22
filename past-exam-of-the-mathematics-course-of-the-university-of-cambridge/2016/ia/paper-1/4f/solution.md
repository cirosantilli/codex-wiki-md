<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Every counted point has [integer](../../../../../integer.md) coordinates and lies in the square $[-n,n]^2$, while the origin is always counted. Hence

$$
1\le a_n\le(2n+1)^2.
$$

No precise circle-area estimate is needed; this elementary bound controls the growth of the [power series](../../../../../power-series.md) coefficients.

The [comparison test for series](../../../../../comparison-test-for-series.md) states that if $0\le u_n\le v_n$, convergence of $\sum v_n$ implies convergence of $\sum u_n$. Equivalently, divergence of the smaller nonnegative series forces divergence of the larger one.

For $|z|=r<1$,

$$
\sum_{n=0}^\infty|a_nz^n|
\le\sum_{n=0}^\infty(2n+1)^2r^n.
$$

For $0<r<1$, the ratio of successive terms on the right tends to $r<1$, so the [ratio test](../../../../../ratio-test.md) and the [comparison test for series](../../../../../comparison-test-for-series.md) show [absolute convergence](../../../../../absolute-convergence.md). The case $r=0$ is immediate.

If $|z|\ge1$, then $|a_nz^n|\ge1$, so the terms do not tend to zero. The [term test for divergence](../../../../../term-test-for-divergence.md) therefore rules out convergence, including every point on the boundary $|z|=1$. Thus the [radius of convergence](../../../../../radius-of-convergence.md) is

$$
\boxed{R=1.}
$$

**The series converges exactly in the open unit disc.** This is an example of [polynomial coefficient growth with unit power-series radius](../../../../../polynomial-coefficient-growth-with-unit-power-series-radius.md): the lattice-count bound is polynomial rather than exponential.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
