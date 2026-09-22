<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\Delta X_{n+1}=X_{n+1}-X_n$ and $Y=\sum_{n\geq0}|\Delta X_{n+1}|\mathbf1_{\{T>n\}}$. Since $T$ is a [stopping time](../../../../../../stopping-time.md), $\{T>n\}\in\mathcal F_n$. The [Tonelli theorem](../../../../../../tonelli-theorem.md), [conditional expectation](../../../../../../conditional-expectation.md), and (c)'s [tail-sum formula for expectation](../../../../../../tail-sum-formula-for-expectation.md) yield

$$
\begin{aligned}
\mathbb EY
&=\sum_{n\geq0}\mathbb E\left[\mathbf1_{\{T>n\}}\mathbb E(|\Delta X_{n+1}|\mid\mathcal F_n)\right]\\
&\leq C\sum_{n\geq0}\mathbb P(T>n)=C\mathbb ET<\infty.
\end{aligned}
$$

Thus $Y$ is an [integrable random variable](../../../../../../integrable-random-variable.md). Since $X_0=0$, telescoping gives $|X_T|\leq Y$ and $|X_n|\mathbf1_{\{T>n\}}\leq Y\mathbf1_{\{T>n\}}$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives $\mathbb E[|X_n|\mathbf1_{\{T>n\}}]\to0$, so (b) gives [uniform integrability](../../../../../../uniform-integrability.md) of the [stopped martingale](../../../../../../stopped-martingale.md).

The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at the bounded [stopping time](../../../../../../stopping-time.md) $n\wedge T$ gives $\mathbb E X_{n\wedge T}=\mathbb E X_0=0$. Passing to the limit using the [convergence in L1](../../../../../../convergence-in-l1.md) proved in (b),

$$
\boxed{\mathbb E X_T=\mathbb E X_0=0.}
$$

One can also pass directly by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), since $|X_{n\wedge T}|\leq Y$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
