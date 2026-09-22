<h1 id="taylor-s-theorem">Taylor's theorem</h1>

↑ **Parent:** [Calculus](calculus-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taylor's_theorem)

[Taylor's theorem](taylor-s-theorem.md) expresses a sufficiently [differentiable function](differentiable-function.md) as a finite [Taylor polynomial](taylor-polynomial.md) plus a [Taylor remainder](taylor-remainder.md). One convenient version assumes $f$ is $n+1$ times continuously [differentiable](differentiable-function.md) on the segment between $a$ and $x$. Then

$$
f(x)=T_{n,a}(x)+R_{n,a}(x),\qquad R_{n,a}(x)=\frac{f^{(n+1)}(\xi)}{(n+1)!}(x-a)^{n+1}
$$

for some intermediate point $\xi$, when $x\ne a$. Thus a bound $|f^{(n+1)}|\leq M$ on that segment gives $|R_{n,a}(x)|\leq M|x-a|^{n+1}/(n+1)!$. The intermediate point usually need not be computed: bounding the [derivative](derivative.md) throughout the segment is enough. This is why local approximation can yield reliable numerical bounds. A finite [Taylor polynomial](taylor-polynomial.md) does not require an infinite [Taylor series](taylor-series.md) to represent the [function](function-split.md).

Historically, the Royal Society holds [Brook Taylor](brook-taylor.md)'s letter of 26 July 1712 to John Machin. Its catalogue connects his work on [Kepler's second law](kepler-s-second-law.md) with the expansion later published in the 1715 Methodus incrementorum directa et inversa. This is a documented route from an orbital calculation to a general approximation method, rather than a claim that every earlier use of such expansions began with Taylor. See [Royal Society archive, letter MS/82/2](https://catalogues.royalsociety.org/calmview/Record.aspx?id=MS%2F82%2F2&src=CalmView.Catalog).

**Table of contents**

- [Taylor expansion from a periodic derivative equation](taylor-expansion-from-a-periodic-derivative-equation.md)
- [Integral first-order Taylor formula for a vector map](integral-first-order-taylor-formula-for-a-vector-map.md)
- [Integral remainder in Taylor theorem](integral-remainder-in-taylor-theorem.md)
  - [Logarithmic series from an integral Taylor remainder](logarithmic-series-from-an-integral-taylor-remainder.md)
- [Taylor expansion](taylor-expansion.md)
  - [Peano zero](peano-zero.md)
  - [Parabolic approximation](parabolic-approximation.md)
- [Taylor formula for a polynomial](taylor-formula-for-a-polynomial.md)
- [Taylor theorem with Lagrange remainder](taylor-theorem-with-lagrange-remainder.md)
  - [Lagrange remainder](lagrange-remainder.md)
- [Taylor remainder](taylor-remainder.md)
- [Taylor formula with integral remainder](taylor-formula-with-integral-remainder.md)
- [Taylor series](taylor-series.md)
  - [Maclaurin series](maclaurin-series.md)

## ↑ Ancestors (6)

1. [Calculus](calculus-split.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (33)

- [Adaptive Euler step doubling for exponential decay](adaptive-euler-step-doubling-for-exponential-decay.md)
- [Consistency of a numerical method](consistency-of-a-numerical-method.md)
- [Hoeffding lemma](hoeffding-lemma.md)
- [Laplacian as departure from a local average](laplacian-as-departure-from-a-local-average.md)
- [Local quadratic convergence of Newton iteration](local-quadratic-convergence-of-newton-iteration.md)
- [Net radiative heat exchange](net-radiative-heat-exchange.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-53/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/12c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/38c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/19d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-1/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-61/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-1/11e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-17/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-2/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/9/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/11/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/11/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/17/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/15/a/solution.md)
- [Small-planet transit weighting](small-planet-transit-weighting.md)
- [Taylor's theorem](taylor-s-theorem.md)
