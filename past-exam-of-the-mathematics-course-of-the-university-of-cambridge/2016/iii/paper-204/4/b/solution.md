<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First obtain a [polynomial critical one-arm upper bound](../../../../../../polynomial-critical-one-arm-upper-bound.md) from part (a). Fix a sufficiently large integer radius $r$. Use rotated-coordinate boxes $B_r=[-r,r]^2$ for this geometric construction, in the axes of part (a). Surround $B_r$ by a square ring inside $B_{3r}$. It can be assembled from the four strips

$$
[-3r,3r]\times[r,3r],\quad[-3r,3r]\times[-3r,-r],\quad[-3r,-r]\times[-3r,3r],\quad[r,3r]\times[-3r,3r].
$$

The first two require horizontal dual crossings; the last two require vertical dual crossings. Their corner overlaps are squares, so the adjacent long crossings intersect there and their union contains a dual [graph cycle](../../../../../../cycle-in-a-graph.md) surrounding the inner box. Translate the strips by the half-lattice displacement of the [planar dual graph](../../../../../../planar-dual-graph.md) and adjust the endpoints by one lattice unit if needed. All aspect ratios remain bounded. Part (a) and the same overlap gluing give a uniform lower bound $c_1>0$ for each dual crossing at $1/2$. Applying the [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) to these [decreasing events](../../../../../../decreasing-event.md) in the primal configuration gives a closed dual circuit with [probability](../../../../../../probability.md) at least $\delta=c_1^4>0$. We may replace $\delta$ by a smaller number in $(0,1)$.

Use the [independent annular barriers for percolation](../../../../../../independent-annular-barriers-for-percolation.md) at radii $r_j=r_0 10^j$. Their supporting [edge](../../../../../../edge-of-a-graph.md) sets are disjoint, so the circuit events are independent. In the original unrotated coordinates, $B_{3r}$ lies inside $\Lambda_{5r}$ and the ring still separates the origin from infinity. These fixed geometric comparisons let us bound the original $g_N$. An open [graph path](../../../../../../path-in-a-graph.md) from $0$ to distance $N$ must avoid every such closed dual circuit inside $\Lambda_N$. Thus, for some constants $C<\infty$ and $\alpha>0$,

$$
g_N(1/2)\leq(1-\delta)^{\lfloor\log_{10}(N/(5r_0))\rfloor+1}\leq C N^{-\alpha},\qquad
\alpha=\frac{-\log(1-\delta)}{\log10}>0,
$$

where the first bound is used only when at least one of the indicated rings fits; increasing $C$ handles smaller $N$.

Now let $\varepsilon=p-1/2>0$ and use the [monotone coupling of Bernoulli percolation](../../../../../../monotone-coupling-of-bernoulli-percolation.md) on [edges](../../../../../../edge-of-a-graph.md). The event $\{0\leftrightarrow\partial\Lambda_N\}$ only needs [edges](../../../../../../edge-of-a-graph.md) whose endpoints lie in $\Lambda_N$, because a first boundary hit gives an internal [graph path](../../../../../../path-in-a-graph.md). There are exactly $4N(2N+1)$ such [edges](../../../../../../edge-of-a-graph.md). Each changes state between parameters $1/2$ and $p$ with [probability](../../../../../../probability.md) $\varepsilon$. The [union bound](../../../../../../boole-s-inequality.md) therefore gives the [finite-box comparison for percolation parameters](../../../../../../finite-box-comparison-for-percolation-parameters.md)

$$
\theta(p)\leq g_N(p)\leq g_N(1/2)+4N(2N+1)\varepsilon\leq C N^{-\alpha}+12N^2\varepsilon.
$$

For sufficiently small $\varepsilon$, choose $N=\lfloor\varepsilon^{-1/(\alpha+2)}\rfloor$, so that $N$ is at least half the unrounded value. Both terms then have order $\varepsilon^{\alpha/(\alpha+2)}$. In particular,

$$
\boxed{\theta(p)\leq A(p-1/2)^\beta,\qquad\beta=\frac\alpha{\alpha+2}>0}
$$

for a finite $A$. Increase $A$ to cover the remaining compact range of parameters by $\theta(p)\leq1$. This [near-critical percolation power upper bound](../../../../../../near-critical-percolation-power-upper-bound.md) requires only a positive crossing constant, not the exact value of a critical exponent. It also implies $\theta(1/2)=0$ through the critical [one-arm probability](../../../../../../one-arm-probability.md) bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
