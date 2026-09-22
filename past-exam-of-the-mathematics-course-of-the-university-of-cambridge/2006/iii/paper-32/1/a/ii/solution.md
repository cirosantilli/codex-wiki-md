<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use conditional [monotone convergence](../../../../../../../monotone-convergence-theorem.md) and the [tower property of conditional expectation](../../../../../../../law-of-total-expectation.md) in the preceding construction:

$$
\begin{aligned}
\mathbb E[M_{n+1}\mid\mathcal F_n]
&=\lim_{p\to\infty}\mathbb E\bigl[\mathbb E[X_p^+\mid\mathcal F_{n+1}]\mid\mathcal F_n\bigr]\\
&=\lim_{p\to\infty}\mathbb E[X_p^+\mid\mathcal F_n]=M_n.
\end{aligned}
$$

This proves the [martingale](../../../../../../../martingale-split.md) property. The construction gives $M_n\geq0$ and $\sup_n\mathbb EM_n\leq C$, so $M$ is bounded in $L^1$. Taking $p=n$ in the increasing family also gives $M_n\geq X_n^+\geq X_n$. Define $Y_n=M_n-X_n$. Then $Y$ is nonnegative and adapted, and

$$
\mathbb E[Y_{n+1}\mid\mathcal F_n]
=M_n-\mathbb E[X_{n+1}\mid\mathcal F_n]\leq M_n-X_n=Y_n.
$$

Thus $Y$ is a [supermartingale](../../../../../../../supermartingale.md), with $\mathbb E|Y_n|\leq\mathbb EM_n+\mathbb E|X_n|\leq2C$. The requested conclusion is

$$
\boxed{X_n=M_n-Y_n,\qquad M\text{ a nonnegative }L^1\text{-bounded martingale},\quad Y\text{ a nonnegative }L^1\text{-bounded supermartingale}.}
$$

This [positive martingale majorant of an L1-bounded submartingale](../../../../../../../positive-martingale-majorant-of-an-l1-bounded-submartingale.md) is not asserted to have [uniform integrability](../../../../../../../uniform-integrability.md); boundedness in $L^1$ alone does not imply that stronger property.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
