<h1 id="b/8/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [logarithmic barrier](../../../../../logarithmic-barrier.md) is

$$
\boxed{\Psi(x,\mu)=x^TAx-\mu\log(1-x^Tx),\qquad\|x\|_2<1,\quad\mu>0.}
$$

Its [gradient](../../../../../gradient.md) is $2Ax+2\mu x/(1-x^Tx)$. Thus every nonzero stationary point satisfies

$$
\boxed{Ax=\lambda_1x,\qquad\lambda_1=-\frac\mu{1-\|x\|_2^2}<0,\qquad\|x\|_2^2=1+\mu/\lambda_1.}
$$

A fixed negative-eigenvalue branch exists for $0<\mu<-\lambda_1$. The zero point is stationary for every $\mu$ as well, and it is not an [eigenvector](../../../../../eigenvector.md); at zero the displayed scalar $-\mu$ need not be an [eigenvalue](../../../../../eigenvalue.md) of $A$. Thus the claimed eigenvalue conclusion requires the nonzero-point qualification. This distinction is essential for the following Hessian analysis.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
