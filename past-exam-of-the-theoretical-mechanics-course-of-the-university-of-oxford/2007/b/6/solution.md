<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For a vector $a$ described in axes rotating at constant [angular velocity](../../../../angular-velocity.md) $\Omega$, the [rotating-axes theorem](../../../../rotating-axes-theorem.md) is $(da/dt)_{\rm inertial}=(da/dt)_{\rm rotating}+\Omega\times a$. Inertial particle [velocity](../../../../velocity.md) is $u+\Omega\times x$. Applying the theorem once more gives inertial acceleration $Du/Dt+2\Omega\times u+\Omega\times(\Omega\times x)$. Thus the rotating momentum equation is

$$
\boxed{\frac{Du}{Dt}+2\Omega\times u+\Omega\times(\Omega\times x)=-\frac1\rho\nabla p+g.}
$$

If $g=-\nabla\Phi$ and [density](../../../../density.md) is constant, the centrifugal term can be absorbed into the [reduced pressure in a rotating fluid](../../../../reduced-pressure-in-a-rotating-fluid.md):

$$
\boxed{P=p+\rho\Phi-\frac\rho2|\Omega\times x|^2,\qquad
u_t+(u\cdot\nabla)u+2\Omega\times u=-\nabla P/\rho.}
$$

For small disturbances with $\Omega=\Omega e_z$, linearize to $u_t-2\Omega v=-P_x/\rho$, $v_t+2\Omega u=-P_y/\rho$, $w_t=-P_z/\rho$, together with [incompressibility](../../../../incompressible-flow.md). Put $\zeta=v_x-u_y$. Taking the vertical [curl](../../../../curl.md) gives $\zeta_t=2\Omega w_z$. Taking divergence gives $\nabla^2P=2\rho\Omega\zeta$. Applying the Laplacian to the vertical momentum equation therefore gives $\partial_t\nabla^2w=-2\Omega\zeta_z$. Another time [derivative](../../../../derivative.md) yields

$$
\boxed{\partial_t^2\nabla^2w+4\Omega^2w_{zz}=0.}
$$

All three [velocity](../../../../velocity.md) components are retained, even for fields independent of $y$; rotation produces the transverse component.

Set $m=\pi/h$ and seek $w=ae^{-i\omega t}W(x)\sin mz$. The rigid-wall conditions are then automatic and the scalar equation gives

$$
W''+m^2\left(\frac{4\Omega^2}{\omega^2}-1\right)W=0,\qquad W(0)=1.
$$

For $0<|\omega|<2|\Omega|$, define $q=m\sqrt{4\Omega^2/\omega^2-1}$. The two possible oscillatory factors are distinguished by energy propagation. With horizontal [wavenumber](../../../../wavenumber.md) $k$, the [dispersion relation](../../../../dispersion-relation-split.md) is $\omega^2=4\Omega^2m^2/(k^2+m^2)$ and $c_{g,x}=-\omega k/(k^2+m^2)$. An outgoing wave in $x>0$ must have $\omega k<0$, giving

$$
\boxed{w=ae^{-i\omega t-i\operatorname{sgn}(\omega)qx}\sin(\pi z/h).}
$$

For $|\omega|>2|\Omega|$, define $\kappa=m\sqrt{1-4\Omega^2/\omega^2}$. Reject the exponentially growing branch, leaving the evanescent response

$$
\boxed{w=ae^{-i\omega t-\kappa x}\sin(\pi z/h).}
$$

The real part is the physical [velocity](../../../../velocity.md). The radiation or bounded-decay condition is needed in addition to the wavemaker boundary value to pick a unique half-channel response. Steady forcing ($\omega=0$) is a singular limit: with nonzero rotation a steady [geostrophic balance](../../../../geostrophic-balance.md) and impermeable top/bottom require $w=0$, incompatible with a nonzero imposed [sine](../../../../sine.md) profile. At the cutoff equality, the bounded outgoing polarization also degenerates. These exceptional cases cannot be obtained by blindly substituting into the two strict-inequality formulas. The propagating sign is the [radiation sign for an inertial wave](../../../../radiation-sign-for-an-inertial-wave.md).

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
