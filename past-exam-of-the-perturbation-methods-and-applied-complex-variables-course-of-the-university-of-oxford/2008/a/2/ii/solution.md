<h1 id="a/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Dropping the small highest-derivative term gives $y_o'+xy_o=0$. The [outer solution](../../../../../outer-expansion.md) satisfying the right endpoint condition is

$$
y_o(x)=e^{(1-x^2)/2}.
$$

It fails the left endpoint condition, so a [boundary layer](../../../../../boundary-layer.md) is needed at $x=0$. If $X=x/\epsilon^\gamma$, diffusion and first [derivative](../../../../../derivative.md) balance when $\epsilon^{1-2\gamma}=\epsilon^{-\gamma}$, giving $\gamma=1$.

With $y(x)=Y(X)$, the exact [inner expansion](../../../../../inner-expansion.md) after multiplication by $\epsilon$ is

$$
Y_{XX}+Y_X+\epsilon^2XY=0.
$$

Its leading solution is $Y=A+B e^{-X}$. The zero boundary value gives $B=-A$, and [asymptotic matching condition](../../../../../asymptotic-matching-condition.md) as $X\to\infty$, $x\to0$ fixes $A=e^{1/2}$. Thus

$$
Y(X)=e^{1/2}(1-e^{-X}).
$$

The common [overlap region](../../../../../overlap-region.md) value is $e^{1/2}$. Add the outer and inner approximations and subtract that [overlap region](../../../../../overlap-region.md):

$$
\boxed{y_c(x)=e^{(1-x^2)/2}-e^{1/2-x/\epsilon}.}
$$

The decaying inner [exponential function](../../../../../exponential-function.md) can accommodate the left condition, whereas a right-end inner coordinate would give a mode that grows into the interval. There is no right [boundary layer](../../../../../boundary-layer.md). The [composite asymptotic expansion](../../../../../additive-composite-expansion.md) satisfies the left condition exactly and the right one up to the exponentially small term $e^{1/2-1/\epsilon}$; the remaining approximation error is algebraic and vanishes as $\epsilon\downarrow0$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
