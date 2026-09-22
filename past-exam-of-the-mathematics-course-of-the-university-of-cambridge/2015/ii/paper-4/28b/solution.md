<h1 id="28b/solution">Solution</h1>

↑ **Parent:** [28B](../28b.md)

A [horseshoe for an interval map](../../../../../horseshoe-for-an-interval-map.md) consists of two branches covering a common interval: there are an open interval $J$ and disjoint open subintervals $K_0,K_1\subseteq J$ with $f(K_0)=f(K_1)=J$. Equivalently one can work with two closed intervals with disjoint interiors whose images cover their union, and then restrict the branches. [Glendinning chaos](../../../../../glendinning-chaos.md) means that some positive iterate $f^m$ has such a horseshoe, rather than requiring one for $f$ itself.

For the three-cycle, use the [intermediate value theorem](../../../../../intermediate-value-theorem.md) on endpoint images. The [interval covering relations](../../../../../interval-covering-relation.md) are $I_a\to I_b$ and $I_b\to I_a,I_b$. Consequently both $f^2(I_a)$ and $f^2(I_b)$ cover $I_a\cup I_b$. This proves **$f^2$ has a horseshoe**. The [directed covering graph of an interval map](../../../../../directed-covering-graph-of-an-interval-map.md) has exactly these forced arrows; a closed walk $a\to b\to b\to a$ has length three and a primitive itinerary. Pulling back the intervals successively and using the fixed-point property produces a point fixed by $f^3$ with this itinerary. It cannot be fixed by $f$, and a shared endpoint belongs to the already given three-cycle, so a genuine period-three orbit results.

For the increasing spatial order of the five-cycle, let $I_j=[x_{j-1},x_j]$, $1\leq j\leq4$. The forced graph is

$$
I_1\to I_2\to I_3\to I_4,\qquad I_4\to I_1,I_2,I_3,I_4.
$$

The primitive loops $I_4$, $I_3I_4$, $I_2I_3I_4$, and $I_1I_2I_3I_4$ force exact periods $\boxed{1,2,3,4}$. For periods below five the known five-cycle endpoints cannot be responsible, so the interval itineraries give distinct interior orbits. Both $g^2(I_3)$ and $g^2(I_4)$ cover $I_3\cup I_4$, so **$g$ is guaranteed to be Glendinning-chaotic**.

A horseshoe for $g$ itself is not guaranteed. As a counterexample put $x_j=j$ on $[0,4]$ and interpolate by $g(x)=x+1$ for $0\leq x\leq3$, $g(x)=16-4x$ for $3\leq x\leq4$. This has the required five-cycle. The unique fixed point is $16/5$, with $g(x)>x$ to its left and $g(x)<x$ to its right. Any nondegenerate closed interval whose image covers itself must contain this fixed point in its interior: an interval entirely on either side, or with the fixed point as an endpoint, fails to cover its extreme endpoint. Two intervals with disjoint interiors therefore cannot both cover themselves, as a horseshoe would require. Hence this example has no one-iterate horseshoe.

For the alternative spatial order, set $y_0=x_4,y_1=x_2,y_2=x_1,y_3=x_3,y_4=x_0$ and $J_j=[y_{j-1},y_j]$. Endpoint images give

$$
J_1\to J_4,\quad J_2\to J_2,J_3,\quad J_3\to J_1,\quad J_4\to J_1,J_2.
$$

The self-loop at $J_2$, the two-cycle $J_1J_4$, and the four-cycle $J_2J_3J_1J_4$ force $\boxed{1,2,4}$; period three is not guaranteed. To see this last claim, take the connect-the-dots map at $y_j=j$ with values $(4,3,1,0,2)$. Its exact interval transitions are those displayed. Any length-three closed itinerary is the repeated self-loop in $J_2$; there the map is the affine decreasing function $5-2x$, whose third iterate has only its original fixed point. Endpoints belong to the five-cycle. Thus no exact three-cycle exists in this example.

Chaos is still guaranteed: from $J_2$ there are two different length-four closed walks, four self-loops and $J_2J_3J_1J_4J_2$. Pullbacks give disjoint branches of $g^4$ over a common interval in $J_2$, hence a [horseshoe for an interval map](../../../../../horseshoe-for-an-interval-map.md) for an iterate. A horseshoe for $g$ itself is again not guaranteed: the same connect-the-dots example is strictly decreasing on $[0,3]$ and increasing on $[3,4]$ with image $[0,2]$. Its unique fixed point is $5/3$, again with $g(x)>x$ to the left and $g(x)<x$ to the right. The same fixed-point argument rules out two self-covering intervals with disjoint interiors. These counterexamples distinguish the three separate questions about periods, chaos and a one-iterate horseshoe.

## ↑ Ancestors (10)

1. [28B](../28b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
