# Radial random walk on a regular tree

↑ **Parent:** [Random walk on a graph](random-walk-on-a-graph.md)

For a [simple random walk](simple-random-walk.md) on an infinite [regular tree](regular-tree.md) of degree $z\geq2$, every [vertex](vertex-graph-theory.md) other than the chosen root has one neighbour closer to the root and $z-1$ farther away. The [graph distance](distance-graph-theory.md) from the root is therefore a nearest-neighbour [Markov chain](markov-chain-split.md) on the nonnegative integers, with the displayed bulk transition [probabilities](probability.md) and a certain outward step from zero. For shell [probabilities](probability.md) $P_r(N)$,

$$
P_0(N+1)=\frac{P_1(N)}z,\qquad
P_1(N+1)=P_0(N)+\frac{P_2(N)}z,
$$



$$
P_r(N+1)=\frac{z-1}{z}P_{r-1}(N)+\frac1zP_{r+1}(N),\qquad r>1.
$$

Shell [probabilities](probability.md) include all [vertices](vertex-graph-theory.md) at the given distance. They differ from single-vertex [probabilities](probability.md) by the shell size, $1$ at the root and $z(z-1)^{r-1}$ for $r\geq1$.

## ↑ Ancestors (9)

1. [Random walk on a graph](random-walk-on-a-graph.md)
2. [Random walk](random-walk-split.md)
3. [Markov chain](markov-chain-split.md)
4. [Markov process](markov-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/6/c/solution.md)
