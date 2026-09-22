<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

On either connected half-line, the [homogeneous linear differential equation](../../../../../homogeneous-linear-differential-equation.md) is

$$
y'+\left(\frac2x-\frac1{x^2}\right)y=0.
$$

Integration gives $\boxed{y_h=Cx^{-2}e^{-1/x}}$, including the zero solution. For the inhomogeneous equation choose the positive [integrating factor](../../../../../integrating-factor.md)

$$
\mu(x)=\exp\left(2\log|x|+\frac1x\right)=x^2e^{1/x}.
$$

It satisfies $\mu'/\mu=2/x-1/x^2$. Multiplication gives the exact derivative

$$
(\mu y)'=\frac1{1+x^2}.
$$

Hence all solutions on either half-line are

$$
\boxed{y(x)=\frac{e^{-1/x}}{x^2}\bigl(C+\arctan x\bigr).}
$$

For $a\ne0$, impose $y(a)=b$ to obtain $C=a^2e^{1/a}b-\arctan a$. The complete [initial value problem](../../../../../initial-value-problem.md) solution is therefore

$$
\boxed{y(x)=\frac{e^{-1/x}}{x^2}\left(a^2e^{1/a}b+\arctan x-\arctan a\right),\qquad ax>0.}
$$

It is smooth throughout the maximal connected interval $(0,\infty)$ if $a>0$, and $(-\infty,0)$ if $a<0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
