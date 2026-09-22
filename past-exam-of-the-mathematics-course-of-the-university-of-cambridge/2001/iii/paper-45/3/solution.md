<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [cell conservation equation](../../../../../cell-conservation-in-a-swimming-suspension.md) has the form $\bar n_{\bar t}=-\bar\nabla\cdot\bar{\mathbf J}$, with

$$
\bar{\mathbf J}=\bar n\bar{\mathbf u}+V_c\bar n\mathbf p-D\bar\nabla\bar n.
$$

The first term is [advection](../../../../../advection.md) by the suspension's fluid [velocity](../../../../../velocity.md), the second is active swimming at fixed speed $V_c$ in direction $\mathbf p$, and the last is an isotropic diffusive flux due to random swimming. Here $D$ has units length squared per time, $\bar n$ is cell number per volume, and the divergence measures local loss by transport. No birth or death term is included.

For a spherical cell of radius $a_c$, its excess [buoyancy](../../../../../buoyancy.md) [force](../../../../../force.md) is $(4\pi a_c^3/3)\Delta\rho g$. The [Stokes drag law](../../../../../stokes-s-law.md) gives passive settling speed $V_{\rm set}=2a_c^2\Delta\rho g/(9\mu)$. Neglecting individual settling requires $V_{\rm set}\ll V_c$, not exact neutral [buoyancy](../../../../../buoyancy.md). A dilute suspension can still generate appreciable collective [buoyancy](../../../../../buoyancy.md) because many small excess masses contribute to the bulk [density](../../../../../density.md).

Use the half-rate convention for the [gyrotactic reorientation time](../../../../../gyrotactic-reorientation-time.md) $B$, required by the coefficients printed in the question:

$$
\boxed{0=\frac{\mathbf e_z-p_z\mathbf p}{2B}
+\frac12\bar{\boldsymbol\omega}\times\mathbf p,\qquad|\mathbf p|=1.}
$$

The first [torque](../../../../../torque.md) tends to point the bottom-heavy cell upward; the second rotates a sphere with half the fluid [vorticity](../../../../../vorticity.md). This is a quasistatic [torque](../../../../../torque.md) balance, assuming orientation relaxation is fast enough to follow the local flow. Keeping orientation dynamics instead would put $d\mathbf p/d\bar t$ on the left. The convention with aligning rate $1/B$ uses a reorientation parameter twice this $B$. Thus the factor of two is a definition, not a physical discrepancy. Close to the upward state the [quasistatic gyrotactic balance with half-rate reorientation](../../../../../quasistatic-gyrotactic-balance-with-half-rate-reorientation.md) gives $\mathbf p_\perp=B\bar{\boldsymbol\omega}\times\mathbf e_z$.

For a dilute Newtonian suspension with the [Boussinesq approximation](../../../../../boussinesq-approximation.md), the other equations are

$$
\bar\nabla\cdot\bar{\mathbf u}=0,\qquad
\frac{\partial\bar{\mathbf u}}{\partial\bar t}
+\bar{\mathbf u}\cdot\bar\nabla\bar{\mathbf u}
=-\frac1\rho\bar\nabla\bar p+\nu\bar\nabla^2\bar{\mathbf u}
-\frac{\upsilon\Delta\rho g}{\rho}\bar n\,\mathbf e_z.
$$

The background-water [hydrostatic pressure](../../../../../hydrostatic-pressure.md) is absorbed in $\bar p$. The cell volume is $\upsilon$, [density](../../../../../density.md) is $\rho$, cell [density](../../../../../density.md) is $\rho+\Delta\rho$, [dynamic viscosity](../../../../../dynamic-viscosity.md) is $\mu=\rho\nu$, and $\upsilon\bar n\ll1$ is the [volume fraction](../../../../../volume-fraction.md). Extra cell [mass](../../../../../mass.md) produces the downward [buoyancy](../../../../../buoyancy.md) term. Constant [viscosity](../../../../../dynamic-viscosity.md) and no explicit swimming stress are part of this closure. Rigid impermeable plates impose [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) and zero normal total cell flux.

