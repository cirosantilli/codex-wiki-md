<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

A family $\mathcal R$ is [uniformly integrable](../../../../../uniform-integrability.md) if

$$
\lim_{K\to\infty}\sup_{X\in\mathcal R}E[|X|\mathbf1_{\{|X|>K\}}]=0.
$$

This implies integrability and a uniform bound on $E|X|$, since $E|X|\leq K+E[|X|\mathbf1_{\{|X|>K\}}]$. [Convergence in probability](../../../../../convergence-in-probability.md) means $P(|X_n-X|>\varepsilon)\to0$ for every $\varepsilon>0$; convergence in $L^1$ means $E|X_n-X|\to0$. The latter implies the former by [Markov's inequality](../../../../../markov-inequality.md). Conversely, [convergence in probability](../../../../../convergence-in-probability.md) together with [uniform integrability](../../../../../uniform-integrability.md) of $\{X_n\}$ implies that $X$ is integrable and $X_n\to X$ in $L^1$. Moreover an $L^1$-convergent sequence is [uniformly integrable](../../../../../uniform-integrability.md). This is the criterion that excludes rare very large values from carrying a nonvanishing first-moment error.

For the sum family, use the pointwise bound

$$
|X+Y|\mathbf1_{\{|X+Y|>K\}}
\leq2|X|\mathbf1_{\{|X|>K/2\}}+2|Y|\mathbf1_{\{|Y|>K/2\}}.
$$

Indeed, if the left indicator is one then the larger of $|X|,|Y|$ exceeds $K/2$, and twice that larger number bounds $|X+Y|$. Taking [expectations](../../../../../expected-value.md) and the [supremum](../../../../../supremum.md) over $\mathcal R_1,\mathcal R_2$ bounds the sum-family tail by the sum of their two uniformly vanishing tails. Thus **the whole family of sums is [uniformly integrable](../../../../../uniform-integrability.md)**, with no [independence](../../../../../independent-random-variables.md) assumption.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
