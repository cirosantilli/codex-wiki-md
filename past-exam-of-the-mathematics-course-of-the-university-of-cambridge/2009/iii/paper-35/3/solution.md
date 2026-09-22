<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For [NP-completeness](../../../../../np-completeness.md), use the decision version with an objective threshold. A [permutation](../../../../../permutation.md) is a polynomial-size certificate, and its [quadratic assignment problem](../../../../../quadratic-assignment-problem.md) cost is computable in $O(n^2)$ arithmetic operations. To reduce the [travelling salesman problem](../../../../../travelling-salesman-problem.md), let $A$ be the adjacency matrix of a directed cycle on the facility labels: $a_{i,i+1}=1$, with indices cyclic, and every other entry zero. Let $B$ be the matrix of city-to-city distances. Then

$$
f(\pi)=\sum_{i=1}^n b_{\pi(i),\pi(i+1)},\qquad\pi(n+1)=\pi(1),
$$

which is exactly the tour length. Every tour arises from such a [permutation](../../../../../permutation.md). Hence the decision [QAP](../../../../../quadratic-assignment-problem.md) is [NP-complete](../../../../../np-completeness.md), and finding its optimal value is [NP-hard](../../../../../np-hardness.md). No factor of two appears in this directed-cycle construction, even when the distance matrix is symmetric.

Fix any complete assignment $\pi$. Its restriction to the facilities other than $i$ is an admissible bijection in the definition of $\ell_{i,\pi(i)}$, so

$$
\sum_{j\ne i}a_{ij}b_{\pi(i),\pi(j)}\geq\ell_{i,\pi(i)}.
$$

Summing this inequality over $i$ gives $f(\pi)\geq\sum_i\ell_{i,\pi(i)}$. Restricting to $\Pi_k$ and minimizing proves

$$
\boxed{\min_{\pi\in\Pi_k}f(\pi)\geq g(\Pi_k).}
$$

This is the [Gilmore-Lawler bound](../../../../../gilmore-lawler-bound.md). Its row minima may come from mutually incompatible assignments, so equality is not automatic. To find $g(\Pi_k)$, fix facility one at location $k$, delete that row and column from $L$, and solve the residual [assignment problem](../../../../../assignment-problem.md) using the [Hungarian algorithm](../../../../../hungarian-algorithm.md), adding $\ell_{1k}$ to its value.

For the supplied instance, the two residual assignment sums at each initial branch are

$$
\begin{aligned}
g(\Pi_1)&=31+\min(26+37,20+48)=94,\\
g(\Pi_2)&=38+\min(22+37,20+41)=97,\\
g(\Pi_3)&=29+\min(22+48,26+41)=96.
\end{aligned}
$$

Use [branch and bound](../../../../../branch-and-bound.md) to explore $\Pi_1$, the branch with smallest bound. Its minimizing linear assignment is $\pi=(1,2,3)$. Evaluating the true ordered-pair objective gives

$$
f(1,2,3)=2(2\cdot5+7\cdot3+4\cdot4)=94.
$$

This supplies an incumbent of value $94$ and meets the lower bound of $\Pi_1$. Alternatively, after branching on facility two, the other leaf $(1,3,2)$ has row-sum bound $31+20+48=99$ and is pruned. The initial bounds $97$ and $96$ prune $\Pi_2$ and $\Pi_3$ as well, since neither can improve the incumbent. Thus

$$
\boxed{\operatorname{OPT}=94,\qquad\pi=(1,2,3)\text{ is optimal}.}
$$

The factor two in this numerical evaluation is necessary because both matrices are symmetric and the objective counts both directions of each unordered pair.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
