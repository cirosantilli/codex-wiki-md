<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $Z_n=X_{n\wedge T}$. The [stopped martingale in discrete time](../../../../../../stopped-martingale-in-discrete-time.md) identity

$$
Z_{n+1}-Z_n=\mathbf1_{\{T>n\}}(X_{n+1}-X_n)
$$

shows that $Z$ is a [martingale](../../../../../../martingale-split.md): the [indicator function](../../../../../../indicator-function.md) is $\mathcal F_n$-[measurable](../../../../../../measurability.md) and the increment has zero [conditional expectation](../../../../../../conditional-expectation.md). Integrability follows because $Z_n$ is selected from the finitely many integrable values $X_0,\ldots,X_n$.

For the [bounded stopping time](../../../../../../bounded-stopping-time.md) $\tau=n\wedge T$, the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) in its conditional form gives

$$
X_\tau=\mathbb E[X_n\mid\mathcal F_\tau].
$$

Here $\mathcal F_\tau$ is the [stopping-time sigma-algebra](../../../../../../stopping-time-sigma-algebra.md). Indeed, for $A\in\mathcal F_\tau$, partition $A$ into $A\cap\{\tau=k\}\in\mathcal F_k$ and apply the [martingale](../../../../../../martingale-split.md) identity $\mathbb E[X_n\mid\mathcal F_k]=X_k$ on each piece. This proves the displayed [conditional expectation](../../../../../../conditional-expectation.md) identity directly.

Let $C=\sup_n\mathbb E|X_n|<\infty$ and $A_n=\{|Z_n|>K\}\in\mathcal F_{n\wedge T}$. Conditional absolute-value domination and the [Markov inequality](../../../../../../markov-inequality.md) give $\mathbb P(A_n)\leq C/K$ and, for any $R>0$,

$$
\begin{aligned}
\mathbb E[|Z_n|\mathbf1_{A_n}]&\leq\mathbb E[|X_n|\mathbf1_{A_n}]\\
&\leq\mathbb E[|X_n|\mathbf1_{\{|X_n|>R\}}]+R\mathbb P(A_n)\\
&\leq\sup_j\mathbb E[|X_j|\mathbf1_{\{|X_j|>R\}}]+\frac{RC}{K}.
\end{aligned}
$$

First choose $R$ using the [uniform integrability](../../../../../../uniform-integrability.md) of $X$, and then choose $K$. The estimate is uniform in $n$, proving **[uniform integrability of a stopped uniformly integrable martingale](../../../../../../uniform-integrability-of-a-stopped-uniformly-integrable-martingale.md)**. No finiteness assumption on $T$ is needed.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
