<h1 id="d/4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For fixed $x>0$, $f_n(x)\to e^{-x}\sin x$; for $x\le0$, the limit is zero. On $0<x<n$, the supplied inequality gives $(1-x/n)^n\le e^{-x}$, so

$$
|f_n(x)|\le\chi_{(0,\infty)}(x)e^{-x}.
$$

This is the given integrable dominating function. By the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md),

$$
\lim_n\int f_n(x)\,dx=\int_0^\infty e^{-x}\sin x\,dx
=\operatorname{Im}\frac1{1-i}=\boxed{\frac12}.
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [D](../../../d.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
