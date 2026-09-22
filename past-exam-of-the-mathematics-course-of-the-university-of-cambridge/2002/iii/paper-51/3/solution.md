<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A large [molecular Schmidt number](../../../../../schmidt-number-fluid-mechanics.md) $\mathrm{Sc}=\nu/\kappa$ separates the velocity's smallest smooth length scale from the scalar's smaller diffusive length scale. Follow a [Lagrangian trajectory](../../../../../lagrangian-trajectory.md) $X(t)$ and measure displacement $x$ from it. Within a sufficiently small scalar packet, Taylor expansion of the smooth [velocity field](../../../../../velocity-field.md) gives

$$
u(X(t)+x,t)-u(X(t),t)=C(t)x+O(\|\nabla^2u\|\,|x|^2),
\qquad C_{ij}(t)=\partial_j u_i(X(t),t),\qquad\operatorname{tr}C=0.
$$

The moving frame removes uniform sweeping, leaving a linear random [velocity gradient tensor](../../../../../velocity-gradient-tensor.md). Thus the local scalar equation is the [advection-diffusion equation](../../../../../advection-diffusion-equation.md) with velocity $Cx$, and averaging over realizations of $C$ gives the corresponding [ensemble average](../../../../../expected-value.md). The approximation requires the packet to lie within the velocity's locally smooth region. Its thin, diffusive direction can satisfy this condition even when its long direction eventually becomes too large for one global linearization; applications to a spatially varying flow then use local packet descriptions. The statistical conclusions below refer to the linear-flow model and the usual mixing assumptions, not to every conceivable trace-free random matrix process.

Write $Q=\int\chi\,dA$ and assume sufficiently rapid decay to discard boundary terms. [Integration by parts](../../../../../integration-by-parts.md) gives

$$
\dot Q=-\int(Cx)\cdot\nabla\chi\,dA+\kappa\int\Delta\chi\,dA
=(\operatorname{tr}C)Q=0.
$$

For $J_{ij}=\int x_ix_j\chi\,dA$, integrate the advective term once and the diffusive term twice. Since $\partial_k(x_ix_j)=\delta_{ki}x_j+\delta_{kj}x_i$ and $\Delta(x_ix_j)=2\delta_{ij}$, one obtains

$$
\boxed{\dot Q=0,\qquad \dot J=CJ+JC^T+2\kappa QI.}
$$

These are [mass conservation](../../../../../mass-conservation.md) and the evolution of the unnormalized second [moment](../../../../../moment.md) [tensor](../../../../../tensor.md). The first moment obeys $\dot M=CM$, so a centered packet stays centered.

