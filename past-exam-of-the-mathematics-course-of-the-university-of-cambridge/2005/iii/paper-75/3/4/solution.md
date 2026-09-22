<h1 id="3/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $B_0>0$, change to logarithmic magnitude and its correctly transformed [probability density function](../../../../../../probability-density-function.md):

$$
x=\log(B/B_0),\qquad f(x,t)=BF(B,t),\qquad f\,dx=F\,dB.
$$

Using $\partial_B=B^{-1}\partial_x$, the radial equation becomes

$$
f_t=Df_{xx}-3Df_x.
$$

This is [diffusion](../../../../../../diffusion.md) with constant drift. Set $y=x-3Dt$ and $g(y,t)=f(y+3Dt,t)$; then $g_t=Dg_{yy}$. The initial [Dirac delta](../../../../../../dirac-delta-function.md) transforms to $f(x,0)=\delta(x)$, so the heat-kernel solution gives

$$
f(x,t)=\frac1{\sqrt{4\pi Dt}}\exp\left[-\frac{(x-3Dt)^2}{4Dt}\right].
$$

Dividing by $B$ yields the [lognormal magnetic-field amplification](../../../../../../lognormal-magnetic-field-amplification.md) law

$$
\boxed{F(B,t)=\frac1{B\sqrt{4\pi Dt}}\exp\left[-\frac{(\log(B/B_0)-3Dt)^2}{4Dt}\right],\qquad B>0.}
$$

Expanding the square and using $B=B_0e^x$ gives the equivalent requested form

$$
\boxed{F(B,t)=\frac{e^{-(9/20)\gamma t}}{B_0\sqrt{(4/5)\pi\gamma t}}\left(\frac B{B_0}\right)^{1/2}\exp\left[-\frac{[\log(B/B_0)]^2}{(4/5)\gamma t}\right].}
$$

The logarithm is a [Gaussian random variable](../../../../../../gaussian-random-variable.md) with mean $3Dt$ and variance $2Dt$, which proves normalization and spreading directly. The exponential moments of that [Gaussian distribution](../../../../../../normal-distribution.md) give $\langle B^q\rangle=B_0^qe^{Dq(q+3)t}$, independently checking the energy growth. The limit at $t\downarrow0$ is the initial [Dirac delta](../../../../../../dirac-delta-function.md) distribution, not a pointwise finite function.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
