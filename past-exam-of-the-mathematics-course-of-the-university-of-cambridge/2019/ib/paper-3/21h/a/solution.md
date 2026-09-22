<h1 id="21h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a set $B$ of $m$ column indices for which the square matrix $A_B$ is invertible. The associated [basic solution](../../../../../../basic-solution.md) sets $x_j=0$ for $j\notin B$ and solves $A_Bx_B=b$. It is a [basic feasible solution](../../../../../../basic-feasible-solution.md) when all its coordinates are nonnegative.

Let $x$ be a basic feasible solution with basis $B$. If $x=(y+z)/2$ for $y,z\in X(b)$, then $x_j=0$ and nonnegativity force $y_j=z_j=0$ for every $j\notin B$. Since $A_By_B=A_Bz_B=b$ and $A_B$ is invertible, $y=z=x$. Thus $x$ is an [extreme point](../../../../../../extreme-point.md).

Conversely, let $x$ be extreme and let $S=\{j:x_j>0\}$. If $|S|>m$, the corresponding columns are linearly dependent, so there is a nonzero vector $d$ supported on $S$ with $Ad=0$. For sufficiently small $\varepsilon>0$, both $x+\varepsilon d$ and $x-\varepsilon d$ remain nonnegative and feasible, contradicting extremality. Hence $|S|\leq m$. Enlarge $S$ to a set $B$ of $m$ indices. By the hypotheses $A_B$ is invertible, and $x$ is the resulting basic feasible solution. Therefore

$$
\boxed{\text{the extreme points of }X(b)\text{ are exactly the basic feasible solutions}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