At rest, the stable cell direction is upward and the steady vertical flux is $V_c\bar n-D\bar n_{\bar z}$. It is constant in depth by conservation and zero at an impermeable plate, so

$$
\boxed{\bar n_0(\bar z)=\bar N_0e^{V_c\bar z/D},\qquad
\bar N_{00}=\bar N_0\frac{e^\beta-1}{\beta},\quad
\bar N_0=\bar N_{00}\frac{\beta}{e^\beta-1},\qquad\beta=\frac{hV_c}{D}.}
$$

The [pressure](../../../../../pressure.md) gradient balances its excess weight. The mean-concentration formula follows by averaging over $0\le\bar z\le h$ and is continuous at $\beta=0$.

Use $\mathbf x=\bar{\mathbf x}/h$, $t=D\bar t/h^2$, $\mathbf u=h\bar{\mathbf u}/D$, $n=\bar n/\bar N_0$, and $p=h^2\bar p/(\rho\nu D)$. Then

$$
n_t+\nabla\cdot[n(\mathbf u+\beta\mathbf p)-\nabla n]=0,\qquad
\nabla\cdot\mathbf u=0,
$$



$$
Sc^{-1}(\mathbf u_t+\mathbf u\cdot\nabla\mathbf u)
=-\nabla p+\nabla^2\mathbf u-\frac R\beta n\mathbf e_z,
$$

where

$$
G=\frac{BD}{h^2},\quad Sc=\frac\nu D,\quad
R=\frac{\beta h^3\upsilon\Delta\rho g\bar N_0}{\rho\nu D}.
$$

The dimensionless base concentration is $n_0=e^{\beta z}$.

Linearize with the horizontal [Fourier mode](../../../../../fourier-mode.md) $e^{\sigma t+ilx+imy}$ and $k^2=l^2+m^2$. Write the first-order orientation perturbation as $\mathbf p=\mathbf e_z+\epsilon\mathbf p_1+\cdots$. Unit length gives $p_{1z}=0$, while [torque](../../../../../torque.md) balance gives $\mathbf p_{1\perp}=G\boldsymbol\omega_1\times\mathbf e_z$. Incompressibility implies

$$
\nabla\cdot\mathbf p_1
=G(\partial_x\omega_{1y}-\partial_y\omega_{1x})
=-G\nabla^2w_1.
$$

Let $\mathcal L=d^2/dz^2-k^2$. The perturbation of fluid [advection](../../../../../advection.md) is $n_0'W=\beta n_0W$, and swimming contributes $\beta N'+\beta n_0\nabla\cdot\mathbf p_1$. Cell conservation therefore gives

$$
\sigma N=\mathcal LN-\beta N'-\beta n_0W+\beta G n_0\mathcal LW,
$$

or

$$
\boxed{(d^2/dz^2-\beta\,d/dz-k^2-\sigma)N
=-\beta e^{\beta z}[G(W''-k^2W)-W].}
$$

This explains the destabilizing concentration-advection term and the gyrotactic redistribution term with their signs.

To eliminate [pressure](../../../../../pressure.md) from the fluid equations, take their divergence, giving $\mathcal Lp_1=-(R/\beta)N'$. Apply $\mathcal L$ to the vertical equation $Sc^{-1}\sigma W=-p_1'+\mathcal LW-(R/\beta)N$. The concentration second [derivatives](../../../../../derivative.md) cancel, leaving

$$
\boxed{(\mathcal L-\sigma/Sc)\mathcal LW=-\frac R\beta k^2N.}
$$

No-slip conditions give $W=0$ and $W'=0$ at each plate; for nonzero $k$, the latter follows from the vanishing horizontal [velocity](../../../../../velocity.md) and [incompressibility](../../../../../incompressible-flow.md). Zero perturbed normal cell flux gives

