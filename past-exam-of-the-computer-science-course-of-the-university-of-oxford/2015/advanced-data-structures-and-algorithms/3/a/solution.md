<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Using the [standard maximum form of a linear program](../../../../../standard-maximum-form-of-a-linear-program.md), write

$$
\boxed{\max c^Tx\quad\text{subject to }Ax\leq b,\quad x\geq0,}
$$

where $x\in\mathbb R^n$, $A\in\mathbb R^{m\times n}$, $b\in\mathbb R^m$, and $c\in\mathbb R^n$. The inequalities are coordinatewise, and $c^Tx$ is the [objective function](../../../../../objective-function.md). General [linear programs](../../../../../linear-programming-split.md) can be put in this form: reverse the sign of a minimization [objective function](../../../../../objective-function.md), reverse lower-bound [linear inequalities](../../../../../linear-inequality.md), replace an equality by two opposite [linear inequalities](../../../../../linear-inequality.md), and replace each unrestricted variable by the difference of two nonnegative variables. Some conventions instead call the equality-constraint version standard form; the convention here is the maximum-with-upper-bounds convention.

Introduce nonnegative [slack variables](../../../../../slack-variable.md) $x_{n+i}=b_i-\sum_{j=1}^n a_{ij}x_j$. The equivalent [slack form of a linear program](../../../../../slack-form-of-a-linear-program.md) is

$$
\boxed{
\begin{aligned}
z&=\sum_{j=1}^n c_jx_j,\\
x_{n+i}&=b_i-\sum_{j=1}^n a_{ij}x_j\quad(1\leq i\leq m),\\
x_j&\geq0\quad(1\leq j\leq n+m).
\end{aligned}}
$$

The original variables are initially nonbasic and the [slack variables](../../../../../slack-variable.md) basic. More generally, a [slack form of a linear program](../../../../../slack-form-of-a-linear-program.md) specifies disjoint index [sets](../../../../../set-split.md) $N,B$ and writes

$$
z=v+\sum_{j\in N}c_jx_j,\qquad
x_i=b_i-\sum_{j\in N}a_{ij}x_j\quad(i\in B),\qquad
x_i\geq0\quad(i\in N\cup B).
$$

Thus each [basic variable](../../../../../basic-variable.md) and the [objective function](../../../../../objective-function.md) are expressed using only [nonbasic variables](../../../../../nonbasic-variable.md). Setting all [nonbasic variables](../../../../../nonbasic-variable.md) to zero gives the associated [basic solution](../../../../../basic-solution.md), which is a [feasible solution](../../../../../feasible-point.md) exactly when the resulting basic values are nonnegative. The [slack form of a linear program](../../../../../slack-form-of-a-linear-program.md) does not itself require that initial [basic solution](../../../../../basic-solution.md) to be feasible.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
