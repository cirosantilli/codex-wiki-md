<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $t=y-1$. Then $y^2-1=t(t+2)$, and a [Frobenius solution](../../../../../frobenius-solution.md) has the form

$$
x=t^\sigma\sum_{j=0}^{\infty}a_jt^j,\qquad a_0\ne0.
$$

In the [differential equation](../../../../../differential-equation-split.md), the lowest power is $t^{\sigma-1}$, whose coefficient is

$$
[2\sigma(\sigma-1)+\sigma]a_0=\sigma(2\sigma-1)a_0.
$$

The [indicial equation](../../../../../indicial-equation.md) and its [indicial roots](../../../../../indicial-root.md) are consequently

$$
\boxed{\sigma(2\sigma-1)=0,\qquad \sigma_1=0,\quad\sigma_2=\frac12.}
$$

Their difference is not an integer, so the [Frobenius method](../../../../../frobenius-method.md) produces two independent series without a logarithmic term:

$$
\boxed{x_1(y)=\sum_{j=0}^{\infty}a_j(y-1)^j,\qquad x_2(y)=(y-1)^{1/2}\sum_{j=0}^{\infty}b_j(y-1)^j,\quad a_0b_0\ne0.}
$$

Choose a branch of $(y-1)^{1/2}$, or take $y>1$ for real solutions. A general local solution is $C_1x_1+C_2x_2$ by [linear independence](../../../../../linear-independence.md) and the [superposition principle](../../../../../superposition-principle.md). The analytic factors converge at least for $|y-1|<2$, up to the next singular point at $y=-1$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
