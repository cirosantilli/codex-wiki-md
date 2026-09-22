<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work with real-valued functions and put $\operatorname{sign}(0)=0$. Let $r=f-p_*$, and write an arbitrary competitor as $p=p_*+v$ with $v\in U$. Pointwise,

$$
|r-v|\geq |r|-v\,\operatorname{sign}(r).
$$

For $r\ne0$ this is $|r-v|\geq\operatorname{sign}(r)(r-v)$; for $r=0$ the right side is zero. Integrating and using the assumed orthogonality gives

$$
\|f-p\|_1=\int|r-v|
\geq\int|r|-\int v\,\operatorname{sign}(r)
=\|f-p_*\|_1.
$$

Thus **$p_*$ is a best $L^1$ approximation from $U$**. This [sign criterion for best L1 approximation](../../../../../../sign-criterion-for-best-l1-approximation.md) is sufficient without any finite-dimensionality or uniqueness assumption; possible residual zeros do not invalidate the inequality.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
