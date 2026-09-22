<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In a [second-price sealed-bid auction](../../../../../vickrey-auction.md), fix the other players' bids and let $a$ be their highest bid. A player of valuation $v$ who wins pays $a$, obtaining [quasilinear utility](../../../../../quasilinear-utility.md) $v-a$; losing gives zero. If $v>a$, winning is optimal and bidding $v$ wins. If $v<a$, losing is optimal and bidding $v$ loses. If $v=a$, winning and losing both give zero, regardless of the fixed tie-breaking rule. Thus truthful bidding is a [dominant strategy](../../../../../dominant-strategy.md). In particular **the profile in which every bidder bids its valuation is a Nash equilibrium**, for every valuation profile, not merely on average.

A [symmetric independent private values model](../../../../../symmetric-independent-private-values-model.md) gives each bidder a private valuation determined by its own type. The types are independent draws from a common distribution, and the bidders have identical roles and preferences. In the standard bidding calculation bidders are [risk-neutral](../../../../../risk-neutrality.md) with [quasilinear utility](../../../../../quasilinear-utility.md): they maximize expected valuation minus payment. Strategies map each bidder's privately observed value to a bid. Equilibrium in this incomplete-information setting means a [Bayesian Nash equilibrium](../../../../../bayesian-nash-equilibrium.md).

Take $n\geq2$ with independent uniform values on $[0,1]$. In a [first-price sealed-bid auction](../../../../../first-price-sealed-bid-auction.md), if all players bid their valuations, a type $v$ earns zero whenever it wins and zero whenever it loses. But for $v>0$, bidding $v/2$ instead yields positive [expected utility](../../../../../expected-utility.md)

$$
\left(v-\frac v2\right)\Pr\{\text{every opposing value}<v/2\}
=\frac v2\left(\frac v2\right)^{n-1}>0.
$$

Therefore **truthful first-price bidding is not an equilibrium**.

For the candidate [uniform private-value first-price bidding equilibrium](../../../../../uniform-private-value-first-price-bidding-equilibrium.md), put $\alpha=(n-1)/n$ and suppose every opponent bids $\alpha$ times its valuation. For a deviation $b\in[0,\alpha]$, winning means that every opposing value is less than $b/\alpha$. Independence gives winning [probability](../../../../../probability.md) $(b/\alpha)^{n-1}$, so the type-$v$ [expected utility](../../../../../expected-utility.md) is

$$
u(v,b)=(v-b)\left(\frac b\alpha\right)^{n-1}.
$$

For $b>0$ its derivative is

$$
\frac{\partial u}{\partial b}
=\frac{b^{n-2}}{\alpha^{n-1}}\bigl((n-1)v-nb\bigr).
$$

For $v>0$ it is positive before $b=\alpha v$ and negative after; for $v=0$, every positive bid has nonpositive utility and zero is optimal. Thus the maximum on $[0,\alpha]$ is $b=\alpha v$. A bid above $\alpha$ wins with [probability](../../../../../probability.md) one but gives $v-b\leq v-\alpha$, which is no better than the already considered endpoint $b=\alpha$, hence no better than $b=\alpha v$. Ties have [probability](../../../../../probability.md) zero under the continuous opposing distributions. All admissible deviations are therefore covered.

Each bidder's best response is the proposed rule, proving

$$
\boxed{\beta(v)=\frac{n-1}{n}v\quad\text{is a symmetric Bayesian Nash equilibrium}.}
$$

Its conditional [expected utility](../../../../../expected-utility.md) is $u(v,\alpha v)=v^n/n$. With only one bidder, bidding zero is optimal and agrees with the same formal rule; the derivative argument is needed only for $n\geq2$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
