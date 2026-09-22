<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $h=\log\psi$, with $\psi>0$, and set $f=2\alpha h_\theta$. Direct differentiation gives

$$
f_Z-ff_\theta-\alpha f_{\theta\theta}
=2\alpha\partial_\theta\left\{h_Z-\alpha h_{\theta\theta}-\alpha h_\theta^2\right\}.
$$

The [heat equation](../../../../../../heat-equation.md) $\psi_Z=\alpha\psi_{\theta\theta}$ implies $h_Z=\alpha(h_{\theta\theta}+h_\theta^2)$, so the bracket vanishes. Conversely its being independent of $\theta$ can be absorbed into a $Z$-dependent multiplicative normalization of $\psi$, leaving $f$ unchanged. This proves the [Cole-Hopf transformation](../../../../../../cole-hopf-transformation.md) with the positive sign appropriate to the negative-flux Burgers convention. Although the algebra works for nonzero $\alpha$, the given forward [Gaussian function](../../../../../../gaussian-function.md) diffusion kernel and a physical vanishing-[viscosity](../../../../../../dynamic-viscosity.md) limit require $\alpha>0$.

Take $U,L>0$ for the stated [Burgers N-wave](../../../../../../burgers-n-wave.md). Integrating $\partial_\theta\log\psi(0,\theta)=f_0(\theta)/(2\alpha)$ and normalizing the exterior value to one gives

$$
\psi_0(\theta)=\begin{cases}
\exp\{U(L^2-\theta^2)/(4\alpha)\},&|\theta|<L,\\
1,&|\theta|\geq L.
\end{cases}
$$

This function is continuous at $\pm L$; its logarithmic derivative has the specified jumps. Convolution with the [heat kernel](../../../../../../heat-kernel.md) is positive and solves the [heat equation](../../../../../../heat-equation.md) for $Z>0$. Splitting the integral into the exterior baseline and the interior correction yields

$$
\psi=1-I_\alpha(\theta,L,Z)
+\frac{e^{UL^2/(4\alpha)}}{\sqrt{4\pi\alpha Z}}
\int_{-L}^{L}\exp\left\{-\frac{U\varphi^2}{4\alpha}-\frac{(\varphi-\theta)^2}{4\alpha Z}\right\}d\varphi.
$$

Put $a=1+UZ$. Completing the square gives

$$
U\varphi^2+\frac{(\varphi-\theta)^2}{Z}
=\frac aZ\left(\varphi-\frac\theta a\right)^2+\frac{U\theta^2}{a}.
$$

Changing the interior integration variable to $\eta=a\varphi$ changes its limits to $\pm La$ and the [Gaussian function](../../../../../../gaussian-function.md) width to $Za$. The Jacobian and normalization leave the factor $a^{-1/2}$. Thus the [Cole-Hopf solution for a Burgers N-wave](../../../../../../cole-hopf-solution-for-a-burgers-n-wave.md) is

$$
\boxed{\psi=1-I_\alpha(\theta,L,Z)+I_\alpha(\theta,La,Za)\widehat\psi,\qquad
\widehat\psi=a^{-1/2}\exp\left\{\frac U{4\alpha}\left(L^2-\frac{\theta^2}{a}\right)\right\},\qquad
f=2\alpha\partial_\theta\log\psi.}
$$

Here $I_\alpha$ is the normalized [Gaussian function](../../../../../../gaussian-function.md) mass of its indicated interval. Its explicit [error function](../../../../../../error-function.md) representation is

$$
I_\alpha(\theta,b,w)=\frac12\left\{
\operatorname{erf}\left(\frac{b-\theta}{\sqrt{4\alpha w}}\right)
+\operatorname{erf}\left(\frac{b+\theta}{\sqrt{4\alpha w}}\right)\right\}.
$$

For fixed $w>0$, the [Gaussian function](../../../../../../gaussian-function.md) concentrates at $\varphi=\theta$ as $\alpha\downarrow0$. Consequently

$$
\boxed{I_\alpha(\theta,L,w)\longrightarrow H(L^2-\theta^2)}
$$

away from the endpoints; at $\theta=\pm L$ the limit is $1/2$. The transition layer has width $O(\sqrt{\alpha w})$. This is an [approximate identity](../../../../../../approximate-identity.md) argument, not a uniform step approximation across the endpoints.

For fixed $Z>0$ and $|\theta|\ll L$, both interval masses tend to one, and the exponentially large positive $\widehat\psi$ dominates the exterior correction. Its logarithmic derivative therefore gives

$$
\boxed{f(Z,\theta)\simeq-\frac{U\theta}{1+UZ}\qquad(|\theta|\ll L,\ \alpha\downarrow0).}
$$

For $|\theta|\gg La$, both interval masses are exponentially small and the weighted interior integral is also negligible, while the exterior contribution tends to one. Therefore $\boxed{f(Z,\theta)\simeq0}$ in the specified far exterior.

An exponentially weighted [Gaussian function](../../../../../../gaussian-function.md) tail should not be discarded solely because its unweighted interval mass tends to zero. In fact, comparing the order-one exterior term with $\widehat\psi$ gives the sharper inviscid [Burgers N-wave](../../../../../../burgers-n-wave.md) fronts $|\theta|=L\sqrt{1+UZ}$, not $La$. Away from these fronts, the [vanishing-viscosity limit](../../../../../../vanishing-viscosity-limit.md) is

$$
f(Z,\theta)\longrightarrow\begin{cases}
-U\theta/(1+UZ),&|\theta|<L\sqrt{1+UZ},\\
0,&|\theta|>L\sqrt{1+UZ}.
\end{cases}
$$

Inside $|\theta|<La$, this follows from the sign of $L^2-\theta^2/a$ in the exponential. Outside $La$, the constrained [Gaussian function](../../../../../../gaussian-function.md) maximum lies at an interval endpoint and has negative exponent. The right [shock wave](../../../../../../shock-wave.md)'s speed is $UL/(2\sqrt a)$, equal both to the derivative of $L\sqrt a$ and to minus half the sum of its two limiting states; the left [shock wave](../../../../../../shock-wave.md) is its reflection. This checks consistency with the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md) and shows that the requested near-center and far-exterior approximations are compatible with the full [entropy](../../../../../../entropy.md) limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
