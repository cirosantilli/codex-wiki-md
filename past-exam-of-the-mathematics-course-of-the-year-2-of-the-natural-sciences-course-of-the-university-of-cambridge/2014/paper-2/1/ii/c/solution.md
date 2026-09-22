<h1 id="1/ii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expand the forcing and the solution in the normalized [eigenfunctions](../../../../../../eigenfunction.md): $1=\sum_n b_ny_n$ and $y=\sum_n c_ny_n$. Their coefficients are

$$
b_n=\int_1^e y_n(x)\frac{dx}{x}=\sqrt2\int_0^1\sin(n\pi t)dt=\frac{\sqrt2[1-(-1)^n]}{n\pi}.
$$

Since all $\lambda_n=n^2\pi^2-1$ are nonzero, the equation gives $c_n=b_n/\lambda_n$. Hence the required [Sturm-Liouville eigenfunction expansion](../../../../../../sturm-liouville-eigenfunction-expansion.md) is

$$
\boxed{y(x)=\sum_{\substack{n\geq1\\n\text{ odd}}}\frac{4\sin(n\pi\ln x)}{n\pi(n^2\pi^2-1)}.}
$$

This is [constant forcing in a logarithmic Dirichlet Sturm-Liouville problem](../../../../../../constant-forcing-in-a-logarithmic-dirichlet-sturm-liouville-problem.md). The coefficients are $O(n^{-3})$, so the solution series converges uniformly and has zero endpoint values. Applying $L$ is justified in the weighted square-integrable sense; the forcing sine series equals one at interior points, while its endpoint sums are zero. The equation is imposed in the interior, so this does not contradict the boundary conditions.

As an independent check, solving $-Y''-Y=1$ directly gives

$$
y(x)=\frac{\cos(\ln x-1/2)}{\cos(1/2)}-1.
$$

It has both zero endpoint values and satisfies $Ly=1$. The invertibility of the Dirichlet operator makes it the same solution as the expansion.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [Ii](../../ii.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
