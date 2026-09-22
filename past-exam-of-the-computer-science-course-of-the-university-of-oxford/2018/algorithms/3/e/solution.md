<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Combine all inequalities, including nonnegativity, into $Cx\leq d$; explicitly, the rows $-e_j^Tx\leq0$ encode $x_j\geq0$. Let $x_*$ be a [vertex of a linear polyhedron](../../../../../vertex-of-a-linear-polyhedron.md), equivalently an [extreme point](../../../../../extreme-point.md) of the feasible [linear polyhedron](../../../../../linear-polyhedron.md), and let $I$ index the [active constraints](../../../../../active-constraint.md) there.

Suppose the active row normals have [rank](../../../../../rank-one-quadratic-form.md) smaller than $n$. By the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) there is a nonzero [vector](../../../../../vector.md) $h$ with $C_ih=0$ for every $i\in I$. Every inactive row has positive [slack variable](../../../../../slack-variable.md) value $s_i=d_i-C_ix_*>0$. Since there are only finitely many rows, choose $\varepsilon>0$ so small that

$$
\varepsilon|C_ih|<s_i\qquad\text{for every inactive row with }C_ih\ne0.
$$

Then both $x_*+\varepsilon h$ and $x_*-\varepsilon h$ are [feasible points](../../../../../feasible-point.md): the [active constraints](../../../../../active-constraint.md) remain equalities and no inactive inequality is violated. They are distinct, and $x_*$ is their [midpoint](../../../../../midpoint.md), contradicting the [extreme point](../../../../../extreme-point.md) property.

Therefore the active row normals have [rank](../../../../../rank-one-quadratic-form.md) $n$, and **at least $n$ [linearly independent](../../../../../linear-independence.md) constraints are satisfied with equality**. In particular at least $n$ constraints are tight, as claimed. Nonnegativity bounds must be counted: for example, at the origin these can supply all $n$ active rows. Degeneracy can make more than $n$ constraints tight, so the result does not assert exactly $n$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
