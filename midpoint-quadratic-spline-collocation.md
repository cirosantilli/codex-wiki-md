# Midpoint quadratic spline collocation

↑ **Parent:** [Quadratic cardinal B-spline](quadratic-cardinal-b-spline.md)

Sampling order-three [Cardinal B-splines](cardinal-b-spline.md) $N_j$ at $x_i=i+3/2$ gives $N_i(x_i)=3/4$, $N_{i-1}(x_i)=N_{i+1}(x_i)=1/8$, and all other entries zero. The [B-spline collocation matrix](b-spline-collocation-matrix.md) therefore has row [strict diagonal dominance](strictly-diagonally-dominant-matrix.md) margin at least $1/2$, giving inverse [operator norm](operator-norm.md) at most two. More precisely, with $q=3-2\sqrt2$, its absolute inverse row sums are $v_i=2[1-(q^i+q^{n+1-i})/(1+q^{n+1})]$. To see this, change signs by $D_{ii}=(-1)^i$: $DAD$ has negative off-diagonal entries and a nonnegative inverse given by a convergent [Neumann series](neumann-series.md). Its inverse row sums solve $6v_i-v_{i-1}-v_{i+1}=8$, $v_0=v_{n+1}=0$. Thus $\|A^{-1}\|_\infty=v_{\lfloor(n+1)/2\rfloor}<2$, tending to two as the dimension grows.

## ↑ Ancestors (10)

1. [Quadratic cardinal B-spline](quadratic-cardinal-b-spline.md)
2. [Cardinal B-spline](cardinal-b-spline.md)
3. [B-spline](b-spline.md)
4. [Spline approximation](spline-approximation.md)
5. [Spline (mathematics)](spline-mathematics.md)
6. [Uniform approximation](uniform-approximation-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/3/2/b/solution.md)
