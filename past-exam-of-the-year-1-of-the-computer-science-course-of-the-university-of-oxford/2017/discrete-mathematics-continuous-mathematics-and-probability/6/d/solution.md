<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Factor the right side as $(x-1)^2(x-3)$. On $-1<x<1$, division by $x^2-1$ gives a [first-order linear differential equation](../../../../../first-order-linear-differential-equation.md) with [integrating factor](../../../../../integrating-factor.md)

$$
\mu(x)=\frac{1+x}{1-x},\qquad \frac{\mu'}\mu=-\frac2{x^2-1}.
$$

Multiplication makes the equation $(\mu y)'=3-x$, so $\mu y=3x-x^2/2+C$. At zero, $\mu(0)y(0)=1$, hence $C=1$. Simplifying gives

$$
\boxed{y(x)=\frac{1-x}{1+x}\left(1+3x-\frac{x^2}{2}\right)=\frac{x^2}{2}-4x+6-\frac5{x+1}.}
$$

Its derivative is

$$
y'(x)=x-4+\frac5{(x+1)^2},\qquad\boxed{y'(0)=1.}
$$

The derivation solves the initial-value problem on $(-1,1)$. The simplified expression also extends smoothly through $x=1$ and satisfies the original undivided equation there, giving a solution on all $x>-1$; its pole prevents continuation through $x=-1$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
