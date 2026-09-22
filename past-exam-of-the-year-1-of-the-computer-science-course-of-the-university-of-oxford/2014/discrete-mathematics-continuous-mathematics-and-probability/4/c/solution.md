<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The homogeneous [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $r^2-4r+3=(r-1)(r-3)=0$, giving $e^x$ and $e^{3x}$. Since the forcing $e^{3x}$ already appears among these solutions, try a [particular solution](../../../../../particular-solution.md) $y_p=Ax e^{3x}$. Differentiation and substitution give

$$
y_p''-4y_p'+3y_p=2Ae^{3x},
$$

so $A=1/2$. The [general solution](../../../../../general-solution.md) is

$$
\boxed{y=C_1e^x+C_2e^{3x}+\frac{x}{2}e^{3x}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
