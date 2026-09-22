<h1 id="6b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Eliminate $R=N-S-I$ to obtain the [two-dimensional autonomous differential equation](../../../../../../autonomous-system-mathematics.md)

$$
\dot S=\alpha(N-S-I)-\beta SI,
\qquad
\dot I=\beta SI-\gamma I.
$$

Its [Jacobian matrix](../../../../../../jacobian-matrix.md) at the endemic equilibrium is

$$
J_*=
\begin{pmatrix}
-\alpha-\beta I^*&-\alpha-\gamma\\
\beta I^*&0
\end{pmatrix}.
$$

Since $I^*>0$,

$$
\operatorname{tr}J_*=-(\alpha+\beta I^*)<0,
\qquad
\det J_*=\beta I^*(\alpha+\gamma)>0.
$$

The [trace-determinant stability criterion](../../../../../../trace-determinant-stability-criterion.md) shows that both [eigenvalues](../../../../../../eigenvalue.md) have negative real part. The [Endemic equilibrium of the SIR model with waning immunity](../../../../../../endemic-equilibrium-of-the-sir-model-with-waning-immunity.md) is therefore locally [asymptotically stable](../../../../../../asymptotic-stability.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6B](../../6b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
