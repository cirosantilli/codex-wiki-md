<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [characteristic function of a coalitional game](../../../../../characteristic-function-of-a-coalitional-game.md) assigns each [coalition](../../../../../coalition-game-theory.md) $S\subseteq N$ its total attainable transferable payoff $v(S)$, with $v(\varnothing)=0$. In a [transferable utility game](../../../../../transferable-utility-game.md) the members may divide that total among themselves. This game-theoretic characteristic function is not the characteristic function of a [probability distribution](../../../../../probability-distribution.md).

The [Shapley value](../../../../../shapley-value.md) assigns to player $i$ the average [marginal contribution](../../../../../marginal-contribution.md) that player makes over all uniformly random orderings of the players. If $P_i^\pi$ is the predecessor set in ordering $\pi$, then

$$
\phi_i(v,N)=\frac1{n!}\sum_\pi\bigl(v(P_i^\pi\cup\{i\})-v(P_i^\pi)\bigr)
=\sum_{S\subseteq N\setminus\{i\}}\frac{|S|!(n-|S|-1)!}{n!}\bigl(v(S\cup\{i\})-v(S)\bigr).
$$

For any ordering, summing all contributions telescopes to $v(N)$, so the [Shapley value](../../../../../shapley-value.md) is efficient. It treats interchangeable players equally, pays a null player zero, and is additive in the characteristic function. These properties give its standard fairness axioms and uniquely characterize the [Shapley value](../../../../../shapley-value.md). The random-order interpretation explains why every position and predecessor [coalition](../../../../../coalition-game-theory.md) receives a principled weight rather than privileging a particular bargaining order.

For a [convex cooperative game](../../../../../convex-cooperative-game.md), couple a uniform ordering of $N$ with its restriction to $T$. The restricted ordering is uniform on $T$. For $i\in T$, the restricted predecessor set is $P_i^\pi\cap T\subseteq P_i^\pi$, so increasing [marginal contributions](../../../../../marginal-contribution.md) give

$$
v(P_i^\pi\cup\{i\})-v(P_i^\pi)
\geq v((P_i^\pi\cap T)\cup\{i\})-v(P_i^\pi\cap T).
$$

Averaging proves [Shapley population monotonicity in a convex game](../../../../../shapley-population-monotonicity-in-a-convex-game.md):

$$
\boxed{\phi_i(v,N)\geq\phi_i(v,T)\qquad(i\in T).}
$$

The comparison is meaningful for players who participate in the restricted game; no restricted value is defined for a player outside $T$. Summing over $i\in T$ and applying efficiency in that restricted game gives

$$
\sum_{i\in T}\phi_i(v,N)\geq\sum_{i\in T}\phi_i(v,T)=v(T).
$$

Together with efficiency for $N$, these are exactly the [core of a cooperative game](../../../../../core-game-theory.md) inequalities. Hence **the [Shapley value](../../../../../shapley-value.md) belongs to the core of a convex game**. This proves the requested stability, not just individual rationality.

Now label the entrepreneur by $0$ and the $n\geq1$ workers by $1,\ldots,n$. A [coalition](../../../../../coalition-game-theory.md) without the entrepreneur has value zero; one containing the entrepreneur and $k$ workers has value $p(k)$. Workers are interchangeable, so their [Shapley values](../../../../../shapley-value.md) agree. Fix one worker. Their contribution is zero if the entrepreneur appears after them. If the entrepreneur and exactly $k$ of the other $n-1$ workers appear before them, it is $p(k+1)-p(k)$. For a fixed choice of those workers, the $k+1$ predecessors can be ordered in $(k+1)!$ ways and the remaining $n-k-1$ successors in $(n-k-1)!$ ways. Therefore the [probability](../../../../../probability.md) of this event, summing over the $\binom{n-1}{k}$ predecessor choices, is

$$
\binom{n-1}{k}\frac{(k+1)!(n-k-1)!}{(n+1)!}
=\frac{k+1}{n(n+1)}.
$$

The fair wage is thus

$$
\boxed{w=\frac1{n(n+1)}\sum_{k=0}^{n-1}(k+1)\bigl(p(k+1)-p(k)\bigr)
=\frac{np(n)-\sum_{k=0}^{n-1}p(k)}{n(n+1)}.}
$$

This is [Shapley wages in an entrepreneur-worker game](../../../../../shapley-wages-in-an-entrepreneur-worker-game.md). The entrepreneur's payoff, by efficiency, is

$$
\boxed{x_0=p(n)-nw=\frac1{n+1}\sum_{k=0}^{n}p(k).}
$$

It also follows directly because the entrepreneur has each possible number $k$ of predecessors with [probability](../../../../../probability.md) $1/(n+1)$, and their contribution is then $p(k)$. When $p(k)=\alpha k$, the differences are all $\alpha$ and $\sum_{k=0}^{n-1}(k+1)=n(n+1)/2$, so

$$
\boxed{w=\frac\alpha2,\qquad x_0=\frac{\alpha n}{2}.}
$$

Finally suppose $p$ is convex and nondecreasing on nonnegative integers, so $d_k=p(k+1)-p(k)$ is nonnegative and nondecreasing. We verify that the entire [coalitional game](../../../../../transferable-utility-game.md) is convex. The entrepreneur's contribution to a set of $k$ workers is $p(k)$, which increases with that set. A worker's contribution is zero when the entrepreneur is absent and is $d_k$ when the entrepreneur and $k$ other workers are present. Enlarging a predecessor set either leaves both contributions zero, introduces the entrepreneur and a nonnegative contribution, or increases $k$ and hence $d_k$. Every player's [marginal contributions](../../../../../marginal-contribution.md) therefore increase, giving a [convex cooperative game](../../../../../convex-cooperative-game.md). The result already proved yields **the complete Shapley allocation lies in the core**, including the entrepreneur's payoff.

One can also verify the [core](../../../../../core-game-theory.md) inequalities directly. Nonentrepreneur [coalitions](../../../../../coalition-game-theory.md) receive $kw\geq0$, their value. For a [coalition](../../../../../coalition-game-theory.md) containing the entrepreneur and $k<n$ workers, it suffices that

$$
w\leq\frac{p(n)-p(k)}{n-k}.
$$

Since $k+1\leq n+1$ in the wage sum, $w\leq\frac1n\sum_{j=0}^{n-1}d_j$. Nondecreasing $d_j$ makes this full average no greater than the average of the final $n-k$ differences, which is the displayed right side. Thus $x_0+kw=p(n)-(n-k)w\geq p(k)$; the grand [coalition](../../../../../coalition-game-theory.md) has equality by efficiency. This confirms the core conclusion without assuming $p(0)=0$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
