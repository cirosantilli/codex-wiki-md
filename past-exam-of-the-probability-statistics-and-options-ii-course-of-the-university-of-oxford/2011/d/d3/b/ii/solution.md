<h1 id="d/d3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the nonnegative parts $h^+=\max(h,0)$ and $h^-=\max(-h,0)$, so $h=h^+-h^-$. The zero-mean assumption gives $H:=\int_0^\pi h^+=\int_0^\pi h^-<\infty$. On the $k$-th period, each of the positive and negative weighted integrals lies between $H/((k+1)\pi)$ and $H/(k\pi)$. Their difference therefore satisfies the stronger estimate

$$
\left|\int_{k\pi}^{(k+1)\pi}\frac{h(x)}x\,dx\right|
\leq\frac H\pi\left(\frac1k-\frac1{k+1}\right)
=\frac H{\pi k(k+1)}\leq\boxed{\frac H{\pi k^2}}.
$$

The sum of the absolute values of these block integrals converges, proving the existence of the finite limit of the integrals from $\pi$ to $n\pi$.

For genuine [Lebesgue integrability](../../../../../../integrability.md) we instead need the integral of the absolute value. Periodicity gives

$$
\int_{k\pi}^{(k+1)\pi}\frac{|h(x)|}x\,dx\geq\frac{2H}{(k+1)\pi}.
$$

If $H>0$, summation diverges by the [harmonic series](../../../../../../harmonic-series.md). If $H=0$, then $h=0$ [almost everywhere](../../../../../../almost-everywhere.md) and the function is integrable. Thus

$$
\boxed{g\in L^1(\pi,\infty)\quad\Longleftrightarrow\quad h=0\text{ almost everywhere}.}
$$

The finite signed block limit therefore need not be a [Lebesgue integral](../../../../../../lebesgue-integral.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [D3](../../../d3.md)
4. [D](../../../../d.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
