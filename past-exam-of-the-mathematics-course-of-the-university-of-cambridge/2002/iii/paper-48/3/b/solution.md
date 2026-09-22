<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here the zero-parameter solution is $y_0=1$, but stopping there erases a weakly excited growing mode. Expand $y=1+\varepsilon y_1+\cdots$ at fixed $x$. The first correction satisfies

$$
x^2y_1''-xy_1'=2,\qquad y_1(1)=y_1'(1)=0,
$$

and therefore

$$
\boxed{y=1+\varepsilon\left[\frac{x^2-1}{2}-\log x\right]+\cdots}.
$$

The $\varepsilon x^2/2$ term eventually dominates the constant, so this is another [singular perturbation](../../../../../../singular-perturbation.md) on the unbounded domain.

Using the exact logarithmic-variable system from part (a), the initial values are now $z(0)=\varepsilon$ and $w(0)=0$. Its linear growing/stable modes have matching coefficients

$$
A=\frac{\varepsilon}{2+\varepsilon},\qquad
B=\frac2{2+\varepsilon},\qquad
C=2\varepsilon A=\frac{2\varepsilon^2}{2+\varepsilon}.
$$

Thus $w\sim Cx$ is order one only at $x=O(\varepsilon^{-2})$, rather than $O(\varepsilon^{-1})$. This is the [nonlinear crossover delayed by a small unstable-mode coefficient](../../../../../../nonlinear-crossover-delayed-by-a-small-unstable-mode-coefficient.md). The first change in the size of $y$ occurs much earlier, at $x=O(\varepsilon^{-1/2})$, when its weak growing mode becomes comparable to the initial constant; that is not yet the [derivative](../../../../../../derivative.md)-nonlinearity crossover.

At $X=Cx=O(1)$ the same [logistic crossover in a weakly nonlinear Euler equation](../../../../../../logistic-crossover-in-a-weakly-nonlinear-euler-equation.md) gives $w=X/(1+X)$ and $H(X)=X-\log(1+X)$. The nonlinear-region solution is now $y\sim H(Cx)/(\varepsilon C)$, or $\varepsilon^{-3}H(\varepsilon^2x)$ at the lowest order. A [composite asymptotic expansion](../../../../../../additive-composite-expansion.md) covering all these regions is

$$
\boxed{y_{\rm comp}(x)=A+B x^{-\varepsilon}
+\frac{H(Cx)-H(C)}{\varepsilon C},\qquad
A=\frac{\varepsilon}{2+\varepsilon},\ B=\frac2{2+\varepsilon},\ C=2\varepsilon A}.
$$

It gives $y(1)=1$ exactly, and its initial [derivative](../../../../../../derivative.md) is $O(\varepsilon^3)$ rather than zero, within leading accuracy. At fixed $x$ its expansion is precisely $1+\varepsilon[(x^2-1)/2-\log x]+O(\varepsilon^2)$; for $Cx\ll1$ it retains the weak $Ax^2$ growth, and for $Cx\gg1$ it gives $y\sim x/\varepsilon$. The positive equilibrium and boundedness argument from part (a) applies after the initially zero [derivative](../../../../../../derivative.md) immediately becomes positive. Thus the same eventual slope saturation occurs, but much farther downstream. Both the seeding calculation and the changed scale are essential to a leading approximation on the entire half-line.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
