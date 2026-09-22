<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

An [exponential distribution](../../../../../exponential-distribution.md) of rate $\lambda>0$ has density $f_X(x)=\lambda e^{-\lambda x}$ for $x\geq0$ and zero for $x<0$, with survival probability $\mathbb P(X>x)=e^{-\lambda x}$. For $s,t\geq0$, its [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md) follows from

$$
\boxed{\mathbb P(X>s+t\mid X>s)=\frac{e^{-\lambda(s+t)}}{e^{-\lambda s}}=e^{-\lambda t}=\mathbb P(X>t).}
$$

For the minimum, [independence](../../../../../independent-random-variables.md) gives $\mathbb P(Z>z)=\mathbb P(X>z)\mathbb P(Y>z)=e^{-2\lambda z}$. Hence

$$
\boxed{f_Z(z)=2\lambda e^{-2\lambda z}\quad(z\geq0),\qquad \mathbb P(X>Y)=\frac12.}
$$

The density is zero for negative $z$. The comparison probability follows from identical continuous laws and zero tie probability; directly it is $\int_0^\infty\lambda e^{-2\lambda y}dy=1/2$. These are [competing exponential clocks](../../../../../competing-exponential-clocks.md).

For the last density, substitute $y=s^2$ into the normalizing integral to obtain $C=2\int_0^\infty e^{-s^2}ds=\sqrt\pi$, the [Gaussian integral](../../../../../gaussian-integral.md). Equivalently, each variable has a [gamma distribution](../../../../../gamma-distribution.md) with shape $1/2$ and rate one. [Independence](../../../../../independent-random-variables.md) permits [convolution](../../../../../convolution.md) of the densities. For $z>0$,

$$
f_{G_1+G_2}(z)=\frac{e^{-z}}{C^2}\int_0^z\frac{dy}{\sqrt{y(z-y)}}.
$$

Putting $y=z\sin^2\theta$ turns the integral into $2\int_0^{\pi/2}d\theta=\pi$. Consequently

$$
\boxed{f_{G_1+G_2}(z)=e^{-z}\quad(z\geq0),\qquad G_1+G_2\sim\operatorname{Exp}(1).}
$$

This is also the [additivity of independent gamma distributions with a common rate](../../../../../additivity-of-independent-gamma-distributions-with-a-common-rate.md): their shapes add to one. Density values at the single endpoint zero are immaterial.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
