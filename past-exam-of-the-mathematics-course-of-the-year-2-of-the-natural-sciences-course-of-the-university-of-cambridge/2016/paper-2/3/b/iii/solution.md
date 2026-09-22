<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $r=|\mathbf r|$, $s=|\mathbf r'|$. For a spherical source, the angular integral needed for the [Green function of the Laplacian](../../../../../../green-function-of-the-laplacian.md) is

$$
\int\frac{d\Omega'}{|\mathbf r-\mathbf r'|}=2\pi\int_{-1}^1\frac{du}{\sqrt{r^2+s^2-2rsu}}=\frac{4\pi}{\max(r,s)}.
$$

This is the angular form of the [spherical shell theorem](../../../../../../spherical-shell-theorem.md). Substituting the source into the [Green function](../../../../../../green-s-function-split.md) integral therefore yields

$$
\phi(r)=-\frac1r\int_0^rs e^{-\beta s}\,ds-\int_r^\infty e^{-\beta s}\,ds.
$$

The elementary integrals are

$$
\int_0^rs e^{-\beta s}\,ds=\frac{1-(1+\beta r)e^{-\beta r}}{\beta^2},\qquad\int_r^\infty e^{-\beta s}\,ds=\frac{e^{-\beta r}}\beta.
$$

The terms proportional to $e^{-\beta r}/\beta$ cancel, leaving

$$
\boxed{\phi(r)=\frac{e^{-\beta r}-1}{\beta^2r},\qquad\phi(0)=-\frac1\beta.}
$$

The value at the origin is the continuous limit. At large radius $\phi\sim-1/(\beta^2r)$, consistent with the integrated source $\int\rho\,dV=-4\pi/\beta^2$ and the factor $1/(4\pi r)$ in the far-field potential.

For a direct check, set $u=r\phi$. Then $u''=e^{-\beta r}$, so $\nabla^2\phi=u''/r=e^{-\beta r}/r=-\rho$ for $r>0$. Boundedness of $\phi$ at zero cancels the singular $1/r$ terms and excludes an extra point source. The original density is itself singular but locally [integrable](../../../../../../integrability.md); the equation at the origin is understood in the sense of [distributions](../../../../../../distribution-mathematical-analysis.md). This is the [Poisson potential of an exponential-over-radius source](../../../../../../poisson-potential-of-an-exponential-over-radius-source.md) with amplitude $A=-1$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
