<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $m^2+3m+2=(m+1)(m+2)=0$, giving the [complementary function](../../../../../homogeneous-solution.md) $C_1e^{-x}+C_2e^{-2x}$. For the forcing term $x$, a linear [particular solution](../../../../../particular-solution.md) $ax+b$ gives $2ax+3a+2b=x$, hence $a=1/2$, $b=-3/4$.

The forcing $-e^{-x}$ gives [resonance in a differential equation](../../../../../resonance-in-a-differential-equation.md), since $e^{-x}$ already appears in the [complementary function](../../../../../homogeneous-solution.md). Try $Kxe^{-x}$. Direct differentiation gives

$$
\left(\frac{d^2}{dx^2}+3\frac d{dx}+2\right)(Kxe^{-x})=Ke^{-x},
$$

so $K=-1$. Combining the two [particular solutions](../../../../../particular-solution.md) gives

$$
\boxed{y=(C_1-x)e^{-x}+C_2e^{-2x}+\frac x2-\frac34.}
$$

The factor $x$ in the [resonant exponential particular solution](../../../../../resonant-exponential-particular-solution.md) is required because $-1$ is already a root of the [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
