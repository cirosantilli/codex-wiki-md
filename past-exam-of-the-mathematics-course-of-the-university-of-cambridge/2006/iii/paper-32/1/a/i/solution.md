<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $C=\sup_p\mathbb E|X_p|<\infty$. Since $x\mapsto x^+$ is an increasing [convex function](../../../../../../../convex-function.md), the [conditional Jensen inequality](../../../../../../../conditional-jensen-inequality.md) and the [submartingale](../../../../../../../submartingale.md) property give

$$
\mathbb E[X_{p+1}^+\mid\mathcal F_p]\geq\bigl(\mathbb E[X_{p+1}\mid\mathcal F_p]\bigr)^+\geq X_p^+.
$$

For fixed $n$ and $p\geq n$, the [tower property of conditional expectation](../../../../../../../law-of-total-expectation.md) therefore implies

$$
\mathbb E[X_{p+1}^+\mid\mathcal F_n]\geq\mathbb E[X_p^+\mid\mathcal F_n].
$$

Choose versions for this countable family so that all these inequalities hold outside one null set. Its nonnegative increasing limit $M_n$ is $\mathcal F_n$-measurable. The [monotone convergence theorem](../../../../../../../monotone-convergence-theorem.md) shows that

$$
\mathbb EM_n=\lim_{p\to\infty}\mathbb EX_p^+\leq C.
$$

In particular the limit is finite [almost surely](../../../../../../../almost-sure-convergence.md). Thus **the increasing conditional means converge to an integrable nonnegative $M_n$**, rather than merely to a possibly infinite extended value. This is the construction of the [positive martingale majorant of an L1-bounded submartingale](../../../../../../../positive-martingale-majorant-of-an-l1-bounded-submartingale.md).

## ↑ Ancestors (12)

1. [I](../i.md)
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
