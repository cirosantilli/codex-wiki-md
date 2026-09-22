<h1 id="15/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Factor out $x^2$ before expanding the [logarithm](../../../../../logarithm.md):

$$
\log(1+x+x^2)=2\log x+\log\left(1+\frac1x+\frac1{x^2}\right)
$$

for large positive $x$. Using $\log(1+u)=u-u^2/2+O(u^3)$ then gives

$$
\boxed{\log(1+x+x^2)=2\log x+\frac1x+\frac1{2x^2}+O(x^{-3}),\qquad x\to+\infty}.
$$

These are the first three nonzero terms, including the leading [logarithm](../../../../../logarithm.md). Replacing $\log x$ by $\log|x|$ yields the corresponding two-sided large-$|x|$ expansion.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [15](../../15.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
