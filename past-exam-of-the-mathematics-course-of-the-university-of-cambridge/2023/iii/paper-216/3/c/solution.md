<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the [stationary distribution](../../../../../../stationary-distribution.md) property, $X_1$ and $X_2$ have the same [marginal distribution](../../../../../../marginal-distribution.md) $\pi$. Expanding the square gives

$$
\begin{aligned}
\frac12\mathbb E[(f(X_2)-f(X_1))^2]
&=\frac12\left(2\langle f,f\rangle_\pi
-2\mathbb E[f(X_1)f(X_2)]\right)\\
&=\langle f,f\rangle_\pi-\langle f,Kf\rangle_\pi\\
&=\langle f,(I-K)f\rangle_\pi
=\mathcal E_K(f).
\end{aligned}
$$

This is the probabilistic representation of the [Dirichlet form of a Markov chain](../../../../../../dirichlet-form-of-a-markov-chain.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
