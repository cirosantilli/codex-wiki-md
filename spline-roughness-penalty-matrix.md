# Spline roughness penalty matrix

↑ **Parent:** [Natural cubic spline interpolant](natural-cubic-spline-interpolant.md)

Let $b_i=N e_i$ be the interpolating cardinal basis and set $\Gamma_{ij}=\int_a^b b_i^{\prime\prime}b_j^{\prime\prime}\,dx$. Linearity gives $J(N\mathbf v)=\mathbf v^T\Gamma\mathbf v$, and this [Gram matrix](gram-matrix.md) is a [positive semidefinite matrix](positive-semidefinite-matrix.md). Its [null space](kernel-of-a-linear-map.md) consists precisely of [vectors](vector.md) $(\alpha+\beta x_i)_i$, by the null-space statement for the [second derivative roughness penalty](second-derivative-roughness-penalty.md). Thus its rank is $n-2$, including the zero [matrix](matrix.md) when $n=2$.

## ↑ Ancestors (10)

1. [Natural cubic spline interpolant](natural-cubic-spline-interpolant.md)
2. [Natural cubic spline](natural-cubic-spline.md)
3. [Cubic spline](cubic-spline.md)
4. [Spline approximation](spline-approximation.md)
5. [Spline (mathematics)](spline-mathematics.md)
6. [Uniform approximation](uniform-approximation-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210/4/solution.md)
