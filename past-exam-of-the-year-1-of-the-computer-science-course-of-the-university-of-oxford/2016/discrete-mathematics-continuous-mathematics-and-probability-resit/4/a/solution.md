<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $Y(t)=y(e^t)$, so $x=e^t>0$. The [chain rule](../../../../../chain-rule.md) gives

$$
Y'(t)=xy'(x),\qquad Y''(t)=xy'(x)+x^2y''(x).
$$

Hence $x^2y''=Y''-Y'$ and the [Cauchy-Euler equation](../../../../../cauchy-euler-equation.md) becomes

$$
\boxed{Y''+3Y'+2Y=0}.
$$

Its [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $r^2+3r+2=(r+1)(r+2)=0$. The distinct roots give $Y(t)=Ae^{-t}+Be^{-2t}$. Returning to the original independent variable gives

$$
\boxed{y(x)=\frac A x+\frac B{x^2}\quad(x>0)}.
$$

The same form holds on any negative interval avoiding $0$, using $t=\log|x|$; the stated substitution covers the positive interval. At $x=0$ the [differential equation](../../../../../differential-equation-split.md) is singular, so crossing it is a separate extension problem.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
