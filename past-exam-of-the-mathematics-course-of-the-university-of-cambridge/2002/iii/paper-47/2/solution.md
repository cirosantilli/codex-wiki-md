<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [material derivative](../../../../../material-derivative.md) follows [surfactant](../../../../../surfactant.md) carried by the moving interface. Tangential [surface divergence](../../../../../surface-divergence.md) changes the local [surface area](../../../../../surface-area.md) and hence dilutes or concentrates insoluble material. Normal motion changes area through the [curvature](../../../../../curvature.md): an expanding [sphere](../../../../../sphere.md) has positive $u_n\nabla_s\cdot\mathbf n$ and its [concentration](../../../../../concentration.md) decreases. The last term is [surface diffusion](../../../../../surface-diffusion.md), which smooths [concentration](../../../../../concentration.md) [gradients](../../../../../gradient.md). There is no exchange with the bulk; this is [conservation of insoluble surfactant on a moving interface](../../../../../conservation-of-insoluble-surfactant-on-a-moving-interface.md).

The interfacial speed is of order $a|\mathbf F|$. Diffusion dominates redistribution when the surface [Péclet number](../../../../../peclet-number.md) satisfies

$$
\boxed{\operatorname{Pe}_s=a^2|\mathbf F|/D_s\ll1.}
$$

Then $C'/C_0=O(\operatorname{Pe}_s)$, and advection of $C'$ is a second-order effect. Write $S=\mathbf n\cdot\mathbf F\mathbf n$. Since $\mathbf u_s=\mathbf F\mathbf x-S\mathbf x$, the projected [divergence](../../../../../divergence.md) of the first term is $\operatorname{tr}\mathbf F-S=-S$, whereas the second has [divergence](../../../../../divergence.md) $2S$; its [gradient](../../../../../gradient.md) contracted with $\mathbf x$ is zero. Hence $\nabla_s\cdot\mathbf u_s=-3S$.

The leading steady transport equation is $D_s\Delta_s C'=C_0\nabla_s\cdot\mathbf u_s=-3C_0S$. Trace-freeness and the supplied [surface Laplacian](../../../../../surface-laplacian.md) identity give $\Delta_s S=-6S/a^2$. Fixing the conserved total [surfactant](../../../../../surfactant.md) removes the uniform null mode and yields

$$
\boxed{C'=AS,\qquad A=\frac{C_0a^2}{2D_s}.}
$$

This is [quadrupolar surfactant distribution on a spherical interface](../../../../../quadrupolar-surfactant-distribution-on-a-spherical-interface.md); its spherical mean is zero because $\langle n_i n_j\rangle=\delta_{ij}/3$.

With $+$ outside, $-$ inside, and the normal directed out of the bubble, the [interfacial stress balance with variable surface tension](../../../../../interfacial-stress-balance-with-variable-surface-tension.md) is

$$
(\boldsymbol\sigma_+-\boldsymbol\sigma_-)\mathbf n=\gamma\kappa\mathbf n-\nabla_s\gamma.
$$

Now $\nabla_s S=2I_s\mathbf F\mathbf n/a$, so $-\nabla_s\gamma=2A\gamma_1I_s\mathbf F\mathbf n/a$. Multiplying the [curvature](../../../../../curvature.md) by the tension and retaining linear terms gives

$$
\boxed{[\boldsymbol\sigma\mathbf n]^+_-=\frac{2\gamma_0}{a}\mathbf n+\frac{4\gamma_0}{a}(\mathbf n\cdot\mathbf D\mathbf n)\mathbf n+\frac{2A\gamma_1}{a}\bigl[I_s\mathbf F\mathbf n-(\mathbf n\cdot\mathbf F\mathbf n)\mathbf n\bigr].}
$$

The undeformed isotropic [pressure](../../../../../pressure.md) jump is kept with its normal; the perturbation terms are evaluated on the reference [sphere](../../../../../sphere.md). Products of deformation and [concentration](../../../../../concentration.md) perturbations are beyond the approximation.

The imposed [tensor](../../../../../tensor.md) is symmetric and traceless, so $\mathbf x\cdot\mathbf E\mathbf x$ is a [harmonic](../../../../../harmonic-function.md) [scalar](../../../../../scalar.md) of degree two. Its decaying partner is $\mathbf E:\nabla\nabla(1/r)$; the corresponding [harmonic](../../../../../harmonic-function.md) [vector](../../../../../vector.md) uses $\mathbf E\nabla(1/r)$. [Linearity](../../../../../linearity.md) and [rotational symmetry](../../../../../rotational-symmetry.md) give precisely these tensorial modes, with the growing [scalar](../../../../../scalar.md) chosen to reproduce the imposed strain. Thus in the unscaled convention one can take

$$
\boldsymbol\Phi=\frac{Pa^3}{3}\mathbf E\nabla(1/r),\qquad\chi=\frac12\mathbf x\cdot\mathbf E\mathbf x+\frac{Qa^5}{3}\mathbf E:\nabla\nabla(1/r).
$$

The coefficients multiply distinct decaying modes. No other angular [harmonic](../../../../../harmonic-function.md) is forced at this order.

No penetration in the steady state gives $P=3Q-1$. The given tangential surface [velocity](../../../../../velocity.md) implies $\alpha=1+2Q$. The tangential [stress](../../../../../stress.md) balance, with $M=A\gamma_1/(\mu a)$, gives $1+P-8Q=M\alpha$, or $-5Q=M(1+2Q)$. Therefore

$$
Q=-\frac M{5+2M},\quad P=-\frac{5(1+M)}{5+2M},\quad\boxed{\alpha=\frac5{5+2M}}.
$$

The nonuniform [normal stress](../../../../../normal-stress.md) is unaffected by the uniform inviscid interior [pressure](../../../../../pressure.md). Its balance is

$$
2\mu(1-3P+12Q)=\frac{4\gamma_0\beta}{a}-\frac{2A\gamma_1\alpha}{a}.
$$

Substitution and rearrangement give

$$
\boxed{\mathbf D=\frac{5\mu a}{\gamma_0}\frac{2+M}{5+2M}\mathbf E.}
$$

As $M\to\infty$, $\alpha\to0$: the concentration-induced [Marangoni stress](../../../../../marangoni-effect.md) suppresses tangential surface motion, making the exterior boundary behave like an immobile surface despite the inviscid interior. The deformation coefficient tends to $5\mu a/(2\gamma_0)$; the clean limit is $2\mu a/\gamma_0$. Both small surface [Péclet number](../../../../../peclet-number.md) and small deformation, of order $\mu a|\mathbf E|/\gamma_0$, are required. This is [Marangoni immobilization of a bubble in straining flow](../../../../../marangoni-immobilization-of-a-bubble-in-straining-flow.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
