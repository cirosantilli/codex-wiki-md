<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Since $f'(x)=2x-2$, [Newton's method](../../../../../newton-s-method-in-optimization.md) becomes

$$
\boxed{x_{n+1}=x_n-\frac{x_n(x_n-2)}{2(x_n-1)}=\frac{x_n^2}{2(x_n-1)}}\qquad(x_n\ne1).
$$

For $x_n>2$, subtraction from $2$ gives

$$
x_{n+1}-2=\frac{(x_n-2)^2}{2(x_n-1)}>0.
$$

Also $x_n-x_{n+1}=x_n(x_n-2)/(2(x_n-1))>0$. Hence **$2<x_{n+1}<x_n$**. Equivalently, the positive excess above $2$ is multiplied by the [function](../../../../../function-split.md) from part (c): $x_{n+1}-2=g(x_n)(x_n-2)$, with $0<g(x_n)<1/2$.

Thus the iterates form a decreasing [sequence](../../../../../sequence.md) bounded below by $2$. By the [monotone convergence theorem for sequences](../../../../../bounded-monotone-sequence-theorem.md) they have a limit $\ell\geq2$. Passing to the limit in the continuous update gives $2\ell(\ell-1)=\ell^2$, or $\ell(\ell-2)=0$. Therefore **$x_n\to2$**. The exact error formula also shows [quadratic convergence](../../../../../quadratic-convergence.md) near this root.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
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
