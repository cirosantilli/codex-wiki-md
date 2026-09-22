<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Consider a triangle of three links, each with capacity $C$. Calls for each pair of its three nodes arrive as independent [Poisson processes](../../../../../../poisson-process.md) at rate $\lambda$ and have independent holding times with an [exponential distribution](../../../../../../exponential-distribution.md) of mean one. Try the direct link first; if it is full, try the two-link path through the third node; if either alternative link is full, reject the call. This is [alternative routing](../../../../../../alternative-routing.md) in a [loss network](../../../../../../loss-network.md).

In the symmetric [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md), let $B$ be each link's blocking probability. A given link receives direct [offered traffic](../../../../../../offered-traffic.md) $\lambda$. Each of the other two call types contributes overflow traffic $\lambda B$, screened by the availability $1-B$ of the other link on its alternative path. Thus

$$
\boxed{B=E\bigl(\lambda[1+2B(1-B)],C\bigr).}
$$

The extra term expresses a feedback: blocking sends calls onto longer paths, which consume more total capacity and can create still more blocking.

Here is an explicit finite-capacity example, not just a limiting argument. Take $C=1000$ and $\lambda=950$, and let $F(B)=E(950[1+2B(1-B)],1000)-B$. Evaluating the [Erlang loss formula](../../../../../../erlang-loss-formula.md) gives

$$
\begin{array}{c|rrrr}
B&0&1/100&1/10&2/5\\\hline
F(B)&0.00364929&-0.000923093&0.0144598&-0.109515
\end{array}
$$

The displayed decimals are rounded, but the four signs can be checked exactly using the rational recursion $E(a,0)=1$, $E(a,k)=aE(a,k-1)/(k+aE(a,k-1))$. By the [intermediate value theorem](../../../../../../intermediate-value-theorem.md), there is a [fixed point](../../../../../../fixed-point.md) in each of $(0,0.01)$, $(0.01,0.1)$, and $(0.1,0.4)$. Numerically these three are

$$
\boxed{B\approx0.00731475,\qquad0.0392115,\qquad0.217394.}
$$

Thus **[alternative routing](../../../../../../alternative-routing.md) can produce multiple [Erlang fixed points](../../../../../../erlang-fixed-point-approximation.md)**. This does not imply multiple [stationary distributions](../../../../../../stationary-distribution.md) for the exact finite [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md), which is irreducible and has a unique [stationary distribution](../../../../../../stationary-distribution.md); the multiplicity belongs to the approximation. The symmetric alternative-routing model is also discussed in [Kelly's review of fixed point models of loss networks](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/FD5AA6764623CC6E4836E7893DFA1524/S0334270000006597a.pdf/fixed_point_models_of_loss_networks.pdf).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 213](../../../paper-213-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
