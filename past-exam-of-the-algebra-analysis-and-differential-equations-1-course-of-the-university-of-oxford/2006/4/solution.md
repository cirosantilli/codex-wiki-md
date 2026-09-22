<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [closed curve](../../../closed-curve.md) has $\gamma(a)=\gamma(b)$. A [simple curve](../../../simple-curve.md) has no repeated points apart from the permitted equality of its two endpoints when it is closed. A [smooth curve](../../../smooth-curve.md), in the regular contour-integration convention, has a continuous nonzero tangent $\gamma'$; piecewise smooth contours are treated by adding the integrals over their smooth pieces. For a continuous integrand, its [contour integral](../../../contour-integral.md) is defined by

$$
\boxed{\int_\gamma f(z)\,dz=\int_a^b f(\gamma(t))\gamma'(t)\,dt.}
$$

For the positively oriented circle, $\gamma'(t)=ire^{it}$ and $(\gamma(t)-z_0)^n=r^ne^{int}$. Direct parameter integration therefore gives

$$
\int_\gamma(z-z_0)^n\,dz=ir^{n+1}\int_0^{2\pi}e^{i(n+1)t}\,dt
=\boxed{\begin{cases}2\pi i,&n=-1,\\0,&n\ne-1.\end{cases}}
$$

For $n\ne-1$, an elementary [antiderivative](../../../antiderivative.md) is $e^{i(n+1)t}/[i(n+1)]$ and its endpoint values agree because $n$ is an integer. For $n=-1$, the integrand of the parameter integral is the constant $i$. No integral theorem is needed.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2006](../../2006-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
