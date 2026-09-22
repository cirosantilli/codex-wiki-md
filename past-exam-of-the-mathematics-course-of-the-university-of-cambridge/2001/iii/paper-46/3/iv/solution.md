<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

On $y=0$, the unperturbed trajectory satisfies $\dot x=\sin x$. Put $a_0=\log\tan(X_0/2)$. Integration with $x(0)=X_0$ gives

$$
x(s)=2\arctan e^{s+a_0},\qquad \sin x(s)=\operatorname{sech}(s+a_0),\qquad \cos x(s)=-\tanh(s+a_0).
$$

It runs from $(0,0)$ to $(\pi,0)$, so it is the appropriate [heteroclinic orbit](../../../../../../heteroclinic-orbit.md). From the perturbed [stream function](../../../../../../stream-function.md),

$$
\mathbf u_1=(\cos x\sin y,-\sin x\cos y)\sin(\omega t).
$$

On the chosen connection, $\nabla\psi_0=(0,-\sin x)$; hence the scalar product in the [heteroclinic Melnikov function for a periodic planar flow](../../../../../../heteroclinic-melnikov-function-for-a-periodic-planar-flow.md) is $\sin^2x\sin(\omega t)$. Therefore

$$
M(X_0,t_0)=\int_{-\infty}^{\infty}\operatorname{sech}^2(\tau-t_0+a_0)\sin(\omega\tau)\,d\tau.
$$

Set $s=\tau-t_0+a_0$. The odd term $\operatorname{sech}^2s\sin(\omega s)$ integrates to zero, leaving the supplied even Fourier integral multiplied by $\sin[\omega(t_0-a_0)]$. Thus

$$
\boxed{M(X_0,t_0)=\frac{\pi\omega}{\sinh(\pi\omega/2)}\sin\left[\omega\left(t_0-\log\tan\frac{X_0}{2}\right)\right].}
$$

For every fixed $\omega\ne0$ the amplitude is nonzero and the phase zeros are simple: $\partial_{t_0}M$ there is $\pm\pi\omega^2/\sinh(\pi\omega/2)\ne0$. At fixed phase, varying $X_0$ also gives simple zeros because $da_0/dX_0=1/\sin X_0$ is nonzero for $0<X_0<\pi$. The [Melnikov splitting of a periodically perturbed cellular flow](../../../../../../melnikov-splitting-of-a-periodically-perturbed-cellular-flow.md) therefore produces transverse manifold intersections at sufficiently small perturbation and fluid-lobe exchange between adjacent cells. The unperturbed separatrix is no longer a material transport barrier.

At high frequency the leading splitting amplitude is asymptotic to $2\pi|\omega|e^{-\pi|\omega|/2}$, so fast forcing has an exponentially weak first-order effect on this connection. This is a fixed-frequency, small-$\epsilon$ result; an exponentially small leading term need not dominate higher orders in a simultaneous high-frequency limit. At exactly $\omega=0$ the perturbation itself vanishes and $M=0$, so the nonzero-frequency conclusion does not apply. Manifold splitting demonstrates intercell [chaotic advection](../../../../../../chaotic-advection.md) locally, not a proof of uniform mixing or ordinary [diffusion](../../../../../../diffusion.md) throughout the entire domain.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
