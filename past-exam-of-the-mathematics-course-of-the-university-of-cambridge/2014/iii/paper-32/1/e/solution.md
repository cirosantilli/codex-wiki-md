<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $X$ and $Y$ denote the first- and second-stage [sample means](../../../../../../sample-mean.md), let $s=\sigma/\sqrt n$, and write $S=(X+Y)/2$. Continuation is the selection event $\mathcal C=\{X\ge sf\}$. The second-stage [sample mean](../../../../../../sample-mean.md) stays independent of $\mathcal C$, so $E(Y\mid\mathcal C)=\delta$. The first-stage [sample mean](../../../../../../sample-mean.md) has a [truncated normal distribution](../../../../../../truncated-normal-distribution.md). With $a=f-\delta/s$ and the upper-tail [Inverse Mills ratio](../../../../../../inverse-mills-ratio.md) $\lambda(a)=\phi(a)/(1-\Phi(a))$,

$$
E(X\mid\mathcal C)=\delta+s\lambda(a),\qquad
\boxed{E(S\mid\mathcal C)-\delta=\frac{s}{2}\lambda\left(f-\frac{\delta}{s}\right)>0.}
$$

The positive [conditional selection bias after futility continuation](../../../../../../conditional-selection-bias-after-futility-continuation.md) comes from selecting unusually large first-stage outcomes. The unconditional [sample mean](../../../../../../sample-mean.md) of a fixed $2n$ observations would be unbiased; that is a different sampling distribution from the one restricted to continued trials.

As $\delta\to\infty$, $a\to-\infty$, $\phi(a)\to0$ and $1-\Phi(a)\to1$, so the [estimator bias](../../../../../../bias-of-an-estimator.md) tends to zero. It decreases with $\delta$: differentiating gives $\lambda'(a)=\lambda(a)(\lambda(a)-a)>0$, because $\lambda(a)=E(Z\mid Z>a)>a$ for a [standard normal random variable](../../../../../../standard-normal-random-variable.md). Thus

$$
\boxed{\text{the bias is upward, decreases as the effect increases, and tends to }0.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
