<h1 id="27j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Writing $S=\sum X_i$, the [likelihood function](../../../../../../likelihood-function.md) is $\theta^S(1-\theta)^{n-S}$ and its supremum occurs at $\widehat\theta=S/n$, including the limiting boundary cases zero and one. The [likelihood ratio](../../../../../../likelihood-ratio.md) compares $2^{-n}$ under the null with that supremum. Thus

$$
\boxed{-2\log\Lambda=T_n=2n[\widehat\theta\log\widehat\theta+(1-\widehat\theta)\log(1-\widehat\theta)+\log2]}.
$$

Use $0\log0=0$ at boundary outcomes. [Wilks theorem](../../../../../../wilks-theorem.md) gives asymptotic $\chi^2_1$ under the regular interior null, because one parameter is constrained. Directly, setting $\widehat\theta=1/2+Z$ and expanding the bracket gives $2Z^2+O(Z^4)$, hence

$$
\boxed{T_n=4nZ_n^2+O(nZ_n^4)}.
$$

Under the null, $2\sqrt nZ_n\xrightarrow d N(0,1)$ and $Z_n=O_P(n^{-1/2})$. The remainder vanishes in probability, proving the same [chi-squared distribution](../../../../../../chi-squared-distribution.md) limit. If an observed $Z_n$ is not small, the quadratic numerical approximation is unreliable and the exact statistic should be used; exact binomial calibration is available. Persistent non-small deviations under a fixed alternative instead make the statistic grow linearly with $n$, rather than having the null [chi-squared distribution](../../../../../../chi-squared-distribution.md) law.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27J](../../27j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
