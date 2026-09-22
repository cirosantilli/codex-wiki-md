<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The stationary solution of

$$
dq=-\nu q\,dt+\sqrt{\alpha\nu}\,dW
$$

is

$$
q(t)=\sqrt{\alpha\nu}\int_{-\infty}^te^{-\nu(t-u)}\,dW_u.
$$

It follows from the [Itô isometry](../../../../../../../ito-isometry.md) that

$$
\boxed{\langle q(t)q(t+\tau)\rangle
=\frac\alpha2e^{-\nu|\tau|}}.
$$

**Thus $q$ is zero-mean [colored noise](../../../../../../../colored-noise.md) with correlation time $\nu^{-1}$. The equation $\dot x=\mu(-\lambda x+q)$ is an overdamped harmonic particle of mobility $\mu$ driven by that correlated random force.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 353](../../../../paper-353-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
