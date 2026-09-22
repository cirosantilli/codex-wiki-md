<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Away from the thin layer, set $\epsilon=0$. The outer equation is

$$
(1+x)^3y_{\rm out}'+y_{\rm out}=0,
$$

and the boundary condition selected by this first-order problem is the right-end condition. Thus

$$
\boxed{
y_{\rm out}(x)
=\exp\left[
\frac1{2(1+x)^2}-\frac18
\right]},
$$

which satisfies $y_{\rm out}(1)=1$ but has $y_{\rm out}(0)=e^{3/8}$.

The missing left condition is supplied by an [outflow boundary layer](../../../../../../outflow-boundary-layer.md). Put $X=x/\epsilon$ and $y=Y(X)$. After multiplication by $\epsilon$, the equation is

$$
Y_{XX}+(1+\epsilon X)^3Y_X+\epsilon Y=0.
$$

At leading order,

$$
Y_{0,XX}+Y_{0,X}=0.
$$

The conditions $Y_0(0)=1$ and $Y_0\to y_{\rm out}(0)=e^{3/8}$ as $X\to\infty$ give

$$
\boxed{
Y_0(X)=e^{3/8}
+(1-e^{3/8})e^{-X}}.
$$

The common overlap is $e^{3/8}$. The [additive composite expansion](../../../../../../additive-composite-expansion.md) is therefore

$$
\boxed{
y_{\rm comp}(x)
=\exp\left[
\frac1{2(1+x)^2}-\frac18
\right]
+(1-e^{3/8})e^{-x/\epsilon}}.
$$

It satisfies both endpoint values up to exponentially small or higher-order errors and is uniformly valid to $O(1)$ on $0\leq x\leq1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
