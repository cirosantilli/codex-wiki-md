<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take $z$ positive upward, and write $b=\widetilde\rho g$. For a straight steady [viscous buoyant conduit](../../../../../viscous-buoyant-conduit.md), the inner and outer axial equations are

$$
\lambda\mu\frac1r(rw_i')'=P_i'-b,\qquad
\mu\frac1r(rw_o')'=P_o'.
$$

Regularity gives $w_i'(0)=0$, the wall has $w_o(R)=0$, and [velocity](../../../../../velocity.md) and tangential traction are continuous at $r=a_0$: $w_i=w_o$, $\lambda\mu w_i'=\mu w_o'$. With no interfacial tension specified, normal traction is continuous; for this straight steady flow that sets $P_i=P_o$ at the interface. Thus the modified gradients are common in this case.

When their value is zero, integration gives

$$
w_o(r)=\frac{ba_0^2}{2\mu}\ln(R/r),\qquad
w_i(r)=w_o(a_0)+\frac b{4\lambda\mu}(a_0^2-r^2).
$$

Consequently

$$
\boxed{\frac{w_i(0)}{w_i(a_0)}=1+\frac1{2\lambda\ln(R/a_0)}.}
$$

The large center-to-interface speed ratio explains why the inner parabolic component dominates at small [viscosity](../../../../../dynamic-viscosity.md) ratio.

For a slowly varying radius, set $B=b-P_{i,z}$. The local inner solution has $w_i=w_a+B(a^2-r^2)/(4\lambda\mu)$, so

$$
q=\pi a^2w_a+\frac{\pi a^4B}{8\lambda\mu}.
$$

The shear-driven outer interface speed has scale $a^2B\ln(R/a)/\mu$. The pressure-driven return flow needed for zero total flux adds a [velocity](../../../../../velocity.md) of order $q/R^2$ and a shear-driven contribution of order $a^2B/\mu$. Relative to the inner parabolic [velocity](../../../../../velocity.md) these terms are $O(\lambda\ln(R/a))$ and $O((a/R)^2)$, which are small under the stated assumptions. Axial viscous derivatives are also smaller because the plume is slender. Therefore

$$
\boxed{q=\frac{\pi a^4}{8\lambda\mu}(b-P_{i,z})\quad\text{to leading order}.}
$$

For clarity, the outer pressure-gradient estimate must include both return flux and transmitted interface shear. Their flux scales are $R^4P_{o,z}/\mu$, $a^2R^2B/\mu$ and $q$. Zero total flux hence implies

$$
\frac{|P_{o,z}|}{|B|}
=O\left((a/R)^2+\frac{(a/R)^4}{\lambda}\right)\ll1.
$$

This justifies the negligible outer [pressure](../../../../../pressure.md) gradient. We subsequently choose its negligible [pressure](../../../../../pressure.md) reference as zero, as in the reduced model.

Near the moving interface the outer [radial source flow](../../../../../radial-source-flow.md) is $u_r=aa_t/r$: the interface's axial advection is smaller because its axial [velocity](../../../../../velocity.md) is small compared with the inner core speed. Its radial strain is $\partial_ru_r=-aa_t/r^2$. Continuity of normal traction at $r=a$, neglecting the much smaller inner normal viscous stress, gives

$$
-P_i=-P_o-2\mu a_t/a,
\qquad\boxed{P_i-P_o=2\mu a_t/a.}
$$

With $A=a^2/a_0^2$, this is $P_i=\mu A_t/A$ after dropping $P_o$. Conservation of plume volume is $\pi(a^2)_t+q_z=0$.

Let the axial and [velocity](../../../../../velocity.md) scales be

$$
\ell=\frac{a_0}{\sqrt{8\lambda}},\qquad
U_0=\frac{ba_0^2}{8\lambda\mu},\qquad
\boxed{Z=z/\ell,\quad T=tU_0/\ell.}
$$

Since $\mu U_0/(b\ell^2)=1$, substitution gives the [conduit equation](../../../../../conduit-equation.md)

$$
\boxed{A_T+\partial_Z\left\{A^2\left[1-\partial_Z(A_T/A)\right]\right\}=0.}
$$

The buoyant flux and the viscous normal-stress [pressure](../../../../../pressure.md) are both retained at this scaling.

Linearizing about unit area gives $a_T+2a_Z-a_{TZZ}=0$. Thus

$$
\boxed{\omega=\frac{2k}{1+k^2},\qquad\omega/k=\frac2{1+k^2}>0.}
$$

Wave crests propagate upward. The [group velocity](../../../../../group-velocity.md) is $2(1-k^2)/(1+k^2)^2$: it is downward for $|k|>1$, so the phase direction is not the direction of every wave packet.

For a [travelling wave](../../../../../travelling-wave.md) $f(\zeta)$, integrating once and using its uniform far field gives

$$
-cf+f^2+c(ff''-f'^2)=f_0^2-cf_0=:K.
$$

Divide by $f^2$, multiply by $f'/f$ and integrate again. A convenient potential, defined up to an additive constant, is

$$
\boxed{\frac c2\frac{f'^2}{f^2}+V(f)=V(f_0),\qquad
V(f)=\ln f+\frac c f+\frac{f_0^2-cf_0}{2f^2}.}
$$

At the positive crest $f=\alpha f_0$, the derivative is zero. Subtracting the far-field potential yields

$$
\boxed{c(1-2/\alpha+\alpha^{-2})
=f_0(2\ln\alpha-1+\alpha^{-2}).}
$$

This is the [solitary-wave amplitude-speed relation for the conduit equation](../../../../../solitary-wave-amplitude-speed-relation-for-the-conduit-equation.md). A nontrivial elevation wave has $\alpha>1$ and $c>2f_0$; as $\alpha\downarrow1$, the speed tends to the long-wave speed $2f_0$. Positive area is required throughout the derivation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
