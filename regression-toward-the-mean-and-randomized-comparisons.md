# Regression toward the mean and randomized comparisons

↑ **Parent:** [Regression toward the mean](regression-toward-the-mean.md)

For [causal inference](causal-inference-split.md), a before-and-after change among units selected by an extreme baseline reading combines any [causal effect](causal-effect.md) with the change expected from selection. In the synthetic model the selected-group [mean](expected-value-split.md) falls by about $0.610$ with no [intervention](treatment.md) at all. Calling that entire fall an intervention effect would attribute a predictable [measurement error](measurement-error.md) contribution to a change in the signal.

One comparison design selects all eligible units by the same rule, then uses [randomization](randomization.md) to assign an [intervention](treatment.md) or a comparison condition, with the same measurement times and instrument in both groups. To see the principle algebraically, let assignment $A\in\{0,1\}$ be independent of $(T,\varepsilon_1,\varepsilon_2)$ within the selected population, and let the intervention add a constant $\delta$ to the second reading: $Y=T+\varepsilon_2+\delta A$. Then

$$
\mathbb E[Y-X\mid X>1,A=1]=-0.610054\ldots+\delta,\qquad
\mathbb E[Y-X\mid X>1,A=0]=-0.610054\ldots.
$$

Subtracting the two expected changes isolates $\delta$ under these assumptions. Both groups experience the same selection tendency in [expectation](expected-value-split.md). A finite experiment still has sampling uncertainty; [randomization](randomization.md) does not guarantee identical realized groups. Without [randomization](randomization.md), the same threshold alone does not establish comparable latent signals or error processes. Different selection rules, selective follow-up, changing instruments, or common temporal changes also require explicit assumptions. This is a [statistical inference](statistical-inference-split.md) principle about comparisons, not evidence that any particular [intervention](treatment.md) works.

## ↑ Ancestors (5)

1. [Regression toward the mean](regression-toward-the-mean.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
