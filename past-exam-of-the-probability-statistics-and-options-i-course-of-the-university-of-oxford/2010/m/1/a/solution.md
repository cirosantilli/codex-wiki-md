<h1 id="m/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an [exponential distribution](../../../../../exponential-distribution.md) with rate $\lambda>0$, direct integration gives the [moment-generating function](../../../../../moment-generating-function.md)

$$
M_X(t)=\int_0^\infty e^{tx}\lambda e^{-\lambda x}dx
=\boxed{\frac\lambda{\lambda-t},\quad t<\lambda.}
$$

It is finite in a neighborhood of zero, so its derivatives there give moments. Differentiating three times gives $M_X^{(3)}(t)=6\lambda/(\lambda-t)^4$, hence

$$
\boxed{\mathbb EX^3=M_X^{(3)}(0)=6/\lambda^3.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [M](../../../m.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
