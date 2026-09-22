<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [outer expansion](../../../../../../outer-expansion.md), the first-order reduced [ordinary differential equation](../../../../../../ordinary-differential-equation.md) gives $w_0=e^{-x^2}$ after imposing the right [boundary condition](../../../../../../boundary-condition.md). Its first correction satisfies

$$
w_1'+2xw_1=-xw_0''=2x(1-2x^2)e^{-x^2},\qquad w_1(1)=0.
$$

An integrating factor gives

$$
\boxed{w_{\mathrm{out}}(x)=e^{-x^2}\left[1+\varepsilon x^2(1-x^2)\right]+O(\varepsilon^2),\qquad x>0\text{ fixed}.}
$$

The left boundary is at $x=\varepsilon$, where the highest-derivative coefficient is already $\varepsilon^2$. Balancing that coefficient against $w'$ gives a layer of width $\varepsilon^2$, not $\varepsilon$. This is a [boundary layer around a moving endpoint](../../../../../../boundary-layer-around-a-moving-endpoint.md):

$$
z=\frac{x-\varepsilon}{\varepsilon^2},\qquad W(z)=w(\varepsilon+\varepsilon^2z),\qquad (1+\varepsilon z)W''+W'+2\varepsilon^3(1+\varepsilon z)W=0.
$$

At leading order $W_0''+W_0'=0$, and matching to the outer limit one while setting $W_0(0)=0$ gives $W_0=1-e^{-z}$. The first correction satisfies

$$
W_1''+W_1'=-zW_0''=ze^{-z}.
$$

Direct differentiation of $-z(z+2)e^{-z}/2$ verifies the forcing. It vanishes both at zero and at infinity, so no homogeneous term is needed. The requested [inner expansion](../../../../../../inner-expansion.md) is

$$
\boxed{w_{\mathrm{in}}(\varepsilon+\varepsilon^2z)=1-e^{-z}-\frac\varepsilon2z(z+2)e^{-z}+O(\varepsilon^2),\qquad z=O(1).}
$$

Its order-$\varepsilon$ overlap constant is zero, agreeing with the [outer expansion](../../../../../../outer-expansion.md) at the moving endpoint. The overlap can be chosen with $1\ll z\ll\varepsilon^{-1}$.

An independent scaling check drops the reaction term only in the layer and integrates $\varepsilon xw''+w'=0$. Its decaying fast solution is proportional to $(x/\varepsilon)^{1-1/\varepsilon}$. Since

$$
(1+\varepsilon z)^{1-1/\varepsilon}=e^{-z}\left[1+\varepsilon\left(z+\frac12z^2\right)+O(\varepsilon^2)\right],
$$

it gives exactly the same first correction. A useful [additive composite expansion](../../../../../../additive-composite-expansion.md), with the left boundary value made exact, is

$$
w_{\mathrm{comp}}(x)=w_{\mathrm{out}}(x)-w_{\mathrm{out}}(\varepsilon)e^{-z}\left[1+\frac\varepsilon2z(z+2)\right].
$$

The exponentially small remainder at the right endpoint is beyond all retained algebraic orders.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
