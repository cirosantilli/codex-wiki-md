<h1 id="13i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The recursive definition of [ordinal addition](../../../../../../ordinal-addition.md) is $\alpha+0=\alpha$, $\alpha+(\beta+1)=(\alpha+\beta)+1$, and $\alpha+\lambda=\sup_{\beta<\lambda}(\alpha+\beta)$ for a nonzero [limit ordinal](../../../../../../limit-ordinal.md) $\lambda$. The synthetic definition is the order type of the ordered disjoint union of a copy of $\alpha$ followed by a copy of $\beta$.

For the synthetic operation, adding the empty order does nothing, adding a successor appends one final point, and concatenation with a limit order is the increasing union of the initial concatenations with all its proper initial segments. Their order types have supremum $\sup_{\beta<\lambda}(\alpha+\beta)$. Thus the synthetic operation satisfies the recursive equations. [Transfinite induction](../../../../../../transfinite-induction.md) gives uniqueness of the recursively defined operation, proving equivalence.

The recursive definitions of [ordinal multiplication](../../../../../../ordinal-multiplication.md) and [ordinal exponentiation](../../../../../../ordinal-exponentiation.md) are

$$
\alpha\cdot0=0,\quad\alpha(\beta+1)=\alpha\beta+\alpha,\quad\alpha\lambda=\sup_{\beta<\lambda}\alpha\beta;
$$



$$
\alpha^0=1,\quad\alpha^{\beta+1}=\alpha^\beta\alpha,\quad\alpha^\lambda=\sup_{\beta<\lambda}\alpha^\beta.
$$

The last equation in each line is for nonzero limit $\lambda$. In particular the convention $0^0=1$ belongs to this recursive definition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13I](../../13i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
