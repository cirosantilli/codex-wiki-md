<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

There are genuine normalization inconsistencies in this PDF. In the standard [linearized chord diagram model](../../../../../linearized-chord-diagram-model.md) $G_n^{(1)}$, time $n$ gives **$n$ [edges](../../../../../edge-of-a-graph.md) and total [vertex degree](../../../../../degree-graph-theory.md) $2n$**, with [self-loops](../../../../../loop-graph-theory.md) counted twice. The paper calls $2n$ the number of [edges](../../../../../edge-of-a-graph.md). Its right-endpoint hint also uses $\sqrt{i/(2n)}$ rather than $\sqrt{i/n}$. These cannot both describe the standard model; part (c)'s exponent is consequently inconsistent as well. We give the definition, prove the alternative construction and its limits, and explicitly identify the corrected conclusion rather than infer an invalid constant from the printed hint.

Start from the empty [graph](../../../../../graph-split.md) at time zero, or from one [vertex](../../../../../vertex-graph-theory.md) with one [self-loop](../../../../../loop-graph-theory.md) at time one. To obtain $G_t$ from $G_{t-1}$, add [vertex](../../../../../vertex-graph-theory.md) $t$ and an [edge](../../../../../edge-of-a-graph.md) directed from $t$ to $I_t$, where

$$
\boxed{\Pr(I_t=i\mid G_{t-1})=\frac{d_i(t-1)}{2t-1}\ (i<t),\qquad\Pr(I_t=t\mid G_{t-1})=\frac1{2t-1}.}
$$

A self-choice creates a [self-loop](../../../../../loop-graph-theory.md). The old [vertex degrees](../../../../../degree-graph-theory.md) sum to $2(t-1)$, so these [probabilities](../../../../../probability.md) sum to one. This is exact [preferential attachment](../../../../../preferential-attachment.md), including the outward half of the new [edge](../../../../../edge-of-a-graph.md) as weight one for the new [vertex](../../../../../vertex-graph-theory.md); it is not a rule normalized by $2t$ or a process adding two [edges](../../../../../edge-of-a-graph.md) at each step. The [degree of a vertex](../../../../../degree-graph-theory.md) here is its total incoming plus outgoing [vertex degree](../../../../../degree-graph-theory.md). The construction in part (a) has exactly one chord per [vertex](../../../../../vertex-graph-theory.md) and makes the edge-count discrepancy explicit.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
