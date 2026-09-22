<h1 id="7/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For distinct nonzero recurrence roots, the [determinant](../../../../../../determinant.md) formula gives

$$
\boxed{D_N=0\quad\Longleftrightarrow\quad\left(\frac{\beta_1}{\beta_2}\right)^{N+1}=1,\qquad\beta_1\ne\beta_2.}
$$

The ratio one is excluded: at that repeated root, part (iii) gives $(N+1)(\pm k)^N\ne0$. Thus the naive extra root corresponding to equal recurrence roots is spurious.

To count the physical solutions without ambiguity from exchanging $\beta_1$ and $\beta_2$, write $\beta_{1,2}=ke^{\pm iq}$ and $d=2k\cos q$ with $0<q<\pi$. Then

$$
D_N=k^N\frac{\sin[(N+1)q]}{\sin q}.
$$

Its $N$ distinct zeros occur at $q=j\pi/(N+1)$, $j=1,\ldots,N$. They give **exactly $N$ distinct positive normal frequencies**, or equivalently $N$ distinct roots in $\omega^2$:

$$
\omega_j=2\sqrt{\frac km}\sin\frac{j\pi}{2(N+1)}.
$$

If signed $\omega$ is counted, the [characteristic equation](../../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) has $2N$ roots $\pm\omega_j$. The sine quotient is the [Chebyshev polynomial of the second kind](../../../../../../chebyshev-polynomial-of-the-second-kind.md) representation of the [fixed-end spring-chain determinant and its repeated-root limit](../../../../../../fixed-end-spring-chain-determinant-and-its-repeated-root-limit.md).

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
