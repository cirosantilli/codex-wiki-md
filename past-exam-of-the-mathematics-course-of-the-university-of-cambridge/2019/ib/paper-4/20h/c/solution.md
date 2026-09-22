<h1 id="20h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the capacities are integers and begin with the zero flow. Inductively, if every edge flow is an integer, then every forward residual capacity $c(u,v)-f(u,v)$ and reverse residual capacity $f(u,v)$ is an integer. The bottleneck on an [augmenting path](../../../../../../augmenting-path.md) is therefore a positive integer. Augmenting by it changes every affected edge flow by an integer, so all edge flows remain integral.

Each augmentation raises the flow value by at least one. On the other hand, every feasible flow satisfies

$$
|f|\leq\sum_{v}c(S,v),
$$

and the right side is a finite integer because the network is finite. There can therefore be only finitely many augmentations. When the algorithm stops, no augmenting path remains, and the source-reachable cut in the residual network has capacity equal to the current flow value. The [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md) proves that the terminating flow is maximum. This proves both termination and the [Integrality of the Ford-Fulkerson algorithm](../../../../../../integrality-of-the-ford-fulkerson-algorithm.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20H](../../20h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
