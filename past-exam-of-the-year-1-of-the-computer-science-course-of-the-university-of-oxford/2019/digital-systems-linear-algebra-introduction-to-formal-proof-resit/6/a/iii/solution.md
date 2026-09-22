<h1 id="6/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Real symmetry and positive definiteness are sufficient**, and the preceding parts establish both properties for this [matrix](../../../../../../matrix.md). If a residual becomes zero, stop: the solution has been reached and the displayed step quotient should not be evaluated as $0/0$.

For a convergence justification, let $x_*$ solve $Ax_*=b$, let $e=x_*-x$, and let $r=Ae$. The quadratic energy error is $E=e^TAe/2$. Moving by $\alpha r$, with $\alpha=(r^Tr)/(r^TAr)$, is [exact line search for a positive-definite quadratic](../../../../../../exact-line-search-for-a-positive-definite-quadratic.md) and gives

$$
E_{\rm new}=E-\frac{(r^Tr)^2}{2r^TAr}.
$$

Writing $\lambda_{\min},\lambda_{\max}>0$ for the extreme [eigenvalues](../../../../../../eigenvalue.md), one has $r^TAr\le\lambda_{\max}r^Tr$ and $r^Tr=e^TA^2e\ge\lambda_{\min}e^TAe$. Therefore

$$
E_{\rm new}\le\left(1-\frac{\lambda_{\min}}{\lambda_{\max}}\right)E.
$$

The factor lies below one, so the energy tends to zero and positive definiteness forces $x\to x_*$. Here the bound is $E_{\rm new}\le(10/11)E$, since the [eigenvalues](../../../../../../eigenvalue.md) are 1 and 11. This proves convergence for every initial [vector](../../../../../../vector.md), rather than merely checking one numerical iteration.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof resit](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
