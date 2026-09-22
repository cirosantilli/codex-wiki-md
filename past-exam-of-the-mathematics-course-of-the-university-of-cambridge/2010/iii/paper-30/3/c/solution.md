<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [alternative routing](../../../../../../alternative-routing.md) term feeds additional traffic back into the link. We can prove the existence of three solutions rather than relying on an iteration that happens to find different answers. Choose $\nu_N=20N$, $C_N=21N$, and define the continuous residual

$$
G_N(B)=E\bigl(20N[1+2B(1-B)],21N\bigr)-B.
$$

By the [proportional scaling limit of the Erlang loss formula](../../../../../../proportional-scaling-limit-of-the-erlang-loss-formula.md), at each fixed $B$,

$$
G_N(B)\longrightarrow G_\infty(B)=\max\left\{0,1-\frac{21/20}{1+2B(1-B)}\right\}-B.
$$

At $B=1/100$, the multiplier is $1.0198<21/20$, so $G_\infty(1/100)=-1/100$. At $B=1/8$ it is $39/32$, giving

$$
G_\infty(1/8)=1-\frac{56}{65}-\frac18=\frac7{520}>0.
$$

Also $G_N(0)>0$ and $G_N(1)<0$ for every $N$, since a finite-capacity [Erlang loss formula](../../../../../../erlang-loss-formula.md) gives a blocking probability strictly between zero and one. For all sufficiently large $N$, the signs at $0,1/100,1/8,1$ therefore alternate. Applying the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) in the three disjoint intervening intervals proves **at least three distinct fixed points**. This supplies a [fluid scaling proof of multiple Erlang fixed points](../../../../../../fluid-scaling-proof-of-multiple-erlang-fixed-points.md).

<a id="3/c/image-three-fixed-points-of-the-alternative-routing-erlang-approximation"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30-erlang-fixed-points.png)

**[Figure 1](#3/c/image-three-fixed-points-of-the-alternative-routing-erlang-approximation). Three fixed points of the alternative-routing Erlang approximation**.

This multiplicity concerns the [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md). It does not imply several equilibrium laws for an exact finite [irreducible Markov chain](../../../../../../irreducible-markov-chain.md), which has a unique [stationary distribution](../../../../../../stationary-distribution.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