For a positive [Gaussian scalar packet in a linear incompressible flow](../../../../../gaussian-scalar-packet-in-a-linear-incompressible-flow.md), $B$ must be a [positive-definite matrix](../../../../../positive-definite-matrix.md). Diagonalizing its [symmetric matrix](../../../../../symmetric-matrix.md) and applying the [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
\boxed{Q=\frac{\pi f}{\sqrt{\det B}},\qquad
J=\frac Q2 B^{-1},\qquad
B=\frac Q2J^{-1},\qquad
f=\frac{Q^2}{2\pi\sqrt{\det J}}.}
$$

The factor $Q^2$ in the last identity matters because $J$ has not been divided by the scalar mass. Substitution into the [advection-diffusion equation](../../../../../advection-diffusion-equation.md) also gives

$$
\dot B=-C^TB-BC-4\kappa B^2,\qquad
\frac{\dot f}{f}=-2\kappa\operatorname{tr}B.
$$

These identities agree with the second [moment](../../../../../moment.md) equation and prove that the Gaussian family is preserved. For an initially negative packet the same analysis applies after replacing $\chi$ by $-\chi$ and taking its positive mass.

To see the roles of stretching and [diffusion](../../../../../diffusion.md) explicitly, let the [deformation gradient](../../../../../deformation-gradient.md) $F$ solve $\dot F=CF$, $F(0)=I$. [Incompressibility](../../../../../incompressible-flow.md) gives $\det F=1$. Differentiating $F^{-1}JF^{-T}$ integrates the moment equation:

$$
J(t)=F(t)\left[J(0)+2\kappa Q\int_0^t F(s)^{-1}F(s)^{-T}\,ds\right]F(t)^T.
$$

Without [diffusion](../../../../../diffusion.md), $J=FJ(0)F^T$ and $\det J$ is constant. In a statistically stationary, mixing flow with positive [Lyapunov exponent](../../../../../lyapunov-exponent.md) $\lambda$, the two stretching exponents are $\lambda$ and $-\lambda$. Writing the ordered [eigenvalues](../../../../../eigenvalue.md) of $J$ as $e^{2\rho_1},e^{2\rho_2}$, their typical initially nondiffusive evolution is

$$
\rho_1\simeq\lambda t+O(\sqrt t),\qquad
\rho_2\simeq-\lambda t+O(\sqrt t),\qquad
\rho_1+\rho_2=\text{constant}.
$$

The fluctuation scale presumes the usual [central limit theorem](../../../../../central-limit-theorem.md) for accumulated strain; it is not implied by incompressibility alone. During this stage the packet becomes long and thin but keeps its area and peak concentration.

In the instantaneous principal-axis basis, write $\widetilde C$ for the rotated [velocity gradient tensor](../../../../../velocity-gradient-tensor.md). Differentiation of an [eigenvalue](../../../../../eigenvalue.md) gives

$$
\dot\rho_i=\widetilde C_{ii}+\kappa Qe^{-2\rho_i},\qquad
\boxed{\frac{d}{dt}(\rho_1+\rho_2)=\kappa Q\operatorname{tr}(J^{-1})\ge0.}
$$

The formulas hold through a repeated [eigenvalue](../../../../../eigenvalue.md) by continuity of their sum. The compressed physical variance is $e^{2\rho_2}/Q$. Its contraction is arrested when it is of order $\kappa/\lambda$, the square of the [Batchelor scalar microscale](../../../../../batchelor-scalar-microscale.md) $\ell_B\sim\sqrt{\kappa/\lambda}$. If its initial length is $L\gg\ell_B$, the crossover occurs at

$$
\boxed{t_B\sim\lambda^{-1}\log(L/\ell_B).}
$$

Thereafter $\rho_2$ has stationary fluctuations associated with the strain and the diffusive floor, while $\rho_1$ continues to grow typically at rate $\lambda$. Under sufficiently fast mixing, the central part of the distribution of $\rho_1$ is approximately Gaussian with mean $\lambda t+O(1)$ and variance $D_\rho t+o(t)$ for a strain-dependent coefficient $D_\rho$. This central approximation does not determine far tails, which control high concentration moments; those require a full [large deviation principle](../../../../../large-deviation-principle.md). The two logarithmic widths need not be independent. The area now increases and $f$ decreases typically as $e^{-\lambda t}$. This is [diffusion arrest of Gaussian packet compression](../../../../../diffusion-arrest-of-gaussian-packet-compression.md).

For example, a constant principal strain $C=\operatorname{diag}(\lambda,-\lambda)$ gives the exact physical variances

$$
\frac{j_1(t)}Q=\left(L_1^2+\frac\kappa\lambda\right)e^{2\lambda t}-\frac\kappa\lambda,
\qquad
\frac{j_2(t)}Q=\left(L_2^2-\frac\kappa\lambda\right)e^{-2\lambda t}+\frac\kappa\lambda.
$$

The thin variance approaches its diffusive floor, the long variance grows exponentially, and the mass-to-area relation gives the quoted typical amplitude decay. A random strain additionally makes rare histories important for concentration moments.

For a precise statistical formulation define the logarithmic area increase

$$
H_t=\rho_1(t)+\rho_2(t)-\rho_1(0)-\rho_2(0)
=\frac12\log\frac{\det J(t)}{\det J(0)}\ge0.
$$

The Gaussian identities give the exact relation $f(t)=f(0)e^{-H_t}$; hence

$$
\langle|\chi(0,t)|^\mu\rangle=|f(0)|^\mu\,\mathbb E e^{-\mu H_t}.
$$

Assume the long-time strain statistics give a [large deviation principle](../../../../../large-deviation-principle.md) for $H_t/t$ on $s\ge0$, with convex good [rate function](../../../../../rate-function.md) $I(s)$, $I(\lambda)=0$. At exponential accuracy the probability of $H_t/t$ near $s$ is $e^{-tI(s)}$. Combining that cost with the amplitude factor and applying the [Laplace principle for probability measures](../../../../../laplace-principle-for-probability-measures.md) gives the [large-deviation decay rates of a Gaussian scalar packet](../../../../../large-deviation-decay-rates-of-a-gaussian-scalar-packet.md)

$$
\boxed{\gamma_\mu=\inf_{s\ge0}\{I(s)+\mu s\},\qquad
\langle|\chi(0,t)|^\mu\rangle=\exp[-\gamma_\mu t+o(t)].}
$$

The initial amplitude only changes a time-independent prefactor. One can see the minimization directly by dividing the possible area-growth rates into small intervals: each contributes its probability cost times $e^{-\mu ts}$, and the interval with least total exponential cost dominates. An interval around a minimizing $s$ gives the matching lower bound. The nonnegative area increase bounds the exponential weight by one, so unusually large positive growth cannot produce a divergent weighted tail. Using the area rather than only $\rho_1$ also avoids discarding possibly important fluctuations of the compressed direction.

Suppose $I$ is strictly convex and differentiable, with its minimum at $\lambda>0$ and finite negative right derivative at zero. Define

$$
\boxed{\mu_*=-I'(0+).}
$$

For $0<\mu<\mu_*$ the minimizing rate $s_\mu$ is positive and uniquely solves

$$
I'(s_\mu)=-\mu,\qquad
\gamma_\mu=I(s_\mu)+\mu s_\mu.
$$

For $\mu\ge\mu_*$, convexity puts the minimum at the endpoint $s=0$, giving

$$
\boxed{\gamma_\mu=I(0)\quad(\mu\ge\mu_*).}
$$

High moments are dominated by rare histories with little net area growth, in which a packet keeps a substantial concentration. Their probability cost is $I(0)$, independent of the moment order. A finite threshold is conditional: if $I'(0+)=-\infty$, the minimizer can approach zero without reaching it at any finite $\mu$.

Below the threshold, differentiation of the minimizing expression cancels the terms involving $s_\mu'$ because $I'(s_\mu)+\mu=0$. Thus $\gamma_\mu'=s_\mu$, and

$$
\boxed{\frac{d}{d\mu}\left(\frac{\gamma_\mu}{\mu}\right)
=-\frac{I(s_\mu)}{\mu^2}<0\qquad(0<\mu<\mu_*).}
$$

Strict negativity uses a nondegenerate [rate function](../../../../../rate-function.md) with a unique zero at $\lambda$: for positive $\mu$, $s_\mu<\lambda$ and $I(s_\mu)>0$. For deterministic strain the ratio can instead be constant. Near the typical rate, if $I(s)\simeq(s-\lambda)^2/(2D)$ with $D>0$, then $\gamma_\mu\simeq\lambda\mu-D\mu^2/2$ for small $\mu$. If this quadratic expression holds all the way to zero, it gives the illustrative full result

$$
\gamma_\mu=\begin{cases}
\lambda\mu-D\mu^2/2,&0<\mu<\lambda/D,\\
\lambda^2/(2D),&\mu\ge\lambda/D.
\end{cases}
$$

The quadratic form is an example, not a universal law of turbulent strain.

A thin scalar packet is stretched until [molecular diffusion](../../../../../molecular-diffusion.md) broadens its compressed direction; conservation of its scalar mass then converts area growth into dilution. [Ensemble averages](../../../../../expected-value.md) sample different stretching histories, producing different decay rates for different moments and saturation when weakly stretched histories dominate. The present moment calculation is specifically for the centered Gaussian packet and averaging over the flow; signed random initial fields with overlapping packets can also have cancellations and require their initial-field statistics.

Finally, positive exponential decay is a statistical conclusion requiring the strain assumptions above, not a consequence of the local differential equation by itself. For $C\equiv0$ and initially isotropic physical variance $L^2$, the exact solution has $J=Q(L^2+2\kappa t)I$ and $f=Q/[2\pi(L^2+2\kappa t)]$. Its moments decay algebraically as $t^{-\mu}$. Thus **the general equations for the exponential rates are the rate-function minimization above; numerical rates and a finite saturation threshold require the long-time statistics of the flow.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
