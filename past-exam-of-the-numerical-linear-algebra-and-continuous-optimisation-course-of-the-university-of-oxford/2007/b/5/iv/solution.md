<h1 id="b/5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The true quadratic has $g(x)=c+Hx$ and the exact expansion

$$
f(x+s)=f(x)+g(x)^Ts+\frac12s^THs.
$$

Subtracting the model with Hessian $I$ yields $f(x+s)-m(s)=\tfrac12s^T(H-I)s$. Since $H$ is symmetric positive definite and $\|H\|_2=1$, its [eigenvalues](../../../../../eigenvalue.md) lie in $(0,1]$, so $\|H-I\|_2\leq1$. Therefore

$$
\boxed{|f(x+s)-m(s)|\leq\frac12\|s\|_2^2\leq\frac12\Delta^2\leq\Delta^2.}
$$

In fact the stated assumptions give a factor one-half better than the requested bound.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [5](../../5.md)
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
