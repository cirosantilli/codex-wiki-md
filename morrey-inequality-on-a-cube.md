# Morrey inequality on a cube

↑ **Parent:** [Sobolev embedding theorem](sobolev-embedding-theorem.md)

For a cube $Q$ of side length $r$ in $\mathbb R^n$, $p>n$, and a [continuously differentiable function](continuously-differentiable-function.md) $v$, its average $v_Q=|Q|^{-1}\int_Qv$ satisfies

$$
|v(y)-v_Q|\leq C_{n,p}r^{1-n/p}\|Dv\|_{L^p(Q)}\qquad(y\in Q).
$$

Averaging the [fundamental theorem of calculus along a line segment](fundamental-theorem-of-calculus-along-a-line-segment.md) from $y$ to $z\in Q$ and changing variables gives $|v(y)-v_Q|\leq C_n\int_Q|Dv(w)|\,|w-y|^{1-n}dw$. The [Holder inequality](holder-inequality.md) applies because $(n-1)p'<n$, and the kernel norm is $O(r^{1-n/p})$. Approximation extends the estimate to the continuous representative of a [Sobolev space](sobolev-space-split.md) function. On $\mathbb R^n$ it yields a [Hölder continuous function](holder-condition.md) of exponent $1-n/p$ representing every $W^{1,p}$ class.

## ↑ Ancestors (7)

1. [Sobolev embedding theorem](sobolev-embedding-theorem.md)
2. [Sobolev space](sobolev-space-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Differentiability almost everywhere of supercritical Sobolev functions](differentiability-almost-everywhere-of-supercritical-sobolev-functions.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/1/b/solution.md)
