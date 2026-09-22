<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The repeated root of the [characteristic equation](../../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) suggests factoring out $e^x$. Set $y=e^xu$. The [product rule](../../../../../../product-rule.md) gives

$$
y'=e^x(u+u'),\qquad y''=e^x(u+2u'+u''),\qquad y''-2y'+y=e^xu''.
$$

Thus the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) reduces to $u''=1$, with [general solution](../../../../../../general-solution.md) $u=x^2/2+Ax+B$. The first [initial condition](../../../../../../initial-condition.md) gives $B=1$. Since $y'(0)=A+B=2$, the other [initial condition](../../../../../../initial-condition.md) gives $A=1$. Therefore

$$
\boxed{y(x)=e^x\left(1+x+\frac{x^2}{2}\right),\qquad x\in\mathbb R.}
$$

Substitution into the reduced [ordinary differential equation](../../../../../../ordinary-differential-equation.md) and the two [initial conditions](../../../../../../initial-condition.md) verifies the result.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
