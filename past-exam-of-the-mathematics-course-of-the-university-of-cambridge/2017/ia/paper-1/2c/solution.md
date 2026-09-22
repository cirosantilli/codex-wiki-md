<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

Componentwise,

$$
[(AB)^T]_{ij}=(AB)_{ji}=\sum_kA_{jk}B_{ki}
=\sum_k(B^T)_{ik}(A^T)_{kj}=(B^TA^T)_{ij},
$$

so

$$
\boxed{(AB)^T=B^TA^T}.
$$

Repeated application gives $(A^k)^T=(A^T)^k$. Transposing the [matrix exponential](../../../../../matrix-exponential.md) term by term therefore yields

$$
\boxed{(e^A)^T=e^{A^T}}.
$$

Multiplication of the two power series gives

$$
e^{tA}e^{tA^T}
=I+t(A+A^T)
+t^2\left(\frac12A^2+AA^T+\frac12(A^T)^2\right)+O(t^3).
$$

Hence

$$
\boxed{Q_0=I,\qquad Q_1=A+A^T,\qquad
Q_2=\frac12A^2+AA^T+\frac12(A^T)^2}.
$$

If $e^{tA}$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md) for every real $t$, then

$$
e^{tA}(e^{tA})^T=e^{tA}e^{tA^T}=I.
$$

Its coefficient of $t$ must vanish, so

$$
\boxed{A^T=-A};
$$

that is, $A$ is a [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md).

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
