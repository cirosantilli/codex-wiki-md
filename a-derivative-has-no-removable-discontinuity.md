# A derivative has no removable discontinuity

↑ **Parent:** [Darboux's theorem (analysis)](darboux-s-theorem-analysis.md)

Let $f$ be [differentiable](differentiable-function.md) on an [open interval](open-interval.md) containing $c$. If the finite [limit of a function](limit-of-a-function.md) $L=\lim_{x\to c}f'(x)$ exists, then $f'(c)=L$.

Choose $h_n>0$ tending to zero with $[c,c+h_n]$ in the [interval](interval-mathematics.md). The [mean value theorem](mean-value-theorem.md) gives $x_n\in(c,c+h_n)$ such that

$$
f'(x_n)=\frac{f(c+h_n)-f(c)}{h_n}.
$$

The right-hand side tends to $f'(c)$ by [differentiability](differentiability.md). Since $x_n\to c$ with $x_n\ne c$, the left-hand side tends to $L$. Uniqueness of the [limit of a sequence](limit-of-a-sequence.md) gives equality. The same reasoning excludes an infinite [limit of a function](limit-of-a-function.md) for $f'$ at $c$.

Thus [derivatives](derivative.md) may be discontinuous, but a [removable discontinuity](removable-discontinuity.md) cannot be repaired by changing the value of a [derivative](derivative.md) at a single point of [differentiability](differentiability.md).

## ↑ Ancestors (8)

1. [Darboux's theorem (analysis)](darboux-s-theorem-analysis.md)
2. [Derivative](derivative.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
