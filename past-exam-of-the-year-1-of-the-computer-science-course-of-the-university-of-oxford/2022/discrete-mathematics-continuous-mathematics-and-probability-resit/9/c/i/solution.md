<h1 id="9/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $Z=U^a$. Since $a>0$, the map is increasing on $[0,1]$, and for $0\leqslant z\leqslant1$,

$$
\mathbb P(Z\leqslant z)=\mathbb P(U\leqslant z^{1/a})=z^{1/a}.
$$

[Differentiation](../../../../../../differentiation.md) gives

$$
f_Z(z)=\frac1a z^{1/a-1},\qquad0<z<1,
$$

and zero outside this interval. Since $B(1/a,1)=a$, this is exactly the [beta distribution](../../../../../../beta-distribution.md) [probability density function](../../../../../../probability-density-function.md) with **parameters $(1/a,1)$**. The [power transform of a uniform random variable](../../../../../../power-transform-of-a-uniform-random-variable.md) therefore satisfies $U^a\sim\operatorname{Beta}(1/a,1)$; the second parameter does not depend on $a$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
