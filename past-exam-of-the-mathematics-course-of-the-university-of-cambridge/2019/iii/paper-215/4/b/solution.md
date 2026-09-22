<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
m=\max_x\mathbb E_xT_A
$$

and choose $x$ attaining the maximum. For every $t$, the [Strong Markov property](../../../../../../strong-markov-property.md) at time $t$ gives

$$
m=\mathbb E_xT_A
\leq t+m\mathbb P_x(T_A>t).
$$

Thus

$$
\mathbb P_x(T_A\leq t)\leq\frac tm.
$$

If $t\geq t_{\mathrm{mix}}(1/4)$, then

$$
\mathbb P_x(X_t\in A)
\geq\pi(A)-\frac14\geq\frac14.
$$

Since $\{X_t\in A\}\subseteq\{T_A\leq t\}$, this is impossible when $t<m/4$. Allowing for integer times, one may take any smaller absolute constant, for example

$$
\boxed{t_{\mathrm{mix}}(1/4)\geq\frac18
\max_x\mathbb E_xT_A.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
