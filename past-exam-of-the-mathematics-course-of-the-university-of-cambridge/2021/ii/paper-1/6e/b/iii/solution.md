<h1 id="6e/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At an [endemic equilibrium](../../../../../../../endemic-equilibrium.md), $I^*>0$. The equation $\dot I=0$ then gives

$$
\boxed{S^*=\frac{d+\delta}{\beta}}.
$$

Since also $S^*>0$, the equation $\dot S=0$ gives

$$
\boxed{\beta I^*+d=be^{-aS^*}},
\qquad
I^*=\frac{be^{-aS^*}-d}{\beta}.
$$

This infective population is positive precisely when

$$
S^*<\frac1a\log\frac bd=N^*,
$$

which is exactly the assumed instability condition for the disease-free equilibrium. Thus the [endemic equilibrium of the susceptible-infective model with exponential birth](../../../../../../../endemic-equilibrium-of-the-susceptible-infective-model-with-exponential-birth.md) exists.

At this equilibrium the relations above reduce the [Jacobian matrix](../../../../../../../jacobian-matrix.md) to

$$
J(S^*,I^*)=
\begin{pmatrix}
-aS^*be^{-aS^*}&-\beta S^*\\
\beta I^*&0
\end{pmatrix}.
$$

Hence

$$
\operatorname{tr}J=-aS^*be^{-aS^*}<0,
\qquad
\det J=\beta^2S^*I^*>0.
$$

By the [trace-determinant stability criterion](../../../../../../../trace-determinant-stability-criterion.md), both eigenvalues have negative real part. The [linearization stability theorem](../../../../../../../linearization-stability-theorem.md) therefore proves that the endemic equilibrium is locally [asymptotically stable](../../../../../../../asymptotic-stability.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6E](../../../6e.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
