<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [streamfunction](../../../../../stream-function.md) convention $u=\psi_z$, $w=-\psi_x$, and take $v=0$. With $J(A,B)=A_xB_z-A_zB_x$, the [material derivative](../../../../../material-derivative.md) is $D=\partial_t-J(\psi,\cdot)$. This convention differs from the horizontal [quasi-geostrophic streamfunction](../../../../../quasi-geostrophic-streamfunction.md) convention used below. The nonlinear [Boussinesq equations](../../../../../boussinesq-equations.md) are

$$
u_t+uu_x+wu_z=-P_x,\qquad w_t+uw_x+ww_z=-P_z+\sigma,\qquad u_x+w_z=0.
$$

The $y$ component of [vorticity](../../../../../vorticity.md) is $\zeta=u_z-w_x=\nabla^2\psi$. Differentiate the first momentum equation in $z$ and subtract the $x$ derivative of the second. The [pressure](../../../../../pressure.md) terms cancel; the derivatives of the advecting [velocity](../../../../../velocity.md) cancel by $u_x+w_z=0$. Thus $D\zeta=-\sigma_x$, or

$$
\boxed{\nabla^2\psi_t+\sigma_x=J(\psi,\nabla^2\psi).}
$$

Conservation of total [buoyancy](../../../../../buoyancy.md), with background gradient $N^2(z)$, gives

$$
\boxed{\sigma_t-N^2\psi_x=J(\psi,\sigma).}
$$

Both equations retain the nonlinear [advection](../../../../../advection.md) terms.

Write $\psi=\bar\psi(z)+\phi$, with $\bar\psi_z=U(z)=\bar u(z)$, and take the background [buoyancy](../../../../../buoyancy.md) anomaly to be zero. The linear equations for $(\phi,\sigma)$ are

$$
(\partial_t+U\partial_x)\nabla^2\phi-U''\phi_x+\sigma_x=0,\qquad (\partial_t+U\partial_x)\sigma-N^2\phi_x=0.
$$

For a [normal mode](../../../../../normal-mode.md) $\phi=\hat\psi(z)e^{ik(x-ct)}$, the second equation gives $\hat\sigma=N^2\hat\psi/(U-c)$. Substitute this into the first to obtain the [Taylor–Goldstein equation](../../../../../taylor-goldstein-equation.md)

$$
\boxed{\hat\psi_{zz}+(\ell^2-k^2)\hat\psi=0,\qquad \ell^2=\frac{N^2}{(U-c)^2}-\frac{U''}{U-c}.}
$$

Here $k\ne0$ and the calculation is initially away from [critical levels](../../../../../critical-level-of-a-shear-flow-wave.md) $U=c$. The first term is the restoring effect of stable [buoyancy](../../../../../buoyancy.md) on vertically displaced parcels. The second comes from [advection](../../../../../advection.md) of the background [vorticity](../../../../../vorticity.md) gradient $U''$: a displacement creates a [vorticity](../../../../../vorticity.md) anomaly, whose induced [velocity](../../../../../velocity.md) acts back on the displacement. This is the shear-flow counterpart of a [Rossby wave](../../../../../rossby-wave.md) restoring mechanism; its sign can also permit instability, so it is not invariably stabilizing.

Rigid boundaries imply $w=-\phi_x=0$, hence $\hat\psi(0)=\hat\psi(\pi H)=0$. For a real, regular [normal mode](../../../../../normal-mode.md), multiply the [Taylor–Goldstein equation](../../../../../taylor-goldstein-equation.md) by $\hat\psi$, integrate, and integrate its second derivative by parts. The endpoint term vanishes, leaving

$$
\boxed{k^2=\frac{\int_0^{\pi H}(\ell^2\hat\psi^2-\hat\psi_z^2)\,dz}{\int_0^{\pi H}\hat\psi^2\,dz}=I(\hat\psi;c).}
$$

For a smooth real dispersion branch, differentiate this identity with respect to $k$. The stated stationarity of $I$ removes the term involving $d\hat\psi/dk$, so $2k=I_c\,dc/dk$. Direct differentiation at fixed $\hat\psi$ gives

$$
\partial_c\ell^2=\frac{2N^2}{(U-c)^3}-\frac{U''}{(U-c)^2}=\frac{N^2}{(U-c)^3}+\frac{\ell^2}{U-c}.
$$

Since the [frequency](../../../../../frequency.md) is $kc$, the [group velocity](../../../../../group-velocity.md) is $d(kc)/dk$, and therefore

