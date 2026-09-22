<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By part (c), write $\lambda=\mu^2$ with $\mu>0$. The equation is $y''+\mu^2y=0$, and the left [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) eliminates the cosine term. Thus $y=A\sin(\mu x)$, with $A\ne0$. The right [Robin boundary condition](../../../../../robin-boundary-condition.md) becomes

$$
\mu\cos(\mu\ell)+k\sin(\mu\ell)=0.
$$

Put $z=\mu\ell$ and $\kappa=k\ell>0$. A root cannot have $\cos z=0$, so this is equivalent to $\tan z=-z/\kappa$.

On each interval $((n-1/2)\pi,n\pi)$, $n\geq1$, the function $\tan z+z/\kappa$ rises from $-\infty$ to a positive value and has derivative $\sec^2z+1/\kappa>0$. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) and strict [monotonicity](../../../../../monotonic-function.md) therefore give exactly one root $z_n$ there. On the intervening positive-tangent intervals both terms are positive, so there are no further positive roots. Consequently

$$
\boxed{\lambda_n=\frac{z_n^2}{\ell^2},\qquad y_n(x)=A_n\sin\frac{z_nx}{\ell},\qquad(n-\tfrac12)\pi<z_n<n\pi,\quad n=1,2,\ldots.}
$$

These intervals establish $\lambda_1<\lambda_2<\cdots$ and an infinite sequence of [eigenvalues](../../../../../eigenvalue.md). The apparent algebraic root $z=0$ of the sine equation is excluded: it gives a zero sine function, and the direct zero-eigenvalue solution $y=Ax$ would require $A(1+k\ell)=0$.

<a id="1/d/image-one-intersection-of-tan-z-with-z-kappa-on-each-negative-tangent-branch-the-illustration-uses-kappa-1"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2-2016-ib-robin-roots.png)

**[Figure 1](#1/d/image-one-intersection-of-tan-z-with-z-kappa-on-each-negative-tangent-branch-the-illustration-uses-kappa-1). One intersection of $\tan z$ with $-z/\kappa$ on each negative-tangent branch; the illustration uses $\kappa=1$**.

For [vector normalization](../../../../../vector-normalization.md) to unit [norm](../../../../../norm.md), the [Dirichlet-Robin eigenvalues on a finite interval](../../../../../dirichlet-robin-eigenvalues-on-a-finite-interval.md) give

$$
A_n=\left[\frac\ell2+\frac{k}{2(k^2+\lambda_n)}\right]^{-1/2}.
$$

The eigenfunctions can otherwise be scaled by any nonzero real constant.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
