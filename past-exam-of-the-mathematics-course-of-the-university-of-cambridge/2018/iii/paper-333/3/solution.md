<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In an adiabatic [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md), [hydrostatic approximation](../../../../../hydrostatic-approximation.md) and [geostrophic balance](../../../../../geostrophic-balance.md) give $b'=f_0\psi_z$. The leading buoyancy equation is $D_gb'+N^2w=0$; hence $w=-D_g(f_0\psi_z/N^2)$. At the rigid surface $z=\alpha y$, the no-normal-flow condition is $D_g(z-\alpha y)=0$, so $w=\alpha v_g=\alpha\psi_x$. The small boundary slope allows the disturbance condition to be evaluated at the flattened boundary $z=0$ to the retained order.

For [thermal wind](../../../../../thermal-wind.md) $U=\Lambda z$, choose the basic [quasi-geostrophic streamfunction](../../../../../quasi-geostrophic-streamfunction.md) $\overline\psi=-\Lambda zy$. Its buoyancy anomaly is $\overline b=-f_0\Lambda y$, and its interior [quasi-geostrophic potential vorticity](../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md) is constant. Therefore the linear disturbance equations are

$$
\boxed{(\partial_t+\Lambda z\partial_x)q'=0,\qquad q'=\nabla_h^2\psi'+\frac{f_0^2}{N^2}\psi'_{zz},}
$$



$$
w'=-\frac{f_0}{N^2}\left[(\partial_t+\Lambda z\partial_x)\psi'_z-\Lambda\psi'_x\right].
$$

The term $-\Lambda\psi'_x$ is the [advection](../../../../../advection.md) of the basic meridional buoyancy gradient. Since $q'$ is simply advected at each fixed height, $q'=0$ initially implies $q'=0$ forever. At the lower boundary define $a=\alpha N^2/f_0$; then

$$
\boxed{\partial_t\psi'_z=(\Lambda-a)\psi'_x\quad(z=0).}
$$

The PDF uses $\alpha$ for the lower-boundary slope throughout; the TeX's isolated $z=cy$ is a transcription error.

For nonzero zonal wavenumber let $\mu=N|k|/|f_0|>0$. The zero-interior-[potential vorticity](../../../../../potential-vorticity.md) condition gives $\widehat\psi_{zz}-\mu^2\widehat\psi=0$. In the semi-infinite domain choose decay as $z\to\infty$. Writing $B_0(t)=\widehat\psi_z(0,t)$, [potential-vorticity inversion](../../../../../potential-vorticity-inversion.md) then gives

$$
\widehat\psi=-\frac{B_0}{\mu}e^{-\mu z},\qquad
\boxed{\dot B_0=-ik\frac{\Lambda-a}{\mu}B_0,\qquad c=\frac{\Lambda-\alpha N^2/f_0}{\mu}.}
$$

This [sloping-boundary Eady edge wave](../../../../../sloping-boundary-eady-edge-wave.md) has all its time dependence in the boundary buoyancy equation; the interior responds instantaneously through elliptic [potential-vorticity inversion](../../../../../potential-vorticity-inversion.md). A single boundary wave oscillates without exponential growth. Vertical shear and topography contribute oppositely to its propagation. The contributions cancel when $\alpha=f_0\Lambda/N^2$, the slope of a background [isopycnal](../../../../../isopycnal.md). For $f_0>0$, positive $\Lambda$ without slope gives eastward propagation, while a positive slope without shear gives westward propagation. The [phase velocity](../../../../../phase-velocity.md) varies as $1/|k|$, and the trapping depth is $1/\mu$. Its frequency is independent of $|k|$ on each signed branch, so its zonal [group velocity](../../../../../group-velocity.md) is zero in this ideal semi-infinite model.

With a rigid horizontal upper boundary, put $B_D(t)=\widehat\psi_z(D,t)$ and $M=\mu D$. Solving the same second-order inversion problem with both derivative data gives

