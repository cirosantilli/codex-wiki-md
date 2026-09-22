<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [simple predictable process](../../../../../simple-predictable-process.md) can be written

$$
H_s=\sum_{j=0}^{m-1}\xi_j\mathbf1_{(t_j,t_{j+1}]}(s),\qquad 0=t_0<t_1<\cdots<t_m\le\infty,
$$

where each $\xi_j$ is bounded and $\mathcal F_{t_j}$-measurable. Define its integral to start at zero:

$$
(H\mathbin\cdot M)_t=\sum_{j=0}^{m-1}\xi_j(M_{t\wedge t_{j+1}}-M_{t\wedge t_j}).
$$

Refining the partition leaves this sum unchanged. Every summand is a [martingale](../../../../../martingale-split.md), by conditioning its future increment on the information at $t_j$. Bounded coefficients and the $L^2$ bound on $M$ make the integral an [L2-bounded continuous martingale](../../../../../l2-bounded-continuous-martingale.md). Its terminal value is the same sum with $M_\infty$ substituted at any infinite endpoint; $L^2$ [martingale](../../../../../martingale-split.md) convergence supplies this limit.

We need the conditional square identity, rather than assuming [independent](../../../../../independent-random-variables.md) increments. The [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md) gives $\mathbb E\sup_t|M_t|^2<\infty$. Localize the square identity for $M^2-[M]$ at level and bracket [stopping times](../../../../../stopping-time.md). The stopped identity and this maximal bound give $\mathbb E[M]_\infty<\infty$ by [monotone convergence](../../../../../monotone-convergence-theorem.md). Now

$$
\sup_t|M_t^2-[M]_t|\le\sup_t|M_t|^2+[M]_\infty
$$

is [integrable](../../../../../integrability.md), so [localization](../../../../../localization-of-a-ring.md) passes to conditional [expectations](../../../../../expected-value.md) and $M^2-[M]$ is a [uniformly integrable martingale](../../../../../uniformly-integrable-martingale.md). Expanding a squared increment and using $\mathbb E(M_t\mid\mathcal F_s)=M_s$ proves

$$
\mathbb E((M_t-M_s)^2\mid\mathcal F_s)=\mathbb E([M]_t-[M]_s\mid\mathcal F_s),\qquad s\le t\le\infty.
$$

The infinite endpoint follows from $L^2$ convergence and [integrability](../../../../../integrability.md) of the bracket. The initial value $M_0$ need not be zero: the integral itself is zero-starting.

In the square of the terminal integral, all cross terms vanish. For $j<k$, the $j$th increment and both coefficients in its cross term are measurable at $t_k$, whereas the conditional mean of the $k$th increment there is zero. For the diagonal terms, the preceding conditional identity can be multiplied by the bounded $\xi_j^2$. Therefore

$$
\begin{aligned}
\mathbb E(H\mathbin\cdot M)_\infty^2
&=\sum_j\mathbb E\bigl[\xi_j^2(M_{t_{j+1}}-M_{t_j})^2\bigr]\\
&=\sum_j\mathbb E\bigl[\xi_j^2([M]_{t_{j+1}}-[M]_{t_j})\bigr]
=\boxed{\mathbb E(H^2\mathbin\cdot[M])_\infty}.
\end{aligned}
$$

This proves the [Itô isometry](../../../../../ito-isometry.md) for these simple integrands. Ordered stopping-time intervals also work, replacing the conditional identity by [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md), but deterministic intervals suffice for the approximation requested here.

For that approximation, put $\mu(A)=\mathbb E\int_0^1\mathbf1_A(\omega,s)ds$ on the [predictable sigma-algebra](../../../../../predictable-sigma-algebra.md). This is a [finite measure](../../../../../finite-measure.md). That [sigma-algebra](../../../../../sigma-algebra.md) is generated, apart from the zero-time slice of measure zero, by rectangles $A\times(s,t]$ with $A\in\mathcal F_s$. The indicator of every such rectangle is a bounded [simple predictable process](../../../../../simple-predictable-process.md).

Here is a density proof. Let $V$ be the closed linear span of these indicators in $L^2(\mu)$, and let $\mathcal D$ contain the [predictable](../../../../../predictable-process.md) sets whose indicators belong to $V$. The whole space belongs to $\mathcal D$; complements stay in $\mathcal D$; and disjoint countable unions do also, because their finite partial indicator sums converge in $L^2$ under the [finite measure](../../../../../finite-measure.md). Thus $\mathcal D$ is a [Dynkin system](../../../../../dynkin-system.md) containing the generating rectangle [pi-system](../../../../../pi-system.md). The [Pi-lambda theorem](../../../../../pi-lambda-theorem.md) makes it the entire [predictable sigma-algebra](../../../../../predictable-sigma-algebra.md). Bounded [predictable](../../../../../predictable-process.md) simple functions therefore belong to $V$. Truncating any $L^2(\mu)$ function and then approximating its truncated range by finitely many levels shows that every such function belongs to $V$. A finite sum of rectangle indicators can be rewritten on one common deterministic time partition, with the coefficient on each interval measurable at its left endpoint; it is exactly an allowed simple process.

Consequently choose $H^n$ of this form with $\|H^n-H\|_{L^2(\mu)}<1/n$. This proves

$$
\boxed{\mathbb E\int_0^1|H_s^n-H_s|^2ds\longrightarrow0.}
$$

It is [density of simple predictable processes for finite measures](../../../../../density-of-simple-predictable-processes-for-finite-measures.md), with a proof of the actual approximation step.

Finally apply the preceding isometry to $M_t=B_{t\wedge1}$, whose bracket is $t\wedge1$. The elementary integrals $I_n=\int_0^1H_s^n dB_s$ satisfy

$$
\mathbb E|I_n-I_m|^2=\mathbb E\int_0^1|H_s^n-H_s^m|^2ds\longrightarrow0.
$$

**Define the [Itô integral](../../../../../ito-integral.md) as the $L^2$ limit of these elementary integrals.** The same identity shows [independence](../../../../../independent-random-variables.md) of the approximating sequence, linearity, mean zero, and $\mathbb E(\int_0^1H_s dB_s)^2=\mathbb E\int_0^1H_s^2ds$. Applying the Doob inequality to the difference processes also gives uniform-in-time $L^2$ convergence on $[0,1]$, with a continuous [martingale](../../../../../martingale-split.md) version of the integral.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
