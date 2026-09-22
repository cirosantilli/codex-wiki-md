<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Boundedness at the origin allows only $r^n$ for nonconstant interior modes; decay at infinity allows only $r^{-n}$ outside. Write the common surface potential in its [Fourier series](../../../../../fourier-series-split.md) as $\sum_{n\geq1}v_n(\theta)$, where $v_n=A_n\cos n\theta+B_n\sin n\theta$. Continuity then makes the corresponding interior and exterior factors $(r/R)^n$ and $(R/r)^n$.

Their outward radial derivatives at the surface are $nv_n/R$ inside and $-nv_n/R$ outside. Thus the jump is $-2nv_n/R$. Equating it to minus the prescribed surface-charge mode gives

$$
v_n(\theta)=\frac{R}{2n}(a_n\cos n\theta+b_n\sin n\theta).
$$

Therefore the [potential of a charged cylindrical shell with angular Fourier data](../../../../../potential-of-a-charged-cylindrical-shell-with-angular-fourier-data.md) is

$$
\boxed{\Phi(r,\theta)=\sum_{n=1}^\infty\frac{R}{2n}\begin{cases}(r/R)^n,&0\leq r\leq R,\\(R/r)^n,&r\geq R\end{cases}(a_n\cos n\theta+b_n\sin n\theta).}
$$

Either branch gives the same value at $R$. The mean angular mode is zero: outside, neither a constant nor a logarithm can survive the condition at infinity; continuity then forces the interior constant to zero. Consequently $\Phi(0)=0$.

The absence of a mean term in the [surface charge density](../../../../../surface-charge-density.md) is essential. A nonzero mean would require a logarithmic exterior potential and would be incompatible with decay at infinity in this two-dimensional reduction. The normalization follows the stated derivative jump, with no additional permittivity factor introduced.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
