<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrating the two linear pieces gives the [cumulative distribution function](../../../../../../../cumulative-distribution-function.md)

$$
F(x)=\begin{cases}
0,&x<1,\\(x-1)^2/12,&1\le x\le3,\\1-(7-x)^2/24,&3\le x\le7,\\1,&x>7.
\end{cases}
$$

The split probability is $F(3)=1/3$. Invert each branch to obtain the [method of inversion](../../../../../../../inverse-transform-sampling.md):

$$
\boxed{X=\begin{cases}1+\sqrt{12U},&0\le U\le1/3,\\7-\sqrt{24(1-U)},&1/3<U\le1.\end{cases}}
$$

Both expressions equal three at the split. For an ideal uniform draw, monotonicity gives $\mathbb P(F^{-1}(U)\le x)=\mathbb P(U\le F(x))=F(x)$, proving the target law. **Inversion is preferable here**: its quantile is explicit, it uses one uniform and one square root per output, and has no rejected draws. Rejection remains useful for densities with no convenient inverse CDF.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
