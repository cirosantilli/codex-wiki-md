<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [linear viscoelastic fluid](../../../../../linear-viscoelastic-fluid.md), causal superposition gives

$$
\boxed{\sigma(t)=-p(t)I+2\int_0^\infty G(s)E(t-s)\,ds.}
$$

The [relaxation modulus](../../../../../relaxation-modulus.md) $G(s)$ is the stress response to a unit small step of shear strain. The equation assumes an isotropic reference state and deformations and rotations small enough over the significant memory times that nonlinear transport and strain products can be neglected. Small-amplitude motion can have high frequency; linearity does not require low frequency by itself. The infinite-past integral encodes the preceding history, rather than assuming that stress vanishes whenever the present rate vanishes.

For a small constant [shear rate](../../../../../shear-rate.md) maintained from the remote past, the rate can be taken outside the integral. Therefore the [zero-shear viscosity](../../../../../zero-shear-viscosity.md) is

$$
\boxed{\mu=\int_0^\infty G(s)\,ds,}
$$

provided the kernel is integrable, with any instantaneous contribution counted fully. A nondecaying solid-like modulus would not yield a finite fluid viscosity.

To linearize the stated [Oldroyd-B model](../../../../../oldroyd-b-model.md), put $A=I+C$ and absorb the isotropic $G_0I$ into pressure. The products of the small deformation tensor C and [velocity gradient](../../../../../velocity-gradient.md) are second order. Using the paper's derivative-index-first gradient convention therefore gives

$$
\partial_tC+\frac C\tau=\nabla v^T+\nabla v=2E.
$$

An [integrating factor](../../../../../integrating-factor.md), with the prescribed preceding history, gives $C(t)=2\int_0^\infty e^{-s/\tau}E(t-s)\,ds$. Thus the linear nonpressure stress is

$$
\sigma^d(t)=2\mu_0E(t)+2G_0\int_0^\infty e^{-s/\tau}E(t-s)\,ds.
$$

The regular relaxation tail is $G_0e^{-s/\tau}$, while the solvent is instantaneous. Equivalently, the [instantaneous solvent term in a relaxation modulus](../../../../../instantaneous-solvent-term-in-a-relaxation-modulus.md) can be represented by

$$
\boxed{G(s)=\mu_0\delta_+(s)+G_0e^{-s/\tau},\qquad\mu=\mu_0+G_0\tau.}
$$

Here the causal endpoint delta is defined by $\int_0^\infty\delta_+(s)f(s)\,ds=f(0)$. If instead a symmetric [Dirac delta](../../../../../dirac-delta-function.md) is assigned half its mass at the endpoint, the same solvent term is written $2\mu_0\delta(s)$. Stating the convention prevents a factor-of-two error in the viscosity; the explicit stress formula above has no such ambiguity.

In a [cone-and-plate rheometer](../../../../../cone-and-plate-rheometer.md), the small-angle gap is $\alpha r$ and the local wall speed is $\Omega r$, so the [shear rate](../../../../../shear-rate.md) is independent of radius to leading order: $g(t)=\Omega(t)/\alpha$. Write $s(t)$ for shear stress and $P(t)$ for its polymer part. The linear constitutive response is

$$
s=\mu_0g+P,\qquad\dot P+\frac P\tau=G_0g.
$$

The uniform shear stress gives torque

$$
T(t)=\int_0^a r\,s(t)\,2\pi r\,dr=\frac{2\pi a^3}{3}s(t).
$$

For the initial steady torque T, put $s_+=3T/(2\pi a^3)$ and $\mu_p=G_0\tau$, $\mu=\mu_0+\mu_p$. The steady polymer stress is $P_+=\mu_pg_+$, with $g_+=s_+/\mu$. Hence the initial angular velocity is

$$
\boxed{\Omega_+=\frac{3\alpha T}{2\pi a^3(\mu_0+G_0\tau)}.}
$$

For $t>0$, the total stress is $s=-s_+$, but the polymer stress is continuous at the torque reversal. Since $\mu_0>0$, a finite jump in shear rate is possible even though P cannot jump. Its immediate value is

$$
g(0^+)=\frac{-s_+-P_+}{\mu_0}=-g_+\left(1+\frac{2\mu_p}{\mu_0}\right).
$$

Eliminating P from the constant-stress equations for $t>0$ gives

$$
\mu_0\tau\dot g+(\mu_0+\mu_p)g=-s_+.
$$

The decay time is the [Retardation time of an Oldroyd fluid](../../../../../retardation-time-of-an-oldroyd-fluid.md) $\lambda_2=\mu_0\tau/(\mu_0+\mu_p)$. Solving this first-order equation with the actual initial value yields the complete [torque reversal of a linear Oldroyd fluid](../../../../../torque-reversal-of-a-linear-oldroyd-fluid.md):

$$
\boxed{\Omega(t)=-\Omega_+\left[1+\frac{2G_0\tau}{\mu_0}\exp\left(-\frac{\mu_0+G_0\tau}{\mu_0\tau}t\right)\right],\qquad t>0.}
$$

In particular, $\Omega(\infty)=-\Omega_+$ but $\Omega(0^+)$ is more negative. The stored polymer stress initially retains its old positive sign, requiring a larger negative solvent shear stress to attain the new negative total torque. This produces the backward-speed overshoot and its subsequent relaxation. Apparatus inertia would smooth the instantaneous jump, but is neglected in the question. The torque must be sufficiently small for the entire transient, including its enhanced initial rate, to remain in the linear viscoelastic regime; small pre-reversal rate alone is not sufficient when $G_0\tau/\mu_0$ is large.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
