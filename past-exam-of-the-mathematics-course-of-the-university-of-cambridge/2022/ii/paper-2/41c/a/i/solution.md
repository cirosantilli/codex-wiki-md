<h1 id="41c/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Multiplication by $e^{-im\theta}$ and summation over $m\in\mathbb Z$ give

$$
\sum_m e^{-im\theta}u^n_{m+k}
=e^{ik\theta}\widehat u^{\,n}(\theta).
$$

Thus the recurrence becomes

$$
A(\theta)\widehat u^{\,n+1}(\theta)
=B(\theta)\widehat u^{\,n}(\theta),
$$

where

$$
A(\theta)=\sum_{k=r}^sa_ke^{ik\theta},
\qquad
B(\theta)=\sum_{k=r}^sb_ke^{ik\theta}.
$$

Assuming $A(\theta)\ne0$, the [amplification factor of a two-sided one-step stencil](../../../../../../../amplification-factor-of-a-two-sided-one-step-stencil.md) is

$$
\boxed{
H(\theta)=\frac{B(\theta)}{A(\theta)}
=\frac{\sum_{k=r}^sb_ke^{ik\theta}}
{\sum_{k=r}^sa_ke^{ik\theta}}
}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [41C](../../../41c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
