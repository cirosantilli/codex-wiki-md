<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the usual continuous-distribution convention $F(0)=0$, $F(1)=1$, and write $f=F'$. After observing $b$, the follower can win by matching it, because ties favor the follower. Its [best response](../../../../../best-response.md) is to match when $v_2>b$ and choose zero when $v_2<b$; the indifferent equality has probability zero. Thus the leader wins with probability $F(b)$ and a leader of type $v$ maximizes

$$
\boxed{h_v(b)=vF(b)-b,\qquad 0\leq b\leq1.}
$$

Bids above $1$ are dominated by bidding $1$. This is the [leader optimization in a sequential private-value all-pay contest](../../../../../leader-optimization-in-a-sequential-private-value-all-pay-contest.md). Since $F$ is a [concave function](../../../../../concave-function.md), $h_v$ is [concave](../../../../../concave-function.md). An interior optimum satisfies $vf(b)=1$, with the usual endpoint conditions when that equation has no interior solution.

For precision, select the smallest maximizer when the leader is indifferent. This defines a [Stackelberg equilibrium](../../../../../stackelberg-equilibrium.md) and supplies the printed strict conditional comparison at the threshold type. Let $q=F^{-1}(1/2)$. The density $f(q)$ is positive: if it vanished there, its nonnegative nonincreasing continuation would force $F$ to remain $1/2$ up to $1$, which is impossible. At the median,

$$
h_v'(q)=vf(q)-1.
$$

If this is positive, every maximizer is strictly greater than $q$, so the leader wins with probability greater than $1/2$. If it is negative, every maximizer is strictly smaller than $q$. If it is zero, $q$ is a maximizer, and the smallest maximizer is at most $q$. Therefore the [median-density threshold for the leader in an all-pay contest](../../../../../median-density-threshold-for-the-leader-in-an-all-pay-contest.md) is

$$
\boxed{\mathbb P(1\text{ wins}\mid v_1=v)>\frac12
\quad\Longleftrightarrow\quad v>\frac1{F'(F^{-1}(1/2))}.}
$$

Strict [concavity](../../../../../concave-function.md) of $F$ would make the optimum unique, removing the selection convention. With mere [concavity](../../../../../concave-function.md), the printed assertion needs that convention at equality. For example, $F(b)=b$ and $v=1$ make all bids optimal, and choosing $b=3/4$ makes the leader more likely to win even though the strict threshold is not exceeded.

The same issue can occur at an interior type, rather than just an endpoint. A continuously differentiable [concave](../../../../../concave-function.md) distribution is

$$
F(t)=2t-\frac{15}{4}\left[(t-\tfrac1{10})_+^2-(t-\tfrac15)_+^2\right]
-\frac{145}{144}(t-\tfrac25)_+^2.
$$

Its density decreases from $2$ to $5/4$, is constant on $[1/5,2/5]$, and then decreases to $1/24$; integration gives $F(1)=1$. Its median is $31/100$. At $v=4/5=1/f(q)$, every bid in $[1/5,2/5]$ maximizes $h_v$, and choosing $2/5$ gives [winning probability](../../../../../winning-probability.md) $49/80>1/2$. This confirms the genuine [best-response selection at a flat leader objective](../../../../../best-response-selection-at-a-flat-leader-objective.md) issue. The smallest-maximizer convention avoids it; the threshold type has zero ex ante probability.

The unconditional comparison is valid for every optimal selection. Zero effort guarantees the leader payoff zero, so an optimal bid satisfies

$$
vF(b(v))-b(v)\geq0\quad\Longrightarrow\quad b(v)\leq vF(b(v))\leq v.
$$

Consequently $F(b(v))\leq F(v)$. If $V$ has the continuous distribution $F$, the [probability integral transform](../../../../../probability-integral-transform.md) makes $F(V)$ uniform on $[0,1]$. Taking expectations proves the [ex ante follower advantage in a sequential all-pay contest](../../../../../ex-ante-follower-advantage-in-a-sequential-all-pay-contest.md):

$$
\boxed{\mathbb P(1\text{ wins})=\mathbb E[F(b(V))]\leq\frac12
\leq\mathbb P(2\text{ wins}).}
$$

For strictly increasing atom-free $F$, optimal bids in fact satisfy $b(v)<v$ for almost every $v\in(0,1)$, so the first inequality is strict. Conditional advantage for unusually high leader types is therefore compatible with an unconditional follower advantage.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
