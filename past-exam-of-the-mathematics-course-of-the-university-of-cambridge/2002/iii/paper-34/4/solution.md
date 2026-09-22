<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [transferable utility game](../../../../../transferable-utility-game.md) on player set $N$, its [characteristic function of a coalitional game](../../../../../characteristic-function-of-a-coalitional-game.md) is $v:2^N\to\mathbb R$, where $v(S)$ is the maximum transferable surplus attainable by [coalition](../../../../../coalition-game-theory.md) $S$ and $v(\varnothing)=0$. An [imputation](../../../../../imputation-in-a-coalitional-game.md) is a payoff vector satisfying efficiency $\sum_{i\in N}x_i=v(N)$ and individual rationality $x_i\ge v(\{i\})$. The [core of a cooperative game](../../../../../core-game-theory.md) consists of the efficient payoff vectors satisfying

$$
\sum_{i\in S}x_i\ge v(S)\quad\text{for every coalition }S.
$$

These conditions prevent any [coalition](../../../../../coalition-game-theory.md) from blocking the allocation; singleton constraints include individual rationality.

The [Shapley value](../../../../../shapley-value.md) payoff is

$$
\phi_i(v)=\sum_{S\subseteq N\setminus\{i\}}
\frac{|S|!(n-|S|-1)!}{n!}\,[v(S\cup\{i\})-v(S)].
$$

Equivalently, it is the expected [marginal contribution](../../../../../marginal-contribution.md) of player $i$ when the players arrive in uniformly random order. The factorial weight counts the orders with exactly $S$ preceding $i$. Summing [marginal contributions](../../../../../marginal-contribution.md) telescopes along each order, proving Shapley efficiency.

In the four-player market a [coalition](../../../../../coalition-game-theory.md) creates one unit of surplus exactly when it contains the seller and at least one buyer. Thus

$$
\boxed{v(S)=\begin{cases}1,&1\in S\text{ and }S\cap\{2,3,4\}\ne\varnothing,\\0,&\text{otherwise}.\end{cases}}
$$

All singleton values are zero and $v(N)=1$. Core constraints for the pairs $\{1,j\}$ require $x_1+x_j\ge1$ for every buyer $j$. Since all payoffs are nonnegative and sum to one, the other two buyers' payoffs must be zero for each such pair. Therefore every buyer receives zero and the seller receives one. This vector satisfies all [coalition](../../../../../coalition-game-theory.md) inequalities, so

$$
\boxed{\operatorname{Core}(v)=\{(1,0,0,0)\}.}
$$

The seller's [marginal contribution](../../../../../marginal-contribution.md) is one unless he arrives before all three buyers, which happens with probability $1/4$. A given buyer contributes one exactly when the seller is first and that buyer is second, with probability $(1/4)(1/3)=1/12$. Hence

$$
\boxed{\phi(v)=\left(\frac34,\frac1{12},\frac1{12},\frac1{12}\right).}
$$

In particular the Shapley allocation need not lie in this market's core.

For the market with $k$ sellers and $3k$ buyers, a [coalition](../../../../../coalition-game-theory.md) containing $s$ sellers and $b$ buyers can make precisely $\min(s,b)$ trades, each producing unit surplus. Thus $v(S)=\min(s(S),b(S))$ and $v(N)=k$. Let $s_k$ and $b_k$ denote the common Shapley payoffs within the two roles. Role symmetry and the telescoping efficiency identity give

$$
s_k+3b_k=1.
$$

It remains to prove $s_k\to1$, rather than infer it only from competitive intuition.

Generate a uniformly random arrival order by giving every player an independent uniform time in $[0,1]$. Conditional on a specified seller's arrival time $t$, the number $B$ of preceding buyers and number $S$ of preceding other sellers are independent, with

$$
B\sim\operatorname{Bin}(3k,t),\qquad S\sim\operatorname{Bin}(k-1,t).
$$

The seller adds a trade precisely when $B>S$. Consequently

$$
s_k=\int_0^1\Pr(B>S\mid t)\,dt.
$$

For $t>0$, the difference $D=B-S$ has [mean](../../../../../expected-value.md) $(2k+1)t$ and [variance](../../../../../variance-split.md) $(4k-1)t(1-t)\le4kt$. By [Chebyshev's inequality](../../../../../chebyshev-inequality.md),

$$
\Pr(D\le0\mid t)\le\frac{4kt}{(2k+1)^2t^2}\le\frac1{kt}.
$$

Split the integral at $\delta=k^{-1/2}$. Using the trivial bound one on the first piece gives

$$
0\le1-s_k\le\delta+\int_\delta^1\frac{dt}{kt}
=\frac1{\sqrt k}+\frac{\log k}{2k}\longrightarrow0.
$$

This proves the [Shapley limit in a buyer-heavy exchange market](../../../../../shapley-limit-in-a-buyer-heavy-exchange-market.md). Since $b_k=(1-s_k)/3$, we conclude

$$
\boxed{s_k\longrightarrow1,\qquad b_k\longrightarrow0.}
$$

The proof accounts for sellers arriving very early, where a fixed-time concentration argument alone would not be uniform.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
