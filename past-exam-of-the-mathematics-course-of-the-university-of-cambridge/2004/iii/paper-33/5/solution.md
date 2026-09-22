<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The total processing time $\sum_{i=1}^{40}t_i$ is constant for a single machine, so only the initial setup and changeover sum depends on the order. Use the [dummy-job reduction for sequence-dependent setup times](../../../../../dummy-job-reduction-for-sequence-dependent-setup-times.md). Add [vertex](../../../../../vertex-graph-theory.md) $0$, and set

$$
c_{0i}=s_i,\qquad c_{ij}=s_{ij}\quad(i,j\ne0,\ i\ne j),
\qquad c_{i0}=0.
$$

Let the binary variable $x_{ij}$ indicate that $j$ follows $i$ in the augmented tour. A [Hamiltonian cycle](../../../../../hamilton-cycle.md) through $0$ specifies exactly one schedule, read starting after $0$. An exact [integer programming](../../../../../integer-programming.md) formulation is

$$
\boxed{\begin{aligned}
\min\quad&\sum_{i=1}^{40}t_i+
\sum_{\substack{i,j\in\{0,\ldots,40\}\\i\ne j}}c_{ij}x_{ij}\\
\text{subject to}\quad&
\sum_{j\ne i}x_{ij}=1\quad(i=0,\ldots,40),\\
&\sum_{i\ne j}x_{ij}=1\quad(j=0,\ldots,40),\\
&\sum_{\substack{i,j\in S\\i\ne j}}x_{ij}\leq |S|-1
\quad(\varnothing\ne S\subsetneq\{0,\ldots,40\}),\\
&x_{ij}\in\{0,1\}.
\end{aligned}}
$$

The degree equations alone describe a [cycle cover of a directed graph](../../../../../cycle-cover-of-a-directed-graph.md), possibly several separate [graph cycles](../../../../../cycle-in-a-graph.md). The [subtour elimination constraints](../../../../../subtour-elimination-constraints.md) exclude every proper directed [graph cycle](../../../../../cycle-in-a-graph.md); the cover is therefore a single tour through all jobs. Conversely every schedule supplies a feasible tour with exactly its completion time as objective. Exponentially many written inequalities are permitted in this exact formulation; an implementation may add them only when violated.

For three parallel machines, the relevant objective is the [parallel-machine makespan with sequence-dependent setups](../../../../../parallel-machine-makespan-with-sequence-dependent-setups.md), not simply total setup cost. Partition jobs into three ordered lists $\pi_r$. For a nonempty list define

$$
C_r=s_{\pi_r(1)}+\sum_{i\in\pi_r}t_i+
\sum_{h=1}^{|\pi_r|-1}s_{\pi_r(h),\pi_r(h+1)};
$$

an empty machine has $C_r=0$. Minimize $C_{\max}$ subject to $C_r\leq C_{\max}$ for each machine and each job assigned once. This can be written as a mixed-integer extension with assignment variables, one dummy tour per machine and conditional subtour cuts.

A practical strategy starts with a balanced assignment, sequences each machine using the single-machine methods, and improves by relocating or swapping jobs between machines together with within-machine [2-opt](../../../../../2-opt.md) moves. Score each move by its change in $\max_r C_r$. [Branch and bound](../../../../../branch-and-bound.md) can combine machine-assignment decisions with within-machine assignment bounds. For nonnegative times, the total processing time divided by three and the largest individual processing time are valid lower bounds, supplemented by setup-dependent route bounds. **Balancing processing and changeovers jointly is essential; independently minimizing the three tour costs does not by itself minimize completion time.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
