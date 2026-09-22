<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At the origin the needed [partial derivatives](../../../../../partial-derivative.md) are

$$
f(0,0)=1,\quad f_x(0,0)=0,\quad f_y(0,0)=-3,\quad f_{xx}(0,0)=2,\quad f_{xy}(0,0)=f_{yy}(0,0)=0.
$$

The [Taylor series](../../../../../taylor-series.md) through total degree two is therefore

$$
f(0,0)+f_x(0,0)x+f_y(0,0)y+\tfrac12\bigl(f_{xx}(0,0)x^2+2f_{xy}(0,0)xy+f_{yy}(0,0)y^2\bigr),
$$

which gives

$$
\boxed{f(x,y)=1-3y+x^2+O(\|(x,y)\|^3)\quad\text{as }(x,y)\to(0,0).}
$$

Here total degree is what matters: $x^2y^2$ is quartic, not quadratic. The exact omitted [polynomial](../../../../../polynomial-split.md) is $y^3+x^2y^2+x^2y^4$, which verifies the stated [Big O notation](../../../../../big-o-notation.md) remainder directly.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
