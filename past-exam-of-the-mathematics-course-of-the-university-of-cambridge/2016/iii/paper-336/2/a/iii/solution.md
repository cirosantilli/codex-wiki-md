<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Define the nested [integral](../../../../../../../integral.md)

$$
H(z)=\int_0^ze^{-t^2}\int_0^te^{u^2}\operatorname{erf}(u)\,du\,dt,\qquad H(z)\sim\frac12\log z+C.
$$

The order-$s^2$ equation in the [inner expansion](../../../../../../../inner-expansion.md) is $\mathcal L_0Y_2=2zY_1$. The preceding result decomposes its forcing into $2z^2E+2bzE-2bz+2bzg$. The [particular solution](../../../../../../../particular-solution.md)s combine to

$$
Y_{2,p}=\frac12z^2E-H+bz(E-1)+b^2g.
$$

For example, $\mathcal L_0H=E$ follows directly by differentiating the nested integral, so the equation can also be verified without relying on the supplied particular-solution formulas. At zero $Y_{2,p}=b^2$; add $-b^2+D E$ to impose the left [boundary condition](../../../../../../../boundary-condition.md). As $z\to\infty$ this gives

$$
Y_2\sim\frac12z^2-\frac12\log z-C-b^2+D.
$$

The [outer expansion](../../../../../../../outer-expansion.md) in the overlap, derived in the previous section, requires the remaining constant to be $-\tfrac12\log s$. Thus $D=C+b^2-\tfrac12\log s$. The logarithmic matching constant is an [error-function logarithmic switchback](../../../../../../../error-function-logarithmic-switchback.md).

The complete answer through order $\varepsilon$ in the [inner expansion](../../../../../../../inner-expansion.md) is

$$
\boxed{\begin{aligned}
y_{\mathrm{in}}(\sqrt\varepsilon z)={}&E+\sqrt\varepsilon\,[zE+b(g+E-1)]\\
&+\varepsilon\left[\frac12z^2E-H(z)+bz(E-1)+b^2(g+E-1)+\left(C-\frac14\log\varepsilon\right)E\right]\\
&+O(\varepsilon^{3/2}|\log\varepsilon|),\qquad z=O(1).
\end{aligned}}
$$

Here $E=\operatorname{erf}z$, $g=e^{-z^2}$ and $b=2/\sqrt\pi$. This expression is zero at $z=0$, and its large-$z$ expansion agrees with $1+x+x^2/2-(\varepsilon/2)\log x$. Together with $y_{\mathrm{out}}=e^x[1-(\varepsilon/2)\log x]$, it covers both requested regions. The overlap uses $1\ll z\ll\varepsilon^{-1/2}$, with the usual termwise ordering restrictions when matching higher terms.

If a single continuous approximation is desired, an [additive composite expansion](../../../../../../../additive-composite-expansion.md) is

$$
y_{\mathrm{comp}}=y_{\mathrm{out}}(x)+y_{\mathrm{in}}(x)-\left[1+x+\frac{x^2}{2}-\frac\varepsilon2\log x\right].
$$

The apparent logarithmic divergence at $x=0$ cancels: its residual is $-(\varepsilon/2)(e^x-1)\log x\to0$. The composite therefore extends continuously to the left endpoint and satisfies the right boundary condition to the requested order.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
