<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [familywise error rate](../../../../../familywise-error-rate.md) is

$$
\operatorname{FWER}=\mathbb P(\text{at least one true null hypothesis is rejected}).
$$

The [Bonferroni correction](../../../../../bonferroni-correction.md) rejects $H_i$ when $p_i\leq\alpha/m$. Since a valid [p-value](../../../../../p-value.md) is [super-uniform](../../../../../super-uniform-random-variable.md) under its null, the [union bound](../../../../../boole-s-inequality.md) gives

$$
\operatorname{FWER}
\leq\sum_{i\in I_0}\mathbb P(p_i\leq\alpha/m)
\leq |I_0|\frac\alpha m\leq\alpha.
$$

**No independence assumption is needed.**

For the [closed testing procedure](../../../../../closed-testing-procedure.md), form the intersection hypothesis $H_I=\bigcap_{i\in I}H_i$ for every nonempty $I\subseteq\{1,\ldots,m\}$ and choose a level-$\alpha$ local test for each $H_I$. Reject $H_i$ exactly when every $H_I$ with $i\in I$ is rejected by its local test. If any true $H_i$ is rejected, then the intersection $H_{I_0}$ of all true nulls is rejected. Since its local test has [significance level](../../../../../significance-level.md) $\alpha$,

$$
\operatorname{FWER}\leq\mathbb P(H_{I_0}\text{ is rejected})\leq\alpha.
$$

This is the [closed-testing control of the familywise error rate](../../../../../closed-testing-control-of-the-familywise-error-rate.md).

Write $W=\sum_{j=1}^m w_j$. Procedure (A) is the [Weighted Bonferroni correction](../../../../../weighted-bonferroni-correction.md): it rejects $H_i$ when $p_i\leq\alpha w_i/W$. Therefore

$$
\operatorname{FWER}
\leq\sum_{i\in I_0}\frac{\alpha w_i}{W}
\leq\alpha.
$$

Procedure (B) is the [Weighted Holm step-down procedure](../../../../../weighted-holm-step-down-procedure.md). Let $k$ be the first rank in the ordering $q_{(1)}<\cdots<q_{(m)}$ whose hypothesis is a true null, and put $W_0=\sum_{i\in I_0}w_i$. If any true null is rejected, the procedure reaches step $k$ and

$$
q_{(k)}\leq\frac\alpha{\sum_{j=k}^m w_{(j)}}\leq\frac\alpha{W_0},
$$

because every true null remains among ranks $k,\ldots,m$. Hence

$$
\{\text{a true null is rejected}\}
\subseteq
\bigcup_{i\in I_0}\left\{p_i\leq\frac{\alpha w_i}{W_0}\right\},
$$

and another [union bound](../../../../../boole-s-inequality.md) gives FWER at most $\alpha$.

At step $k$, procedure (B) divides by the total weight still under consideration, which is no larger than $W$. Its critical values therefore increase as hypotheses are rejected. Moreover, if procedure (A) would reject a hypothesis, every earlier ordered $q$ also passes the initial threshold, so procedure (B) reaches and rejects it. Thus (B) contains every rejection of (A) and can make strictly more rejections while retaining the same strong FWER control.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
