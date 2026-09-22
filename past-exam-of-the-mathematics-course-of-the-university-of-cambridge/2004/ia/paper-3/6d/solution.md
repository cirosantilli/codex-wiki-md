<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

A real three-by-three [matrix](../../../../../matrix.md) represents a proper [rotation](../../../../../rotation-mathematics.md) in the standard orthonormal basis precisely when $A^TA=I$ and $\det A=1$, that is, when $A\in\mathrm{SO}(3)$. For the supplied integer numerator $B=3A$, direct multiplication gives $B^TB=9I$ and $\det B=27$, verifying both conditions.

The rotation axis is the [eigenspace](../../../../../eigenspace.md) for [eigenvalue](../../../../../eigenvalue.md) one. Solving $(A-I)n=0$ gives $n_3=0$ and $n_2=2n_1$, so

$$
\boxed{n=\frac1{\sqrt5}(1,2,0)^T}
$$

is a unit axis vector; its negative describes the same axis. On its perpendicular plane the [rotation matrix](../../../../../rotation-matrix.md) has eigenvalues $e^{i\theta}$ and $e^{-i\theta}$. The [rotation trace formula](../../../../../trace-of-a-three-dimensional-rotation.md) therefore gives $\operatorname{tr}A=1+2\cos\theta$. Since the trace is $-1/3$,

$$
\boxed{\cos\theta=-\frac23.}
$$

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
