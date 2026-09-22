# Average conditional variance decreases with more information

↑ **Parent:** [Conditional variance](conditional-variance.md)

For [square-integrable](square-integrable-function.md) $X$ and nested information $\mathcal H\subseteq\mathcal G$, let $m_{\mathcal H}=\mathbb E[X\mid\mathcal H]$ and $m_{\mathcal G}=\mathbb E[X\mid\mathcal G]$. The predictor $m_{\mathcal H}$ is also $\mathcal G$-measurable, so the [conditional variance](conditional-variance.md) error identity gives

$$
\mathbb E[\operatorname{Var}(X\mid\mathcal H)]-\mathbb E[\operatorname{Var}(X\mid\mathcal G)]=\mathbb E[(m_{\mathcal G}-m_{\mathcal H})^2]\geq0.
$$

More information cannot increase the average best squared prediction error. Equality holds exactly when the two [conditional means](conditional-expectation.md) agree [almost surely](almost-sure-convergence.md); additional information can change the [conditional distribution](conditional-distribution.md) without changing its mean.

This is an averaged statement. Take $X=-4,0,4$ with equal probabilities, and learn only whether $X$ is zero. The unconditional [variance](variance-split.md) is $32/3$. In the nonzero group, the [conditional variance](conditional-variance.md) is $16$, which is larger; in the zero group it is zero. Their weighted average remains $(2/3)16+(1/3)0=32/3$. Both groups have [conditional mean](conditional-expectation.md) zero, so the extra information has not improved squared-error prediction, even though it has revealed whether the outcome is extreme or central. An individual group's [conditional variance](conditional-variance.md) need not decrease.

## ↑ Ancestors (8)

1. [Conditional variance](conditional-variance.md)
2. [Variance](variance-split.md)
3. [Expected value](expected-value.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