$$
\boxed{c_g=c+\frac{2k^2\int_0^{\pi H}\hat\psi^2\,dz}{\int_0^{\pi H}\left(\frac{N^2}{(U-c)^3}+\frac{\ell^2}{U-c}\right)\hat\psi^2\,dz}.}
$$

This is [variational group velocity of a Taylor-Goldstein mode](../../../../../variational-group-velocity-of-a-taylor-goldstein-mode.md). Singular [critical levels](../../../../../critical-level-of-a-shear-flow-wave.md) or a vanishing denominator require separate limiting analysis; no stationarity proof is needed here.

For the sinusoidal profiles, choose **$c=0$**. In the interior,

$$
\ell^2=\frac{N_0^2}{U_0^2}+\frac{1}{H^2},\qquad \hat\psi_n=\sin(nz/H),\qquad \boxed{k_n^2=\frac{N_0^2}{U_0^2}+\frac{1-n^2}{H^2}.}
$$

The profile ratios extend to the endpoints in this reduced equation. Thus **$n=1$ always gives a nonzero real $k$**, with $k_1^2=N_0^2/U_0^2$. For this [normal mode](../../../../../normal-mode.md),

$$
\int_0^{\pi H}\hat\psi_1^2\,dz=\frac{\pi H}{2},\qquad \int_0^{\pi H}\frac{\hat\psi_1^2}{\sin(z/H)}\,dz=2H.
$$

The denominator in the [group velocity](../../../../../group-velocity.md) expression is $2H(2N_0^2/U_0^3+1/(U_0H^2))$. It follows that

$$
\boxed{c_{g,1}=\frac{\pi U_0}{2}\frac{N_0^2H^2}{2N_0^2H^2+U_0^2}.}
$$

Although $U$ vanishes at the endpoints, this weighted integral is finite; the vanishing of $\hat\psi_1$ supplies the required cancellation. The formula is the limiting derivative approached from the regular real branch with $c<0$, before any interior critical level is encountered.

If instead $N=N_0$ and $U=U_0$ are constant, still take $c=0$. The same vertical [eigenfunctions](../../../../../eigenfunction.md) satisfy the [Taylor–Goldstein equation](../../../../../taylor-goldstein-equation.md), now with

$$
\boxed{k_n^2=\frac{N_0^2}{U_0^2}-\frac{n^2}{H^2}.}
$$

There is **no value of $n\ge1$ guaranteed to give real $k$** for arbitrary positive parameters: if $N_0H<U_0$, all these squared [wavenumbers](../../../../../wavenumber.md) are negative. A nonzero real $k$ exists exactly when $N_0H>U_0$; equality gives only the degenerate $n=1$, $k=0$ limit. For a real branch the same [group velocity](../../../../../group-velocity.md) calculation gives $c_g=k_n^2U_0^3/N_0^2$.

To test exact nonlinear validity, take a real [normal mode](../../../../../normal-mode.md) $\phi=A\sin(nz/H)\cos(kx)$ and its corresponding [buoyancy perturbation](../../../../../buoyancy-perturbation.md) $\sigma=a(z)\phi$, where $a=N^2/(U-c)$. Because

$$
\nabla^2\phi=-\left(k^2+\frac{n^2}{H^2}\right)\phi,
$$

the quadratic [vorticity](../../../../../vorticity.md) self-advection is zero: $J(\phi,\nabla^2\phi)=0$. The quadratic [buoyancy](../../../../../buoyancy.md) self-advection, however, is

$$
\boxed{J(\phi,a\phi)=a'(z)\phi\phi_x.}
$$

This [nonlinear exactness test for a stratified streamfunction mode](../../../../../nonlinear-exactness-test-for-a-stratified-streamfunction-mode.md) distinguishes the cases. For constant $N,U$, $a=N_0^2/U_0$ is constant, so both quadratic terms vanish. The background-mode terms already satisfy the linear equations, hence **the constant-profile modes are exact finite-amplitude solutions** of the ideal [Boussinesq equations](../../../../../boussinesq-equations.md). [Pressure](../../../../../pressure.md) can be recovered from the momentum equations: the [vorticity equation](../../../../../vorticity-equation.md) supplies their compatibility condition in this simply connected strip.

For the sinusoidal profiles, $a=(N_0^2/U_0)\sin(z/H)$ has a nonzero derivative in the interior. For every nonzero $A$ and nonzero real $k$, $a'\phi\phi_x$ is not identically zero; it produces a second horizontal harmonic that is absent from the proposed solution. Thus **none of these nontrivial sinusoidal-profile modes is an exact finite-amplitude solution**. A $k=0$ field is merely an added horizontal shear with no vertical motion and is a degenerate exception to the wave calculation, not a propagating member of it.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
