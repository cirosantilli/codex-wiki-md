# Radius of convergence

↑ **Parent:** [Power series](power-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radius_of_convergence)

The [radius of convergence](radius-of-convergence.md) of $\sum_{n\ge0}a_n(z-c)^n$ is the unique $R\in[0,\infty]$ separating interior [absolute convergence](absolute-convergence.md) from exterior divergence. It converges absolutely when $|z-c|<R$ and diverges when $|z-c|>R$. At the centre it always has the finite value $a_0$, since all positive powers vanish. The [boundary convergence of a power series](boundary-convergence-of-a-power-series.md) is a separate question.

For $0<R<\infty$, the interior is a [disk](disk-mathematics.md) in the [complex plane](complex-plane.md) and an open [interval](interval-mathematics.md) $(c-R,c+R)$ on the [real line](real-line.md). A [power series](power-series.md) converges uniformly on every smaller closed disk $|z-c|\le r<R$. This gives stable [polynomial approximation](polynomial-approximation.md) over a whole compact region, rather than a separate limiting calculation at each point. See [Jiří Lebl, Basic Analysis, §11.3.2: convergence of power series](https://www.jirka.org/ra/html/sec_analfuncs.html).

Four examples reveal what $R$ measures:
- $\sum_{n\ge0}z^n$ has $R=1$, since its [coefficients](coefficient.md) have constant magnitude one.
- $\sum_{n\ge1}z^n/n$ also has $R=1$: a factor $1/n$ changes boundary behaviour without changing the limiting coefficient-root growth.
- $\sum_{n\ge0}z^n/n!$ has $R=\infty$. The [ratio test](ratio-test.md) gives successive term ratio $|z|/(n+1)\to0$ for every fixed $z$, producing the [exponential function](exponential-function.md).
- $\sum_{n\ge0}n!z^n$ has $R=0$. For any $z\ne0$, successive term magnitudes have ratio $(n+1)|z|\to\infty$, so the terms do not tend to zero.

The [Cauchy-Hadamard theorem](cauchy-hadamard-theorem.md) computes $R$ directly from the [coefficients](coefficient.md). The attractive feature is that one growth statistic decides convergence throughout the interior and exterior, including sparse series with many zero [coefficients](coefficient.md). Finite changes to the coefficients do not alter the radius, though they can change the sum.

**Table of contents**

- [Boundary convergence of a power series](boundary-convergence-of-a-power-series.md)
- [Bounded power-series terms force interior absolute convergence](bounded-power-series-terms-force-interior-absolute-convergence.md)
- [Sum of power series with unequal radii of convergence](sum-of-power-series-with-unequal-radii-of-convergence.md)
- [Terms of a power series are unbounded outside its convergence disc](terms-of-a-power-series-are-unbounded-outside-its-convergence-disc.md)
- [Radius of convergence of a sparse power series](radius-of-convergence-of-a-sparse-power-series.md)
- [Polynomial-coefficient power series](polynomial-coefficient-power-series.md)
- [Polynomial coefficient growth with unit power-series radius](polynomial-coefficient-growth-with-unit-power-series-radius.md)
- [Cauchy-Hadamard theorem](cauchy-hadamard-theorem.md)
- [Radius of convergence after powering coefficients](radius-of-convergence-after-powering-coefficients.md)
- [Half-plane of convergence of an exponential power series](half-plane-of-convergence-of-an-exponential-power-series.md)

## ↑ Ancestors (7)

1. [Power series](power-series.md)
2. [Sequence and series](sequence-and-series.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (47)

- [Analytic continuation](analytic-continuation.md)
- [Boundary convergence of a power series](boundary-convergence-of-a-power-series.md)
- [Bounded power-series terms force interior absolute convergence](bounded-power-series-terms-force-interior-absolute-convergence.md)
- [Cauchy-Hadamard theorem](cauchy-hadamard-theorem.md)
- [Even-length walk generating function on a bipartite graph](even-length-walk-generating-function-on-a-bipartite-graph.md)
- [Factorial-gap power series](factorial-gap-power-series.md)
- [Generating function](generating-function.md)
- [Geometric power-series remainder](geometric-power-series-remainder.md)
- [Lacunary power series](lacunary-power-series.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/9d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/9d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/4c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/4c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/4c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-1/4d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-1/4d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/4d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-1/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/4e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/3d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/4d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/12f/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/12f/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/12f/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-26/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-1/4f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-1/4f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/4e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-1/4e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-1/4d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-304/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-1/4f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1/12f/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/11f/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/35b/iii/solution.md)
- [Polynomial coefficient growth with unit power-series radius](polynomial-coefficient-growth-with-unit-power-series-radius.md)
- [Polynomial-coefficient power series](polynomial-coefficient-power-series.md)
- [Power series](power-series.md)
- [Radius of convergence](radius-of-convergence.md)
- [Self-avoiding walk generating function](self-avoiding-walk-generating-function.md)
- [Sum of power series with unequal radii of convergence](sum-of-power-series-with-unequal-radii-of-convergence.md)
- [Taylor series](taylor-series.md)
- [Terms of a power series are unbounded outside its convergence disc](terms-of-a-power-series-are-unbounded-outside-its-convergence-disc.md)
- [Termwise differentiation of a power series](termwise-differentiation-of-a-power-series.md)
