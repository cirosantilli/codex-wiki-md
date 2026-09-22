<h1 id="12f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At $x=1/4$ the terms are $c_n$. Their decay to zero alone is insufficient for convergence. In fact

$$
\frac{c_{n+1}}{c_n}=\frac{2n+1}{2n+2}
\geq\frac{n+1}{n+2},
$$

because the difference has numerator $n\geq0$. Since $c_1=1/2$, induction gives $c_n\geq1/(n+1)$. The comparison [harmonic series](../../../../../../harmonic-series.md) diverges, so

$$
\boxed{x=1/4:\ \text{the series diverges to }+\infty.}
$$

At $x=-1/4$ the terms are $(-1)^nc_n$. Part (ii) gives positive decreasing magnitudes tending to zero, so the [alternating series test](../../../../../../alternating-series-test.md) applies. To see the convergence directly, let $S_N=\sum_{n=1}^N(-1)^nc_n$. Then

$$
S_{2k+2}-S_{2k}=-c_{2k+1}+c_{2k+2}<0,
$$

while $S_{2k}\geq-c_1$, obtained by grouping $S_{2k}=-c_1+(c_2-c_3)+\cdots+(c_{2k-2}-c_{2k-1})+c_{2k}$. Thus the even [partial sums](../../../../../../partial-sum.md) have a finite limit. The odd [partial sums](../../../../../../partial-sum.md) differ from them by $-c_{2k+1}\to0$, so the whole [sequence](../../../../../../sequence.md) of [partial sums](../../../../../../partial-sum.md) has the same limit. Absolute convergence would require convergence of $\sum c_n$, already disproved. Hence

$$
\boxed{x=-1/4:\ \text{the series converges conditionally}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
