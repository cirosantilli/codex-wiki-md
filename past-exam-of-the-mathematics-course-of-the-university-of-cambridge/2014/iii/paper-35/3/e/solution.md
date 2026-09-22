<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Under the point hypothesis $\beta=0$, the [test statistic](../../../../../../test-statistic.md) $\sqrt n\,\overline Y$ has a standard [normal distribution](../../../../../../normal-distribution.md). The observed statistic is three, giving a two-sided [p-value](../../../../../../p-value.md) $2[1-\Phi(3)]\simeq0.00270$. This is conventionally strong evidence against that point hypothesis. The narrow model $H_0$ is a continuous [prior distribution](../../../../../../prior-probability.md) around zero, rather than a point hypothesis.

For $n_0/n=100$ and $c=100$, [normal-normal conjugacy](../../../../../../normal-normal-conjugacy-with-known-observation-variance.md) gives

$$
\boxed{\beta\mid y,H_0\sim N\left(\frac{3}{101\sqrt n},\frac1{101n}\right),\qquad
\beta\mid y,H_1\sim N\left(\frac{300}{101\sqrt n},\frac{100}{101n}\right).}
$$

The narrow-model [posterior mean](../../../../../../posterior-mean.md) is strongly pulled toward zero and its [standard deviation](../../../../../../standard-deviation.md) is about $0.0995/\sqrt n$. The wide-model [posterior mean](../../../../../../posterior-mean.md) is about $2.9703/\sqrt n$, very close to the observation, with [standard deviation](../../../../../../standard-deviation.md) about $0.9950/\sqrt n$. **Each model produces a markedly different posterior**, so choosing between them requires their predictive evidence.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
