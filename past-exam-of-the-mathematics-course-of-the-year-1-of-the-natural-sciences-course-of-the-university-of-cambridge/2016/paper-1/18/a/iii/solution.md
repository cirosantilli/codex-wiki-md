<h1 id="18/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [binomial series](../../../../../../binomial-series.md) gives $(1+\epsilon)^{-\alpha}=1-\alpha\epsilon+O(\epsilon^2)$. Therefore

$$
U_\epsilon=\frac{\epsilon}{\alpha\epsilon+O(\epsilon^2)}\longrightarrow\frac1\alpha.
$$

To justify the limiting approximation over the infinite interval, also use the right-endpoint sum. It is $L_\epsilon=(1+\epsilon)^{-1-\alpha}U_\epsilon$, and monotonicity gives $L_\epsilon\leq I\leq U_\epsilon$. Both bounds have the same limit. The [geometric partition bounds for a power-law improper integral](../../../../../../geometric-partition-bounds-for-a-power-law-improper-integral.md) and the [squeeze theorem](../../../../../../squeeze-theorem.md) thus prove

$$
\boxed{I=\frac1\alpha,\qquad\alpha>0.}
$$

This bounding argument matters because the geometric partition has unbounded widths far along the half-line; a finite-interval maximum-mesh argument cannot simply be applied to the entire infinite partition at fixed $\epsilon$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [18](../../../18.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
