<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interpret the contests as standard [all-pay auctions](../../../../../all-pay-auction.md): the highest effort among entrants wins, ties are shared uniformly, and an unentered contest awards no prize. The printed question does not specify a [prize allocation rule](../../../../../prize-allocation-rule.md); the highest-effort convention is the one used for standard all-pay contests in [the course author's 2014 lecture slides](https://www.slideshare.net/slideshow/crowdsourding-and-allpay-contests/41832099). Under this convention, we can characterize the unique symmetric participation probabilities and bid marginals. Uniqueness of the entire joint [mixed strategy](../../../../../mixed-strategy.md) requires a further restriction on dependence, as explained below.

Let $q_j$ be the probability that a player omits contest $j$. Since every player enters exactly two contests, $q_1+q_2+q_3=1$. Let $G_j(b)$ be the probability that a rival is absent from contest $j$ or enters it with effort at most $b$. Rivals' strategy draws are independent between players. For a positive bid $b$ outside a [measure atom](../../../../../atom-measure-theory.md), the expected payoff from this contest is

$$
w_jG_j(b)^{n-1}-b.
$$

An [all-pay auction](../../../../../all-pay-auction.md) cannot have a positive-effort [measure atom](../../../../../atom-measure-theory.md) in a symmetric equilibrium: slightly overbidding that [measure atom](../../../../../atom-measure-theory.md) gives a positive discrete increase in the [winning probability](../../../../../winning-probability.md) at an arbitrarily small extra cost. Nor can active bids have a [measure atom](../../../../../atom-measure-theory.md) at zero when entry has positive probability, because a small positive bid beats tied zero bids. Gaps inside the active [effort support](../../../../../effort-support.md) are impossible: moving a bid from the top of a gap to just above its bottom preserves its winning probability and lowers its cost. The [effort support](../../../../../effort-support.md) starts at zero, because lowering its positive lower endpoint would preserve the chance that every rival is absent.

The [all-pay indifference equation with random entry](../../../../../all-pay-indifference-equation-with-random-entry.md) consequently gives the maximal per-contest payoff

$$
u_j=w_jq_j^{n-1},\qquad
G_j(b)=\left(\frac{b+u_j}{w_j}\right)^{1/(n-1)},
\quad0\leq b\leq w_j-u_j.
$$

Every $q_j$ lies strictly between zero and one. First, if $q_j=1$, the other two contests have certain entry and zero per-contest payoff, while deviating into the unused contest wins a positive prize. This contradicts equilibrium. Next, if $q_j=0$, the remaining omission probabilities sum to one and neither can equal one, so both are positive. Contest $j$ has zero per-contest payoff, whereas both other contests have strictly positive payoffs. Every pair containing $j$ is then worse than omitting it and entering the other two, contradicting certain entry in $j$.

Every omission therefore occurs with positive probability. The three entered pairs must give the same maximal payoff, which forces $u_1=u_2=u_3=u>0$. Normalizing the omission probabilities gives the [two-of-three all-pay participation equilibrium](../../../../../two-of-three-all-pay-participation-equilibrium.md):

$$
\boxed{u=\left(\sum_{\ell=1}^3w_\ell^{-1/(n-1)}\right)^{-(n-1)},\qquad
q_j=\left(\frac u{w_j}\right)^{1/(n-1)}
=\frac{w_j^{-1/(n-1)}}{\sum_{\ell=1}^3w_\ell^{-1/(n-1)}}.}
$$

Conditional on entering contest $j$, the effort has [distribution function](../../../../../cumulative-distribution-function.md)

$$
\boxed{H_j(b)=\frac{((b+u)/w_j)^{1/(n-1)}-q_j}{1-q_j},
\quad0\leq b\leq w_j-u,}
$$

extended by zero below this interval and one above it. The inequalities $q_1\leq q_2\leq q_3$ show that the larger prizes are entered more often.

To construct an equilibrium, omit $j$ with probability $q_j$, then draw the two active efforts independently with their respective [conditional distributions](../../../../../conditional-distribution.md) $H_k$. Every bid in a contest's [effort support](../../../../../effort-support.md) earns $u$; a bid above $w_j-u$ earns at most $w_j-b<u$. Thus no effort deviation or choice of a different pair improves on total payoff $2u$. This proves existence and verifies the [Nash equilibrium](../../../../../nash-equilibrium.md) without relying only on the indifference equations. The arguments above also prove uniqueness of the omission probabilities and the per-contest [marginal distributions](../../../../../marginal-distribution.md).

<a id="3/image-equilibrium-omission-probabilities-and-conditional-effort-distributions-for-three-all-pay-contests"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-42-entry-and-effort.png)

**[Figure 1](#3/image-equilibrium-omission-probabilities-and-conditional-effort-distributions-for-three-all-pay-contests). Equilibrium omission probabilities and conditional effort distributions for three all-pay contests**.

For the full joint strategy law, however, the printed uniqueness claim is too strong. Given an entered pair $k,\ell$, either use two independent [uniform random variables](../../../../../uniform-random-variable.md) $U,V$ and bids $(H_k^{-1}(U),H_\ell^{-1}(V))$, or use a single uniform $U$ and bids $(H_k^{-1}(U),H_\ell^{-1}(U))$. These are different [copulas](../../../../../copula-probability-theory.md) with the same conditional marginals. A fixed deviation's expected additive payoff only uses the rivals' per-contest [marginal distributions](../../../../../marginal-distribution.md), so both constructions remain [Nash equilibria](../../../../../nash-equilibrium.md). This is the [marginal-equivalent equilibria in additive contests](../../../../../marginal-equivalent-equilibria-in-additive-contests.md) phenomenon. **The participation probabilities and bid marginals are unique; the full joint mixed strategy is not unique unless a dependence convention is imposed.** Independent conditional sampling gives one canonical representative.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
