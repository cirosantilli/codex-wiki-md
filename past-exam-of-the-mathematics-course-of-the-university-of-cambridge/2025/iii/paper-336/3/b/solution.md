<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The reduced first-order equation cannot satisfy both endpoint values. The given [outer expansion](../../../../../../outer-expansion.md) satisfies $y(1)=2$ but has $y_0(0)=e$, so the [boundary layer](../../../../../../boundary-layer.md) lies at $x=0$ and has stretched coordinate $X=x/\epsilon$.

Write the [inner expansion](../../../../../../inner-expansion.md) as $Y=Y_0+\epsilon Y_1+\cdots$. After multiplying the differential equation by $\epsilon$, it becomes

$$
Y_{XX}+(1+\epsilon X)Y_X+\epsilon^2XY=0.
$$

At leading order,

$$
Y_0''+Y_0'=0.
$$

The boundary condition $Y_0(0)=0$ and matching to $y_0(0)=e$ give

$$
\boxed{Y_0=e(1-e^{-X}).}
$$

At the next order,

$$
Y_1''+Y_1'=-XY_0'=-eXe^{-X}.
$$

Matching to $y_1(0)=e(\ln2-1)$ and imposing $Y_1(0)=0$ gives

$$
\boxed{
Y_1=e(\ln2-1)
+ee^{-X}\left(\frac{X^2}{2}+X+1-\ln2\right).}
$$

The [additive composite expansion](../../../../../../additive-composite-expansion.md) is outer plus inner minus their common part. With $X=x/\epsilon$, it is

$$
\boxed{
\begin{aligned}
y_{\rm comp}(x)={}&(1+x)e^{1-x}\\
&+\epsilon[-(1+x)\ln(1+x)+(1+x)\ln2+(x-1)]e^{1-x}\\
&+ee^{-x/\epsilon}\left[-1+\epsilon\left(
\frac12\left(\frac x\epsilon\right)^2
+\frac x\epsilon+1-\ln2\right)\right].
\end{aligned}}
$$

It satisfies $y_{\rm comp}(0)=0$ exactly through the retained order, satisfies the right boundary condition up to exponentially small terms, and is uniformly accurate to $O(\epsilon)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
