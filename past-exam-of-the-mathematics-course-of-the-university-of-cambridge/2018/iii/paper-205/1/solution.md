<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Estimate the signal by [one-dimensional total variation denoising](../../../../../one-dimensional-total-variation-denoising.md), which penalizes adjacent differences rather than the constant level:

$$
\boxed{\widehat\mu_\lambda=\arg\min_{\mu\in\mathbb R^n}\left\{\frac1{2n}\|Y-\mu\|_2^2+\lambda\sum_{i=1}^{n-1}|\mu_{i+1}-\mu_i|\right\},\qquad\lambda>0.}
$$

This is a [fused Lasso](../../../../../fused-lasso.md) objective. Its [L1 norm](../../../../../l1-norm.md) penalty makes many adjacent differences exactly zero, producing a piecewise-constant fit. For [change-point detection](../../../../../change-point-detection.md), estimate the locations by $\widehat S=\{i:\widehat\mu_i\ne\widehat\mu_{i+1}\}$. The tuning parameter controls the strength of the penalty; it can be chosen, for example, using a validation criterion appropriate to the noise model.

For a general family of elementary nulls $H_1,\ldots,H_m$, the [closed testing procedure](../../../../../closed-testing-procedure.md) forms every nonempty intersection $H_B=\bigcap_{j\in B}H_j$ and gives it a local test of level $\alpha$. Reject $H_j$ precisely when all intersections with $j\in B$ are locally rejected. This gives strong control of the [familywise error rate](../../../../../familywise-error-rate.md): let $T_0$ be the indices of the true elementary nulls. If $T_0$ is empty there is no false rejection. Otherwise, rejecting any $H_j$ with $j\in T_0$ requires rejection of the true intersection $H_{T_0}$. Its local test has rejection probability at most $\alpha$, hence

$$
\boxed{\mathbb P(\text{at least one false rejection})\leq\alpha.}
$$

This proof of [closed-testing control of the familywise error rate](../../../../../closed-testing-control-of-the-familywise-error-rate.md) needs no independence of the tests.

For the interval procedure, a true tested interval is contained in one maximal constant block $B\in\mathcal T$. If $I\subseteq B$, the intervals over which $p_B$ takes its maximum are a subset of those used for $p_I$, so $p_I\geq p_B$. Therefore rejection of a true $I$ forces rejection of its containing block. Conversely, a rejected block is itself a rejected true null.

There is a small indexing issue in the PDF: its testing family excludes singleton intervals, while $\mathcal T$ may contain singleton blocks. Put $\mathcal T_* =\{B\in\mathcal T:|B|\geq2\}$. Every true tested interval lies in one of these blocks, so the exact statement, using only hypotheses defined in the paper, is

$$
\boxed{\{\text{some false rejection}\}=\bigcup_{B\in\mathcal T_*}\{p_B\leq\alpha\}.}
$$

Singleton blocks contain no eligible tested interval and can be ignored. Equivalently, one may define their nulls as never rejected.

For each $B\in\mathcal T_*$, the term $J=B$ occurs in the maximum defining $p_B$, giving $p_B\geq nq_B/|B|$. A valid [p-value](../../../../../p-value.md) is a [super-uniform random variable](../../../../../super-uniform-random-variable.md) under its null, so for $0\leq\alpha\leq1$,

$$
\mathbb P(p_B\leq\alpha)\leq\mathbb P\left(q_B\leq\frac{\alpha|B|}{n}\right)\leq\frac{\alpha|B|}{n}.
$$

The [union bound](../../../../../boole-s-inequality.md) and disjointness of the constant blocks now give

$$
\mathbb P(\text{some false rejection})\leq\frac\alpha n\sum_{B\in\mathcal T_*}|B|\leq\alpha,
\qquad
\boxed{\mathbb P(\text{no false rejections})\geq1-\alpha.}
$$

This establishes [weighted interval testing for a piecewise-constant mean](../../../../../weighted-interval-testing-for-a-piecewise-constant-mean.md) even when the interval p-values are dependent. Values $p_I>1$ do not affect rejection at levels at most one.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
