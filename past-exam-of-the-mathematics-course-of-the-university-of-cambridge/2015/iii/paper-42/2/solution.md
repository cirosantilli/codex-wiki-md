<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Assume the usual continuous nonnegative valuation distribution, so ties occur only on [zero-probability events](../../../../../zero-probability-event.md). Put $t=F(v)$. In a monotone symmetric [Bayesian Nash equilibrium](../../../../../bayesian-nash-equilibrium.md), a type $v$ is first with probability $t^{n-1}$ and second with probability $(n-1)(1-t)t^{n-2}$. Its [rank-order expected prize allocation](../../../../../rank-order-expected-prize-allocation.md) in $G_1$ is therefore

$$
a_1(v)=2t^{n-1}+(n-1)(1-t)t^{n-2}.
$$

The [all-pay effort identity](../../../../../all-pay-effort-identity.md) gives $b_1(v)=\int_{\underline v}^v s a_1'(s)ds$. It also verifies equilibrium directly: a type $v$ imitating type $z$ has utility $v a_1(z)-b_1(z)$, whose derivative is $(v-z)a_1'(z)$, so the true type is a [best response](../../../../../best-response.md).

In the first version of $G_2$, the two contests have expected allocations

$$
a_{21}(v)=t^{n-1},\qquad
a_{22}(v)=t^{n-1}+(n-1)(1-t)t^{n-2}.
$$

There is no common effort budget, and [quasilinear utility](../../../../../quasilinear-utility.md) makes the two effort choices separable. Since $a_{21}+a_{22}=a_1$, adding their [all-pay effort identities](../../../../../all-pay-effort-identity.md) yields

$$
\boxed{b_{21}(v)+b_{22}(v)=b_1(v),\qquad
\mathbb E[\text{total effort in }G_2]=\mathbb E[\text{total effort in }G_1].}
$$

The equality holds type by type for aggregate effort, rather than only after taking expectations. The within-player correlation of the two efforts does not enter these additive expected payoffs.

For the second version of $G_2$, let $V_{[1]}\geq\cdots\geq V_{[n]}$ denote [descending order statistics](../../../../../descending-order-statistics.md). The [expected effort in a rank-order contest](../../../../../expected-effort-in-a-rank-order-contest.md) with prize vector $(2,1,0,\ldots)$ is

$$
\mathbb E E_1=\mathbb E V_{[2]}+2\mathbb E V_{[3]}.
$$

Equivalently, decompose the allocation into a unit award to the best player and a unit award to each of the best two players, then use [revenue equivalence](../../../../../revenue-equivalence.md): the corresponding total auction payments are $V_{[2]}$ and $2V_{[3]}$. Two separate first-place contests with prize values one and two instead generate

$$
\mathbb E E_2=3\mathbb E V_{[2]}.
$$

Consequently

$$
\boxed{\mathbb E E_2-\mathbb E E_1
=2\mathbb E[V_{[2]}-V_{[3]}]\geq0.}
$$

For a nondegenerate continuous distribution, the inequality is strict. No regularity of [virtual valuations](../../../../../virtual-valuation.md) is needed for this comparison. With a [uniform distribution](../../../../../continuous-uniform-distribution.md) on $[0,1]$, the two totals are $(3n-5)/(n+1)$ and $3(n-1)/(n+1)$, giving a difference of $4/(n+1)$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
