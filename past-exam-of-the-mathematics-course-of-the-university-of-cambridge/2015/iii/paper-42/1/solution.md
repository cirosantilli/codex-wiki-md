<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the usual [independent private values model](../../../../../independent-private-values-model.md), [quasilinear utility](../../../../../quasilinear-utility.md), and voluntary participation with zero outside utility. These assumptions matter: without [individual rationality](../../../../../individual-rationality.md), arbitrary type-independent entry charges make revenue unbounded, and correlated types cannot in general be described by their marginal priors alone.

The [revelation principle](../../../../../revelation-principle.md) lets us optimize over [direct revelation mechanisms](../../../../../direct-revelation-mechanism.md) satisfying [Bayesian incentive compatibility](../../../../../bayesian-incentive-compatibility.md). Write $x(v)\in[0,1]$ for the common project allocation, $X_i(t)=\mathbb E_{V_{-i}}x(t,V_{-i})$ for player $i$'s interim allocation, and $P_i(t)$ for its interim payment. The [interim payment identity](../../../../../interim-payment-identity.md) gives

$$
P_i(t)=tX_i(t)-\int_{\underline v_i}^tX_i(s)ds-U_i(\underline v_i).
$$

Since [interim individual rationality](../../../../../interim-individual-rationality.md) requires $U_i(\underline v_i)\geq0$, the [virtual-surplus revenue identity](../../../../../virtual-surplus-revenue-identity.md) bounds expected revenue by

$$
\mathbb E\sum_iP_i(V_i)\leq\mathbb E\left[x(V)\sum_i\phi_i(V_i)\right],
\qquad\phi_i(t)=t-\frac{1-F_i(t)}{f_i(t)}.
$$

The best feasible common allocation at each valuation profile therefore provides the project when total [virtual surplus](../../../../../virtual-surplus.md) is nonnegative:

$$
\boxed{x^*(v)=\mathbf1_{\{\sum_i\phi_i(v_i)\geq0\}}.}
$$

Because each [regular prior](../../../../../regular-distribution-economics.md) has a nondecreasing [virtual valuation](../../../../../virtual-valuation.md), this allocation is a [nondecreasing function](../../../../../nondecreasing-function.md) of each player's report. Hold $v_{-i}$ fixed and charge the [critical-value payment](../../../../../critical-value-payment.md)

$$
p_i^*(v)=v_i x^*(v)-\int_{\underline v_i}^{v_i}x^*(t,v_{-i})dt.
$$

This is the winning threshold when it lies in the support, the lowest allowed value if every type wins, and zero if the player loses. A truthful winner never pays more than its value; a losing type cannot profit by crossing the threshold. Thus the mechanism has [dominant-strategy incentive compatibility](../../../../../dominant-strategy-incentive-compatibility.md) and [ex post individual rationality](../../../../../ex-post-individual-rationality.md), with zero utility at every lowest type. It attains the revenue bound, proving optimality even among mechanisms requiring only [Bayesian incentive compatibility](../../../../../bayesian-incentive-compatibility.md). At a zero-virtual-surplus tie, choose any fixed rule that preserves monotonicity.

For independent [uniform distributions](../../../../../continuous-uniform-distribution.md) on $[0,1]$, the [virtual valuations](../../../../../virtual-valuation.md) are $\phi_i(v_i)=2v_i-1$. The [revenue-optimal public-project auction](../../../../../revenue-optimal-public-project-auction.md) becomes

$$
\boxed{\text{Provide the project exactly when }\sum_i v_i\geq\frac n2.}
$$

When it is provided, player $i$ pays

$$
\boxed{p_i^*(v)=\max\left\{0,\frac n2-\sum_{j\ne i}v_j\right\};}
$$

otherwise every payment is zero. If the displayed threshold exceeds one, player $i$ cannot induce provision within its allowed support; if it is negative, provision is independent of its own report and its payment is zero. For $n=1$, this specializes to a reserve value and payment of $1/2$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
