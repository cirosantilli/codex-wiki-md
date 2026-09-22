<h1 id="iterated-ito-integral">Iterated Itô integral</h1>

↑ **Parent:** [Itô integral](ito-integral.md)

For [Brownian motion](brownian-motion-split.md), an ordered iterated Itô integral is defined by the displayed recursion. It represents integration on $0\leq s_1\leq\cdots\leq s_n\leq t$, with time increasing toward the outermost [Itô integral](ito-integral.md). The [Itô isometry](ito-isometry.md) proves inductively that

$$
\mathbb E I_n(t)^2=\int_0^t\mathbb E I_{n-1}(s)^2ds=\frac{t^n}{n!}.
$$

Thus every recursive integrand is a [square-integrable stochastic integrand](square-integrable-stochastic-integrand.md) on each finite interval, and $I_n$ is a [martingale](martingale-split.md) for $n\geq1$. For $n=1,2,3$, increment algebra gives $I_1=B_t$, $I_2=(B_t^2-t)/2$ and $I_3=(B_t^3-3tB_t)/6$. These are the corresponding [space-time Hermite polynomials](space-time-hermite-polynomial.md) divided by $n!$.

## ↑ Ancestors (9)

1. [Itô integral](ito-integral.md)
2. [Stochastic integral](stochastic-integral.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford/2023/2/c/ii/solution.md)
- [Solution](past-exam-of-the-continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford/2023/2/c/iii/solution.md)
