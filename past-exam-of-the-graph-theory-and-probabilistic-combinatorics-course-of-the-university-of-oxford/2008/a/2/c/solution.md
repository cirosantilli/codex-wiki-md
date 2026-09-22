<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Deletion-contraction also proves the alternating-sign form with nonnegative coefficients. If $G$ has $n$ vertices, $G/e$ has $n-1$, so subtracting its alternating expansion adds its coefficient at each succeeding index:

$$
a_i(G)=a_i(G-e)+a_{i-1}(G/e).
$$

Starting from an edgeless [graph](../../../../../graph-split.md) gives $a_0=1$ and no constant term when $n>0$.

For the first coefficients, inclusion-exclusion over the forbidden monochromatic edges gives the precise expression

$$
p_G(x)=\sum_{F\subseteq E(G)}(-1)^{|F|}x^{c(F)},
$$

where $c(F)$ counts components of the spanning [graph](../../../../../graph-split.md) $(V(G),F)$, including isolated vertices. Only $F=\varnothing$ gives $x^n$. A rank-one edge set is a single edge, giving coefficient $-m$ at $x^{n-1}$. Rank two comes from every two-edge subset, each with positive sign, and every triangle, each with negative sign. No other simple edge set has rank two: its nontrivial components must be a three-vertex component or two separate edges. Thus

$$
\boxed{a_0=1,\qquad a_1=m,\qquad a_2=\binom m2-t}.
$$

The displayed $a_2$ assertion concerns $n\ge3$; below this degree the corresponding coefficient is absent and its expression is zero.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