$$
\boxed{\widehat\psi(z,t)=-\frac{\cosh[\mu(z-D)]}{\mu\sinh M}B_0(t)+\frac{\cosh(\mu z)}{\mu\sinh M}B_D(t).}
$$

Differentiation at $0$ and $D$ checks the prescribed values. At the upper boundary $w'=0$, so $(\partial_t+ik\Lambda D)B_D=ik\Lambda\widehat\psi(D)$. Combining this with the lower-boundary condition gives

$$
\boxed{\begin{aligned}
\dot B_0&=\frac{ik(\Lambda-a)}{\mu\sinh M}(-\cosh M\,B_0+B_D),\\
\dot B_D&=-ik\Lambda D\,B_D+\frac{ik\Lambda}{\mu\sinh M}(-B_0+\cosh M\,B_D).
\end{aligned}}
$$

Thus two [Boundary Rossby waves](../../../../../boundary-rossby-wave.md) interact across the layer. For normal modes proportional to $e^{-ikct}$ their dimensional wave-speed matrix is

$$
c\begin{pmatrix}B_0\\B_D\end{pmatrix}
=\begin{pmatrix}
(\Lambda-a)\coth M/\mu&-(\Lambda-a)\operatorname{csch}M/\mu\\
\Lambda\operatorname{csch}M/\mu&\Lambda D-\Lambda\coth M/\mu
\end{pmatrix}\begin{pmatrix}B_0\\B_D\end{pmatrix}.
$$

For $\Lambda\ne0$, define $C=c/(\Lambda D)$ and $\widetilde\alpha=a/\Lambda$. Its characteristic polynomial is the [Eady model with a sloping lower boundary](../../../../../eady-model-with-a-sloping-lower-boundary.md) dispersion relation

$$
\boxed{C^2-\left(1-\widetilde\alpha\frac{\coth M}{M}\right)C+(1-\widetilde\alpha)\left(\frac{\coth M}{M}-\frac1{M^2}\right)=0.}
$$

The source writes $\widetilde\mu=NkD/f_0$; for $k,f_0>0$ this is $M$, and the dispersion relation is unchanged by replacing that signed quantity by its absolute value. Its two roots are

$$
C_\pm=\frac12\left[1-\widetilde\alpha\frac{\coth M}{M}\pm\sqrt{\Delta}\right],\qquad
\Delta=\left[1-(2-\widetilde\alpha)\frac{\coth M}{M}\right]^2-4(1-\widetilde\alpha)\frac{\operatorname{csch}^2M}{M^2}.
$$

If $\widetilde\alpha>1$, the second term is positive, so $\Delta>0$ for every $M>0$: all modes are spectrally stable. If $\widetilde\alpha<1$, the increasing function $M\tanh M$ runs from zero to infinity, so there is a unique $M$ with

$$
M\tanh M=2-\widetilde\alpha.
$$

There the squared term is zero and $\Delta<0$, giving an exponentially growing member of the [complex conjugate](../../../../../complex-conjugate.md) pair. By continuity it lies in an unstable band. This proves both the requested instability for $0\leq\widetilde\alpha<1$ and [instability for negative slopes in the sloping-boundary Eady model](../../../../../instability-for-negative-slopes-in-the-sloping-boundary-eady-model.md). It does not assert that every wavelength is unstable. Strongly negative slopes move the resonant band to large $M$, where the coupling is exponentially weak.

At $\widetilde\alpha=1$ the speeds are real, but their crossing at $M=\coth M$ can give a defective neutral mode and algebraic growth; absence of exponential instability is weaker than boundedness of every initial disturbance. The nondimensional slope is undefined when $\Lambda=0$; the dimensional matrix remains valid and then has two real speeds. The instability for $\widetilde\alpha<1$ is the [counterpropagating wave instability](../../../../../counterpropagating-wave-instability.md) mechanism: lower and upper boundary waves can match their laboratory phase speeds and exchange energy with the vertical shear.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
