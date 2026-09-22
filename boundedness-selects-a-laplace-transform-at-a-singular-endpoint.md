# Boundedness selects a Laplace transform at a singular endpoint

↑ **Parent:** [Laplace transform](laplace-transform.md)

A bounded [function](function-split.md) on $[0,\infty)$ has a [Laplace transform](laplace-transform.md) satisfying the displayed bound, by integration of $|y(t)e^{-pt}|$. Consequently its [Laplace transform](laplace-transform.md) cannot have a pole of order two or higher at $p=0$. This can eliminate the arbitrary constant introduced when multiplication by $t$ turns an [ordinary differential equation](ordinary-differential-equation.md) into a first-order [differential equation](differential-equation-split.md) for its [Laplace transform](laplace-transform.md).

For example, transforming $ty''+(t-1)y'-y=0$ with $y(0)=1$ gives $p(p+1)Y'+(3p+2)Y=2$. An [integrating factor](integrating-factor.md) $p^2(p+1)$ yields

$$
Y(p)=\frac1{p+1}+\frac{C}{p^2(p+1)}.
$$

The bound forces $C=0$, selecting $y=e^{-t}$. This selection can be justified without assuming unproved endpoint regularity for every solution: $e^{-t}$ and $t-1$ have nonzero [Wronskian](wronskian.md) $te^{-t}$ on $(0,\infty)$, so they form a [fundamental system of solutions](fundamental-system-of-solutions.md). Boundedness removes $t-1$, and the limit at zero fixes the remaining coefficient. The endpoint limit by itself does not select a unique solution.

## ↑ Ancestors (6)

1. [Laplace transform](laplace-transform.md)
2. [Integral transform](integral-transform-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2007/9/solution.md)
