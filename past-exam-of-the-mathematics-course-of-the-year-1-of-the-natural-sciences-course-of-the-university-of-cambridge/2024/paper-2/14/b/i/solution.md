<h1 id="14/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $E$ be the finish-time offset from the start of its displayed minute. The elapsed time is $25+E-S$, so $T=E-S$. To obtain the stated density, use the intended model that $E$ and $S$ are [independent random variables](../../../../../../independent-random-variables.md), both with the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $[0,1)$.

Their joint [probability density function](../../../../../../probability-density-function.md) is one on the unit square. Equivalently, the [convolution of probability densities](../../../../../../convolution-of-independent-random-variables.md) gives

$$
q(t)=\int_{\mathbb R}p(s)p(s+t)\,ds.
$$

The [integrand](../../../../../../integrand.md) is one exactly where $s\in[0,1]$ and $s+t\in[0,1]$. The overlap has length $1+t$ for $-1\leq t<0$, length $1-t$ for $0\leq t<1$, and zero otherwise. Therefore

$$
\boxed{q(t)=\begin{cases}1-|t|,&|t|<1,\\0,&|t|\geq1.\end{cases}}
$$

This is a symmetric [triangular distribution](../../../../../../triangular-distribution.md). The independence and finish-time uniformity are additional modelling assumptions: the two truncated clock readings alone do not imply them. For example, if $E=S$ then the elapsed time is exactly twenty-five minutes and $T=0$, even though each endpoint offset is individually uniform.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [14](../../../14.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
