<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The intersection–union definition of a [submodular set function](../../../../../submodular-set-function.md) is

$$
f(A)+f(B)\geq f(A\cap B)+f(A\cup B)\qquad(A,B\subseteq V).
$$

The [diminishing returns characterization of submodularity](../../../../../diminishing-returns-characterization-of-submodularity.md) says that its [marginal increments](../../../../../marginal-increment-of-a-set-function.md) decrease as the conditioning [set](../../../../../set-split.md) grows:

$$
\Delta_x f(A):=f(A\cup\{x\})-f(A)\geq f(B\cup\{x\})-f(B)=:\Delta_x f(B)
\quad(A\subseteq B,\ x\notin B).
$$

To obtain [diminishing returns](../../../../../diminishing-returns-characterization-of-submodularity.md) from [submodularity](../../../../../submodular-set-function.md), apply the intersection–union inequality to $A\cup\{x\}$ and $B$. Their [intersection](../../../../../set-intersection.md) is $A$ and their [union](../../../../../set-union.md) is $B\cup\{x\}$, giving exactly the displayed comparison.

Conversely, assume [diminishing returns](../../../../../diminishing-returns-characterization-of-submodularity.md), and enumerate $A\setminus B=\{x_1,\ldots,x_m\}$. Put $C_j=(A\cap B)\cup\{x_1,\ldots,x_j\}$ and $D_j=B\cup\{x_1,\ldots,x_j\}$. Since $C_{j-1}\subseteq D_{j-1}$ and $x_j\notin D_{j-1}$, summing the [marginal increment](../../../../../marginal-increment-of-a-set-function.md) comparisons gives the [telescoping sum](../../../../../telescoping-sum.md)

$$
f(A)-f(A\cap B)=\sum_{j=1}^m\Delta_{x_j}f(C_{j-1})
\geq\sum_{j=1}^m\Delta_{x_j}f(D_{j-1})=f(A\cup B)-f(B).
$$

Rearrangement proves [submodularity](../../../../../submodular-set-function.md). When $A\setminus B$ is empty, both sums are zero, so the proof includes that case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Combinatorial optimisation](../../../combinatorial-optimisation-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
