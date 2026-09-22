<h1 id="22f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [open mapping theorem](../../../../../../open-mapping-theorem-functional-analysis.md) states that every surjective bounded linear map $S:X\to Y$ between [Banach spaces](../../../../../../banach-space-split.md) maps open sets to open sets. Equivalently, there is $c>0$ such that

$$
B_Y(0,c)\subseteq S(B_X(0,1)).
$$

The [closed graph theorem](../../../../../../closed-graph-theorem.md) states that a linear map $T:X\to Y$ between Banach spaces is continuous if and only if its [graph](../../../../../../graph-of-a-linear-operator.md)

$$
\Gamma(T)=\{(x,Tx):x\in X\}
$$

is closed in $X\times Y$.

Assume the open mapping theorem and suppose $\Gamma(T)$ is closed. As a closed subspace of the Banach space $X\times Y$, the graph is itself Banach. The coordinate projection

$$
P:\Gamma(T)\longrightarrow X,\qquad (x,Tx)\longmapsto x
$$

is a bounded linear bijection. By the open mapping theorem, $P^{-1}$ is bounded. The other coordinate projection $Q:\Gamma(T)\to Y$ is bounded, and

$$
T=Q\circ P^{-1}.
$$

**Thus $T$ is bounded and hence continuous. This is the [closed graph theorem from the bounded inverse theorem](../../../../../../closed-graph-theorem-from-the-bounded-inverse-theorem.md) argument.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22F](../../22f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
