<h1 id="22i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [bounded inverse theorem](../../../../../../bounded-inverse-theorem.md) states that a bounded bijective linear map between Banach spaces has a bounded inverse.

The [closed graph theorem](../../../../../../closed-graph-theorem.md) states that if $X$ and $Y$ are Banach spaces and $T:X\to Y$ is linear, then $T$ is continuous if and only if its graph

$$
\Gamma(T)=\{(x,Tx):x\in X\}
$$

is closed in the Banach space $X\times Y$.

If $T$ is continuous and $(x_n,Tx_n)\to(x,y)$, then $Tx_n\to Tx$, so uniqueness of limits gives $y=Tx$. Hence the graph is closed.

Conversely, suppose $\Gamma(T)$ is closed. It is then a Banach space. The coordinate projection

$$
P_X:\Gamma(T)\longrightarrow X,
\qquad (x,Tx)\longmapsto x,
$$

is bounded and bijective. By the bounded inverse theorem, $P_X^{-1}:x\mapsto(x,Tx)$ is bounded. Composing it with the bounded second-coordinate projection gives

$$
T=P_Y\circ P_X^{-1},
$$

so $T$ is continuous.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22I](../../22i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
