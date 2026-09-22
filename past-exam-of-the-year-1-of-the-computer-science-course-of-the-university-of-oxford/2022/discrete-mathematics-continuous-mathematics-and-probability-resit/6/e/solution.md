<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**Not near the minimum at $1$.** The [derivative](../../../../../derivative.md) being set to zero factors as

$$
f'(x)=\frac{2(x-1)^3(x+1)}{x^3},
$$

so $1$ has [multiplicity of a root](../../../../../multiplicity-of-a-root.md) equal to three. The ordinary [Newton iteration at a multiple root](../../../../../newton-iteration-at-a-multiple-root.md) is generally only linearly convergent, with error ratio $(3-1)/3=2/3$ here.

In fact, cancellation in $x-f'(x)/f''(x)$ gives the exact error identity, away from the original undefined quotient at the root,

$$
x_{n+1}-1=(x_n-1)\frac{x_n+3}{x_n^2+2x_n+3}.
$$

For iterates approaching $1$, the factor tends to $2/3$, proving [linear convergence](../../../../../linear-convergence.md). The other zero of $f'$ at $-1$ is simple and could instead give quadratic local convergence; the failure at $1$ is due to its multiplicity, not to every [stationary point](../../../../../stationary-point.md) of this [rational function](../../../../../rational-function.md).

## ↑ Ancestors (12)

1. [E](../e.md)
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
