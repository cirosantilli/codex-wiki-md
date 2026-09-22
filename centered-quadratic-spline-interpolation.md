# Centered quadratic spline interpolation

↑ **Parent:** [Spline interpolation operator](spline-interpolation-operator.md)

For unit-spaced order-three [B-splines](b-spline.md) sampled at [support](support.md) midpoints $i+3/2$, the [B-spline collocation matrix](b-spline-collocation-matrix.md) has diagonal $3/4$ and neighboring entries $1/8$. Conjugating by alternating diagonal signs reduces its inverse absolute values to the nonnegative inverse of $\operatorname{tridiag}(-1,6,-1)/8$. With $\tau=3-2\sqrt2$, the absolute row sums are $r_i=2[1-(\tau^i+\tau^{n+1-i})/(1+\tau^{n+1})]$. This follows by solving $6r_i-r_{i-1}-r_{i+1}=8$ with $r_0=r_{n+1}=0$. The maximum occurs at the middle row or rows and tends to two as $n$ grows. Nonnegativity and subpartition of unity of the [B-splines](b-spline.md) transfer this bound to the [spline interpolation operator](spline-interpolation-operator.md).

## ↑ Ancestors (9)

1. [Spline interpolation operator](spline-interpolation-operator.md)
2. [Spline interpolation](spline-interpolation.md)
3. [Spline approximation](spline-approximation.md)
4. [Spline (mathematics)](spline-mathematics.md)
5. [Uniform approximation](uniform-approximation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/4/2/b/solution.md)
