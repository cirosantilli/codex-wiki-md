# Nested conditioning keeps the coarser information

↑ **Parent:** [Law of total expectation](law-of-total-expectation.md)

For [integrable random variable](integrable-random-variable.md) $X$ and nested sub-[sigma-algebras](sigma-algebra.md) $\mathcal H\subseteq\mathcal G$, the [tower property](law-of-total-expectation.md) says

$$
\mathbb E[\mathbb E[X\mid\mathcal G]\mid\mathcal H]
=\mathbb E[X\mid\mathcal H].
$$

The finer-information [conditional mean](conditional-expectation.md) can be averaged within each coarser group, recovering the coarser-information [conditional mean](conditional-expectation.md). Conversely, conditioning an already $\mathcal H$-measurable [conditional mean](conditional-expectation.md) on $\mathcal G$ leaves it unchanged. Both orders therefore recover $\mathbb E[X\mid\mathcal H]$ when the information is nested.[Theorem 4.1.13, p. 212](probability-theory-and-examples-fifth-edition-by-rick-durrett/4-1-conditional-expectation.md)

For the finite example in [law of total expectation](law-of-total-expectation.md), exact knowledge of $X$ gives the finer mean $X$ itself. Averaging within the groups $A,B$ recovers two and eight. Forgetting the group then gives $13/2$. The nesting condition is essential; [iterated conditional expectation over nonnested sigma-algebras](iterated-conditional-expectation-over-nonnested-sigma-algebras.md) describes why arbitrary successive conditioning cannot simply be replaced by conditioning on an intersection.

## ↑ Ancestors (8)

1. [Law of total expectation](law-of-total-expectation.md)
2. [Conditional expectation](conditional-expectation.md)
3. [Measure theory](measure-theory-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
