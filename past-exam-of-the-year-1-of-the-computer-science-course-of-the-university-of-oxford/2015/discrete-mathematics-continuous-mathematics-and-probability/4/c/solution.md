<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On an interval with $x\ne0$, set $y=xv$. The [product rule](../../../../../product-rule.md) gives $y'=v+xv'$, and substitution gives

$$
x^2(v+xv')=x^2+x^2v+x^2v^2,
\qquad\boxed{xv'=1+v^2.}
$$

This is a [separable differential equation](../../../../../separable-differential-equation.md). Since $1+v^2>0$ for real $v$, separation loses no real constant solution:

$$
\frac{dv}{1+v^2}=\frac{dx}{x},
\qquad \arctan v=\log|x|+C.
$$

Thus the [general solution](../../../../../general-solution.md) on any interval avoiding zero and the poles of the [tangent function](../../../../../tangent-function.md) is

$$
\boxed{y(x)=x\tan(\log|x|+C).}
$$

At $x=0$ the original [differential equation](../../../../../differential-equation-split.md) forces $y(0)=0$, but no real solution from this family extends over a whole interval through zero: $\log|x|+C$ encounters infinitely many poles as $x\to0$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
