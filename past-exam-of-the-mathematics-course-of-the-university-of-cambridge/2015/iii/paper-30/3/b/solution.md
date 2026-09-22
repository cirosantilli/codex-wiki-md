<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $s<t$ and an event $A\in\mathcal F_s$. Multiplying the conditional [characteristic function](../../../../../../characteristic-function.md) identity by $1_A$ and taking expectation gives

$$
\mathbb E[1_Ae^{i\theta(X_t-X_s)}]
=\mathbb P(A)e^{-\theta^2(t-s)/2}.
$$

The left side is the Fourier transform of the finite measure

$$
\mu_A(D)=\mathbb P(A\cap\{X_t-X_s\in D\}).
$$

By the [uniqueness theorem for characteristic functions](../../../../../../uniqueness-theorem-for-characteristic-functions.md), this measure equals $\mathbb P(A)$ times the $N(0,t-s)$ distribution. Thus, for every Borel set $D$,

$$
\mathbb P(A\cap\{X_t-X_s\in D\})
=\mathbb P(A)\,\mathbb P(N(0,t-s)\in D).
$$

Taking $A$ to be the whole sample space identifies the increment's law, and the full identity proves independence from $\mathcal F_s$. Together with the assumed adaptation, continuity, and initial value, these are exactly the defining Brownian properties. This proves the [conditional characteristic-function criterion for Brownian increments](../../../../../../conditional-characteristic-function-criterion-for-brownian-increments.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
