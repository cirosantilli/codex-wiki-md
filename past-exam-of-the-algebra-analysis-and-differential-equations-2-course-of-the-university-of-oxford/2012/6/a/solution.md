<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [tangent half-angle substitution](../../../../tangent-half-angle-substitution.md) $u=\tan(t/2)$ maps $0\leq t<\pi$ to $0\leq u<\infty$, with

$$
\cos t=\frac{1-u^2}{1+u^2},\qquad dt=\frac{2\,du}{1+u^2}.
$$

Because $a>1$, both $a+1$ and $a-1$ are positive. Thus

$$
\int_0^\pi\frac{dt}{a+\cos t}=2\int_0^\infty\frac{du}{(a+1)+(a-1)u^2}=\frac2{\sqrt{a^2-1}}\left[\arctan\left(u\sqrt{\frac{a-1}{a+1}}\right)\right]_0^\infty.
$$

Evaluating the [improper integral](../../../../improper-integral.md) gives

$$
\boxed{\frac{\pi}{\sqrt{a^2-1}}.}
$$

Although the change of variable has an infinite endpoint, the original integrand is continuous on the closed interval, and the transformed integrand decays as $u^{-2}$, so the limiting substitution is justified.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
