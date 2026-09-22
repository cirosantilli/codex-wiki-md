<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $u_i$ denote player $i$'s expected [payoff](../../../../../payoff.md), so the definition also covers [mixed strategies](../../../../../mixed-strategy.md). If $p_i^*$ is a [dominant strategy](../../../../../dominant-strategy.md), then

$$
u_i(p_i^*,p_{-i})\geq u_i(q_i,p_{-i})
$$

for every opponents' profile $p_{-i}$ and every alternative $q_i$. In particular this holds at $p_{-i}=p_{-i}^*$. Thus no player can improve its [payoff](../../../../../payoff.md) by a unilateral deviation from $(p_1^*,\ldots,p_n^*)$, which is exactly the definition of a [Nash equilibrium](../../../../../nash-equilibrium.md). **A profile of [dominant strategies](../../../../../dominant-strategy.md) is a [Nash equilibrium](../../../../../nash-equilibrium.md).**

For the [second-price sealed-bid auction](../../../../../vickrey-auction.md), use the usual [private-value auction](../../../../../private-value-auction.md) assumptions: a bidder with value $v$ has [quasilinear utility](../../../../../quasilinear-utility.md) $v$ minus its payment if it wins, and zero if it loses. Fix the highest opposing bid $h$. If $h<v$, winning gives $v-h>0$, and bidding $v$ wins. If $h>v$, winning gives $v-h<0$, and bidding $v$ loses. If $h=v$, winning or losing gives zero, irrespective of the tie rule. Any other bid can only change whether the bidder wins, not the payment $h$ conditional on winning. It therefore cannot improve on the truthful bid in any of these cases. Hence **bidding the true value is a weakly [dominant strategy](../../../../../dominant-strategy.md)**. Neither symmetry nor independence of the opposing values is needed for this argument.

For part (a), in a [first-price sealed-bid auction](../../../../../first-price-sealed-bid-auction.md) with $n\geq2$, continuous nonnegative bids and $v>0$, no fixed bid is a [dominant strategy](../../../../../dominant-strategy.md). A positive bid $b$ can be improved against opponents all bidding zero: replace it by $b/2>0$, still win, and increase the [payoff](../../../../../payoff.md) by $b/2$. Bid zero can be improved against an opposing highest bid $h=v/2$: bidding $3v/4$ wins and earns $v/4>0$, whereas zero loses. This proves the [no dominant positive-value bid in a first-price auction](../../../../../no-dominant-positive-value-bid-in-a-first-price-auction.md) result.

Allowing [mixed strategies](../../../../../mixed-strategy.md) does not change that conclusion. Against all-zero opponents, a random bid has expected [payoff](../../../../../payoff.md) strictly below $v$ unless it is always zero and the tie rule awards this bidder the item with certainty. Any positive bid incurs a strictly positive payment, and any [probability](../../../../../probability.md) of losing at zero also reduces the [payoff](../../../../../payoff.md) below $v$. In the strict case choose a sufficiently small positive fixed bid $\delta$ so that $v-\delta$ exceeds the random bid's expected [payoff](../../../../../payoff.md). In the exceptional case the preceding deviation against $h=v/2$ still improves it. The assumptions matter: for value zero, bid zero is weakly dominant; with only one bidder it is also optimal. Consequently **there is no [dominant strategy](../../../../../dominant-strategy.md) for a positive-value bidder in the standard first-price setting**.

Part (b)'s printed nonexistence request is false under the stated [symmetric independent private values model](../../../../../symmetric-independent-private-values-model.md). Lack of a [dominant strategy](../../../../../dominant-strategy.md) does not imply lack of a [Nash equilibrium](../../../../../nash-equilibrium.md). For incomplete private information the appropriate equilibrium is a [Bayesian Nash equilibrium](../../../../../bayesian-nash-equilibrium.md), a [Nash equilibrium](../../../../../nash-equilibrium.md) of the game whose strategies are bidding rules as functions of private values. Here is an explicit counterexample with a full deviation check.

Let the $n\geq2$ [risk-neutral](../../../../../risk-neutrality.md) bidders have independent valuations with the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $[0,1]$, and put $a=(n-1)/n$. Suppose every opponent bids $\beta(w)=aw$. A bidder with value $v$ who bids $b\in[0,a]$ wins with [probability](../../../../../probability.md) $(b/a)^{n-1}$, since the opposing values must all be below $b/a$. Ties have [probability](../../../../../probability.md) zero, including at either endpoint. Its expected [quasilinear utility](../../../../../quasilinear-utility.md) is

$$
U_v(b)=(v-b)(b/a)^{n-1}.
$$

For $b>0$,

$$
U_v'(b)=a^{-(n-1)}b^{n-2}\bigl((n-1)v-nb\bigr).
$$

Thus $U_v$ increases up to $b=av$ and decreases thereafter. For $v=0$, bid zero is optimal directly. A bid above $a$ wins with certainty and pays more than bidding $a$, so it cannot improve on the maximum already found in $[0,a]$. A randomized bid is a mixture of these [payoffs](../../../../../payoff.md) and also cannot improve on their maximum. The [best response](../../../../../best-response.md) for every value is therefore the proposed bidding rule itself. This proves the [uniform private-value first-price bidding equilibrium](../../../../../uniform-private-value-first-price-bidding-equilibrium.md):

$$
\boxed{\beta(v)=\frac{n-1}{n}v\quad\text{is a symmetric Bayesian Nash equilibrium}.}
$$

The value-$v$ expected equilibrium [payoff](../../../../../payoff.md) is $v^n/n$. The bidding rule is a [pure strategy](../../../../../pure-strategy.md) in the Bayesian game, even though values are random. Therefore **the requested general nonexistence claim in (b) has a counterexample**, rather than a valid proof. The defect is present in the original PDF, not introduced by the converted text.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
