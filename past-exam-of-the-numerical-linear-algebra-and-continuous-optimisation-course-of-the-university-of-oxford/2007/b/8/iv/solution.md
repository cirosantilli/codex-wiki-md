<h1 id="b/8/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $d=1-x^Tx>0$. Differentiating the barrier [gradient](../../../../../gradient.md) gives

$$
\boxed{H=2A+\frac{2\mu}dI+\frac{4\mu}{d^2}xx^T.}
$$

At a nonzero stationary point on the branch $Ax=\lambda_1x$, $\mu/d=-\lambda_1$. Choose an orthonormal eigenbasis of the symmetric matrix $A$ whose first vector is $x/\|x\|_2$. On each of the remaining eigenvectors the rank-one term vanishes, so the corresponding Hessian eigenvalues are

$$
\boxed{2(\lambda_i-\lambda_1),\qquad i=2,\ldots,n.}
$$

Along $x$, the first two terms cancel and the remaining eigenvalue is

$$
\boxed{\frac{4\mu\|x\|_2^2}{d^2}=\frac{4\lambda_1^2\|x\|_2^2}{\mu}.}
$$

If $\lambda_1$ repeats, a transverse eigenvalue can be zero. If a lower eigenvalue than $\lambda_1$ exists, a transverse eigenvalue is negative, identifying this stationary branch as a saddle rather than a minimum.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
