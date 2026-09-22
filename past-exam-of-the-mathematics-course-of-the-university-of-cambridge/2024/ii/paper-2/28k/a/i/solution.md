<h1 id="28k/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $E_n$ be the holding time in state $n$. The variables are independent with $E_n\sim\operatorname{Exp}(n\lambda)$, and the explosion time would be

$$
T_\infty=\sum_{n\geq1}E_n.
$$

For $s>0$,

$$
\mathbb E e^{-sT_\infty}
=\prod_{n\geq1}\frac{n\lambda}{n\lambda+s}.
$$

This product is zero because  
$\sum_n\log(1+s/(n\lambda))=\infty$. If $T_\infty$ were finite with positive probability, the nonnegative variable $e^{-sT_\infty}$ would have positive expectation. Therefore $T_\infty=\infty$ almost surely, and the [Yule process](../../../../../../../yule-process.md) is nonexplosive.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [28K](../../../28k.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
