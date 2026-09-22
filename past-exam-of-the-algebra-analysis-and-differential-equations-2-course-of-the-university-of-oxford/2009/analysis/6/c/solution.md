<h1 id="analysis/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a small positively oriented circle $|w|=\rho$ in $U$ within the convergence disk of the inverse series. Cauchy's coefficient formula gives

$$
c_n=\frac1{2\pi i}\int_{|w|=\rho}\frac{g(w)}{w^{n+1}}dw.
$$

Let $\gamma=g(\{|w|=\rho\})$. The [biholomorphism](../../../../../biholomorphism.md) property makes it a simple positively oriented closed curve about zero. Under $w=f(z)$, $g(w)=z$ and $dw=f'(z)dz$, so

$$
c_n=\frac1{2\pi i}\int_\gamma\frac{zf'(z)}{f(z)^{n+1}}dz=\frac1{2\pi in}\int_\gamma\frac{dz}{f(z)^n}.
$$

The last equality is (a). Apply (b), giving

$$
\boxed{c_n=\frac1{n!}\left[\frac{d^{n-1}}{dz^{n-1}}\left(\frac z{f(z)}\right)^n\right]_{z=0}.}
$$

This is the local [Lagrange inversion theorem](../../../../../lagrange-inversion-theorem.md); the [simple zero](../../../../../simple-zero.md) ensures that the expression being differentiated has a removable singularity and a nonzero value at zero.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Analysis](../../../analysis.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
