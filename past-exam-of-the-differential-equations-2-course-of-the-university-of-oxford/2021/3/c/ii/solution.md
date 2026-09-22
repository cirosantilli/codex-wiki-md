<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The reduced equation and the left [boundary condition](../../../../../boundary-condition.md) give the leading [outer solution](../../../../../outer-expansion.md)

$$
y_{\mathrm{out},0}'=y_{\mathrm{out},0},\qquad y_{\mathrm{out},0}(1)=1,
\qquad\boxed{y_{\mathrm{out},0}(x)=e^{x-1}.}
$$

Introduce the right [inner variable](../../../../../inner-variable.md) $X=(2-x)/\epsilon\geq0$ and write $Y(X)=y(2-\epsilon X)$. The [chain rule](../../../../../chain-rule.md) gives $y'=-Y_X/\epsilon$ and $y''=Y_{XX}/\epsilon^2$. Multiplying the rescaled [differential equation](../../../../../differential-equation-split.md) by $\epsilon$ gives the exact equation

$$
Y_{XX}+(2-\epsilon X)Y_X+\epsilon(2-\epsilon X)Y=0.
$$

At leading order, $Y_{0,XX}+2Y_{0,X}=0$, with [general solution](../../../../../general-solution.md) $Y_0=A+Be^{-2X}$. The right [boundary condition](../../../../../boundary-condition.md) gives $Y_0(0)=0$. The [asymptotic matching condition](../../../../../asymptotic-matching-condition.md) in the [overlap region](../../../../../overlap-region.md) $\epsilon\ll2-x\ll1$ gives

$$
\lim_{X\to\infty}Y_0(X)=\lim_{x\to2^-}y_{\mathrm{out},0}(x)=e.
$$

Thus $A=e$ and $B=-e$, yielding the leading [inner expansion](../../../../../inner-expansion.md)

$$
\boxed{Y_0(X)=e(1-e^{-2X}),\qquad
y_{\mathrm{in},0}(x)=e\left(1-e^{-2(2-x)/\epsilon}\right).}
$$

Equivalently, the [inner variable](../../../../../inner-variable.md) $\xi=2(2-x)/\epsilon$ gives $Y_0=e(1-e^{-\xi})$. Both normalizations describe the same [boundary layer](../../../../../boundary-layer.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
