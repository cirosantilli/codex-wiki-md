<h1 id="m4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Write a first return time as $2J$, where $\mathbb P(J=j)=2^{-j}$ for $j\geq1$. It has mean $2\cdot2=4$ and period two, so the stationary [probability](../../../../probability.md) at one is $1/4$. The periodic convergence theorem would give limits $1/2$ along even times and zero along odd times.

Here one can obtain them directly. Put $u_n=\mathbb P_1(X_{2n}=1)$, with $u_0=1$. Splitting according to the first return gives the [renewal equation](../../../../renewal-equation.md)

$$
u_n=\sum_{j=1}^n2^{-j}u_{n-j}.
$$

Induction gives $u_n=1/2$ for every $n\geq1$: the right side is $2^{-n}+\tfrac12\sum_{j=1}^{n-1}2^{-j}=1/2$. Odd-time returns are impossible because every return interval is even. Therefore the exact set of limit points is

$$
\boxed{\{0,\tfrac12\}.}
$$

The [sequence](../../../../sequence.md) does not converge to the stationary mass $1/4$, precisely because it is periodic.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [M4](../../m4.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
