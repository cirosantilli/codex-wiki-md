<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The far field is proportional to $rP_1(\cos\theta)$, since $P_1(\cos\theta)=\cos\theta$. After matching the growing terms, write the exterior solution as

$$
U=v_0rP_1(\cos\theta)+\sum_{n=0}^\infty B_nr^{-n-1}P_n(\cos\theta).
$$

An added constant has here been excluded by interpreting the far-field condition as $U-v_0r\cos\theta\to0$. Differentiate and impose the radial [Neumann boundary condition](../../../../../../neumann-boundary-condition.md):

$$
0=v_0P_1(\cos\theta)-\sum_{n=0}^\infty(n+1)B_nr_0^{-n-2}P_n(\cos\theta).
$$

The [Orthogonality of Legendre polynomials](../../../../../../orthogonality-of-legendre-polynomials.md) makes each coefficient vanish separately. Thus $B_n=0$ for $n\ne1$, and $2B_1/r_0^3=v_0$. Consequently

$$
\boxed{U(r,\theta)=v_0\left(r+\frac{r_0^3}{2r^2}\right)\cos\theta,\qquad r\geq r_0.}
$$

Indeed $\partial_rU=v_0(1-r_0^3/r^3)\cos\theta$, which vanishes at the boundary, while the correction decays at infinity. If the far-field condition is intended to specify only the leading growing term, an arbitrary additive constant is also allowed; its gradient has no effect on the [Neumann boundary condition](../../../../../../neumann-boundary-condition.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
