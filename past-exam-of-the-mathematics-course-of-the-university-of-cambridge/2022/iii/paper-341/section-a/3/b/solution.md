<h1 id="section-a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $H_h$ be the periodic centered second-difference matrix minus the real diagonal matrix containing $V(x_m)$. It is a [Hermitian matrix](../../../../../../../hermitian-operator.md), so the [semidiscrete system](../../../../../../../method-of-lines.md) is

$$
\mathbf u'=-iH_h\mathbf u
$$

with a [skew-Hermitian matrix](../../../../../../../skew-hermitian-matrix.md) generator. Consequently

$$
\frac d{dt}\|\mathbf u(t)\|_2^2
=2\operatorname{Re}\langle\mathbf u,-iH_h\mathbf u\rangle=0.
$$

Its exact propagator $e^{-itH_h}$ is a [unitary matrix](../../../../../../../unitary-matrix.md), and therefore the semidiscretization is stable in the discrete $2$-norm, uniformly for all times and mesh sizes.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Section A](../../../section-a.md)
4. [Paper 341](../../../../paper-341-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
