<h1 id="19/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $r\ne1$, differentiate the [finite geometric series](../../../../../finite-geometric-series.md) and multiply by $r$:

$$
\sum_{n=1}^Nnr^n
=r\frac d{dr}\left(\frac{1-r^{N+1}}{1-r}\right)
=\frac{r[1-(N+1)r^N+Nr^{N+1}]}{(1-r)^2}.
$$

The required terms are $-nr^n$ with $r=-1/3$. The [finite weighted geometric sum](../../../../../finite-weighted-geometric-sum.md) therefore gives

$$
\boxed{S_N=\frac3{16}\left[1-\left(1+\frac{4N}{3}\right)
\left(-\frac13\right)^N\right].}
$$

Since $N/3^N\to0$, the correction tends to zero, proving convergence and yielding

$$
\boxed{\sum_{n=1}^{\infty}\frac{(-1)^{n+1}n}{3^n}=\frac3{16}.}
$$

In fact the [ratio test](../../../../../ratio-test.md) also proves [absolute convergence](../../../../../absolute-convergence.md), since the ratio of consecutive absolute terms tends to $1/3$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
