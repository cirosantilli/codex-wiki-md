<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

For $c\ne0$ and on an interval where $x\ne0$, the [logarithmic derivative](../../../../../logarithmic-derivative.md) substitution gives

$$
y'=\frac{x''}{cx}-\frac{x'^2}{cx^2},\qquad cy^2=\frac{x'^2}{cx^2}.
$$

The quadratic terms cancel. Multiplying by $cx$ gives the [linearization of a Riccati equation](../../../../../linearization-of-a-riccati-equation.md):

$$
\boxed{x''+a(t)x'+cb(t)x=0.}
$$

Multiplying $x$ by a nonzero constant leaves $y$ unchanged. If $c=0$, that substitution is undefined, but the original equation is already a first-order [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md), solvable by an [integrating factor](../../../../../integrating-factor.md).

For the particular equation, $c=1$ and the linear equation is $x''+x'/t-\lambda^2x/t^2=0$. Use the PDF's logarithmic coordinate $\tau=\log t$ and write $X(\tau)=x(e^\tau)$. The [chain rule](../../../../../chain-rule.md) gives $x'=X'/t$ and $x''=(X''-X')/t^2$, leaving $X''-\lambda^2X=0$. Thus $x=A t^\lambda+B t^{-\lambda}$, as also follows from the [Euler-Cauchy equation](../../../../../euler-cauchy-equation.md). Recovering the [Riccati equation](../../../../../riccati-equation.md) solution yields

$$
y(t)=\frac\lambda t\frac{A t^{2\lambda}-B}{A t^{2\lambda}+B}.
$$

The initial value imposes $A=-3B$; choose $A=3,B=-1$. Therefore

$$
\boxed{y(t)=\frac\lambda t\frac{3t^{2\lambda}+1}{3t^{2\lambda}-1},\qquad t_*=3^{-1/(2\lambda)}.}
$$

The denominator vanishes only at $t_*>0$, and its numerator is then nonzero. This is a simple pole: $y(t)\sim1/(t-t_*)$. The maximal interval containing $t=1$ is $(t_*,\infty)$; the same expression on $(0,t_*)$ is a separate solution branch. These are [poles of a Riccati solution from zeros of its linearizing solution](../../../../../poles-of-a-riccati-solution-from-zeros-of-its-linearizing-solution.md).

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
