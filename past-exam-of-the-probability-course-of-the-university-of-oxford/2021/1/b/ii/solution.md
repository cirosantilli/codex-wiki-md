<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The definition of [convergence in distribution](../../../../../convergence-in-distribution.md) gives $F_n(t)\to F(t)$ at each [continuity point](../../../../../continuity-point.md) $t$ of $F$. We must handle a moving argument rather than assume this convergence is uniform.

A [cumulative distribution function](../../../../../cumulative-distribution-function.md) has at most countably many [discontinuities](../../../../../discontinuity.md): each is a jump of positive size, and there are at most $r$ jumps of size at least $1/r$, since their sizes sum to at most one. Thus we can choose [continuity points](../../../../../continuity-point.md) $u_j<c<v_j$ with $u_j\uparrow c$ and $v_j\downarrow c$. For fixed $j$, eventually $u_j<c_n<v_j$. The [monotonicity](../../../../../monotonic-function.md) of each [cumulative distribution function](../../../../../cumulative-distribution-function.md) implies

$$
F_n(u_j)\leq F_n(c_n)\leq F_n(v_j).
$$

First let $n\to\infty$, using the definition of [convergence in distribution](../../../../../convergence-in-distribution.md) at $u_j,v_j$. Then let $j\to\infty$, using [continuity](../../../../../continuous-function.md) at $c$:

$$
F(u_j)\leq\liminf_nF_n(c_n)\leq\limsup_nF_n(c_n)\leq F(v_j),\qquad
\boxed{F_n(c_n)\longrightarrow F(c).}
$$

No result relating different [convergence of random variables](../../../../../convergence-of-random-variables-split.md) has been assumed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
