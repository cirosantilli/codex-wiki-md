<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [secant method](../../../../../../secant-method.md) starts from two approximations $x_0,x_1$. Replace the [function](../../../../../../function-split.md) near its [zero of a function](../../../../../../zero-of-a-function.md) by the [secant line](../../../../../../secant-line.md) through $(x_{k-1},f(x_{k-1}))$ and $(x_k,f(x_k))$; the zero of that line is the next approximation:

$$
\boxed{x_{k+1}=x_k-f(x_k)\frac{x_k-x_{k-1}}{f(x_k)-f(x_{k-1})}.}
$$

Stop immediately if $f(x_k)=0$; otherwise the denominator must be nonzero. Each further step needs one new [function](../../../../../../function-split.md) evaluation and no [derivative](../../../../../../derivative.md). There is no automatic bracketing or global [convergence](../../../../../../convergence.md) guarantee.[§3.8(iii), Secant Method and equation 3.8.6](../../../../../../nist-digital-library-of-mathematical-functions/3-8-nonlinear-equations.md)

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
