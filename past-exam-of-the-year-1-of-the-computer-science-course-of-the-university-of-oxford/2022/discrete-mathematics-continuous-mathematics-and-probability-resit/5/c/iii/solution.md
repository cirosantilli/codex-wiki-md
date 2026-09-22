<h1 id="5/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use [mathematical induction](../../../../../../mathematical-induction.md) on the iteration. Initially $x_0=b=1\cdot b$. If $x_n=\lambda_nb$, then $Ax_n=\lambda_nb/2$, $x_n^Tb=\lambda_n$, and $x_n^TAx_n=\lambda_n^2/2$. Therefore

$$
\nabla h(x_n)=\tfrac32\lambda_n^2b.
$$

A [gradient descent](../../../../../../gradient-descent-split.md) step with any scalar step length $\alpha_n$ consequently has the form

$$
x_{n+1}=x_n-\alpha_n\nabla h(x_n)
=\left(\lambda_n-\tfrac32\alpha_n\lambda_n^2\right)b.
$$

Thus every iterate remains on the same [eigenline](../../../../../../eigenline.md), with

$$
\boxed{\lambda_0=1,\qquad
\lambda_{n+1}=\lambda_n-\tfrac32\alpha_n\lambda_n^2.}
$$

This proves that [gradient descent preserves an eigenline for a cubic product](../../../../../../gradient-descent-preserves-an-eigenline-for-a-cubic-product.md). The statement is invariance, not convergence to a minimum: along the negative direction of this line the [cubic polynomial](../../../../../../cubic-polynomial.md) objective is unbounded below.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
