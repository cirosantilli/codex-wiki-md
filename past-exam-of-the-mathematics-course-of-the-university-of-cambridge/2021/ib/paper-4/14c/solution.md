<h1 id="14c/solution">Solution</h1>

↑ **Parent:** [14C](../14c.md)

For

$$
\theta(x,t)=t^{-1/2}e^{-x^2/(4Dt)},
$$

direct [differentiation](../../../../../partial-derivative.md) gives

$$
\theta_t
=\left(-\frac1{2t}+\frac{x^2}{4Dt^2}\right)\theta
$$

and

$$
D\theta_{xx}
=D\left(-\frac1{2Dt}+\frac{x^2}{4D^2t^2}\right)\theta
=\left(-\frac1{2t}+\frac{x^2}{4Dt^2}\right)\theta.
$$

Thus $\theta_t=D\theta_{xx}$.

Its total mass is found from the [Gaussian integral](../../../../../gaussian-integral.md):

$$
\int_{-\infty}^{\infty}\theta(x,t)\,dx
=2\sqrt{\pi D}.
$$

The unit-mass solution converging to the [Dirac delta function](../../../../../dirac-delta-function.md) as $t\downarrow0$ is therefore the [heat kernel](../../../../../heat-kernel.md)

$$
\boxed{
K(x,t)=\frac1{\sqrt{4\pi Dt}}
\exp\left(-\frac{x^2}{4Dt}\right)
}.
$$

For the second initial condition, the [heat-kernel solution](../../../../../heat-kernel-solution.md) is the [convolution](../../../../../convolution.md)

$$
\theta(x,t)
=\int_{-1}^1
\frac1{\sqrt{4\pi Dt}}
\exp\left(-\frac{(x-y)^2}{4Dt}\right)\,dy.
$$

With $u=(x-y)/(2\sqrt{Dt})$ and the definition of the [error function](../../../../../error-function.md), this becomes

$$
\boxed{
\theta(x,t)=\frac12\left[
\operatorname{Erf}\left(\frac{x+1}{2\sqrt{Dt}}\right)
-\operatorname{Erf}\left(\frac{x-1}{2\sqrt{Dt}}\right)
\right]
}.
$$

This is the [heat equation with interval-indicator initial data](../../../../../heat-equation-with-interval-indicator-initial-data.md) for $a=1$.

At $t=0$ the graph is the rectangle of height one on $[-1,1]$. For every $t>0$ it is smooth, positive and even, with its maximum at $x=0$. As time increases the graph broadens and its maximum falls, while its total area remains $2$; pointwise it tends to zero as $t\to\infty$.

## ↑ Ancestors (10)

1. [14C](../14c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
