<h1 id="o/o2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Independence and common error [variance](../../../../../../variance-split.md) give $\operatorname{Var}(\epsilon)=\sigma^2I_n$. For the fixed matrix $A=(X^TX)^{-1}X^T$, the [covariance](../../../../../../covariance.md) transformation rule gives

$$
\begin{aligned}
\operatorname{Var}(\widehat\theta)&=A\operatorname{Var}(\epsilon)A^T\\
&=\sigma^2(X^TX)^{-1}X^TX(X^TX)^{-1}\\
&=\boxed{\sigma^2(X^TX)^{-1}}.
\end{aligned}
$$

Thus the [covariance](../../../../../../covariance.md) is determined by the error [variance](../../../../../../variance-split.md) and the inverse [Gram matrix](../../../../../../gram-matrix.md) of the design columns.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [O2](../../../o2.md)
4. [O](../../../../o.md)
5. [2012](../../../../../2012-split.md)
6. [Past exam of the options I course of the University of Oxford](../../../../../split.md)
7. [Options I course of the University of Oxford](../../../../../../options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
