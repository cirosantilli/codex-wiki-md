<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

When $n=0$, the forcing has nonzero integral $\int_{-1}^11\,dx=2$, violating the [Fredholm alternative](../../../../fredholm-alternative.md) condition. There is no bounded solution. Directly, integration gives $(1-x^2)y'=x+B$; cancellation of its logarithmic divergence at $x=-1$ requires $B=1$, while cancellation at $x=1$ requires $B=-1$.

For $n\geq1$, the constant $1/[n(n+1)]$ is a [particular solution](../../../../particular-solution.md). Subtract it from any solution. The remainder satisfies the [Legendre differential equation](../../../../legendre-differential-equation.md), whose [general solution](../../../../general-solution.md) is a combination of $P_n$ and the logarithmically unbounded [Legendre function of the second kind](../../../../legendre-function-of-the-second-kind.md). Boundedness removes the latter coefficient, giving

$$
\boxed{\begin{cases}
\text{no bounded solution},&n=0,\\
y(x)=\dfrac1{n(n+1)}+CP_n(x),\quad C\in\mathbb R,&n\geq1.
\end{cases}}
$$

The constant forcing is [orthogonal](../../../../orthogonal-vectors.md) to $P_n$ for $n\geq1$, consistently with [Orthogonality of Legendre polynomials](../../../../orthogonality-of-legendre-polynomials.md) and the [Fredholm alternative](../../../../fredholm-alternative.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
