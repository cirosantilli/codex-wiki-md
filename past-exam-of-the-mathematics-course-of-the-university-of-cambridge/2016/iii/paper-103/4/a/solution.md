<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a cell $x=(i,j)$ in a [Young diagram](../../../../../../young-diagram.md), its [hook of a Young diagram](../../../../../../hook-of-a-young-diagram.md) consists of $x$, all cells to its right in row $i$, and all cells below it in column $j$. If $\lambda'$ is the conjugate partition, its [hook length](../../../../../../hook-length.md) is

$$
h(i,j)=\lambda_i-j+\lambda'_j-i+1.
$$

The [hook-length formula](../../../../../../hook-length-formula.md) is

$$
\boxed{f_\lambda=\frac{n!}{\prod_{x\in\lambda}h(x)}}.
$$

In the [Greene–Nijenhuis–Wilf hook walk](../../../../../../greene-nijenhuis-wilf-hook-walk.md), a walk at a noncorner cell chooses uniformly one of the other $h(i,j)-1$ cells in its hook, and stops at a corner. Moves are strictly rightwards or downwards, so termination is certain. A terminal cell must be a [Removable node of a Young diagram](../../../../../../removable-node-of-a-young-diagram.md). For a chosen corner $(\alpha,\beta)$, its probability is zero unless the start satisfies $a\leq\alpha$ and $b\leq\beta$.

For a start in that northwest rectangle, define

$$
A_i=h(i,\beta)-1=\lambda_i-\beta+\alpha-i,\qquad
B_j=h(\alpha,j)-1=\beta-j+\lambda'_j-\alpha.
$$

The corner conditions are $\lambda_\alpha=\beta$ and $\lambda'_\beta=\alpha$, so $A_\alpha=B_\beta=0$, and all earlier $A_i,B_j$ are positive. Define

$$
F_\alpha=1,\qquad
F_a=\frac1{A_a}\prod_{i=a+1}^{\alpha-1}\left(1+\frac1{A_i}\right)\quad(a<\alpha),
$$

and

$$
G_\beta=1,\qquad
G_b=\frac1{B_b}\prod_{j=b+1}^{\beta-1}\left(1+\frac1{B_j}\right)\quad(b<\beta).
$$

Then **the closed conditional probability is**

$$
\boxed{p(\alpha,\beta\mid a,b)=F_aG_b}.
$$

In particular, if both inequalities are strict, this is

$$
\frac{1}{(h(a,\beta)-1)(h(\alpha,b)-1)}
\prod_{i=a+1}^{\alpha-1}\left(1+\frac1{h(i,\beta)-1}\right)
\prod_{j=b+1}^{\beta-1}\left(1+\frac1{h(\alpha,j)-1}\right).
$$

The separate definitions of $F_\alpha,G_\beta$ handle starts in the terminal row, in the terminal column, or at the corner itself without division by zero.

To prove the formula, the product definitions give the identities

$$
A_iF_i=\sum_{r=i+1}^{\alpha}F_r,\qquad
B_jG_j=\sum_{s=j+1}^{\beta}G_s,
$$

with the terminal zero identities interpreted as empty sums. For example, summing the $F$ recurrence backwards gives $\sum_{r=i+1}^\alpha F_r=\prod_{r=i+1}^{\alpha-1}(1+A_r^{-1})$. Also

$$
h(i,j)-1=A_i+B_j.
$$

The first-step equation for the [hook walk terminal probability](../../../../../../hook-walk-terminal-probability.md) is

$$
(h(i,j)-1)p_{i,j}
=\sum_{r=i+1}^{\alpha}p_{r,j}+\sum_{s=j+1}^{\beta}p_{i,s}.
$$

Jumps beyond the target rectangle contribute zero. Substituting $p_{i,j}=F_iG_j$ proves this equation, and $p_{\alpha,\beta}=1$ gives its boundary value. Since every step increases a coordinate, backward recursion determines the probability uniquely. This proves the claimed expression.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
