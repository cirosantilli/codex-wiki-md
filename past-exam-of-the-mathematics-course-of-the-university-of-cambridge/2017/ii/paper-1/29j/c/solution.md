<h1 id="29j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The bounded-time [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) states that if $X$ is an integrable discrete-time [martingale](../../../../../../martingale-split.md) and $\tau$ is a [stopping time](../../../../../../stopping-time.md) bounded by a deterministic integer $N$, then $X_\tau$ is integrable and $\mathbb E X_\tau=\mathbb E X_0$. Indeed $|X_\tau|\le\sum_{j=0}^N|X_j|$ proves integrability, and

$$
X_\tau=X_0+\sum_{j=1}^N\mathbf1_{\{\tau\ge j\}}(X_j-X_{j-1}).
$$

The event $\{\tau\ge j\}=\{\tau>j-1\}$ belongs to $\mathcal F_{j-1}$. [Conditional expectation](../../../../../../conditional-expectation.md) of each summand given $\mathcal F_{j-1}$ is zero, so

$$
\boxed{\mathbb E X_\tau=\mathbb E X_0}.
$$

More generally, if $\sigma\le\tau\le N$ are [stopping times](../../../../../../stopping-time.md), $\mathbb E[X_\tau\mid\mathcal F_\sigma]=X_\sigma$. To prove this, test against $A\in\mathcal F_\sigma$ and apply the same argument to $\mathbf1_A\mathbf1_{\{\sigma<j\le\tau\}}(X_j-X_{j-1})$; its coefficient is $\mathcal F_{j-1}$-measurable. Boundedness of the [stopping times](../../../../../../stopping-time.md) makes the sums finite, so no limiting optional-stopping hypothesis is being omitted.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
