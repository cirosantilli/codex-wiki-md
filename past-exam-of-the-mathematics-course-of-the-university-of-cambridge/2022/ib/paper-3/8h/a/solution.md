<h1 id="8h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expand according to the hitting time and use [detailed balance](../../../../../../detailed-balance.md) to reverse each finite path:

$$
\begin{aligned}
\mathbb P_\pi(X_{T_A}=z)
&=\sum_{n\geq0}
\sum_{x_0,\ldots,x_{n-1}\notin A}
\pi(x_0)P(x_0,x_1)\cdots P(x_{n-1},z)\\
&=\pi(z)\sum_{n\geq0}
\mathbb P_z(X_1,\ldots,X_n\notin A).
\end{aligned}
$$

The event in the final probability is $\{T_A^+>n\}$. The tail-sum formula for a nonnegative integer-valued random variable gives

$$
\sum_{n\geq0}\mathbb P_z(T_A^+>n)=\mathbb E_zT_A^+.
$$

Therefore

$$
\boxed{\mathbb P_\pi(X_{T_A}=z)=\pi(z)\mathbb E_zT_A^+}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8H](../../8h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
