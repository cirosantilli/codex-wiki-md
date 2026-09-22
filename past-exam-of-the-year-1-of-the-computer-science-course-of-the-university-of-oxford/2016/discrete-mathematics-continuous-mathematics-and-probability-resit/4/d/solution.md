<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The substitution $y=xv$ gives $y'=v+xv'$. Cancelling $x^3v$ on both sides of the [differential equation](../../../../../differential-equation-split.md), for $x>0$, gives

$$
\boxed{xv'=v^3}.
$$

The [initial condition](../../../../../initial-condition.md) is $v(1)=1$. This selects a positive solution locally, so [separation of variables](../../../../../separation-of-variables.md) gives

$$
\int v^{-3}\,dv=\int x^{-1}\,dx,
\qquad -\frac1{2v^2}=\log x+C.
$$

Using $v(1)=1$ gives $C=-1/2$, and continuity selects the positive square root:

$$
v=\frac1{\sqrt{1-2\log x}},\qquad
\boxed{y=\frac{x}{\sqrt{1-2\log x}}=\sqrt{\frac{x^2}{1-\log(x^2)}},\quad m=2}.
$$

The real solution containing $x=1$ has maximal positive domain **$0<x<\sqrt e$**. Its denominator tends to zero and $y\to+\infty$ as $x\uparrow\sqrt e$, a [finite-time blow-up of an ordinary differential equation](../../../../../finite-time-blow-up-of-an-ordinary-differential-equation.md) in the independent variable $x$. Thus the source's wording “for $x>0$” needs this domain restriction; the prescribed initial value admits no real solution on the whole positive half-line. The division by $v^3$ loses the separate solution $v=0$, but that solution does not meet the [initial condition](../../../../../initial-condition.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
