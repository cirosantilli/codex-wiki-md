<h1 id="o/o4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $D^*=D-A$, with $A=(X^TX)^{-1}X^T$. Then $D^*X=0$, and therefore $D^*A^T=D^*X(X^TX)^{-1}=0$; its transpose also vanishes. Expanding gives

$$
DD^T=(A+D^*)(A+D^*)^T=(X^TX)^{-1}+D^*D^{*T}.
$$

Hence

$$
\boxed{\operatorname{Cov}(\widetilde\theta)=\sigma^2\left((X^TX)^{-1}+D^*D^{*T}\right)}.
$$

The difference from the least-squares covariance is positive semidefinite, since $v^TD^*D^{*T}v=\|D^{*T}v\|^2\geq0$. In particular its $i$th diagonal entry is $\sigma^2\sum_j(D^*_{ij})^2$, proving every stated [variance](../../../../../variance-split.md) inequality. For estimating $\theta_1$, **prefer least squares**: among linear unbiased estimators it has minimum [variance](../../../../../variance-split.md), and therefore minimum mean squared error in that class. A competitor can tie if the first row of $D^*$ is zero. This is the [Gauss-Markov theorem](../../../../../gauss-markov-theorem.md); it does not assert optimality against all biased or nonlinear estimators.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [O4](../../o4.md)
3. [O](../../../o.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
