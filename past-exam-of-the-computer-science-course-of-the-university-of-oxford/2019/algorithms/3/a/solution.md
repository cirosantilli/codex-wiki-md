<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A parameterized [decision problem](../../../../../decision-problem.md) is [fixed-parameter tractable](../../../../../fixed-parameter-tractability.md) if there is an [algorithm](../../../../../algorithm-split.md) deciding inputs of encoded length $N$ and parameter $k$ in [running time](../../../../../running-time.md) at most **$f(k)N^c$**, where $f$ is a computable [function](../../../../../function-split.md) and $c$ is a constant independent of $k$. Arbitrarily expensive dependence on the parameter is permitted; putting $k$ in the exponent of $N$ does not by itself establish [fixed-parameter tractability](../../../../../fixed-parameter-tractability.md).

For a minimization problem with nonnegative costs, a factor-two [approximation algorithm](../../../../../approximation-algorithm.md) runs in [polynomial time](../../../../../polynomial-time.md), always returns a [feasible solution](../../../../../feasible-point.md), and satisfies **$\operatorname{cost}(\operatorname{ALG})\leq2\operatorname{OPT}$** on every feasible input. A [feasible solution](../../../../../feasible-point.md) also satisfies $\operatorname{OPT}\leq\operatorname{cost}(\operatorname{ALG})$. If the optimum is zero, the guarantee requires an answer of zero cost.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
