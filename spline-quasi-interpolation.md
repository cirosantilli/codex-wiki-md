# Spline quasi-interpolation

↑ **Parent:** [Spline approximation](spline-approximation.md)

A [spline](spline-mathematics.md) quasi-interpolant synthesizes a [B-spline](b-spline.md) expansion from local bounded [linear functionals](linear-functional.md), instead of solving a global interpolation system. Suppose each functional is bounded by $c_k\|f\|_{C[t_i,t_{i+k}]}$ and the operator reproduces every [spline](spline-mathematics.md). On a knot cell $[t_j,t_{j+1}]$, only indices $j+1-k\le i\le j$ contribute. Their [supports](support.md) lie in $[t_{j+1-k},t_{j+k}]$, and [subpartition of unity for B-splines](subpartition-of-unity-for-b-splines.md) proves local [operator norm](operator-norm.md) at most $c_k$. Reproduction of degree-$k-1$ [polynomials](polynomial-split.md) and a local [Taylor theorem](taylor-theorem.md) remainder then give error at most $(1+c_k)(2k-1)^k h^k\|f^{(k)}\|_\infty/k!$, on the basic knot domain with the usual completed boundary [basis](basis.md).

## ↑ Ancestors (7)

1. [Spline approximation](spline-approximation.md)
2. [Spline (mathematics)](spline-mathematics.md)
3. [Uniform approximation](uniform-approximation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [De Boor–Fix spline coefficient functional](de-boor-fix-spline-coefficient-functional.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/6/solution.md)
