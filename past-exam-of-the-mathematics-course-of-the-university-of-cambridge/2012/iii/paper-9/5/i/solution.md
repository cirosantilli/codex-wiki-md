<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the standard [Achlioptas process](../../../../../../achlioptas-process.md) with two independent uniform candidate [edges](../../../../../../edge-of-a-graph.md) per step and a rule choosing one. The [component-band vertex count](../../../../../../component-band-vertex-count.md) $N_{[k,Dk)}$ counts [vertices](../../../../../../vertex-graph-theory.md), not the number of [graph components](../../../../../../component-graph-theory.md). Integer time rounding changes the arguments below by $O(1)$ steps.

First, at $t_k$ the eventual [graph component](../../../../../../component-graph-theory.md) of order at least $\delta n$ is assembled from [graph components](../../../../../../component-graph-theory.md) already present at $t_k$. Contract those initial [graph components](../../../../../../component-graph-theory.md). During $s=t_c-t_k$ steps, at most $s$ new [edges](../../../../../../edge-of-a-graph.md) are added, so the eventual connected contracted [graph](../../../../../../graph-split.md) contains at most $s+1$ initial [graph components](../../../../../../component-graph-theory.md). Initial [graph components](../../../../../../component-graph-theory.md) of order less than $k$ can therefore contribute at most

$$
(s+1)(k-1)\leq\delta n/2
$$

[vertices](../../../../../../vertex-graph-theory.md), for sufficiently large $n$ and fixed $k$, since $s=\delta n/(2k)+O(1)$. For $k=1$ their contribution is zero. Consequently $N_{\geq k}(G_{t_k})\geq\delta n/2$.

We now use [forced merging of large components](../../../../../../forced-merging-of-large-components.md). If at a time $m$ the [graph components](../../../../../../component-graph-theory.md) of order at least $K$ contain at least $an$ [vertices](../../../../../../vertex-graph-theory.md), then after at most $A(a)n/K+O(1)$ steps there is a [graph component](../../../../../../component-graph-theory.md) of order at least $an/3$, except on an event of [probability](../../../../../../probability.md) exponentially small in $n/K$. One explicit choice is $A(a)=81(\log2+2)/a^4$. The proof is a [union bound](../../../../../../boole-s-inequality.md) over [set partitions](../../../../../../set-partition.md) of the at most $n/K$ initial large [graph components](../../../../../../component-graph-theory.md): if all final [graph components](../../../../../../component-graph-theory.md) were small, a [balanced component cut](../../../../../../balanced-component-cut.md) would split their initial [vertices](../../../../../../vertex-graph-theory.md) into sets of size at least $an/3$, and both candidate [edges](../../../../../../edge-of-a-graph.md) cross that fixed cut with [probability](../../../../../../probability.md) at least $a^4/81$ in every step. The rule cannot avoid such a forced crossing. The failure bound is $e^{-2n/K}$, and a [union bound](../../../../../../boole-s-inequality.md) makes the estimate simultaneous over all starting times at most $3n$, for each fixed $K$.

Set $a=\delta/4$ and choose a fixed integer $D\geq2$ with $D\geq4A(a)/\delta$. If $N_{\geq Dk}(G_{t_k})\geq\delta n/4$, this lemma would produce a [graph component](../../../../../../component-graph-theory.md) of order at least $\delta n/12$ by time

$$
t_k+\frac{A(a)n}{Dk}+O(1)\leq t_c-\frac{\delta n}{4k}+O(1)<t'_c.
$$

That contradicts the assumed $L_1(G_{t'_c})=o(n)$. Thus $N_{\geq Dk}(G_{t_k})<\delta n/4$, and subtraction gives

$$
\boxed{N_{[k,Dk)}(G_{t_k})\geq\delta n/4\quad\text{with high probability}.}
$$

The same $D$ works for every fixed $k$; it depends only on $\delta$, with the number of offered [edges](../../../../../../edge-of-a-graph.md) fixed at two.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
