<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $Y(t)=y(e^t)$, so $t=\log x$. The [chain rule](../../../../../chain-rule.md) gives

$$
y'(x)=\frac{Y'(t)}x,\qquad
y''(x)=\frac{Y''(t)-Y'(t)}{x^2}.
$$

Substitution into the [Cauchy-Euler equation](../../../../../cauchy-euler-equation.md) therefore gives $Y''+Y'-2Y=0$. Its [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) factors as $(r-1)(r+2)=0$, so $Y=C_1e^t+C_2e^{-2t}$. Returning to $x$ gives

$$
\boxed{y(x)=C_1x+C_2x^{-2},\qquad x>0.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
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
