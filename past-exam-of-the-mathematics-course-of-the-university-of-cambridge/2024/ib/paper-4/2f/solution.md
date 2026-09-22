<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

A subset $A\subseteq X$ is connected if it cannot be written as $A=U\cup V$, where $U,V$ are disjoint, nonempty sets open in the subspace topology on $A$.

If $f(X)$ were disconnected as $U\cup V$, continuity would make $f^{-1}(U)$ and $f^{-1}(V)$ a disconnection of $X$. Thus the [continuous image of a connected space](../../../../../continuous-image-of-a-connected-space.md) is connected.

For $Y=\{0,1\}$ with the discrete topology, a nonconstant continuous $h:X\to Y$ gives the disconnection

$$
X=h^{-1}(\{0\})\cup h^{-1}(\{1\}).
$$

Conversely, a disconnection $X=U\cup V$ defines a continuous nonconstant [function](../../../../../function-split.md) by assigning $0$ on $U$ and $1$ on $V$. Hence $X$ is connected exactly when every such $h$ is constant.

Finally suppose $C$ is connected but $\operatorname{Cl}(C)=U\cup V$ is a disconnection. The intersections $C\cap U$ and $C\cap V$ cannot both be nonempty, so, after interchanging $U,V$, we have $C\subseteq U$. For any $v\in V$, the relatively open neighbourhood $V$ of $v$ in $\operatorname{Cl}(C)$ is disjoint from $C$, contradicting $v\in\operatorname{Cl}(C)$. Therefore the [closure of a connected set](../../../../../closure-of-a-connected-set.md) is connected.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
