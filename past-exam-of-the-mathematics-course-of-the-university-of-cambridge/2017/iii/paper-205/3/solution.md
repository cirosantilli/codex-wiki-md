<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $R$ denote the number of rejected [null hypotheses](../../../../../null-hypothesis.md) and $V$ the number of rejected true [null hypotheses](../../../../../null-hypothesis.md). The [familywise error rate](../../../../../familywise-error-rate.md) is $\Pr(V\ge1)$, whereas the [false discovery rate](../../../../../false-discovery-rate.md) is $\mathbb E[V/(R\vee1)]$, with a zero contribution when $R=0$. A valid true-null [p-value](../../../../../p-value.md) satisfies $\Pr(p_i\le t)\le t$ for $0\le t\le1$.

For the [closed testing procedure](../../../../../closed-testing-procedure.md), choose a level-$\alpha$ local test of every nonempty intersection $H_I=\bigcap_{i\in I}H_i$. Reject $H_i$ only if every intersection containing it is rejected by its local test. If any true [null hypothesis](../../../../../null-hypothesis.md) is rejected, the local test of $H_{I_0}$ must reject. Since that intersection is true, its rejection [probability](../../../../../probability.md) is at most $\alpha$. If $I_0$ is empty there can be no false rejection. This proves strong [closed-testing control of the familywise error rate](../../../../../closed-testing-control-of-the-familywise-error-rate.md), under arbitrary dependence, provided each local test is valid under its whole intersection null.

For the [Benjamini-Hochberg procedure](../../../../../benjamini-hochberg-procedure.md), order the [p-values](../../../../../p-value.md) and set

$$
R=\max\{r\in\{1,\ldots,m\}:p_{(r)}\le\alpha r/m\},
$$

with maximum zero if the set is empty; reject the first $R$ hypotheses. To prove its [false discovery rate](../../../../../false-discovery-rate.md) bound, fix a true-null index $i$. Replace $p_i$ by zero and let $R_i$ be the modified rejection count. This is a [function](../../../../../function-split.md) of the other [p-values](../../../../../p-value.md) and satisfies $R_i\ge1$.

The [Benjamini-Hochberg leave-one-out identity](../../../../../benjamini-hochberg-leave-one-out-identity.md) is

$$
\frac{\mathbf1\{i\text{ rejected}\}}{R\vee1}=\frac{\mathbf1\{p_i\le\alpha R_i/m\}}{R_i}.
$$

Here is its deterministic justification. If $i$ was rejected, lowering its value cannot decrease $R$, and leaves all ordered values of ranks greater than $R$ unchanged. No such rank can newly satisfy its threshold, so $R_i=R$. Conversely, if $R_i=r$ and $p_i\le\alpha r/m$, at least $r-1$ other values and $p_i$ are at most this threshold. Therefore the original procedure has $R\ge r$. Monotonicity under decreasing $p_i$ also gives $R\le R_i=r$, so $R=r$ and $i$ is rejected. This establishes the identity; harmless deterministic tie-breaking also covers the artificial zero introduced in the modified data.

The assumed [independence](../../../../../independent-random-variables.md) makes $p_i$ independent of $R_i$. Conditional on $R_i=r$, validity of the [p-value](../../../../../p-value.md) implies

$$
\mathbb E\left[\left.\frac{\mathbf1\{p_i\le\alpha R_i/m\}}{R_i}\right|R_i=r\right]\le\frac1r\frac{\alpha r}{m}=\frac\alpha m.
$$

Sum over $i\in I_0$ to obtain

$$
\boxed{\operatorname{FDR}\le\frac{m_0}{m}\alpha\le\alpha.}
$$

If true-null [p-values](../../../../../p-value.md) are exactly uniform rather than merely valid, the first inequality is equality. No restriction on dependence among the false-null [p-values](../../../../../p-value.md) is needed beyond their joint independence from the true-null values.

For the requested [Simes inequality](../../../../../simes-inequality.md), apply this result to the $m_0$ true-null [p-values](../../../../../p-value.md) alone, for $m_0>0$. Every rejection is now false, so $V=R$ and the [false discovery rate](../../../../../false-discovery-rate.md) is the [probability](../../../../../probability.md) of any rejection. The event of at least one [Benjamini-Hochberg procedure](../../../../../benjamini-hochberg-procedure.md) rejection is exactly

$$
\left\{\min_{1\le r\le m_0}\frac{p_{(r,I_0)}}r\le\frac\alpha{m_0}\right\}.
$$

Its [probability](../../../../../probability.md) is at most $\alpha$. This holds for $\alpha\in[0,1]$; with no true nulls the written minimum and division by $m_0$ are undefined and the error-control statement is instead vacuous.

The final step-up rule is the [Hochberg procedure](../../../../../hochberg-procedure.md). Use [Simes tests](../../../../../simes-test.md) as the local tests for a [closed testing procedure](../../../../../closed-testing-procedure.md): reject $H_I$ when $\min_r p_{(r,I)}/r\le\alpha/|I|$. Under any true intersection all its [p-values](../../../../../p-value.md) are valid and independent, so the [Simes inequality](../../../../../simes-inequality.md) proves level $\alpha$ for its local test. The implication supplied in the question says that whenever the [Hochberg procedure](../../../../../hochberg-procedure.md) rejects $H_{(i)}$, every intersection containing $(i)$ passes its local [Simes test](../../../../../simes-test.md). Thus every such rejection is also a closed-testing rejection. Consequently

$$
\boxed{\operatorname{FWER}(\text{Hochberg})\le\operatorname{FWER}(\text{closed Simes tests})\le\alpha.}
$$

The true-null [independence](../../../../../independent-random-variables.md) assumption is essential to this particular proof of local-test validity; the arbitrary-dependence guarantee of closed testing does not create valid local tests automatically.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
