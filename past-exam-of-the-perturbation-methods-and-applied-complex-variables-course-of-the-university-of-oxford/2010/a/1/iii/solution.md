<h1 id="a/1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the left inner coordinate $X=x/\delta$, the equation becomes $Y_{XXX}-Y_X+\delta^2XY=0$. At leading order the solution that matches a bounded outer expansion is $Y_0=A+De^{-X}$; the growing exponential is excluded. The boundary value gives $A+D=1$. Since $y'(0)=1$ is finite, the possible $O(\delta^{-1})$ [derivative](../../../../../derivative.md) must vanish, so $D=0$ and $A=1$.

At the next order, $Y_{1/2}=B+Ee^{-X}$. Its boundary value is zero, giving $E=-B$, while its physical [derivative](../../../../../derivative.md) at zero is $-E=1$. Hence $B=1$, and the left inner expansion is $1+\delta(1-e^{-X})+O(\delta^2)$.

At the right endpoint put $\xi=(1-x)/\delta$. The equation is $Y_{\xi\xi\xi}-Y_\xi=\delta(1-\delta\xi)Y$. Matching the outer expansion at one and imposing $Y(0)=1$ give

$$
Y_0=\sqrt e+(1-\sqrt e)e^{-\xi}.
$$

At the next order, $Y_{1/2}^{(3)}-Y_{1/2}'=Y_0$. The solution with no growing exponential, the correct matching polynomial, and $Y_{1/2}(0)=0$ is

$$
Y_{1/2}=\sqrt e(1-\xi)+
\left[\frac{1-\sqrt e}{2}\xi-\sqrt e\right]e^{-\xi}.
$$

Indeed the operator $D^3-D$ sends $-\sqrt e\,\xi$ to $\sqrt e$ and sends $\xi e^{-\xi}$ to $2e^{-\xi}$.

Add the two decaying inner corrections to the [outer solution](../../../../../outer-expansion.md), subtracting their common matching parts. Since $\delta\xi=1-x$, the [composite asymptotic expansion](../../../../../additive-composite-expansion.md) is

$$
\boxed{\begin{aligned}
y_c(x)={}&e^{x^2/2}(1+\delta)-\delta e^{-x/\delta}\\
&+e^{-(1-x)/\delta}\left[(\sqrt e-1)\left(\frac x2-\frac32\right)-\delta\sqrt e\right].
\end{aligned}}
$$

It reproduces all three boundary conditions to the retained algebraic orders, with exponentially small interactions between endpoints. The right endpoint has an $O(1)$ [boundary layer](../../../../../boundary-layer.md) in $y$. The left correction has only [amplitude](../../../../../wave-amplitude.md) $O(\sqrt\epsilon)$ in $y$, but its [derivative](../../../../../derivative.md) is $O(1)$ and is necessary for the [derivative](../../../../../derivative.md) [boundary condition](../../../../../boundary-condition.md). Thus the left layer is a [weak derivative boundary layer](../../../../../weak-derivative-boundary-layer.md); if “genuine” refers specifically to an order-one change in the function itself, only the right layer is genuine in that sense. Both nonzero corrections belong in the expansion through $O(\sqrt\epsilon)$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
