<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $u=\cos\theta$, the boundary data have the finite [Legendre polynomial](../../../../../legendre-polynomial.md) expansion

$$
-2+2u+3u^2=-P_0(u)+2P_1(u)+2P_2(u).
$$

Inside the sphere, every $r^{-\ell-1}$ term is singular at the origin and must be absent. Matching at $r=a$ therefore gives

$$
\boxed{\Psi_{\mathrm{in}}(r,\theta)
=-1+2\frac ra\cos\theta+\frac{r^2}{a^2}(3\cos^2\theta-1)}.
$$

In the exterior, decay at infinity excludes all $r^\ell$ terms, including the constant term at $\ell=0$. Thus

$$
\boxed{\Psi_{\mathrm{out}}(r,\theta)
=-\frac ar+2\frac{a^2}{r^2}\cos\theta
+\frac{a^3}{r^3}(3\cos^2\theta-1)}.
$$

Both [harmonic functions](../../../../../harmonic-function.md) have the prescribed [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md), and each is finite throughout its own domain. The interior expression is regular even at the origin because $r\cos\theta=z$ and $r^2(3\cos^2\theta-1)=2z^2-x^2-y^2$. [Uniqueness of the Dirichlet problem](../../../../../uniqueness-of-the-dirichlet-problem.md) identifies these as the respective solutions. Their normal derivatives need not match: the two [Dirichlet problems](../../../../../dirichlet-problem.md) do not require a single [harmonic function](../../../../../harmonic-function.md) across the bounding sphere.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
