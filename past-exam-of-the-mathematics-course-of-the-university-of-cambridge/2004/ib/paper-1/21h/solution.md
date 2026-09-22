<h1 id="21h/solution">Solution</h1>

↑ **Parent:** [21H](../21h.md)

The [Rao-Blackwell theorem](../../../../../rao-blackwell-theorem.md) states that if an estimator $D$ has finite second moment and $T$ is a [sufficient statistic](../../../../../sufficient-statistic.md), then $D^*(T)=\mathbb E[D\mid T]$ can be chosen without knowing the parameter. It has the same expectation as $D$ and no larger [variance](../../../../../variance-split.md). In particular an [unbiased estimator](../../../../../unbiased-estimator.md) remains unbiased and its squared-error risk cannot increase. Sufficiency makes the [conditional distribution](../../../../../conditional-distribution.md), hence the function of $T$ used here, parameter-independent.

The tower property gives $\mathbb E D^*=\mathbb E D$. The [law of total variance](../../../../../law-of-total-variance.md) gives

$$
\operatorname{Var}(D)=\operatorname{Var}(\mathbb E[D\mid T])+\mathbb E[\operatorname{Var}(D\mid T)],
$$

so the [variance](../../../../../variance-split.md) decreases, with equality exactly when $D$ is already a function of $T$ almost surely. Since the bias is unchanged, the same identity proves the squared-error risk claim. More generally the corresponding convex-loss inequality follows from conditional [Jensen's inequality](../../../../../jensen-s-inequality.md).

For the given [geometric distribution](../../../../../geometric-distribution.md), the joint mass is $(1-p)^np^{\sum x_j-n}$ on positive-integer sample vectors. Thus $T=\sum_jX_j$ is a one-dimensional [sufficient statistic](../../../../../sufficient-statistic.md). Directly, conditional on $T=t$, every positive-integer composition of $t$ into $n$ parts has the same [probability](../../../../../probability.md); there are $\binom{t-1}{n-1}$ such compositions, independently of $p$.

The simple estimator $D=1_{\{X_1>1\}}$ is unbiased for $p$, since $\Pr(X_1>1)=p$. For $n\geq2$, compositions with $X_1>1$ are counted by subtracting one from their first part, giving $\binom{t-2}{n-1}$ when $t>n$. Consequently the [Rao-Blackwell estimator of a geometric failure probability](../../../../../rao-blackwell-estimator-of-a-geometric-failure-probability.md) is

$$
\boxed{\widehat p=\mathbb E[D\mid T]=\frac{T-n}{T-1},\qquad n\geq2.}
$$

At $T=n$ its value is zero, as it must be when all observations are one. For the possible one-observation case, use $\widehat p=1_{\{T>1\}}$; the displayed fraction would otherwise be undefined at $T=1$. The conditional-expectation argument proves unbiasedness without needing to sum the negative-binomial mass explicitly.

## ↑ Ancestors (10)

1. [21H](../21h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
