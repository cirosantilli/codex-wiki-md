<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed observed colour $\widetilde c_s$, [Bayes' theorem](../../../../../../bayes-theorem.md) gives

$$
p(E_s\mid\widetilde c_s)
\propto
\exp\!\left[-\frac{(\widetilde c_s-E_s-c_0)^2}{2\sigma_c^2}-\frac{E_s}{\tau}\right]
\mathbf1_{\{E_s\geq0\}}.
$$

Completing the square shows that this is a [truncated normal distribution](../../../../../../truncated-normal-distribution.md) with variance $\sigma_c^2$, lower endpoint zero, and untruncated location

$$
e_s=\widetilde c_s-c_0-\frac{\sigma_c^2}{\tau}.
$$

Hence

$$
\overline E_s
\equiv\mathbb E[E_s\mid\widetilde c_s]
=e_s+\sigma_c\frac{\phi(e_s/\sigma_c)}{\Phi(e_s/\sigma_c)}.
$$

Conditioning first on $E_s$ and using the [law of total expectation](../../../../../../law-of-total-expectation.md) yields the dusty colour-magnitude relation

$$
\mathbb E[\widetilde M_s\mid\widetilde c_s]
=M_0+\beta\widetilde c_s+(R-\beta)\overline E_s.
$$

As $\widetilde c_s\to-\infty$, the [Inverse Mills ratio](../../../../../../inverse-mills-ratio.md) implies $\overline E_s\to0$ with vanishing derivative, so the asymptotic slope is $\beta$. As $\widetilde c_s\to+\infty$, $\overline E_s\sim\widetilde c_s-c_0-\sigma_c^2/\tau$, so the asymptotic slope is $R$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
