<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $C>0$ and use the unnormalized sum convention for the penalty. The linear [soft-margin support vector machine](../../../../../../soft-margin-support-vector-machine.md) solves

$$
\boxed{\min_{w,b,\xi}\left\{\frac12\lVert w\rVert_2^2+C\sum_{i=1}^n\xi_i\right\}\quad\text{subject to}\quad y_i(w^Tx_i+b)\geq1-\xi_i,\quad\xi_i\geq0.}
$$

Eliminating the [slack variables of a support vector machine](../../../../../../slack-variables-of-a-support-vector-machine.md) gives $\frac12\lVert w\rVert^2+C\sum_i\max\{0,1-y_if(x_i)\}$, where $f(x)=w^Tx+b$ and the maximum is the [hinge loss](../../../../../../hinge-loss.md). The classifier uses the sign of $f$ and its [support-vector-machine decision boundary](../../../../../../support-vector-machine-decision-boundary.md) is $f=0$.

For clarity about [dual support vectors and margin degeneracy](../../../../../../dual-support-vectors-and-margin-degeneracy.md), let $\alpha_i$ be the multipliers of the margin constraints. The [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) give

$$
w=\sum_i\alpha_iy_ix_i,\qquad\sum_i\alpha_iy_i=0,\qquad0\leq\alpha_i\leq C,
$$



$$
\alpha_i\{y_if(x_i)-1+\xi_i\}=0,\qquad(C-\alpha_i)\xi_i=0.
$$

The dual [support vectors](../../../../../../support-vector.md) are those with $\alpha_i>0$. A coefficient strictly between $0$ and $C$ puts a point exactly on its margin boundary; a point with positive slack has $\alpha_i=C$. A zero coefficient implies zero slack and signed margin at least one. Geometrically one often counts all points with $y_if(x_i)\leq1$ as [support vectors](../../../../../../support-vector.md). At a degeneracy, equality can occur with $\alpha_i=0$, so the two descriptions need not coincide. Either convention supports the bound in the following part when stated consistently.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
