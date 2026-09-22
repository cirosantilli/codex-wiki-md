<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply positive affine payoff transformations, if necessary, so both [payoff matrices](../../../../../../payoff-matrix.md) have strictly positive entries. Such transformations preserve [best responses](../../../../../../best-response.md) and [Nash equilibria](../../../../../../nash-equilibrium.md). The [Lemke-Howson algorithm](../../../../../../lemke-howson-algorithm.md) uses unnormalized nonnegative strategy vectors and [slack variables](../../../../../../slack-variable.md) satisfying

$$
\boxed{x\geq0,\quad Q^Tx+s=\mathbf1,\quad s\geq0;\qquad y\geq0,\quad Py+r=\mathbf1,\quad r\geq0.}
$$

Thus its two polytopes are $\{x\geq0:Q^Tx\leq\mathbf1\}$ and $\{y\geq0:Py\leq\mathbf1\}$. A label $i\leq m$ occurs when $x_i=0$ or $r_i=0$; a label $m+j$ occurs when $y_j=0$ or $s_j=0$. The [complementary pivoting](../../../../../../complementary-pivoting.md) path drops one label from the artificial zero pair and resolves each duplicated label until all labels return.

**Terminate at a completely labelled pair other than the artificial zero pair.** This is equivalent to [complementary slackness](../../../../../../complementary-slackness.md)

$$
x_ir_i=0\quad(1\leq i\leq m),\qquad y_js_j=0\quad(1\leq j\leq n).
$$

A nonzero completely labelled pair has both vectors nonzero: if $x=0$, then $s=\mathbf1$ forces $y=0$, and the converse is analogous. Normalize to [mixed strategies](../../../../../../mixed-strategy.md)

$$
p=\frac{x}{\mathbf1^Tx},\qquad q=\frac{y}{\mathbf1^Ty}.
$$

The inequalities $Py\leq\mathbf1$ imply that every row payoff against $q$ is at most $1/(\mathbf1^Ty)$, with equality on every row receiving positive probability in $p$. Thus $p$ is a [best response](../../../../../../best-response.md) to $q$. Likewise $q$ is a [best response](../../../../../../best-response.md) to $p$ using $Q^Tx+s=\mathbf1$. Hence $(p,q)$ is a [Nash equilibrium](../../../../../../nash-equilibrium.md). [Nondegeneracy of a bimatrix game](../../../../../../nondegeneracy-of-a-bimatrix-game.md) ensures the usual [complementary pivoting](../../../../../../complementary-pivoting.md) path has a unique continuation after the label choice.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
