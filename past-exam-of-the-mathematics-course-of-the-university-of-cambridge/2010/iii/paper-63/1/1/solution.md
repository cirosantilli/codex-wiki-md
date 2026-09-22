<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For an autonomous [ordinary differential equation](../../../../../../ordinary-differential-equation.md), the [chain rule](../../../../../../chain-rule.md) gives $y''=f'(y)f(y)$. The formula is therefore a [multiderivative multistep method](../../../../../../multiderivative-multistep-method.md). Insert the exact solution and expand the two earlier values about $t=t_{n+2}$:

$$
y(t-h)=y-hy'+\tfrac12h^2y''-\tfrac16h^3y'''+\tfrac1{24}h^4y^{(4)}+O(h^5),
$$



$$
y(t-2h)=y-2hy'+2h^2y''-\tfrac43h^3y'''+\tfrac23h^4y^{(4)}+O(h^5).
$$

The unscaled [local truncation error](../../../../../../local-truncation-error.md) is

$$
y-\tfrac67hy'+\tfrac27h^2y''-\tfrac87y(t-h)+\tfrac17y(t-2h)
=\frac{h^4}{21}y^{(4)}+O(h^5).
$$

The coefficients through $h^3$ vanish, but the fourth-order coefficient does not. Hence **the method has order three**, not four: the one-step residual is $O(h^{p+1})$ for an order-$p$ multistep formula. Its [zero-stability](../../../../../../zero-stability.md) [polynomial](../../../../../../polynomial-split.md) is $(\zeta-1)(\zeta-1/7)$, with a simple unit root and the other root inside the [unit disk](../../../../../../unit-disk.md). Thus the stated order is also the convergence order for smooth solutions, starting errors $O(h^3)$, and the nearby implicit solution branch, by [convergence of a zero-stable multiderivative method](../../../../../../convergence-of-a-zero-stable-multiderivative-method.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
