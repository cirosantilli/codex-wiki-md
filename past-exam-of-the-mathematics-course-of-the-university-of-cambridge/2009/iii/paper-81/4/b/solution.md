<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First distinguish concentration conventions. If $C$ is cell number density, the excess mixture density is $v\Delta\rho C$. If $\varphi=vC$ is cell volume fraction, it is $\Delta\rho\varphi$. **The printed definition of $R$ is dimensionless for number density, whereas the prose calls $\hat n_0$ a volume fraction.** Use $C_0$ for mean number density and $\varphi_0=vC_0$ for mean volume fraction. Then the consistent [Rayleigh number](../../../../../../rayleigh-number.md) is

$$
\boxed{R=\frac{gC_0v\Delta\rho H^3}{\rho\nu D}=\frac{g\varphi_0\Delta\rho H^3}{\rho\nu D}.}
$$

The dimensionless concentration $n=C/C_0=\varphi/\varphi_0$ is the same in both conventions. The extra factor $v$ must be removed if the source symbol is literally a volume fraction.

Remove the hydrostatic basic pressure and use a dilute [Boussinesq approximation](../../../../../../boussinesq-approximation.md). With $\widehat C_e=\widehat C-C_0\bar n$ and perturbation fluid [velocity](../../../../../../velocity.md) $\widehat{\mathbf u}$, the linear incompressible [Newtonian fluid](../../../../../../newtonian-fluid.md) equations are

$$
\widehat\nabla\cdot\widehat{\mathbf u}=0,\qquad
\partial_{\hat t}\widehat{\mathbf u}=-\frac1\rho\widehat\nabla\widehat P_e+\nu\widehat\Delta\widehat{\mathbf u}-\frac{gv\Delta\rho}{\rho}\widehat C_e\mathbf e_3.
$$

The [cell conservation equation](../../../../../../cell-conservation-in-a-swimming-suspension.md) linearizes to

$$
\partial_{\hat t}\widehat C_e+\widehat w\,C_0\frac{d\bar n}{d\hat z}+V_s\partial_{\hat z}\widehat C_e+V_sC_0\widehat\nabla_\perp\cdot(\bar n\mathbf p_\perp)=D\widehat\Delta\widehat C_e.
$$

At this order the vertical orientation perturbation is zero, because $|\mathbf p|=1$. The instantaneous-orientation approximation from the introductory calculation gives

$$
\mathbf p_\perp=\frac B2(\widehat{\boldsymbol\omega}\times\mathbf e_3)_\perp.
$$

Incompressibility implies $\widehat\nabla_\perp\cdot(\widehat{\boldsymbol\omega}\times\mathbf e_3)_\perp=-\widehat\Delta\widehat w$. This identity fixes the sign of the gyrotactic term.

Apply the length, viscous-time, [velocity](../../../../../../velocity.md), concentration and pressure scales in the paper. Writing $n_e=n-\bar n$, the dimensionless equations are

$$
\begin{aligned}
\nabla\cdot\mathbf u&=0,\\
\partial_t\mathbf u&=-\nabla P_e+\Delta\mathbf u-Rn_e\mathbf e_3,\\
S\partial_tn_e&=\Delta n_e-h\partial_zn_e-\bar n'w+G\bar n\Delta w,
\end{aligned}
$$

where $S=\nu/D$ and $G=V_sB/(2H)$. The factor $S$ appears in the cell equation because its diffusive time differs from the viscous time used for $t$.

For a [normal mode](../../../../../../normal-mode.md) $[n_e,w]=[N,W]e^{\sigma t+i\kappa x}$, set $\mathcal L=d^2/dz^2-\kappa^2$. Taking the divergence of the momentum equation gives $\mathcal LP_e=-RN'$. Applying $\mathcal L$ to its vertical component eliminates pressure and yields

$$
\boxed{(\mathcal L-\sigma)\mathcal LW=-R\kappa^2N.}
$$

The concentration equation becomes

$$
\boxed{\left(\frac{d^2}{dz^2}-h\frac d{dz}-\kappa^2-S\sigma\right)N=\bar n'W-G\bar n\left(\frac{d^2}{dz^2}-\kappa^2\right)W.}
$$

These reproduce the requested modal equations, with the physically consistent sign of the orientation balance and concentration convention made explicit.

At both plates, the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) gives $w=0$ and horizontal perturbation [velocity](../../../../../../velocity.md) zero. For a nonzero horizontal [wavenumber](../../../../../../wavenumber.md), incompressibility then gives $W'=0$. The normal cell flux is $\bar n w+hN-N'$; the orientation correction has no vertical component at this order. Impermeability therefore gives

$$
\boxed{W=W'=0,\qquad N'-hN=0\quad\text{at }z=-1,0.}
$$

If orientation lag is retained rather than the given instantaneous balance, $\mathbf p_\perp$ acquires the relaxation response $(1+B\partial_{\hat t})^{-1}$ and the modal gyrotactic term changes accordingly. The displayed equations are the quasistatic-orientation model requested here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
