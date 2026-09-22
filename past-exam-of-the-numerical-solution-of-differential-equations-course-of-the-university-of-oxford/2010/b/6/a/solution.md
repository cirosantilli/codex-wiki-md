<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With zero boundary values eliminated, the diagonal of $L_h$ is $-4I/h^2$. The [Jacobi method](../../../../../jacobi-method.md) is therefore

$$
J=I+\tfrac14h^2L_h,
$$

which averages the four neighboring components. The [sine](../../../../../sine.md) addition identity shows that the supplied product vectors are [eigenvectors](../../../../../eigenvector.md), with

$$
\boxed{\lambda_{pq}(J)=\tfrac12[\cos(p\pi h)+\cos(q\pi h)].}
$$

The discrete [sine](../../../../../sine.md) vectors form a basis, so these are all [eigenvalues](../../../../../eigenvalue.md). Their largest modulus is

$$
\boxed{\rho(J)=\cos(\pi h),}
$$

attained at the lowest and highest [sine](../../../../../sine.md) frequencies. Thus the asymptotic error reduction factor per iteration is $\cos(\pi h)$. If the convergence rate is expressed logarithmically, $R=-\log\rho(J)\sim\pi^2h^2/2$ as $h\to0$. A fixed error reduction therefore takes $O(h^{-2})$ Jacobi sweeps. For the special grid $m=2$, $J=0$ and one sweep solves its single interior equation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
