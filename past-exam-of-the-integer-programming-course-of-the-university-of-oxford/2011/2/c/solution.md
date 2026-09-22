<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each [branch and bound](../../../../branch-and-bound.md) node, relax the unfixed binary variables to $[0,1]$. The [fractional knapsack problem](../../../../fractional-knapsack-problem.md) is solved by decreasing profit-to-weight ratios, here

$$
\frac{15}2>\frac{18}3>\frac{21}4>\frac{25}5.
$$

Its value is an upper bound for the node's [integer](../../../../integer-split.md) optimum. At the root, greedy filling gives $x=(1,1,1/2,0)$ and upper bound $\boxed{43.5}$, so branch on $x_3$.

In the child $x_3=0$, the relaxed optimum is $(1,1,0,2/5)$ with value $43$. Branch on $x_4$. Taking $x_4=1$ leaves capacity two, giving the integral solution $(1,0,0,1)$ of value $40$, our incumbent. Taking $x_4=0$ gives the integral relaxed optimum $(1,1,0,0)$ of value $33$, so that node is closed.

In the child $x_3=1$, item four cannot be selected in any [integer](../../../../integer-split.md) feasible solution, since their combined weight is nine. Fixing $x_4=0$ is therefore valid binary feasibility propagation. Its LP optimum is $(1,1/3,1,0)$ with value $42$. Branch on $x_2$. The child $x_2=1$ leaves no residual capacity and has integral solution $(0,1,1,0)$ of value $39$. The child $x_2=0$ has integral solution $(1,0,1,0)$ of value $36$. Both are below the incumbent.

The complete short search is

$$
\begin{array}{l|c|c}
\text{Node restrictions}&\text{LP upper bound}&\text{Outcome}\\\hline
\text{none}&43.5&\text{branch on }x_3\\
x_3=0&43&\text{branch on }x_4\\
x_3=0,\ x_4=1&40&\text{integral incumbent}\\
x_3=0,\ x_4=0&33&\text{close}\\
x_3=1,\ x_4=0&42&\text{branch on }x_2\\
x_3=1,\ x_4=0,\ x_2=1&39&\text{close}\\
x_3=1,\ x_4=0,\ x_2=0&36&\text{close}
\end{array}
$$

All [integer](../../../../integer-split.md) feasible solutions lie in these branches, and every terminal node is integral with value at most forty. Therefore the LP bounds and incumbent certify $\boxed{z_{\mathrm{IP}}=40}$ independently of the dynamic program.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
