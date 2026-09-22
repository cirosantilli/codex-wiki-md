<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [Shearer independence bound for a triangle-free graph](../../../../../../shearer-independence-bound-for-a-triangle-free-graph.md). It states that an $n$-vertex [triangle-free graph](../../../../../../triangle-free-graph.md) of maximum degree at most $d$ has an [independent set](../../../../../../independent-set-graph-theory.md) of size

$$
\alpha(G)\ge c\frac{n\log d}{d}
$$

for an absolute $c>0$. The result is immediate for bounded $d$ after reducing $c$, while the theorem gives the asserted logarithmic gain for $d$ large. Thus

$$
\boxed{\alpha(G)\ge c n\log d/d.}
$$

For completeness, the key input in Shearer's proof is to expose a random independent set one degree scale at a time. Triangle-freeness makes every neighbourhood independent, so conditioning on earlier choices creates no edges inside the available neighbours. The expected gain at degree scale $j$ is $\Omega(n_j/d)$; summing over the $\Theta(\log d)$ nonempty scales gives $\Omega(n\log d/d)$. The entropy, or hard-core-model, form of the argument makes this scale calculation rigorous without losing vertices counted at adjacent scales.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
