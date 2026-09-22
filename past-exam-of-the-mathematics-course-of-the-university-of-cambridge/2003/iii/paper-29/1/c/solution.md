<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Again put $Y=\mathbb E[X\mid\mathcal G]$. For any fixed real $c$, the [random variable](../../../../../../random-variable-split.md)

$$
D_c=|X-c|-\operatorname{sign}(Y-c)(X-c)
$$

is nonnegative and [integrable](../../../../../../integrability.md). The [sign function](../../../../../../sign-function.md) of $Y-c$ is bounded and $\mathcal G$-[measurable](../../../../../../measurability.md), so conditioning and equality of the [probability distributions](../../../../../../probability-distribution.md) give

$$
\mathbb E D_c=\mathbb E|X-c|-\mathbb E[\operatorname{sign}(Y-c)(Y-c)]=\mathbb E|X-c|-\mathbb E|Y-c|=0.
$$

Thus $D_c=0$ [almost surely](../../../../../../almost-sure-convergence.md). On $\{Y>c\}$ this forces $X\geq c$; on $\{Y<c\}$ it forces $X\leq c$; on $\{Y=c\}$ it forces $X=c$. In particular $\{Y=c\}\subseteq\{X=c\}$ up to a null set. These two [events](../../../../../../event.md) have equal [probability](../../../../../../probability.md), again by equality of the [probability distributions](../../../../../../probability-distribution.md), so they agree up to a null set. Consequently

$$
\operatorname{sign}(X-c)=\operatorname{sign}(Y-c)\quad\text{almost surely}.
$$

Taking $c=0$ establishes the suggested sign assertion, but this alone would not exclude unequal positive values. Apply the same argument simultaneously to the [countable](../../../../../../countable-set.md) set of rational $c$. Outside the union of their null sets, unequal $X$ and $Y$ would have a rational strictly between them, giving opposite signs. This proves the [conditional expectation preserving a distribution](../../../../../../conditional-expectation-preserving-a-distribution.md) result:

$$
\boxed{X=\mathbb E[X\mid\mathcal G]\quad\text{almost surely}.}
$$

Only [integrability](../../../../../../integrability.md) was used; no finite second moment or hidden square-integrability assumption is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
