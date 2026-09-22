<h1 id="16h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the [axiom of choice](../../../../../../axiom-of-choice.md), identify every infinite cardinal $\kappa$ with its [initial ordinal](../../../../../../initial-ordinal.md). We prove $\kappa^2=\kappa$ by [transfinite induction](../../../../../../transfinite-induction.md) on infinite cardinals. The countable case follows from the usual diagonal enumeration of $\mathbb N\times\mathbb N$.

For the induction step, well-order the [Cartesian product](../../../../../../cartesian-product.md) $\kappa\times\kappa$ by first comparing

$$
\max\{\alpha,\beta\}
$$

and then using lexicographic order among pairs with the same maximum. The predecessors of $(\alpha,\beta)$ lie in $(\eta+1)\times(\eta+1)$, where $\eta=\max\{\alpha,\beta\}<\kappa$. Put $\mu=|\eta+1|<\kappa$. If $\mu$ is infinite, the induction hypothesis makes this predecessor set have cardinal at most $\mu^2=\mu<\kappa$; if $\mu$ is finite, the same conclusion is immediate.

Let $\theta$ be the order type of this well-order. Every proper initial segment of $\theta$ therefore has cardinal less than $\kappa$. Hence $\theta<\kappa^+$, since otherwise its initial segment of order type $\kappa$ would have cardinal $\kappa$. Thus $|\kappa\times\kappa|=|\theta|\leq\kappa$. The map $\alpha\mapsto(\alpha,0)$ gives the reverse injection, and the [Cantor-Schröder-Bernstein theorem](../../../../../../cantor-schroder-bernstein-theorem.md) yields

$$
\boxed{\kappa^2=\kappa.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16H](../../16h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
