<h1 id="p/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $M_j=s''(j)$. A [natural cubic spline](../../../../natural-cubic-spline.md) has $M_0=M_2=0$. The interior spline equation on equal unit intervals is

$$
M_0+4M_1+M_2=6[(4-0)-(0-0)]=24,
$$

so $M_1=6$. The standard second-derivative interpolation formula, or direct integration of the linear second derivative, gives

$$
\boxed{s(x)=
\begin{cases}
x^3-x,&0\leq x\leq1,\\
-x^3+6x^2-7x+2,&1\leq x\leq2.
\end{cases}}
$$

The two pieces have equal value, first derivative, and second derivative at one, and $s''$ vanishes at zero and two.

Adding the linear function $x$ changes the nodal data by $(0,1,2)$ without affecting second derivatives. By uniqueness, the second requested natural cubic spline is **$s(x)+x$**, with pieces $x^3$ and $-x^3+6x^2-6x+2$ respectively.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [P](../../p.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
