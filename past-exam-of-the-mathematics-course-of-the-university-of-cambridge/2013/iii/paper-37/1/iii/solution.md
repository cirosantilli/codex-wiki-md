<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With [alternative routing](../../../../../../alternative-routing.md), a rejected direct call can try a longer route. The attempt rates now depend on blocking itself, giving an additional feedback absent from [fixed routing](../../../../../../fixed-routing.md).

For an explicit example, take three nodes with a unit-resource link between each pair, all of capacity $C=1000$. For every unordered pair, direct calls arrive at rate $v=940$ and have mean holding time one. A call first tries its direct link; if that link is full, it tries the unique two-link route through the third node, and otherwise is lost. Under a symmetric [Erlang fixed point approximation](../../../../../../erlang-fixed-point-approximation.md), all links have blocking $B$. A given link sees its own direct load $v$. It can also carry overflow from either of the other two pairs; each contributes reduced load $vB(1-B)$, since the direct link must block and the other link of the alternative route must accept. Hence

$$
\boxed{B=E\bigl(1000,940[1+2B(1-B)]\bigr)}.
$$

This is an instance of [multiple Erlang fixed points under alternative routing](../../../../../../multiple-erlang-fixed-points-under-alternative-routing.md). Put $f(B)=E(1000,940[1+2B(1-B)])-B$. Evaluation using the positive [Erlang B formula](../../../../../../erlang-loss-formula.md) recurrence $E(0,v)=1$, $E(k,v)=vE(k-1,v)/(k+vE(k-1,v))$ gives

$$
\begin{array}{c|rrrr}
B&0&0.01&0.10&0.25\\\hline
f(B)&0.00198354&-0.00426318&0.00560008&-0.02112421.
\end{array}
$$

The sign statements can be certified with rational arithmetic at these rational arguments. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) gives a distinct root in each of $(0,0.01)$, $(0.01,0.10)$ and $(0.10,0.25)$; numerical roots are approximately $0.002748$, $0.071037$ and $0.189785$.

Thus **the alternative-routing fixed point is not unique**. The mechanism is extra link occupancy from overflow: moderate blocking stimulates two-link calls and can reinforce congestion. This multiplicity belongs to the approximation. The exact finite stochastic model has a unique stationary law on its reachable communicating class; the extra approximate solutions do not create three exact invariant distributions.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
