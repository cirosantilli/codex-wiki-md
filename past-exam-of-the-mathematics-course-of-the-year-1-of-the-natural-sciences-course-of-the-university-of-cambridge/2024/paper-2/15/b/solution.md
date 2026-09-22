<h1 id="15/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The associated [homogeneous linear differential equation](../../../../../homogeneous-linear-differential-equation.md) has [characteristic roots](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) $2\pm i$, so its [complementary function](../../../../../homogeneous-solution.md) is $e^{2x}(A\cos x+B\sin x)$. For a [particular integral](../../../../../particular-solution.md), the [method of undetermined coefficients](../../../../../method-of-undetermined-coefficients.md) suggests $y_p=ax^2+bx+c$. Substitution and comparison of [coefficients](../../../../../coefficient.md) gives

$$
5a=125,\qquad -8a+5b=0,\qquad 2a-4b+5c=0,
$$

so $y_p=25x^2+40x+22$. The [general solution](../../../../../general-solution.md) is therefore

$$
y=25x^2+40x+22+e^{2x}(A\cos x+B\sin x).
$$

The first [boundary condition](../../../../../boundary-condition.md) gives $A=-21$. At $x=\pi/2$, the polynomial part already equals the assigned boundary value and the cosine vanishes, so $e^\pi B=0$. Thus

$$
\boxed{y(x)=25x^2+40x+22-21e^{2x}\cos x}.
$$

This is the unique solution satisfying the two [boundary conditions](../../../../../boundary-condition.md); here the phrase “particular solution” means that selected member of the full family, rather than only the polynomial [particular integral](../../../../../particular-solution.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [15](../../15.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
