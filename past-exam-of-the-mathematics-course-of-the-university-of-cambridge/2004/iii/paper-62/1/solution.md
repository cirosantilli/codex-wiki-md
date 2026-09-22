<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose the planar [magnetic field](../../../../../magnetic-field.md) convention $\mathbf B=\nabla\times(A\mathbf e_z)$, so $B_s=s^{-1}A_\phi$ and $B_\phi=-A_s$. The [resistive induction equation](../../../../../resistive-induction-equation.md), with constant [magnetic diffusivity](../../../../../magnetic-diffusivity.md) and a suitable time-dependent gauge constant removed, reduces to advection and diffusion of this [Cartesian magnetic flux function](../../../../../cartesian-magnetic-flux-function.md):

$$
\boxed{\partial_tA+\mathbf u\cdot\nabla A=\eta\nabla^2 A.}
$$

For the specified [differential rotation](../../../../../differential-rotation.md), its mth azimuthal Fourier mode obeys

$$
\partial_ta+im(\Omega_0+\omega s^2)a=\eta\left(a_{ss}+\frac1s a_s-\frac{m^2}{s^2}a\right).
$$

The physical field is the real part of the complex mode. Substitute $a=s^mg(t)\exp[-im\Omega_0t-is^2f(t)]$. A direct radial differentiation gives

$$
\frac1a\left(a_{ss}+\frac1s a_s-\frac{m^2}{s^2}a\right)=-4i(m+1)f-4s^2f^2.
$$

On the left, rigid rotation cancels, leaving $\dot g/g-is^2\dot f+im\omega s^2$. Equating the constant and quadratic coefficients yields

$$
\dot f=m\omega-4i\eta f^2,\qquad \frac{\dot g}{g}=-4i\eta(m+1)f.
$$

The initial condition fixes $f(0)=0$ and $g(0)=1$, since the constant C was already factored out. Set $\mu^2=4i\eta m\omega$. Then the [exact quadratic-shear magnetic flux solution](../../../../../exact-quadratic-shear-magnetic-flux-solution.md) follows by differentiation:

$$
\boxed{f(t)=\frac{m\omega}{\mu}\tanh(\mu t),\qquad g(t)=[\cosh(\mu t)]^{-(m+1)}.}
$$

Indeed $\dot f=m\omega\operatorname{sech}^2(\mu t)$ and $4i\eta f^2=m\omega\tanh^2(\mu t)$. Also $\dot g/g=-(m+1)\mu\tanh(\mu t)=-4i\eta(m+1)f$. For an unspecified initial normalization the second formula has a multiplicative constant $C'$, but here $C'=1$.

For $\eta>0$ and $\omega>0$, choose $\mu=(1+i)\sqrt{2\eta m\omega}$. The asymptotic condition is $\operatorname{Re}(\mu)t\gg1$: then $f$ tends to the finite constant $m\omega/\mu$ and $g\sim2^{m+1}\exp[-(m+1)\mu t]$. At any fixed s, differentiating A to obtain the [magnetic field](../../../../../magnetic-field.md) multiplies it by factors involving $m/s$ and $sf$, which have no additional exponential time dependence. Therefore its envelope decays as

$$
\boxed{|\mathbf B|\ \hbox{has decay time}\ \tau=\frac1{(m+1)\sqrt{2\eta m\omega}}.}
$$

Using the paper's [magnetic Reynolds number](../../../../../magnetic-reynolds-number.md) definition gives the precise scaling

$$
\tau=\frac{\sqrt{\operatorname{Rm}}}{(m+1)\sqrt{2m}\,|\Omega_0|},\qquad \operatorname{Rm}=\frac{\Omega_0^2}{\eta\omega}.
$$

Thus **the decay time scales as $\operatorname{Rm}^{1/2}/\Omega_0$ for positive $\Omega_0$ and fixed m**. The mechanism is [magnetic phase mixing under differential rotation](../../../../../magnetic-phase-mixing-under-differential-rotation.md): winding produces progressively fine radial structure on which [magnetic diffusion](../../../../../magnetic-diffusion.md) acts efficiently. For negative $\omega$, choose the square root with positive real part, replacing $\omega$ by $|\omega|$ in the decay time. If $\omega=0$, the initial harmonic mode simply rotates, with $f=0$, $g=1$; there is no shear-enhanced decay. The printed positive-root and Reynolds-number expressions implicitly use $\omega>0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
