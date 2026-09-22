<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $S(z)=d\rho_s/dz$, $N^2=-gS/\rho_0>0$, and define the [quasi-geostrophic streamfunction](../../../../../quasi-geostrophic-streamfunction.md) by $\psi=\widetilde p/(\rho_0f_0)$. Use horizontal scale $L$, vertical scale $D$, [velocity](../../../../../velocity.md) scale $U$ and advective time $L/U$. The required [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md) has small [Rossby number](../../../../../rossby-number.md) $\varepsilon=U/(|f_0|L)$, $\beta L/|f_0|=O(\varepsilon)$, and [Burger number](../../../../../burger-number.md) $N^2D^2/(f_0^2L^2)=O(1)$. Hydrostatic, thin-layer scaling has $D/L\ll1$; [density](../../../../../density.md) variations are small compared with $\rho_0$, as required by the [Boussinesq approximation](../../../../../boussinesq-approximation.md). The leading horizontal flow is nondivergent, with vertical [velocity](../../../../../velocity.md) $w=O(\varepsilon UD/L)$. Retain forcing of the same slow order as [density](../../../../../density.md) advection, $r=O(U\widetilde\rho/L)$; stronger forcing need not preserve this balanced scaling.

Leading [geostrophic balance](../../../../../geostrophic-balance.md) and the [hydrostatic approximation](../../../../../hydrostatic-approximation.md) give

$$
u_g=-\psi_y,\qquad v_g=\psi_x,\qquad
\widetilde\rho=-\frac{\rho_0f_0}{g}\psi_z.
$$

Write $D_g/Dt=\partial_t-\psi_y\partial_x+\psi_x\partial_y$. The [density](../../../../../density.md) equation becomes

$$
f_0\frac{D_g\psi_z}{Dt}+N^2w=-\frac g{\rho_0}r,
\qquad
w=-\frac{f_0}{N^2}\frac{D_g\psi_z}{Dt}-\frac{g}{\rho_0N^2}r.
$$

Taking the curl of the horizontal momentum equations at the next order and using continuity gives the stretching equation

$$
\frac{D_g}{Dt}(\nabla_h^2\psi+\beta y)=f_0w_z.
$$

Substitute the expression for $w$. Vertical differentiation commutes with the geostrophic [material derivative](../../../../../material-derivative.md) acting on $\psi_z$ here: the extra Jacobian is $J(\psi_z,\psi_z)=0$. Since $N$ depends only on height, this yields the [diabatically forced quasi-geostrophic potential vorticity](../../../../../diabatically-forced-quasi-geostrophic-potential-vorticity.md) equation

$$
\boxed{\frac{D_gq}{Dt}=-\frac{gf_0}{\rho_0}\partial_z\left(\frac r{N^2}\right),\qquad
q=\nabla_h^2\psi+\partial_z\left(\frac{f_0^2}{N^2}\psi_z\right)+\beta y.}
$$

The minus sign is appropriate to the specified [density](../../../../../density.md) forcing; a positive upward [buoyancy](../../../../../buoyancy.md) forcing is $R=-gr/\rho_0$ and gives $D_gq/Dt=f_0\partial_z(R/N^2)$.

Now take constant $N$ and linearize about rest. Put $s=f_0^2/N^2$ and $S_0=gf_0\mu r_0/(\rho_0N^2)$. The forced equation is

$$
\partial_t(\psi_{xx}+s\psi_{zz})+\beta\psi_x=S_0e^{-\mu z}\cos kx\cos\omega_0t.
$$

For the [harmonic heating response of quasi-geostrophic flow](../../../../../harmonic-heating-response-of-quasi-geostrophic-flow.md), represent the two traveling Fourier components with frequencies $\omega_+=\omega_0$ and $\omega_-=-\omega_0$:

$$
\psi=\operatorname{Re}\sum_{\sigma=\pm}\phi_\sigma(z)e^{i(kx-\omega_\sigma t)}.
$$

Each component of the forcing has amplitude $S_0/2$, so

$$
-i\omega_\sigma(s\phi_\sigma''-k^2\phi_\sigma)+i\beta k\phi_\sigma
=\frac{S_0}{2}e^{-\mu z}.
$$

Equivalently its vertical structure obeys

$$
\boxed{\phi_\sigma''-\lambda_\sigma^2\phi_\sigma=C_\sigma e^{-\mu z},\quad
\lambda_\sigma^2=\frac{N^2}{f_0^2}\left(k^2+\frac{\beta k}{\omega_\sigma}\right),\quad
C_\sigma=\frac{ig\mu r_0}{2\rho_0f_0\omega_\sigma}.}
$$

These are the time-periodic forced responses; unspecified initial data may add free [Rossby waves](../../../../../rossby-wave.md). Selecting no incoming waves describes forcing switched on causally and then its persistent harmonic part.

For $\beta>0$, the eastward component always has $\lambda_+^2>0$. Let $\lambda_+>0$. The growing exponential would introduce an unbounded [velocity](../../../../../velocity.md) and [pressure](../../../../../pressure.md) disturbance at infinity, so discard it. The bottom condition $\phi_+(0)=0$ then gives

$$
\boxed{\phi_+(z)=\frac{C_+}{\mu^2-\lambda_+^2}\left(e^{-\mu z}-e^{-\lambda_+z}\right).}
$$

If $\mu=\lambda_+$, this expression has the regular limit $-C_+ze^{-\mu z}/(2\mu)$, rather than a physical singularity.

For $\omega_0>\beta/k$, the westward component also has positive $\lambda_-^2$. Choose $\lambda_->0$ and use the same decaying expression with minus subscripts, including the same coincident-exponent limit. Thus **both components are vertically evanescent above the heating**.

For $0<\omega_0<\beta/k$, put

$$
m=\frac{N}{|f_0|}\sqrt{\frac{\beta k}{\omega_0}-k^2}>0,
\qquad\lambda_-^2=-m^2.
$$

Both homogeneous solutions $e^{\pm imz}$ are bounded, so boundedness is insufficient. A free [Rossby wave](../../../../../rossby-wave.md) with phase $kx+mz-\omega t$ has

$$
\omega=-\frac{\beta k}{k^2+sm^2},\qquad
c_{gz}=\frac{\partial\omega}{\partial m}=\frac{2\beta ksm}{(k^2+sm^2)^2}.
$$

The [radiation condition](../../../../../radiation-condition.md) demands [energy](../../../../../energy.md) propagation away from the heating, upward into $z>0$. For $\beta,k>0$ that selects positive $m$, hence $e^{imz}$ in the westward component. The resulting solution is

$$
\boxed{\phi_-(z)=\frac{C_-}{\mu^2+m^2}\left(e^{-\mu z}-e^{imz}\right).}
$$

It satisfies $\phi_-(0)=0$ and, away from the decaying forcing, $\phi_-'\sim im\phi_-$. Its far-field amplitude does not decay in this nondissipative model: continuous forcing supplies an outgoing wave train. Thus **the low-frequency westward component propagates vertically while the eastward component remains evanescent**.

At the threshold $\omega_0=\beta/k$, the westward vertical [wavenumber](../../../../../wavenumber.md) is zero. Excluding the linearly growing homogeneous solution and retaining the bottom condition gives $\phi_-=C_-(e^{-\mu z}-1)/\mu^2$. This bounded limiting response tends to a constant and has zero vertical [group velocity](../../../../../group-velocity.md); demanding both bottom zero and decay to zero at infinity would overdetermine this threshold problem. For $\beta\le0$, the branch labels and propagation inequality must be reconsidered; the comparison stated here assumes the usual positive beta-plane gradient.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
