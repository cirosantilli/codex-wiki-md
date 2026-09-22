<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [simple random walk](../../../../../../simple-random-walk.md) on the loopless undirected unweighted [graph](../../../../../../graph-split.md), with transition [probability](../../../../../../probability.md) $1/\deg(x)$ to each [graph neighbour](../../../../../../neighbour-of-a-vertex.md), and take $a\ne z$. Set $T_z=\inf\{t\geq0:X_t=z\}$. Returns to $a$ before visiting $z$ do not end the commute. After its first visit to $z$, stop at the subsequent first visit to $a$, so $\tau=T_z+T_a\circ\vartheta_{T_z}$. Count transitions with departure times $0\leq t<\tau$, including the final step arriving at $a$. The [expected hitting times](../../../../../../expected-hitting-time.md) are finite: in a finite [connected graph](../../../../../../connected-graph.md) there is a uniformly positive [probability](../../../../../../probability.md) to reach any fixed target within a fixed number of steps, giving a geometric tail bound.

We prove the needed [killed-walk occupation voltage](../../../../../../killed-walk-occupation-voltage.md) identity from its visit balance equation. Define

$$
g_{az}(x)=\mathbb E_a\sum_{t=0}^{T_z-1}\mathbf1_{\{X_t=x\}},\qquad v(x)=\frac{g_{az}(x)}{\deg(x)},\qquad v(z)=0.
$$

For $x\ne z$, counting arrivals before absorption gives

$$
g_{az}(x)=\mathbf1_{\{x=a\}}+\sum_{y\sim x}\frac{g_{az}(y)}{\deg(y)}.
$$

Hence, for the [Graph Laplacian](../../../../../../laplacian-matrix.md) $Lv(x)=\deg(x)v(x)-\sum_{y\sim x}v(y)$, we have $Lv(x)=\mathbf1_{\{x=a\}}$ away from $z$. Since the sum of all Laplacian coordinates is zero, $Lv(z)=-1$. Thus $v$ is the electrical [voltage](../../../../../../voltage.md) of a [unit flow](../../../../../../unit-flow.md) from $a$ to $z$, grounded at $z$, and $v(a)=R_{\mathrm{eff}}(a,z)$.

Construct $w(x)=g_{za}(x)/\deg(x)$ for the opposite killed leg. It satisfies $Lw=\delta_z-\delta_a$ and $w(a)=0$. Therefore $L(v+w)=0$. The [harmonic maximum principle on a finite graph](../../../../../../harmonic-maximum-principle-on-a-finite-graph.md) makes $v+w$ constant: at a maximum its value equals the average over its [graph neighbours](../../../../../../neighbour-of-a-vertex.md), forcing all of them to share that value, and connectedness propagates it. At $a$ the constant equals $R_{\mathrm{eff}}(a,z)$.

For any oriented [edge](../../../../../../edge-of-a-graph.md) $(x,y)$, each visit to $x$ before the target hit produces a transition to $y$ with conditional [probability](../../../../../../probability.md) $1/\deg(x)$. The expected traversals during the first killed leg are therefore $v(x)$, and those during the second leg are $w(x)$ by the [Strong Markov property](../../../../../../strong-markov-property.md) at $T_z$. This proves [directed edge occupation in a random-walk commute](../../../../../../directed-edge-occupation-in-a-random-walk-commute.md):

$$
\boxed{\mathbb E_a S(x,y)=v(x)+w(x)=R_{\mathrm{eff}}(a,z).}
$$

In particular, both directions of every unoriented [edge](../../../../../../edge-of-a-graph.md) have this same [expected value](../../../../../../expected-value.md), although their counts on an individual commute need not coincide. Summing over the $2|E|$ directed [edges](../../../../../../edge-of-a-graph.md) also recovers the [commute time identity](../../../../../../commute-time-identity.md) $\mathbb E_a\tau=2|E|R_{\mathrm{eff}}(a,z)$.

The distinct-terminal convention is necessary for the printed “returns” interpretation. If $a=z$ and $\tau$ is the first positive return, a [graph](../../../../../../graph-split.md) with two [graph vertices](../../../../../../vertex-graph-theory.md) and one [edge](../../../../../../edge-of-a-graph.md) gives $S(a,y)=1$ while $R_{\mathrm{eff}}(a,a)=0$. Thus either take $a\ne z$, as intended, or explicitly define the degenerate commute as $\tau=0$. A general nonuniform [random walk](../../../../../../random-walk.md) is not covered by the unweighted simple-walk formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
