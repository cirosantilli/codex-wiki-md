<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $h=\log\psi$ and $f=2\alpha h_\theta$. Direct substitution into the [viscous Burgers equation](../../../../../../viscous-burgers-equation.md) gives

$$
f_Z-ff_\theta-\alpha f_{\theta\theta}=2\alpha\partial_\theta\left(h_Z-\alpha h_{\theta\theta}-\alpha h_\theta^2\right).
$$

If $\psi_Z=\alpha\psi_{\theta\theta}$, then $h_Z=\alpha(h_{\theta\theta}+h_\theta^2)$, proving the [Cole-Hopf transformation](../../../../../../cole-hopf-transformation.md). A function of $Z$ inside the parentheses can be removed by rescaling $\psi$ by a time-dependent factor, which leaves $f$ unchanged.

For the forward [heat equation](../../../../../../heat-equation.md) and the displayed Gaussian kernel we require **$\alpha>0$ and $Z>0$**. The algebraic transformation works for nonzero $\alpha$, but the printed convolution is not a forward solution for negative $\alpha$: its Gaussian then grows and the step-data integral diverges.

Integrating the initial logarithmic derivative fixes a convenient positive initial heat datum,

$$
\psi(0,\phi)=\begin{cases}1,&\phi<0,\\e^{U\phi/(2\alpha)},&\phi>0.\end{cases}
$$

Split the [heat kernel](../../../../../../heat-kernel.md) convolution at zero and complete the square in the positive half. With $h_*=U(2\theta+UZ)/(4\alpha)$, put

$$
A_0=\int_\theta^\infty e^{-y^2/(4\alpha Z)}dy,\qquad C_0=\int_{-(\theta+UZ)}^\infty e^{-y^2/(4\alpha Z)}dy.
$$

Then $\psi=(A_0+e^{h_*}C_0)/\sqrt{4\pi\alpha Z}$. On differentiation, the moving-limit terms cancel because $e^{h_*}e^{-(\theta+UZ)^2/(4\alpha Z)}=e^{-\theta^2/(4\alpha Z)}$. Hence

$$
\boxed{f(Z,\theta)=\frac{Ue^{h_*}C_0}{A_0+e^{h_*}C_0}=\frac{U}{1+J e^{-U(2\theta+UZ)/(4\alpha)}},\qquad J=\frac{A_0}{C_0}.}
$$

This is the [viscous Burgers step solution with negative flux](../../../../../../viscous-burgers-step-solution-with-negative-flux.md). Both integrals can be written as $\sqrt{\pi\alpha Z}$ times a [complementary error function](../../../../../../complementary-error-function.md).

For fixed $Z>0$, the Gaussian-tail asymptotics give **$f\to U$ as $\theta\to+\infty$** and **$f\to0$ as $\theta\to-\infty$**. For example $Je^{-h_*}$ tends to zero on the right with a Gaussian factor $e^{-(\theta+UZ)^2/(4\alpha Z)}$, while on the left it diverges with a Gaussian factor $e^{\theta^2/(4\alpha Z)}$. This holds for either sign of $U$; for $U=0$ the solution is already zero.

The Gaussian tail is strictly decreasing in its lower limit, so $J=1$ occurs exactly at $\theta=-UZ/2$. There $h_*=0$, and **$f=U/2$**. For $U>0$, the two lower limits are both far into the negative tail in the mature shock region, so $J\simeq1$ throughout its thin transition. The solution is then approximately the traveling viscous front

$$
f\simeq\frac U2\left[1+\tanh\frac{U(\theta+UZ/2)}{4\alpha}\right],
$$

centred at the inviscid shock position, with thickness of order $\alpha/U$.

In the [vanishing-viscosity limit](../../../../../../vanishing-viscosity-limit.md), for $U>0$ the solution tends to the compressive [entropy solution](../../../../../../entropy-solution.md) of part (a), away from its shock. For $U<0$, it tends instead to the [rarefaction wave](../../../../../../rarefaction-wave.md). To see the latter explicitly inside $0<\theta<-UZ$, both tails have positive lower limits, and their leading asymptotics give $Je^{-h_*}\to(-\theta-UZ)/\theta$. Thus $f\to-\theta/Z$ in the fan, with the constant states outside. Although $J=1$ still marks the fan midpoint, it is not approximately one throughout the expanding fan; replacing it by one there would create an inadmissible compressive-front approximation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
