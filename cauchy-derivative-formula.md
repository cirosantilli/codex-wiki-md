# Cauchy derivative formula

↑ **Parent:** [Complex analysis](complex-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy_derivative_formula)

Suppose $f$ is a [holomorphic function](holomorphic-function.md) on an [open set](open-set.md) containing the closed disc $|z-a|\le R$, with $R>0$. For any nonnegative integer $n$ and $|w-a|<R$, the counterclockwise boundary [contour](complex-integration-contour.md) satisfies

$$
f^{(n)}(w)=\frac{n!}{2\pi i}\oint_{|z-a|=R}\frac{f(z)}{(z-w)^{n+1}}\,dz.
$$

The case $n=0$ is the [Cauchy integral formula](cauchy-integral-formula.md). On a smaller closed disc, the denominator stays uniformly away from zero, allowing repeated differentiation under the [contour integral](contour-integral.md). This proves that a [holomorphic function](holomorphic-function.md) has complex [derivatives](derivative.md) of every order. [Orloff, MIT Topic 4, derivative formula](https://ocw.mit.edu/courses/18-04-complex-variables-with-applications-spring-2018/b1a90df19f643b974555bbbb93138a48_MIT18_04S18_topic4.pdf)

At the centre, if $M=\max_{|z-a|=R}|f(z)|$, taking [absolute values](absolute-value.md) gives the [Cauchy estimate](cauchy-estimate.md) $|f^{(n)}(a)|\le n!M/R^n$. Boundary size therefore limits interior variation. For $f(z)=z^2$ on the [unit disc](unit-disc.md), $M=1$, and the $n=2$ estimate is exact: $|f''(0)|=2$. This is one quantitative reason that [holomorphic functions](holomorphic-function.md) are so rigid.

**Table of contents**

- [Recovering an analytic derivative from the boundary real part](recovering-an-analytic-derivative-from-the-boundary-real-part.md)
- [Lipschitz bound inside a bounded analytic half-plane](lipschitz-bound-inside-a-bounded-analytic-half-plane.md)

## ↑ Ancestors (5)

1. [Complex analysis](complex-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Holomorphic function](holomorphic-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4/4a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/4g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/13g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3/2h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-3/13g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/12b/a/solution.md)
- [Recovering an analytic derivative from the boundary real part](recovering-an-analytic-derivative-from-the-boundary-real-part.md)
