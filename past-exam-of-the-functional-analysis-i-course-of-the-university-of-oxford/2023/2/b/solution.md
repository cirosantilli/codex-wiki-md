<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $p'$ be the [Holder conjugate exponent](../../../../conjugate-exponents.md) of $p$, with $1/\infty=0$. The [indicator function](../../../../indicator-function.md) $\mathbf1_{(-h,h)}$ has [Lp norm](../../../../lp-norm.md) $(2h)^{1/p'}$ in $L^{p'}$, including the value one when $p'=\infty$. The [Holder inequality](../../../../holder-inequality.md) therefore gives

$$
|T_hf|\leq h^{-1/p'}\|f\|_p\|\mathbf1_{(-h,h)}\|_{p'}
=2^{1/p'}\|f\|_p.
$$

The [Lebesgue integral](../../../../lebesgue-integral.md) is unchanged by equality [almost everywhere](../../../../almost-everywhere.md), so $T_h$ is well-defined on the [Lp space](../../../../lp-space.md); its [linearity](../../../../linearity.md) and the bound put it in the [continuous dual space](../../../../continuous-dual-space-split.md) $X^*$.

For $p<\infty$, the [function](../../../../function-split.md) $f_h=(2h)^{-1/p}\mathbf1_{(-h,h)}$ has [Lp norm](../../../../lp-norm.md) one and satisfies

$$
T_hf_h=h^{-1/p'}(2h)^{1-1/p}=2^{1/p'}.
$$

For $p=\infty$, use $f_h=\mathbf1_{(-h,h)}$, whose [L-infinity norm](../../../../l-infinity-norm.md) is one and whose image is $2$. Thus all endpoints are included in

$$
\boxed{T_h\in X^*,\qquad\|T_h\|=2^{1/p'}\quad(0<h<1).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the functional analysis I course of the University of Oxford](../../../split.md)
5. [Functional analysis I course of the University of Oxford](../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
