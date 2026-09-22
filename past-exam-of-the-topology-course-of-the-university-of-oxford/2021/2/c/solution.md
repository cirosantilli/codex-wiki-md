<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

Write $Z=\coprod_{n\in\mathbb N}X_n$, where each $X_n$ is a labelled copy of the [topological space](../../../../topological-space.md) $X$, with its [topological disjoint union](../../../../topological-disjoint-union.md) topology. Define the [bijection](../../../../bijection.md)

$$
\boxed{F:Z\longrightarrow\mathbb N\times X,\qquad F(x\text{ in }X_n)=(n,x).}
$$

For a [subset](../../../../subset.md) $U\subseteq\mathbb N\times X$, let $U_n=\{x\in X:(n,x)\in U\}$. By definition of the [topological disjoint union](../../../../topological-disjoint-union.md), $F^{-1}(U)$ is [open](../../../../open-set.md) in $Z$ exactly when each $U_n$ is [open](../../../../open-set.md) in $X$.

The same condition characterizes [open sets](../../../../open-set.md) in the [product topology](../../../../product-topology.md) on $\mathbb N\times X$. If $U$ is [open](../../../../open-set.md), the map $x\mapsto(n,x)$ is [continuous](../../../../continuous-function.md), so each $U_n$ is [open](../../../../open-set.md). Conversely, if each $U_n$ is [open](../../../../open-set.md), then

$$
U=\bigcup_{n\in\mathbb N}(\{n\}\times U_n)
$$

is [open](../../../../open-set.md), since the [discrete topology](../../../../discrete-space.md) makes every $\{n\}$ [open](../../../../open-set.md) in $\mathbb N$. Hence $F$ and its [inverse function](../../../../inverse-function.md) are [continuous](../../../../continuous-function.md), proving the required [homeomorphism](../../../../homeomorphism.md). This also covers the case $X=\varnothing$.

## ↑ Ancestors (12)

1. [c](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the topology course of the University of Oxford](../../../split.md)
5. [Topology course of the University of Oxford](../../../../topology-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
