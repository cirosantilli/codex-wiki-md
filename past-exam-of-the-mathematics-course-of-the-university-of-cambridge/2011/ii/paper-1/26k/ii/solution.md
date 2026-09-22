<h1 id="26k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $X_n\to X$ in probability. For a fixed real $t$ and any $\delta>0$, split according to $|X_n-X|\leq\delta$. The supplied exponential inequality and the bound $|e^{itX_n}-e^{itX}|\leq2$ give

$$
|\varphi_{X_n}(t)-\varphi_X(t)|\leq\mathbb E|e^{itX_n}-e^{itX}|\leq|t|\delta+2\mathbb P(|X_n-X|>\delta).
$$

Let $n\to\infty$, then $\delta\downarrow0$. Thus the [characteristic functions](../../../../../../characteristic-function.md) converge pointwise to $\varphi_X$. The [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) states that pointwise convergence of characteristic functions to a characteristic function continuous at zero implies [convergence in distribution](../../../../../../convergence-in-distribution.md). Every characteristic function is continuous at zero, so

$$
\boxed{X_n\xrightarrow{\mathbb P}X\ \Longrightarrow\ X_n\Rightarrow X.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [26K](../../26k.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
