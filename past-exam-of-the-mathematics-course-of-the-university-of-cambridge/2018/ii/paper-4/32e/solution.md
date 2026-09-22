<h1 id="32e/solution">Solution</h1>

↑ **Parent:** [32E](../32e.md)

An [interval map](../../../../../interval-map.md) has a [horseshoe for an interval map](../../../../../horseshoe-for-an-interval-map.md) when two disjoint subintervals are each mapped across a common interval. It is [Glendinning-chaotic](../../../../../glendinning-chaos.md) when one of its positive iterates has such a horseshoe.

Let the points of the three-cycle be $x_1<x_2<x_3$ and put $I_0=[x_1,x_2]$, $I_1=[x_2,x_3]$. There are two possible cyclic orders. If $x_1\mapsto x_2\mapsto x_3\mapsto x_1$, the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives

$$
I_0\longrightarrow I_1,
\qquad I_1\longrightarrow I_0,
\qquad I_1\longrightarrow I_1
$$

for the [interval covering relation](../../../../../interval-covering-relation.md). Thus there are two closed covering walks of length two based at $I_1$. In the reverse cyclic order there are instead the arrows $I_0\to I_0$, $I_0\to I_1$ and $I_1\to I_0$, again giving two closed walks of length two. The [horseshoe from two closed covering walks](../../../../../horseshoe-from-two-closed-covering-walks.md) therefore shows that $F^2$ has a horseshoe in either case, so $F$ is chaotic.

The [Sharkovsky theorem](../../../../../sharkovskii-s-theorem.md) orders the positive integers as

$$
3\prec5\prec7\prec\cdots
\prec2\cdot3\prec2\cdot5\prec\cdots
\prec2^2\cdot3\prec\cdots
\prec\cdots\prec2^3\prec2^2\prec2\prec1,
$$

and says that a cycle of a given period forces cycles of every period to its right.

Suppose $N=2^rq$ with $q>1$ odd. Then $F^{2^r}$ has a $q$-cycle. The [Sharkovsky theorem](../../../../../sharkovskii-s-theorem.md) gives that map a six-cycle, and squaring it produces a three-cycle. Hence $F^{2^{r+1}}$ has a three-cycle and an iterate of $F$ has a horseshoe. Thus

$$
\boxed{N\text{ not a power of two and an }N\text{-cycle}\implies F\text{ is Glendinning-chaotic}.}
$$

A horseshoe contains the symbolic dynamics of the [Bernoulli shift](../../../../../bernoulli-shift.md). Periodic binary words give cycles of every symbolic period; after translating from an iterate back to $F$, this supplies cycles of many periods that are not powers of two.

For the [logistic map](../../../../../logistic-map.md), a ten-cycle would imply chaos because $10$ is not a power of two. Hence there is no ten-cycle for $\mu<\mu_\infty$. A three-cycle forces every period, so a ten-cycle exists for $\mu>1+\sqrt8$. The stated facts alone give no conclusion for the intermediate range:

$$
\boxed{\mu<\mu_\infty:\ 	ext{no ten-cycle};
\qquad \mu>1+\sqrt8:\ 	ext{a ten-cycle exists}.}
$$

## ↑ Ancestors (10)

1. [32E](../32e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
