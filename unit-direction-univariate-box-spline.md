# Unit-direction univariate box spline

↑ **Parent:** [Box spline](box-spline.md)

The unit-direction univariate [box spline](box-spline.md) is the density of the sum of $m$ independent uniform unit-interval coordinates. It is the order-$m$ [Cardinal B-spline](cardinal-b-spline.md): its closed support is $[0,m]$, it is strictly positive on the interior, and its [polynomial](polynomial-split.md) degree is $m-1$. For $m\geq2$ it is $C^{m-2}$, generally not $C^{m-1}$. The recurrence $B_m(x)=\int_0^1B_{m-1}(x-u)du$ proves its support and positivity. Starting with a half-open unit interval, integrating the translate partition recursively proves $\sum_{j\in\mathbb Z}B_m(x-j)=1$. Orthogonal projection onto the unit diagonal rescales support width from $m$ to $\sqrt m$.

## ↑ Ancestors (8)

1. [Box spline](box-spline.md)
2. [Spline approximation](spline-approximation.md)
3. [Spline (mathematics)](spline-mathematics.md)
4. [Uniform approximation](uniform-approximation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/5/solution.md)