$$
\boxed{W=W'=0,\qquad N'-\beta N=0\quad\text{at }z=0,1.}
$$

The normal orientation correction is zero at this order, and the fluid [velocity](../../../../../velocity.md) is zero at the plate, so neither adds another term to this concentration condition.

Now use the stated distinguished scalings $k=\beta\alpha$, $\sigma=\beta^2\sigma_2$, $G=\beta^{-1}G_{-1}$, $N=N_0+\beta N_1+\beta^2N_2+\cdots$, $W=\beta W_1+\beta^2W_2+\cdots$, and $R=R_0+\beta R_1+\cdots$. Here $\alpha$ is a scaled [wavenumber](../../../../../wavenumber.md), unrelated to Question 2's shear rate. At order one, the concentration equation and [boundary conditions](../../../../../boundary-condition.md) give $N_0''=0$, $N_0'=0$ at both endpoints, so $N_0$ is constant. Absorb its nonzero value into the perturbation amplitude and choose

$$
\boxed{N_0=1.}
$$

At order $\beta$, the fluid equation is $W_1^{(4)}=-R_0\alpha^2$ with $W_1=W_1'=0$ at both ends. Its unique solution is

$$
\boxed{W_1=-\frac{R_0\alpha^2}{24}z^2(1-z)^2.}
$$

A homogeneous difference is cubic and the four clamped conditions make it zero.

The concentration equation at order $\beta$ gives

$$
N_1''=-G_{-1}W_1'',\qquad N_1'(0)=N_1'(1)=1,
$$

so $N_1=z-G_{-1}W_1+C_1$, where $C_1$ fixes the amplitude normalization. At order $\beta^2$ it gives

$$
N_2''-N_1'-(\alpha^2+\sigma_2)
=-G_{-1}W_2''+W_1-zG_{-1}W_1''.
$$

The [boundary conditions](../../../../../boundary-condition.md) expand to $N_2'=N_1$ at each endpoint. Integrating this equation from zero to one cancels $[N_2']_0^1$ against $[N_1]_0^1$. Also $[W_2']_0^1=0$ and

$$
\int_0^1zW_1''dz=[zW_1']_0^1-[W_1]_0^1=0.
$$

Thus the required solvability condition is

$$
\boxed{\alpha^2+\sigma_2=-\int_0^1W_1dz.}
$$

Since $\int_0^1z^2(1-z)^2dz=1/30$, the [clamped-quartic solvability in shallow bioconvection](../../../../../clamped-quartic-solvability-in-shallow-bioconvection.md) gives

$$
\boxed{\sigma_2=\alpha^2\left(\frac{R_0}{720}-1\right).}
$$

For nonzero long horizontal waves, $R_0<720$ gives decay and $R_0>720$ gives growth; the leading neutral threshold is $R_0=720$. The leading instability is stationary and independent of $G_{-1}$ and $Sc$. The exactly uniform horizontal mode $\alpha=0$ has zero growth at this order because total cell number is conserved, so it does not determine the threshold. Upward swimming produces a dense upper layer; the unstable disturbance is its buoyancy-driven overturning, or [bioconvection](../../../../../bioconvection.md). Higher orders are needed for wavelength selection and finite-depth threshold corrections.

With fixed material parameters and mean concentration, $R\sim h^4V_c\upsilon\Delta\rho g\bar N_{00}/(\rho\nu D^2)$ for small $\beta$, so a sufficiently thin chamber is stable to this branch. Formally its threshold corresponds to $h_c\sim[720\rho\nu D^2/(V_c\upsilon\Delta\rho g\bar N_{00})]^{1/4}$ when the weak-stratification and distinguished-gyrotaxis assumptions apply. In particular, the assumed $G=O(\beta^{-1})$ is a specified [asymptotic analysis](../../../../../asymptotic-analysis.md); at fixed $B,D,V_c$ and decreasing $h$, one instead has $G=O(\beta^{-2})$. The leading result should not be asserted unchanged in that different ordering without redoing the expansion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
