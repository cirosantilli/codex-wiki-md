<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the positive coefficient of $y''$, setting $\epsilon=0$ gives the reduced equation $y_0'+xy_0=0$, with [general solution](../../../../../general-solution.md) $y_0=Ce^{-x^2/2}$. A fast decaying [homogeneous solution](../../../../../homogeneous-solution.md) of $\epsilon y''+y'=0$ is $e^{-x/\epsilon}$, placing the [boundary layer](../../../../../boundary-layer.md) at the left endpoint. Thus use the right [boundary condition](../../../../../boundary-condition.md) for the [outer solution](../../../../../outer-expansion.md): $y_0(1)=0$ implies

$$
\boxed{y_{\mathrm{out},0}(x)=0}.
$$

The [dominant balance](../../../../../dominant-balance.md) $\epsilon/\delta^2\sim1/\delta$ gives width $\delta=\epsilon$. With the [inner variable](../../../../../inner-variable.md) $X=x/\epsilon$ and $Y(X)=y(\epsilon X)$, the exact rescaled equation is

$$
Y_{XX}+Y_X+\epsilon^2XY=0.
$$

At leading order, $Y_{0,XX}+Y_{0,X}=0$, so $Y_0=A+Be^{-X}$. The [asymptotic matching condition](../../../../../asymptotic-matching-condition.md) $Y_0(\infty)=y_{\mathrm{out},0}(0)=0$ sets $A=0$, and $Y_0(0)=1$ sets $B=1$. Therefore

$$
\boxed{Y_0(X)=e^{-X},\qquad y_{\mathrm{comp},0}(x)=e^{-x/\epsilon}}.
$$

The [additive composite expansion](../../../../../additive-composite-expansion.md) has zero overlap to subtract. Its graph starts at one, decreases steeply over $x=O(\epsilon)$, and then stays close to zero; its initial slope is $-1/\epsilon$. The right endpoint discrepancy $e^{-1/\epsilon}$ is exponentially small. The left panel of the figure below sketches this profile. A right-end [inner expansion](../../../../../inner-expansion.md) would instead contain a growing $e^X$ term and could not repair the left endpoint mismatch.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
