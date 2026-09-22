<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [matched asymptotic expansion](../../../../../../../matched-asymptotic-expansion.md), first determine the [outer expansion](../../../../../../../outer-expansion.md). Setting $\varepsilon=0$ away from $x=0$ gives $y_0'=y_0$, and the right [boundary condition](../../../../../../../boundary-condition.md) sets $y_0=e^x$. At first order,

$$
y_1'-y_1=-\frac{e^x}{2x},\qquad y_1(1)=0,
$$

so

$$
\boxed{y_{\mathrm{out}}(x)=e^x\left[1-\frac\varepsilon2\log x\right]+O(\varepsilon^2),\qquad x>0\text{ fixed}.}
$$

There is no outer $\sqrt\varepsilon$ term: its homogeneous coefficient would be forced to zero by the right boundary condition. The logarithmic overlap forces a [switchback term](../../../../../../../switchback-term.md) in the [inner expansion](../../../../../../../inner-expansion.md).

Near zero, balance $\varepsilon y''$ against $2xy'$ to get the [square-root boundary layer at a vanishing drift](../../../../../../../square-root-boundary-layer-at-a-vanishing-drift.md):

$$
s=\sqrt\varepsilon,\qquad x=sz,\qquad Y(z)=y(sz),\qquad Y''+2zY'-2szY=0.
$$

For fixed $z$ expand $Y=Y_0+sY_1+s^2Y_2+\cdots$, allowing logarithmic dependence on $s$ in $Y_2$. With $\mathcal L_0=\partial_z^2+2z\partial_z$, the leading equation is $\mathcal L_0Y_0=0$. Its bounded solutions are a constant plus an [error function](../../../../../../../error-function.md). The left boundary condition and the overlap value one fix

$$
\boxed{Y_0(z)=\operatorname{erf}z.}
$$

The following two solution sections complete the half-order and first-order matching; their headings retain the scaffold's organization of the supplied hints.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 336](../../../../paper-336-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
