# L1 bound for a Volterra power-kernel integral

↑ **Parent:** [Volterra power-kernel integral](volterra-power-kernel-integral.md)

For nonnegative integrable $f$, [Tonelli's theorem](tonelli-theorem.md) applied on the triangle $0<y<x<1$ gives the exact identity

$$
\|V_\beta f\|_1=\int_0^1f(y)\left(\int_y^1(x-y)^{\beta-1}\,dx\right)dy
=\frac1\beta\int_0^1(1-y)^\beta f(y)\,dy\leq\frac1\beta\|f\|_1.
$$

For signed or complex integrable $f$, first apply the same calculation to $|f|$ and use the [triangle inequality for an integral](integral-triangle-inequality.md). The defining [integral](integral-split.md) then exists absolutely for [almost every](almost-everywhere.md) $x$, and the same [L1 norm](l1-norm.md) bound holds. The constant $1/\beta$ is sharp: use $f_n=n\mathbf1_{(0,1/n)}$, whose [L1 norm](l1-norm.md) is one and whose weighted [integrals](integral-split.md) above tend to $1/\beta$.

Finiteness at every point is stronger than this [L1 space](l1-space.md) assertion. For $0<\beta<1$, take $x_0=1/2$, $\gamma=(1+\beta)/2$, and $f(y)=(x_0-y)^{-\gamma}$ on $(0,x_0)$, zero otherwise. It is integrable because $\gamma<1$, but $(V_\beta f)(x_0)=\infty$ because the power near $y=x_0$ is $\beta-1-\gamma=(\beta-3)/2<-1$. This is compatible with an integrable output after changing values on a [null set](null-set.md).

## ↑ Ancestors (8)

1. [Volterra power-kernel integral](volterra-power-kernel-integral.md)
2. [Volterra operator](volterra-operator.md)
3. [Integral operator](integral-operator.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2014/3/c/ii/solution.md)
- [Volterra power-kernel integral](volterra-power-kernel-integral.md)
