<h1 id="3/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a smooth approximation, the [fundamental theorem of calculus](../../../../../../../fundamental-theorem-of-calculus.md) and [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) give

$$
|u_n(x)-u_n(y)|\le\int_{[x,y]}|u_n'|\le|x-y|^{1/2}\|u_n'\|_{L^2(I)}.
$$

Let $E\subset I$ be one full-measure set on which $u_n\to u$. Passing to the limit for all $x,y\in E$ gives

$$
\boxed{\mathop{\mathrm{ess\,sup}}_{x\ne y}\frac{|u(x)-u(y)|}{|x-y|^{1/2}}\le\|u'\|_2\le\|u\|_{H^1(I)}.}
$$

The full-measure set $E$ is dense, and the estimate extends its representative uniquely to a $1/2$-[Hölder continuous function](../../../../../../../holder-condition.md) on $\overline I$. Its classical [Hölder seminorm](../../../../../../../holder-seminorm.md) satisfies the same bound. Changing the original representative on a null set does not affect the [essential supremum](../../../../../../../essential-supremum.md) in the assertion.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
