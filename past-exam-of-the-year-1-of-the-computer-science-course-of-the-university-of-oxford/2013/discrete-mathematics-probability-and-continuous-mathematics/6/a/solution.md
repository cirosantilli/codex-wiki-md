<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the suggested [substitution](../../../../../substitution-algebra.md), put $y=xv(x)$. Then the [product rule](../../../../../product-rule.md) gives $y'=v+xv'$, while the right side of the [ordinary differential equation](../../../../../ordinary-differential-equation.md) becomes $v+v^{-3}$. Cancelling $v$ leaves the [separable differential equation](../../../../../separable-differential-equation.md)

$$
x\frac{dv}{dx}=v^{-3},\qquad v^3\,dv=\frac{dx}{x}.
$$

Integration yields $v^4/4=\log x+C$. The [initial condition](../../../../../initial-condition.md) gives $v(1)=1$, so $v^4=1+4\log x$. The positive root is forced by the initial value and continuity:

$$
\boxed{y(x)=x(1+4\log x)^{1/4},\qquad x>e^{-1/4}.}
$$

This is the maximal connected interval containing $1$ on which the real solution exists. At the left endpoint $y=0$, where the original [ordinary differential equation](../../../../../ordinary-differential-equation.md) is undefined; extending the fourth-root formula further left would also cease to be real.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
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
