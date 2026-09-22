<h1 id="o/o5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $A=(X^TX)^{-1}X^T$. Since $AX=I$, the estimator is $\widehat\theta=\theta+A\epsilon$. Therefore

$$
\boxed{\mathbb E\widehat\theta=\theta,\qquad
\operatorname{Var}(\widehat\theta)=A(\sigma^2I)A^T=\sigma^2(X^TX)^{-1}.}
$$

Its [expectation](../../../../../expected-value-split.md) proves unbiasedness. It is also jointly normal, being an affine transformation of the normal error [vector](../../../../../vector.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
