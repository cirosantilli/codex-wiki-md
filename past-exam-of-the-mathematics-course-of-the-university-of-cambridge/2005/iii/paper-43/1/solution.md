<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Condition on the [claim count](../../../../../claim-count.md), defining the empty sum to be zero. [Independence](../../../../../independent-random-variables.md) gives $\mathbb E[S\mid N=k]=k\mathbb E X_1$. By the [law of total expectation](../../../../../law-of-total-expectation.md),

$$
\boxed{\mathbb ES=\mathbb EN\,\mathbb EX_1.}
$$

For nonnegative claims this also follows from [Tonelli theorem](../../../../../tonelli-theorem.md); for signed claims finite $\mathbb EN$ and $\mathbb E|X_1|$ ensure [integrability](../../../../../integrability.md). [Conditional independence](../../../../../conditional-independence.md) likewise gives

$$
\mathbb E[e^{tS}\mid N=k]=\prod_{j=1}^k\mathbb E[e^{tX_j}]=M_{X_1}(t)^k,
\qquad
\boxed{M_S(t)=G_N(M_{X_1}(t)).}
$$

This [random-sum transform identity](../../../../../random-sum-transform-identity.md) holds wherever the composed series is finite, or as an extended nonnegative [expectation](../../../../../expected-value.md). It is not permission to use an algebraic continuation outside the convergence domain.

For the zero-based [geometric distribution](../../../../../geometric-distribution.md), summing the [geometric series](../../../../../geometric-series.md) gives

$$
G_N(z)=\frac p{1-qz},\qquad \mathbb EN=G_N'(1)=\frac qp.
$$

The [exponential distribution](../../../../../exponential-distribution.md) of mean $\mu$ has $M_{X_1}(t)=(1-\mu t)^{-1}$ for $t<1/\mu$. Therefore

$$
\boxed{\mathbb ES=\frac{q\mu}p,\qquad
M_S(t)=\frac p{1-q/(1-\mu t)}
=\frac{p(1-\mu t)}{p-\mu t}\quad(t<p/\mu).}
$$

The stricter bound $t<p/\mu$ is necessary: the [geometric series](../../../../../geometric-series.md) requires $qM_{X_1}(t)<1$. At and above $p/\mu$ that series diverges; at and above $1/\mu$ even one claim has an infinite transform. Thus the displayed rational expression represents the [moment-generating function](../../../../../moment-generating-function.md) only on its stated domain.

Since all claims are strictly positive, $S=0$ exactly when $N=0$, so $\mathbb P(S=0)=p$. Splitting the transform gives

$$
M_S(t)=p+q\frac{p/\mu}{p/\mu-t}.
$$

Uniqueness of the [moment-generating function](../../../../../moment-generating-function.md) identifies a [mixture distribution](../../../../../mixture-distribution.md) with a zero atom of weight $p$ and an exponential positive component of weight $q$ and rate $p/\mu$. In particular,

$$
\boxed{\mathbb P(S=0)=p,\qquad f_S(x)=\frac{qp}{\mu}e^{-px/\mu}\quad(x>0).}
$$

The density integrates to $q$, not one. One can also verify it directly: conditional on $N=k\geq1$, the sum has [Erlang distribution](../../../../../erlang-distribution.md) density $x^{k-1}e^{-x/\mu}/[\mu^k(k-1)!]$. Multiplying by $pq^k$ and summing over $k$ gives $(pq/\mu)e^{-x/\mu}e^{qx/\mu}$, the same density. This is the [zero-based geometric sum of exponential variables](../../../../../zero-based-geometric-sum-of-exponential-variables.md).

Under [excess of loss reinsurance](../../../../../excess-of-loss-reinsurance.md), the ceded amount for each claim is $(X_j-M)_+$, and the monthly reduction is their [random sum](../../../../../random-sum.md). The [tail integral formula for moments](../../../../../tail-integral-formula-for-moments.md) gives

$$
\mathbb E(X_1-M)_+=\int_M^\infty\mathbb P(X_1>x)\,dx
=\mu e^{-M/\mu}.
$$

Conditioning on $N$ again yields

$$
\boxed{\mathbb E\sum_{j=1}^N(X_j-M)_+=\frac{q\mu}p e^{-M/\mu}.}
$$

The retained payment is $\sum_{j=1}^N\min(X_j,M)$; it is generally not $\min(S,M)$.

Under [aggregate stop loss reinsurance](../../../../../aggregate-stop-loss-reinsurance.md), the reduction is $(S-\widetilde M)_+$. The aggregate tail is $\mathbb P(S>x)=q e^{-px/\mu}$ for $x\geq0$, so

$$
\mathbb E(S-\widetilde M)_+=\int_{\widetilde M}^\infty q e^{-px/\mu}\,dx
=\frac{q\mu}p e^{-p\widetilde M/\mu}.
$$

The prefactor is positive. Equality with the per-claim recovery is equivalent to $p\widetilde M=M$, giving the unique [reinsurance retention](../../../../../reinsurance-retention.md)

$$
\boxed{\widetilde M=\frac Mp.}
$$

This is the relation for [equal expected recoveries from excess of loss and stop loss](../../../../../equal-expected-recoveries-from-excess-of-loss-and-stop-loss.md); since $p<1$, the aggregate [reinsurance retention](../../../../../reinsurance-retention.md) exceeds the individual [reinsurance retention](../../../../../reinsurance-retention.md). These are reductions in claim payouts, before any reinsurance premium is deducted.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
