<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Mixed endpoint spectrum.** For $y''+\lambda y=0$, integration against $y$ and [integration by parts](../../../../../integration-by-parts.md), using $y(0)=0,y'(\pi/2)=0$, gives $\lambda\int y^2=\int(y')^2>0$ for every nonzero real [eigenfunction](../../../../../eigenfunction.md). Thus $\lambda=k^2>0$ and the first condition makes $y=A\sin(kx)$. The second requires $\cos(k\pi/2)=0$, so $k=2n+1$, $n\geq0$. Since

$$
\int_0^{\pi/2}\sin^2((2n+1)x)\,dx=\frac\pi4,
$$

the normalized [eigenfunctions](../../../../../eigenfunction.md) and [eigenvalues](../../../../../eigenvalue.md) are

$$
\boxed{u_n(x)=\frac2{\sqrt\pi}\sin((2n+1)x),\qquad\lambda_n=(2n+1)^2,\qquad n=0,1,\ldots.}
$$

The [orthogonality](../../../../../orthogonal-vectors.md) also follows by applying [integration by parts](../../../../../integration-by-parts.md) to two different [eigenfunctions](../../../../../eigenfunction.md) of the same [self-adjoint differential operator](../../../../../self-adjoint-differential-operator.md).

**Forced expansion.** Let $k_n=2n+1$ and write $x=\sum f_nu_n$, $y=\sum c_nu_n$. The [Fourier coefficients](../../../../../fourier-coefficient.md) of the forcing are

$$
f_n=\frac2{\sqrt\pi}\int_0^{\pi/2}x\sin(k_nx)\,dx=\frac{2(-1)^n}{\sqrt\pi\,k_n^2},
$$

because the boundary cosine vanishes and $\sin(k_n\pi/2)=(-1)^n$. Applying $d^2/dx^2+\kappa$ to the [eigenfunction expansion](../../../../../eigenfunction-expansion.md) gives $(\kappa-k_n^2)c_n=f_n$. Since $\kappa$ is not an [eigenvalue](../../../../../eigenvalue.md),

$$
\boxed{y(x)=\frac4\pi\sum_{n=0}^\infty\frac{(-1)^n\sin(k_nx)}{k_n^2(\kappa-k_n^2)}.}
$$

The coefficients are $O(k_n^{-4})$, so the series and its first two differentiated series converge absolutely and uniformly on the interval. Each term satisfies the two endpoint conditions, and $y''+\kappa y$ equals the mixed-endpoint [Fourier series](../../../../../fourier-series-split.md) of $x$. The forcing coefficients are $O(k_n^{-2})$, giving uniform convergence of that series as well. Uniqueness follows because the homogeneous problem has a nonzero solution only at one of the excluded [eigenvalues](../../../../../eigenvalue.md).

**Odd fourth-power sum.** Set $\kappa=0$. Direct integration of $y''=x$, with the same endpoint conditions, gives

$$
y(x)=\frac{x^3}6-\frac{\pi^2x}8,\qquad y(\pi/2)=-\frac{\pi^3}{24}.
$$

At $x=\pi/2$, the [eigenfunction expansion](../../../../../eigenfunction-expansion.md) instead gives $y(\pi/2)=-(4/\pi)\sum_{n\geq0}k_n^{-4}$. Equating the two values yields

$$
\boxed{\sum_{n=0}^\infty\frac1{(2n+1)^4}=1+\frac1{3^4}+\frac1{5^4}+\cdots=\frac{\pi^4}{96}.}
$$

Absolute and uniform convergence justify evaluation at the endpoint.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
