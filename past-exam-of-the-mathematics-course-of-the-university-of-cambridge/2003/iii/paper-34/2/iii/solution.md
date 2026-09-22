<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Consider a triangle of three equal links, each with capacity $1000$. Each vertex pair receives direct calls of [offered load](../../../../../../offered-traffic.md) $945$. A call tries its direct link first; on finding it full, it tries the two-link path through the third vertex. Take [exponential distributions](../../../../../../exponential-distribution.md) of mean one, so the arrival rates are also $945$.

In a symmetric [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md), let $B$ be the blocking probability of each link. A given link sees its own direct load $945$. Each of the other two call classes offers overflow only if its direct link blocks and the other link of its two-link path accepts. The reduced load into the given link therefore has two extra terms $945B(1-B)$. The scalar consistency equation is

$$
B=E\bigl(945[1+2B(1-B)],1000\bigr).
$$

Write its continuous residual as $f(B)=E(945[1+2B(1-B)],1000)-B$. The following strict intervals certify alternating signs:

$$
\begin{aligned}
0.002722&<f(0)<0.002723,\\
-0.002714&<f(1/100)<-0.002713,\\
0.010042&<f(1/10)<0.010043,\\
-0.113238&<f(2/5)<-0.113237.
\end{aligned}
$$

These are exact rational certificates, not rounded floating-point evidence. For each rational argument, start with $b_0=1$ and iterate $b_j=ab_{j-1}/(j+ab_{j-1})$ for $j=1,\ldots,1000$; all operations are rational. Direct integer comparisons with the displayed thresholds certify the intervals. This uses [rational certificates for the Erlang loss recursion](../../../../../../rational-certificates-for-the-erlang-loss-recursion.md).

The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) now supplies at least one zero in each of

$$
\boxed{(0,1/100),\quad(1/100,1/10),\quad(1/10,2/5).}
$$

Thus the alternative-routing approximation has at least three distinct symmetric solutions. The mechanism is positive overflow feedback at moderate blocking, followed by saturation at high blocking. This does not give several [stationary distributions](../../../../../../stationary-distribution.md) for the exact finite [loss network](../../../../../../loss-network.md): its reachable [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) still has a unique [stationary distribution](../../../../../../stationary-distribution.md). Multiple approximate fixed points concern the self-consistency model.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
