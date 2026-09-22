# Complex differentiability

↑ **Parent:** [Holomorphic function](holomorphic-function-split.md)

A complex-valued [function](function-split.md) is complex differentiable at $z_0$ if

$$
f'(z_0)=\lim_{\substack{h\to0\\h\in\mathbb C\setminus\{0\}}}\frac{f(z_0+h)-f(z_0)}{h}
$$

exists. The same limit must hold for every approach, including curved paths. Equivalently,

$$
f(z_0+h)=f(z_0)+f'(z_0)h+o(|h|).
$$

The error divided by $|h|$ tends to zero. Thus the [derivative](derivative.md) is a single complex multiplier, not an arbitrary real [linear map](linear-map.md) of the plane. If the real coordinate map is differentiable, [complex differentiability](complex-differentiability.md) is equivalent to its satisfying the [Cauchy-Riemann equations](cauchy-riemann-equations.md) at that point.

The simplest failure is [complex conjugation](complex-conjugation.md), $f(z)=\overline z$. At every $z_0$ its increment quotient is $\overline h/h$. For real $h=t\ne0$ it is $1$, while for $h=it$ it is $-1$. More generally, $h=te^{i\theta}$ gives $e^{-2i\theta}$. Although [complex conjugation](complex-conjugation.md) is a smooth real reflection and has every real [directional derivative](directional-derivative.md), these incompatible quotients rule out a complex [derivative](derivative.md) everywhere.

Agreement on two axes is necessary, but does not by itself establish a limit over the whole [complex plane](complex-plane.md). The [Cauchy-Riemann equations](cauchy-riemann-equations.md) need the real differentiability condition above, or a sufficient regularity condition such as continuous [partial derivatives](partial-derivative.md) near the point. There is a second distinction: $f(z)=|z|^2$ has complex [derivative](derivative.md) zero at zero because its quotient there is $\overline h\to0$, but its [Cauchy-Riemann equations](cauchy-riemann-equations.md) fail at every nonzero point. It is complex differentiable at zero without being a [holomorphic function](holomorphic-function-split.md) on any neighbourhood of zero.

**Table of contents**

- [Complex differentiability at a point without holomorphy nearby](complex-differentiability-at-a-point-without-holomorphy-nearby.md)

## ↑ Ancestors (6)

1. [Holomorphic function](holomorphic-function-split.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Complex analysis](complex-analysis-split.md)
- [Complex differentiability](complex-differentiability.md)
- [Complex differentiability at a point without holomorphy nearby](complex-differentiability-at-a-point-without-holomorphy-nearby.md)
- [Conjugate reflection of a holomorphic function](conjugate-reflection-of-a-holomorphic-function.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2012/5/a/solution.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2006/analysis/4/ii/solution.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2010/analysis/4/i/solution.md)
- [Solution](past-exam-of-the-algebra-and-analysis-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford/2013/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/7/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/7/a/solution.md)
- [Solution](past-exam-of-the-metric-spaces-and-complex-analysis-course-of-the-university-of-oxford/2021/3/a/iv/solution.md)
- [Solution](past-exam-of-the-metric-spaces-and-complex-analysis-course-of-the-university-of-oxford/2023/3/a/solution.md)
- [Solution](past-exam-of-the-metric-spaces-and-complex-analysis-course-of-the-university-of-oxford/2023/6/a/ii/solution.md)
- [Solution](past-exam-of-the-short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford/2017/s1/1/1/solution.md)
