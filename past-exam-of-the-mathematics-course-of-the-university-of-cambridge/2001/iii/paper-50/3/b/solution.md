<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the positive-drift equation, the [outer expansion](../../../../../../outer-expansion.md) obeys $(1+x)y_0'+y_0=0$. Select the boundary condition at the right endpoint, obtaining $y_0=2/(1+x)$. The first correction satisfies

$$
(1+x)y_1'+y_1=-y_0''=-\frac4{(1+x)^3},\qquad y_1(1)=0.
$$

Integrating $[(1+x)y_1]'=-4/(1+x)^3$ gives

$$
\boxed{y_{\rm out}=\frac2{1+x}+\epsilon\left[\frac2{(1+x)^3}-\frac1{2(1+x)}\right]+O(\epsilon^2).}
$$

The [boundary condition](../../../../../../boundary-condition.md) mismatch is at $x=0$. Set $X=x/\epsilon$ and use the [inner expansion](../../../../../../inner-expansion.md) $Y=Y_0+\epsilon Y_1+\cdots$. The inner equation is $Y_{XX}+(1+\epsilon X)Y_X+\epsilon Y=0$. At leading order, matching to $2$ and imposing $Y(0)=1$ give $Y_0=2-e^{-X}$. At first order,

$$
Y_1''+Y_1'=-2+(1-X)e^{-X},\qquad Y_1(0)=0.
$$

The outer expansion in the overlap is $2+\epsilon(3/2-2X)$. Matching its constant and linear terms gives

$$
\boxed{Y_{\rm in}=2-e^{-X}+\epsilon\left[-2X+\frac32+\left(\frac{X^2}2-\frac32\right)e^{-X}\right]+O(\epsilon^2).}
$$

The [additive composite expansion](../../../../../../additive-composite-expansion.md) adds inner and outer approximations and subtracts the common overlap:

$$
\boxed{y_{\rm comp}=\frac2{1+x}+\epsilon\left[\frac2{(1+x)^3}-\frac1{2(1+x)}\right]-e^{-x/\epsilon}+\epsilon\left[\frac{x^2}{2\epsilon^2}-\frac32\right]e^{-x/\epsilon}.}
$$

It meets the left condition exactly and the right condition up to exponentially small terms, with an $O(\epsilon^2)$ uniform asymptotic error. This is the [first-order composite expansion for a positive drift](../../../../../../first-order-composite-expansion-for-a-positive-drift.md) specialized to the present coefficients.

Reversing the drift moves the decaying [boundary layer](../../../../../../boundary-layer.md) to $x=1$; the outer solution is selected at $x=0$. For the second equation, $y_{\rm out}=1+x$ is in fact an exact solution, but predicts $2$ at the right boundary instead of $1+\epsilon$. Put $X=(1-x)/\epsilon$. The inner equation becomes

$$
Y_{XX}+(2-\epsilon X)Y_X+\epsilon Y=0.
$$

Matching to $2-\epsilon X$ gives

$$
Y_0=2-e^{-2X},\qquad Y_1=-X+(1-X-X^2/2)e^{-2X}.
$$

Indeed, $Y_1''+2Y_1'=-2+(1+2X)e^{-2X}$ and $Y_1(0)=1$, as required by the order-$\epsilon$ boundary value. Since $d/dx=-\epsilon^{-1}d/dX$, $Y_0'(0)=2$ and $Y_1'(0)=-4$ give the [endpoint derivative in a negative-drift boundary layer](../../../../../../endpoint-derivative-in-a-negative-drift-boundary-layer.md):

$$
\boxed{y'(1)=-\frac2\epsilon+4+O(\epsilon).}
$$

The order-one term cannot be obtained by differentiating the leading inner solution alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
