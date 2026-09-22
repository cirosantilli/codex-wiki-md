<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $e_n=x_n-x_*$ for the [limit](../../../../../limit-of-a-function.md) $x_*$. [Quadratic convergence](../../../../../quadratic-convergence.md) means that eventually $|e_{n+1}|\leq C|e_n|^2$ for a fixed constant $C$; exact asymptotic order two has $|e_{n+1}|/|e_n|^2\to c$ with $0<c<\infty$.

For this iteration and $x_*=3$, direct algebra gives

$$
x_{n+1}-3=x_n-6+\frac9{x_n}=\frac{(x_n-3)^2}{x_n}.
$$

Using the stipulated convergence $x_n\to3$, the ratio of successive squared errors is

$$
\boxed{\frac{|e_{n+1}|}{|e_n|^2}=\frac1{|x_n|}\longrightarrow\frac13.}
$$

Thus the convergence is quadratic. The iteration is well defined here: $x_1=7/2$, and thereafter $x_n>3$ implies $3<x_{n+1}<x_n$. The initial point is not already the [limit](../../../../../limit-of-a-function.md), so the error ratio is meaningful.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
