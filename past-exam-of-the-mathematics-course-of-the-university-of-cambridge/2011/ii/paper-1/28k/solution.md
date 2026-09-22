<h1 id="28k/solution">Solution</h1>

↑ **Parent:** [28K](../28k.md)

For a [decision rule](../../../../../decision-rule.md) $\delta$ and loss $L$, its [risk function](../../../../../risk-function.md) is $R(\theta,\delta)=\mathbb E_\theta L(\theta,\delta(X))$. It is an [admissible estimator](../../../../../admissible-estimator.md) if there is no rule with risk everywhere no larger and somewhere strictly smaller. A [Bayes decision rule](../../../../../bayes-decision-rule.md) minimizes $\int R(\theta,\delta)\,\pi(d\theta)$ for a specified prior $\pi$. A [minimax decision rule](../../../../../minimax-decision-rule.md) minimizes $\sup_\theta R(\theta,\delta)$ over all rules.

Here the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is $\delta_0(X)=X$, and its squared-error risk is

$$
\boxed{R(\theta,\delta_0)=\sum_{i=1}^3\mathbb E_\theta(X_i-\theta_i)^2=3.}
$$

Write the proposed estimator as $\delta(X)=X+g(X)$ with $g(x)=-x/\|x\|^2$ for $x\ne0$, and assign any value at zero, an event of probability zero. Expanding the squared loss gives

$$
R(\theta,\delta)=3+\mathbb E_\theta\|g(X)\|^2+2\sum_i\mathbb E_\theta[(X_i-\theta_i)g_i(X)].
$$

[Stein's lemma](../../../../../stein-s-lemma-probability.md) for a unit-covariance normal vector says $\mathbb E[(X_i-\theta_i)g_i(X)]=\mathbb E[\partial_i g_i(X)]$ when the relevant derivatives and expectations are integrable. With $r=\|x\|$,

$$
\|g(x)\|^2=r^{-2},\qquad\sum_{i=1}^3\partial_ig_i(x)=-\frac3{r^2}+\frac{2\sum_i x_i^2}{r^4}=-r^{-2}.
$$

The singularity causes no difficulty in three dimensions: $r^{-2}$ is locally integrable against the volume element $r^2dr\,d\Omega$, and the normal tails control infinity. More formally apply Stein's lemma first to $g_\epsilon(x)=-x/(r^2+\epsilon)$, then let $\epsilon\downarrow0$; its squared norm and derivative magnitudes are bounded by constants times $r^{-2}$, so [dominated convergence](../../../../../dominated-convergence-theorem.md) justifies the limit. Consequently

$$
\boxed{R(\theta,\delta)=3-\mathbb E_\theta\frac1{\|X\|^2}<3\quad\text{for every }\theta\in\mathbb R^3.}
$$

The expectation is finite and strictly positive. Thus this [James–Stein estimator](../../../../../james-stein-estimator.md) strictly dominates the maximum likelihood estimator, which is inadmissible under the specified squared-error loss.

## ↑ Ancestors (11)

1. [28K](../28k.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
