# Laplacian as departure from a local average

↑ **Parent:** [Laplacian](laplacian.md)

The [Laplacian](laplacian.md) detects whether a value lies below or above nearby values, to second order. For a [scalar field](scalar-field.md) whose [partial derivatives](partial-derivative.md) through order four are [continuous functions](continuous-function.md), take the [arithmetic mean](arithmetic-mean.md) of four equally spaced neighbors:

$$
A_hf(x,y)=\frac{f(x+h,y)+f(x-h,y)+f(x,y+h)+f(x,y-h)}4.
$$

Applying [Taylor's theorem](taylor-s-theorem.md) in each coordinate cancels the first- and third-order terms between opposite neighbors. The two pairs leave

$$
A_hf(x,y)-f(x,y)=\frac{h^2}4\Delta f(x,y)+O(h^4),\qquad h\to0.
$$

This is an [asymptotic expansion](asymptotic-expansion-split.md), rather than an equality for arbitrary $h$. Rearranging gives the familiar [central finite difference](central-finite-difference.md) approximation

$$
\Delta f(x,y)=\frac{f(x+h,y)+f(x-h,y)+f(x,y+h)+f(x,y-h)-4f(x,y)}{h^2}+O(h^2).
$$

This [finite difference](finite-difference-split.md) replaces [partial derivatives](partial-derivative.md) by five sampled values. The [arithmetic mean](arithmetic-mean.md) lies above the center for a sufficiently small $h$ if the [Laplacian](laplacian.md) is strictly positive there, and below if it is strictly negative. A zero [Laplacian](laplacian.md) cancels this second-order discrepancy without requiring equality of individual values.

At $(0,0)$, the bowl $x^2+y^2$ has center value zero and four neighbor values $h^2$, so the discrepancy is exactly $h^2$. The saddle $x^2-y^2$ has neighbor values $h^2,h^2,-h^2,-h^2$, whose [arithmetic mean](arithmetic-mean.md) is exactly zero. For the [Gaussian function](gaussian-function.md) $e^{-x^2-y^2}$ the discrepancy is $e^{-h^2}-1=-h^2+O(h^4)$, agreeing with $\Delta f(0,0)=-4$.

A [harmonic function](harmonic-function.md) need not equal this four-neighbor [arithmetic mean](arithmetic-mean.md) for a finite $h$. The [polynomial](polynomial-split.md) $f(x,y)=x^4-6x^2y^2+y^4$ has $\Delta f=0$ everywhere, but $A_hf(0,0)=h^4$. Higher-order terms remain even when the second-order terms cancel.

At a [local minimum](local-minimum.md), each coordinate [second derivative](second-derivative.md) is at least zero, hence the [Laplacian](laplacian.md) is at least zero. At a [local maximum](local-maximum.md) the inequality reverses. The sum alone does not characterize an extremum: cancellation at a [saddle point of a scalar function](saddle-point-of-a-scalar-function.md) can also produce zero. The local-average interpretation explains why the [heat equation](heat-equation.md) smooths differences, and helps motivate the [heat equation maximum principle](heat-equation-maximum-principle.md).

## ↑ Ancestors (9)

1. [Laplacian](laplacian.md)
2. [Vector calculus](vector-calculus.md)
3. [Multivariable calculus](multivariable-calculus-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
