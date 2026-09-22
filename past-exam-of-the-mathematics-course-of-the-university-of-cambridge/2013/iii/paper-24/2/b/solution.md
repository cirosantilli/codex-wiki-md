<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $u\in\mathbb R$ and let $s\to t$. For any $\delta>0$, use $|e^{ia}-e^{ib}|\leq\min(2,|a-b|)$ to obtain

$$
\begin{aligned}
|\varphi_{X_s}(u)-\varphi_{X_t}(u)|
&\leq\mathbb E|e^{iuX_s}-e^{iuX_t}|\\
&\leq |u|\delta+2\mathbb P(|X_s-X_t|>\delta).
\end{aligned}
$$

The probability tends to zero by [stochastic continuity](../../../../../../stochastic-continuity.md). Taking the limit superior and then letting $\delta\downarrow0$ proves

$$
\boxed{\varphi_{X_s}(u)\longrightarrow\varphi_{X_t}(u).}
$$

This proves [continuity of Lévy characteristic functions](../../../../../../continuity-of-levy-characteristic-functions.md) from the elementary estimate, without requiring [moments](../../../../../../moment.md) or replacing [convergence in probability](../../../../../../convergence-in-probability.md) by an unjustified almost sure limit. At $t=0$, time approaches from the right. If stochastic continuity is formulated only at zero, [stationary increments](../../../../../../stationary-increments.md) give the same argument at every $t$: the absolute value of $X_s-X_t$ has the law of $|X_{|s-t|}|$. For $u=0$ the [characteristic function](../../../../../../characteristic-function.md) is identically one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
