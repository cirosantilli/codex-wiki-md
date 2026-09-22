<h1 id="f/f2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [partial derivatives](../../../../../../partial-derivative.md) satisfy a global bound of $1$ in absolute value. For example,

$$
|\partial_xf(x,y)|\leq\frac{2|x|}{(1+x^2)^2}\leq1,
$$

because $2|x|\leq1+x^2$ and $1+x^2\geq1$; the same argument applies to $\partial_y f$. Apply the one-dimensional [mean value theorem](../../../../../../mean-value-theorem.md) first along a horizontal segment and then along a vertical segment:

$$
\begin{aligned}
|f(x,y)-f(u,v)|
&\leq|f(x,y)-f(u,y)|+|f(u,y)-f(u,v)|\\
&\leq\boxed{|x-u|+|y-v|}.
\end{aligned}
$$

Thus $f$ is [Lipschitz](../../../../../../lipschitz-continuity.md) with constant $1$ for the coordinate-sum [norm](../../../../../../norm.md).

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [F2](../../../f2.md)
4. [F](../../../../f.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
