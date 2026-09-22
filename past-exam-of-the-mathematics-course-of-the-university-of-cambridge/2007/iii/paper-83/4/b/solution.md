<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the conventional [kinematic plume fluxes](../../../../../../kinematic-plume-fluxes.md)

$$
\boxed{Q=b^2w,\qquad M=b^2w^2,\qquad F=b^2wg'.}
$$

Then $\pi Q$ is the [volume flux](../../../../../../volumetric-flow-rate.md), $\pi\rho_r Q$ the dimensional [mass flux](../../../../../../mass-flux.md), $\pi\rho_r M$ the dimensional [momentum flux](../../../../../../momentum-flux.md), and $\pi F$ the kinematic [buoyancy flux](../../../../../../buoyancy-flux.md). Calling $\pi Q$ a [mass flux](../../../../../../mass-flux.md) uses a density-normalized convention: the reference [density](../../../../../../density.md) has been suppressed. If density-weighted momentum and [buoyancy](../../../../../../buoyancy.md) fluxes are desired, multiply $M$ and $F$ by the same constant $\rho_r$ throughout. Here the conventional kinematic definitions make the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) explicit.

For an upward plume with $Q,M>0$, the inverse relations are

$$
A=\frac{Q^2}{M},\qquad w=\frac MQ,\qquad b=\frac Q{\sqrt M},\qquad B=Ag'=\frac{FQ}{M}.
$$

The [volume conservation](../../../../../../volume-conservation.md), vertical [momentum conservation](../../../../../../momentum-conservation.md), and [buoyancy](../../../../../../buoyancy.md) balances from part a become

$$
\boxed{\begin{aligned}
\partial_t\left(\frac{Q^2}{M}\right)+Q_z&=2\alpha\sqrt M,\\
Q_t+M_z&=\frac{FQ}{M},\\
\partial_t\left(\frac{FQ}{M}\right)+F_z&=-N^2Q.
\end{aligned}}
$$

Here the vertical [momentum conservation](../../../../../../momentum-conservation.md) equation uses $\rho_r$ in the inertia and retains $(\rho_0-\rho)gA=\rho_r B$ in the [buoyancy](../../../../../../buoyancy.md) force. The ambient has no imposed vertical momentum at entrainment.

To classify the resulting [partial differential equations](../../../../../../partial-differential-equation-split.md), work in the nonsingular primitive variables $(A,w,g')$ with $A>0$. Subtract $w$ times the volume equation from the momentum equation and $g'$ times the volume equation from the [buoyancy](../../../../../../buoyancy.md) equation. This gives

$$
\begin{aligned}
A_t+wA_z+Aw_z&=2\alpha w\sqrt A,\\
w_t+ww_z&=g'-\frac{2\alpha w^2}{\sqrt A},\\
g'_t+wg'_z&=-N^2w-\frac{2\alpha wg'}{\sqrt A}.
\end{aligned}
$$

The principal matrix is therefore

$$
K=\begin{pmatrix}w&A&0\\0&w&0\\0&0&w\end{pmatrix},\qquad
\det(K-\lambda I)=(w-\lambda)^3.
$$

All three [characteristic speeds](../../../../../../characteristic-speed.md) are real and equal to $w$, so the model is a [hyperbolic system](../../../../../../hyperbolic-system.md) if that term means only reality of the characteristic roots. However, for $A>0$, $(K-wI)v=0$ requires $v_w=0$, leaving only two independent [eigenvectors](../../../../../../eigenvector.md). Hence

$$
\boxed{\text{the top-hat system is weakly hyperbolic, not strictly or strongly hyperbolic}.}
$$

This [weak hyperbolicity of the unsteady top-hat plume](../../../../../../weak-hyperbolicity-of-the-unsteady-top-hat-plume.md) prevents a complete set of independent characteristic fields. For example, freezing $A,w$ in the homogeneous principal part gives $D_t\delta w=0$ and $D_t\delta A=-A\partial_z\delta w$. A Fourier perturbation of wave number $k$ therefore produces a term proportional to $kt$ in $\delta A$. Real characteristic roots alone do not provide uniform control of high-frequency perturbations. The flux-variable transformation above is invertible in the stated region, so changing to $(Q,M,F)$ does not remove this degeneracy.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
