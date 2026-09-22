<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [familywise error rate](../../../../../familywise-error-rate.md) is the probability of rejecting at least one true null:

$$
\boxed{\operatorname{FWER}=\mathbb P\left(\bigcup_{i\in I_0}\{H_i\text{ is rejected}\}\right).}
$$

A valid [p-value](../../../../../p-value.md) is [super-uniform](../../../../../super-uniform-random-variable.md) under its null: $\mathbb P(p_i\leq t)\leq t$ for $0\leq t\leq1$. The [Bonferroni correction](../../../../../bonferroni-correction.md) rejects $H_i$ if $p_i\leq\alpha/m$. The [union bound](../../../../../boole-s-inequality.md) gives

$$
\operatorname{FWER}\leq\sum_{i\in I_0}\mathbb P(p_i\leq\alpha/m)\leq\frac{|I_0|}{m}\alpha\leq\alpha.
$$

This controls the [familywise error rate](../../../../../familywise-error-rate.md) for every configuration of true and false nulls, without any independence assumption on the [p-values](../../../../../p-value.md).

For a nonempty index set $I\subseteq\{1,\ldots,m\}$, the [intersection hypothesis](../../../../../intersection-hypothesis.md) $H_I=\bigcap_{i\in I}H_i$ asserts that every null indexed by $I$ holds. The [closure of a family of statistical hypotheses](../../../../../closure-of-a-family-of-statistical-hypotheses.md) consists of all these nonempty intersections, including the original hypotheses. For each intersection choose a local test $\phi_I$ of size at most $\alpha$ under $H_I$. Such tests always exist: for example, within $I$ use the [Bonferroni correction](../../../../../bonferroni-correction.md), rejecting $H_I$ if $\min_{i\in I}p_i\leq\alpha/|I|$. More powerful local intersection tests can be substituted whenever valid.

The [closed testing procedure](../../../../../closed-testing-procedure.md) rejects an elementary hypothesis $H_i$ only when every local test $\phi_I$ with $i\in I$ rejects its intersection hypothesis. If $I_0\ne\varnothing$, the intersection $H_{I_0}$ is true. Rejecting any true $H_i$ requires rejection by its local test $\phi_{I_0}$, so

$$
\boxed{\operatorname{FWER}\leq\mathbb P(\phi_{I_0}=1)\leq\alpha.}
$$

If $I_0=\varnothing$, there is no possible false rejection. This proves [closed-testing control of the familywise error rate](../../../../../closed-testing-control-of-the-familywise-error-rate.md). The same argument applies if [intersection hypotheses](../../../../../intersection-hypothesis.md) themselves are reported as rejected: requiring all their supersets to reject includes $I_0$ whenever the reported intersection is true.

Finally, consider the given hierarchical family as a [laminar family of sets](../../../../../laminar-family-of-sets.md). Call a set $I\in\mathcal I$ true when $I\subseteq I_0$, so its entire [intersection hypothesis](../../../../../intersection-hypothesis.md) is true. Let $\mathcal M$ be the inclusion-maximal true sets in $\mathcal I$. Distinct members of $\mathcal M$ are disjoint: if they met, laminarity would make one contain the other, contradicting maximality. Consequently,

$$
\sum_{J\in\mathcal M}|J|\leq|I_0|\leq m.
$$

Every true set $I$ lies in a maximal true $J$. If $H_I$ is rejected by the prescribed adjusted [p-value](../../../../../p-value.md) rule, the maximum over its ancestors includes $J$, hence

$$
p_J\leq\frac{\alpha|J|}{m}.
$$

Thus the event of any false rejection is contained in the union of these events over the disjoint maximal true sets. Using validity of each $p_J$ under its true intersection and the [union bound](../../../../../boole-s-inequality.md),

$$
\boxed{\mathbb P(\text{at least one false rejection})
\leq\sum_{J\in\mathcal M}\frac{\alpha|J|}{m}\leq\alpha.}
$$

Equivalently, with probability at least $1-\alpha$ every rejection is correct. This proves [familywise error control for a laminar hypothesis family](../../../../../familywise-error-control-for-a-laminar-hypothesis-family.md). It requires neither independence nor the presence of all possible intersections or singletons in $\mathcal I$. Empty index sets are excluded, as required by the denominator $|J|$; if there are no true sets the result is immediate. Adjusted values exceeding one can be truncated at one without changing decisions for $\alpha<1$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
