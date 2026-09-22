<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $E=\operatorname{erf}z$, $g=e^{-z^2}$ and $b=2/\sqrt\pi$. The first correction in the [inner expansion](../../../../../../../inner-expansion.md) satisfies $\mathcal L_0Y_1=2zE$. Direct differentiation verifies that $zE+bg$ is a [particular solution](../../../../../../../particular-solution.md). Adding the constant and [error function](../../../../../../../error-function.md) [homogeneous solutions](../../../../../../../homogeneous-solution.md) gives $Y_1=zE+bg+A+B E$.

The left [boundary condition](../../../../../../../boundary-condition.md) forces $A=-b$. Re-expanding the [outer expansion](../../../../../../../outer-expansion.md) at $x=sz$ gives

$$
y_{\mathrm{out}}(sz)=1+sz+s^2\left[\frac{z^2}{2}-\frac12\log z-\frac12\log s\right]+\cdots.
$$

Therefore $Y_1\sim z$, with no constant term in its large-$z$ overlap. Since $E\to1$ and $g\to0$, this sets $B=b$. Thus the required half-order correction is

$$
\boxed{Y_1(z)=z\operatorname{erf}z+\frac2{\sqrt\pi}\left[e^{-z^2}+\operatorname{erf}z-1\right].}
$$

It vanishes at zero and has the correct linear overlap. Keeping this $O(\sqrt\varepsilon)$ term is essential even though the outer solution has no correction of that order.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
