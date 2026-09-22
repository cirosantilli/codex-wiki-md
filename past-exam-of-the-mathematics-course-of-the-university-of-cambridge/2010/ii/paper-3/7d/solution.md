<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Use [binary expansions](../../../../../binary-expansion.md) ending in zeros at dyadic rationals. The [doubling map](../../../../../dyadic-transformation.md) shifts the expansion left:

$$
x=0.b_1b_2b_3\ldots\quad\Longrightarrow\quad F(x)=0.b_2b_3b_4\ldots.
$$

In ordinary coordinates it is $2x$ on $[0,1/2)$ and $2x-1$ on $[1/2,1)$. The branches are continuous; the left limit at $1/2$ is $1$ while its value and right limit are $0$. This is its only discontinuity in the half-open interval.

For every $N\ge2$, the repeating binary block $0^{N-1}1$ gives

$$
\boxed{x_N=\frac1{2^N-1},\qquad F^N(x_N)=x_N.}
$$

Its least period is $N$: a shorter repeating block would make more than one digit equal to one in a length-$N$ period. The orbit avoids the discontinuity, and its multiplier is $(F^N)'=2^N>1$, so **these periodic orbits are repelling and unstable**. The same multiplier argument applies to every periodic orbit, with the endpoint [fixed point](../../../../../fixed-point.md) treated one-sidedly.

In the two-branch horseshoe formulation of [Glendinning chaos](../../../../../glendinning-chaos.md), disjoint subintervals are each mapped onto the same interval by an iterate. Here $J=(0,1)$, $K_0=(0,1/2)$ and $K_1=(1/2,1)$ already satisfy $F(K_0)=F(K_1)=J$. Their inverse branches $x\mapsto x/2$ and $x\mapsto(x+1)/2$ realize every binary itinerary. This is a horseshoe for a piecewise continuous map; on the circle the endpoint jump disappears. The symbolic explanation also shows [dense periodic points](../../../../../dense-periodic-points.md), by repeating any prescribed finite prefix, and [topological transitivity](../../../../../topological-transitivity.md), because an iterate maps any sufficiently small dyadic cylinder onto $(0,1)$. Finally every neighborhood contains points sharing an arbitrarily long prefix but with different subsequent digits; an appropriate iterate separates their images by a fixed amount, for instance more than $1/4$. This proves [sensitive dependence on initial conditions](../../../../../butterfly-effect.md) as well. **The binary shift has full two-symbol chaotic dynamics.**

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
