<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**Use a [Rao-Blackwell estimator after interim selection](../../../../../../rao-blackwell-estimator-after-interim-selection.md), which is exactly conditionally unbiased.** The second-stage [sample mean](../../../../../../sample-mean.md) $Y$ alone is unbiased conditional on continuation, but discards the earlier observations. Apply the [Rao-Blackwell theorem](../../../../../../rao-blackwell-theorem.md) by averaging $Y$ conditional on the combined [sample mean](../../../../../../sample-mean.md) $S$ and the fact of continuation.

Set $c=sf$ and $v=s/\sqrt2=\sigma/\sqrt{2n}$. Before truncation, $X\mid S$ is $N(S,v^2)$, a distribution whose mean no longer involves the unknown $\delta$. After imposing $X\ge c$, its mean is $S+v\lambda((c-S)/v)$. Since $Y=2S-X$, the resulting estimator is

$$
\boxed{\widetilde\delta=E(Y\mid S,\mathcal C)=S-v\lambda\left(\frac{c-S}{v}\right).}
$$

It uses the outcomes from both stages through their combined [sample mean](../../../../../../sample-mean.md). By iterated [expectation](../../../../../../expected-value.md), $E(\widetilde\delta\mid\mathcal C)=E(Y\mid\mathcal C)=\delta$, so its conditional [estimator bias](../../../../../../bias-of-an-estimator.md) is zero, compared with the strictly positive [estimator bias](../../../../../../bias-of-an-estimator.md) above. Its conditional [variance](../../../../../../variance-split.md) is no larger than that of the second-stage-only estimate. This does not assert a smaller [mean squared error](../../../../../../mean-squared-error.md) than every biased estimator.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
