<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Substitution gives

$$
f(1)=-6,\qquad f'(1)=f''(1)=f^{(3)}(1)=0,\qquad f^{(4)}(1)=24.
$$

In particular, $1$ is a [stationary point](../../../../../stationary-point.md). For $x$ sufficiently close to $1$, [Taylor's theorem](../../../../../taylor-s-theorem.md) with fifth-order remainder gives

$$
\boxed{f(x)=-6+(x-1)^4+\frac{f^{(5)}(\xi)}{120}(x-1)^5,}
$$

where $\xi$ lies between $1$ and $x$. The fifth [derivative](../../../../../derivative.md) is bounded near $1$, so the remainder is $O((x-1)^5)$ and is smaller in magnitude than half the positive quartic term for sufficiently small nonzero $x-1$. Therefore **$x=1$ is a strict [local minimum](../../../../../local-minimum.md)**, despite the vanishing [second derivative](../../../../../second-derivative.md).

An exact algebraic check gives the stronger global conclusion:

$$
f(x)+6=\frac{(x-1)^4}{x^2}\geq0\qquad(x\ne0).
$$

Equality holds only at $x=1$, so it is the unique [global minimum](../../../../../global-minimum.md) on the actual domain.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
