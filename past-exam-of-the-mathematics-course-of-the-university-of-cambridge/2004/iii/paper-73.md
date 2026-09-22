# Paper 73

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper73.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper73.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [Circulation application](#4/i)
    - [Solution](#4/i/solution)

## 1

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $c=\sqrt{gH}$ and $R_d=c/|f|$, with $f\ne0$. For the profiles below take $f>0$, so $\alpha=L/R_d$ agrees with the stated parameter; changing the sign of $f$ reverses the balanced meridional [velocity](../../../classical-mechanics.md#velocity) but not the height profile. The linearized [shallow water equations](../../../physics.md#shallow-water-equations) are

$$
u_t-fv=-g\eta_x,\qquad v_t+fu=-g\eta_y,\qquad \eta_t+H(u_x+v_y)=0.
$$

Taking the horizontal curl gives $(v_x-u_y)_t=-f(u_x+v_y)=f\eta_t/H$. Hence the signed linear [shallow-water potential vorticity](../../../geophysical-fluid-dynamics.md#shallow-water-potential-vorticity) anomaly is conserved:

$$
\boxed{\partial_t\left(v_x-u_y-\frac fH\eta\right)=0.}
$$

The initial data are independent of $y$, so the solution remains independent of $y$ and $v_x=f(\eta-\eta_0)/H$. Differentiating continuity in time and using the zonal momentum equation gives

$$
\eta_{tt}=-H(fv_x-g\eta_{xx}),\qquad
\boxed{\eta_{tt}-c^2\eta_{xx}+f^2\eta=f^2\eta_0,\quad \eta(0)=\eta_0,\quad\eta_t(0)=0.}
$$

For a horizontal [Fourier mode](../../../fourier-analysis.md#fourier-mode) with wavenumber $k$, put $\Omega_k^2=f^2+c^2k^2$. The solution splits into a balanced component and [inertia-gravity waves](../../../geophysical-fluid-dynamics.md#inertia-gravity-wave):

$$
\widehat\eta_s=\frac{f^2}{\Omega_k^2}\widehat\eta_0,\qquad
\widehat\eta(t)=\widehat\eta_s+(\widehat\eta_0-\widehat\eta_s)\cos(\Omega_k t).
$$

These waves have frequencies $|\omega|\ge|f|$, [phase velocity](../../../wave-equation.md#phase-velocity) $\omega/k$, and [group velocity](../../../wave-equation.md#group-velocity) $c^2k/\omega$, whose magnitude is less than $c$. They have zero perturbation [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity) and carry the unbalanced part away. On the unbounded line, the localized difference between the initial and balanced profiles disperses, leaving a local steady limit. No damping is needed for this local [geostrophic adjustment](../../../geophysical-fluid-dynamics.md#geostrophic-adjustment); in a closed periodic domain, undamped waves would persist and a literal pointwise steady limit would generally not exist.

The bounded steady height satisfies the [modified Helmholtz equation](../../../partial-differential-equation.md#modified-helmholtz-equation)

$$
R_d^2\eta_s''-\eta_s=-\eta_0.
$$

Oddness removes the even homogeneous solution in the central region. The exterior solution is bounded and tends to the appropriate plateau. Matching both height and its first derivative at $x=\pm L$ gives the [geostrophic adjustment of a finite-width height ramp](../../../geophysical-fluid-dynamics.md#geostrophic-adjustment-of-a-finite-width-height-ramp):

$$
\boxed{\frac{\eta_s(x)}h=
\begin{cases}
\displaystyle\frac{x}{L}-\frac{e^{-\alpha}}{\alpha}\sinh\frac{x}{R_d},&|x|\le L,\\
\displaystyle\operatorname{sgn}(x)\left[1-\frac{\sinh\alpha}{\alpha}e^{-|x|/R_d}\right],&|x|\ge L.
\end{cases}}
$$

For example, writing the interior solution as $hx/L+B\sinh(x/R_d)$, matching its slope to the decaying exterior at $L$ gives $B=-he^{-\alpha}/\alpha$.

The steady meridional momentum equation gives $u_s=0$, and the zonal equation gives the [geostrophic balance](../../../physics.md#geostrophic-balance) $fv_s=g\eta_s'$. Thus

$$
\boxed{u_s=0,\qquad v_s(x)=\frac{gh}{fL}
\begin{cases}
1-e^{-\alpha}\cosh(x/R_d),&|x|\le L,\\
\sinh\alpha\,e^{-|x|/R_d},&|x|\ge L.
\end{cases}}
$$

The height is odd and monotone, and the meridional current is even, with maximum $v_s(0)=gh(1-e^{-\alpha})/(fL)$ for $h>0$.

For $\alpha\ll1$, the initial ramp is narrow compared with the [Rossby deformation radius](../../../physics.md#rossby-deformation-radius). To leading order,

$$
\eta_s\simeq h\operatorname{sgn}(x)(1-e^{-|x|/R_d}),\qquad
v_s\simeq\frac{gh}{c}e^{-|x|/R_d}
=\frac{gh\alpha}{fL}e^{-|x|/R_d}.
$$

Near the origin the height rises with slope $h/R_d$, rather than $h/L$; the current has width $R_d=L/\alpha$ and peak $gh\alpha/(fL)$. For $\alpha\gg1$, the central height remains nearly $hx/L$ and the central [velocity](../../../classical-mechanics.md#velocity) nearly $gh/(fL)$. Around each end of the ramp there is a matching layer of width $R_d=L/\alpha$, with height correction of order $h/\alpha$; the exterior current decays over the same width. At $x=\pm L$ the current is approximately half its central value. In both limits the zonal current is zero. These are the broad rotational adjustment of a narrow disturbance and the weak edge adjustment of a broad disturbance, respectively.

<a id="1/image-balanced-height-and-velocity-profiles-for-narrow-and-wide-initial-ramps-with-scales-shown-on-each-axis"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-73-adjustment-profiles.png)

**[Figure 1](#1/image-balanced-height-and-velocity-profiles-for-narrow-and-wide-initial-ramps-with-scales-shown-on-each-axis). Balanced height and velocity profiles for narrow and wide initial ramps, with scales shown on each axis**.

Use the [energy](../../../classical-mechanics.md#energy) normalization specified for the height [energy](../../../classical-mechanics.md#energy): the linear total [energy](../../../classical-mechanics.md#energy) [density](../../../fluid-mechanics.md#density) is $(u^2+v^2)/2+g\eta^2/(2H)$. The linear equations imply

$$
\partial_t\left[\frac{u^2+v^2}{2}+\frac{g\eta^2}{2H}\right]+\partial_x(g\eta u)=0.
$$

For $\alpha\ll1$, let the [potential energy](../../../classical-mechanics.md#potential-energy) loss mean the positive difference between the initial and final values, per unit transverse length. Although both absolute potential energies diverge on the infinite line, their difference is finite. The leading step approximation gives

$$
\Delta V=\frac{gh^2}{2H}\int_{-\infty}^{\infty}\left[2e^{-|x|/R_d}-e^{-2|x|/R_d}\right]dx
\simeq\boxed{\frac{3gh^2R_d}{2H}=\frac{3gh^2L}{2H\alpha}}.
$$

The finite ramp changes this leading expression by a relative $O(\alpha)$ correction. The initial [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is zero and the final gain is

$$
\Delta T=\frac12\left(\frac{gh}{c}\right)^2\int_{-\infty}^{\infty}e^{-2|x|/R_d}\,dx
\simeq\boxed{\frac{gh^2R_d}{2H}=\frac{gh^2L}{2H\alpha}},\qquad
\boxed{\frac{\Delta T}{\Delta V}\longrightarrow\frac13}.
$$

The remainder $\Delta V-\Delta T\simeq gh^2R_d/H$ is [energy](../../../classical-mechanics.md#energy) carried away by the outgoing [inertia-gravity waves](../../../geophysical-fluid-dynamics.md#inertia-gravity-wave). This explains why the ratio is less than one without invoking dissipation: [conservation of energy](../../../physics.md#conservation-of-energy) includes the waves, not only the final balanced flow.

## 2

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $S(z)=d\rho_s/dz$, $N^2=-gS/\rho_0>0$, and define the [quasi-geostrophic streamfunction](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-streamfunction) by $\psi=\widetilde p/(\rho_0f_0)$. Use horizontal scale $L$, vertical scale $D$, [velocity](../../../classical-mechanics.md#velocity) scale $U$ and advective time $L/U$. The required [quasi-geostrophic approximation](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-approximation) has small [Rossby number](../../../geophysical-fluid-dynamics.md#rossby-number) $\varepsilon=U/(|f_0|L)$, $\beta L/|f_0|=O(\varepsilon)$, and [Burger number](../../../geophysical-fluid-dynamics.md#burger-number) $N^2D^2/(f_0^2L^2)=O(1)$. Hydrostatic, thin-layer scaling has $D/L\ll1$; [density](../../../fluid-mechanics.md#density) variations are small compared with $\rho_0$, as required by the [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation). The leading horizontal flow is nondivergent, with vertical [velocity](../../../classical-mechanics.md#velocity) $w=O(\varepsilon UD/L)$. Retain forcing of the same slow order as [density](../../../fluid-mechanics.md#density) advection, $r=O(U\widetilde\rho/L)$; stronger forcing need not preserve this balanced scaling.

Leading [geostrophic balance](../../../physics.md#geostrophic-balance) and the [hydrostatic approximation](../../../fluid-mechanics.md#hydrostatic-approximation) give

$$
u_g=-\psi_y,\qquad v_g=\psi_x,\qquad
\widetilde\rho=-\frac{\rho_0f_0}{g}\psi_z.
$$

Write $D_g/Dt=\partial_t-\psi_y\partial_x+\psi_x\partial_y$. The [density](../../../fluid-mechanics.md#density) equation becomes

$$
f_0\frac{D_g\psi_z}{Dt}+N^2w=-\frac g{\rho_0}r,
\qquad
w=-\frac{f_0}{N^2}\frac{D_g\psi_z}{Dt}-\frac{g}{\rho_0N^2}r.
$$

Taking the curl of the horizontal momentum equations at the next order and using continuity gives the stretching equation

$$
\frac{D_g}{Dt}(\nabla_h^2\psi+\beta y)=f_0w_z.
$$

Substitute the expression for $w$. Vertical differentiation commutes with the geostrophic [material derivative](../../../continuum-mechanics.md#material-derivative) acting on $\psi_z$ here: the extra Jacobian is $J(\psi_z,\psi_z)=0$. Since $N$ depends only on height, this yields the [diabatically forced quasi-geostrophic potential vorticity](../../../geophysical-fluid-dynamics.md#diabatically-forced-quasi-geostrophic-potential-vorticity) equation

$$
\boxed{\frac{D_gq}{Dt}=-\frac{gf_0}{\rho_0}\partial_z\left(\frac r{N^2}\right),\qquad
q=\nabla_h^2\psi+\partial_z\left(\frac{f_0^2}{N^2}\psi_z\right)+\beta y.}
$$

The minus sign is appropriate to the specified [density](../../../fluid-mechanics.md#density) forcing; a positive upward [buoyancy](../../../fluid-mechanics.md#buoyancy) forcing is $R=-gr/\rho_0$ and gives $D_gq/Dt=f_0\partial_z(R/N^2)$.

Now take constant $N$ and linearize about rest. Put $s=f_0^2/N^2$ and $S_0=gf_0\mu r_0/(\rho_0N^2)$. The forced equation is

$$
\partial_t(\psi_{xx}+s\psi_{zz})+\beta\psi_x=S_0e^{-\mu z}\cos kx\cos\omega_0t.
$$

For the [harmonic heating response of quasi-geostrophic flow](../../../geophysical-fluid-dynamics.md#harmonic-heating-response-of-quasi-geostrophic-flow), represent the two traveling Fourier components with frequencies $\omega_+=\omega_0$ and $\omega_-=-\omega_0$:

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

These are the time-periodic forced responses; unspecified initial data may add free [Rossby waves](../../../geophysical-fluid-dynamics.md#rossby-wave). Selecting no incoming waves describes forcing switched on causally and then its persistent harmonic part.

For $\beta>0$, the eastward component always has $\lambda_+^2>0$. Let $\lambda_+>0$. The growing exponential would introduce an unbounded [velocity](../../../classical-mechanics.md#velocity) and [pressure](../../../thermodynamics.md#pressure) disturbance at infinity, so discard it. The bottom condition $\phi_+(0)=0$ then gives

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

Both homogeneous solutions $e^{\pm imz}$ are bounded, so boundedness is insufficient. A free [Rossby wave](../../../geophysical-fluid-dynamics.md#rossby-wave) with phase $kx+mz-\omega t$ has

$$
\omega=-\frac{\beta k}{k^2+sm^2},\qquad
c_{gz}=\frac{\partial\omega}{\partial m}=\frac{2\beta ksm}{(k^2+sm^2)^2}.
$$

The [radiation condition](../../../gravity-wave.md#radiation-condition) demands [energy](../../../classical-mechanics.md#energy) propagation away from the heating, upward into $z>0$. For $\beta,k>0$ that selects positive $m$, hence $e^{imz}$ in the westward component. The resulting solution is

$$
\boxed{\phi_-(z)=\frac{C_-}{\mu^2+m^2}\left(e^{-\mu z}-e^{imz}\right).}
$$

It satisfies $\phi_-(0)=0$ and, away from the decaying forcing, $\phi_-'\sim im\phi_-$. Its far-field amplitude does not decay in this nondissipative model: continuous forcing supplies an outgoing wave train. Thus **the low-frequency westward component propagates vertically while the eastward component remains evanescent**.

At the threshold $\omega_0=\beta/k$, the westward vertical [wavenumber](../../../wave-equation.md#wavenumber) is zero. Excluding the linearly growing homogeneous solution and retaining the bottom condition gives $\phi_-=C_-(e^{-\mu z}-1)/\mu^2$. This bounded limiting response tends to a constant and has zero vertical [group velocity](../../../wave-equation.md#group-velocity); demanding both bottom zero and decay to zero at infinity would overdetermine this threshold problem. For $\beta\le0$, the branch labels and propagation inequality must be reconsidered; the comparison stated here assumes the usual positive beta-plane gradient.

## 3

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The hydrostatic [buoyancy](../../../fluid-mechanics.md#buoyancy) anomaly is $b'=f_0\psi_z$, and its leading adiabatic evolution is $D_gb'/Dt+N_0^2w=0$. The small vertical [velocity](../../../classical-mechanics.md#velocity) advects the background stratification; vertical advection of the perturbation [buoyancy](../../../fluid-mechanics.md#buoyancy) is higher order. Consequently

$$
\boxed{w=-\frac{D_g}{Dt}\left(\frac{f_0}{N_0^2}\psi_z\right).}
$$

The [impermeability condition](../../../viscous-fluid-flow.md#no-penetration-boundary-condition) at a stationary lower boundary $z=\alpha y$ is $w=\alpha v$. Using $v_g=\psi_x$ gives the [topographic buoyancy boundary condition for quasi-geostrophic flow](../../../geophysical-fluid-dynamics.md#topographic-buoyancy-boundary-condition-for-quasi-geostrophic-flow)

$$
\frac{D_g}{Dt}\left(\frac{f_0}{N_0^2}\psi_z\right)+\alpha\psi_x=0.
$$

For application at the reference plane, the actual small-height condition is $|\alpha|L/D\ll1$. Slopes scaled by $D/L$ are of Rossby-number order, so this topographic contribution is retained alongside the small ageostrophic vertical [velocity](../../../classical-mechanics.md#velocity). The dimensional slope should not be compared to the [Rossby number](../../../geophysical-fluid-dynamics.md#rossby-number) without also specifying the aspect ratio.

The basic [quasi-geostrophic streamfunction](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-streamfunction) is $\overline\psi=-\Lambda zy$. It gives $U=\Lambda z$, basic [buoyancy](../../../fluid-mechanics.md#buoyancy) gradient $\overline b_y=-f_0\Lambda$, and spatially constant interior [quasi-geostrophic potential vorticity](../../../geophysical-fluid-dynamics.md#three-dimensional-quasi-geostrophic-potential-vorticity). Linearizing its conservation law therefore gives

$$
\boxed{(\partial_t+\Lambda z\partial_x)q'=0,\qquad
q'=\psi'_{xx}+\psi'_{yy}+s\psi'_{zz},\quad s=f_0^2/N_0^2.}
$$

The printed equation omits the shear-advection term. This cannot be omitted for general disturbances: an interior anomaly proportional to $\cos[k(x-\Lambda zt)]$ is materially conserved but not independent of time at a fixed location. The intended zero-interior-PV [Eady model](../../../hydrodynamic-stability.md#eady-model) modes do have $q'=0$ and satisfy both expressions; the ensuing mode calculation is valid in that subspace.

At either boundary, linearizing the geostrophic [material derivative](../../../continuum-mechanics.md#material-derivative) includes $v'\overline\psi_{zy}=-\Lambda\psi'_x$. Let

$$
A_0=\Lambda-\frac{N_0^2\alpha}{f_0},\qquad
A_D=\Lambda-\frac{N_0^2\gamma}{f_0},\qquad
b_0=\psi'_z(0),\quad b_D=\psi'_z(D).
$$

The two boundary equations are

$$
\boxed{\partial_tb_0=A_0\psi'_x(0),\qquad
(\partial_t+\Lambda D\partial_x)b_D=A_D\psi'_x(D).}
$$

These are exactly the respective bottom and top slope corrections to the [rigid-boundary buoyancy condition for quasi-geostrophic waves](../../../geophysical-fluid-dynamics.md#rigid-boundary-buoyancy-condition-for-quasi-geostrophic-waves).

Assume periodicity horizontally and first consider $q'=0$. Multiply its defining equation by $\psi'_x$ and integrate over the layer. The two horizontal Laplacian terms vanish by [integration by parts](../../../calculus.md#integration-by-parts); the remaining volume term after one vertical integration is an $x$-derivative. Therefore

$$
0=\int\psi'_xq'\,dV
=s\int dx\,dy\,[\psi'_x\psi'_z]_{0}^{D}.
$$

For nonzero $A_0,A_D$, the boundary equations give

$$
\frac{d}{dt}\int\frac{b_0^2}{2f_0A_0}\,dx\,dy=\frac1{f_0}\int b_0\psi'_x(0)\,dx\,dy,
\qquad
\frac{d}{dt}\int\frac{b_D^2}{2f_0A_D}\,dx\,dy=\frac1{f_0}\int b_D\psi'_x(D)\,dx\,dy.
$$

The top advection term integrates to zero. Subtracting proves conservation of the [boundary pseudomomentum of a sloping Eady layer](../../../hydrodynamic-stability.md#boundary-pseudomomentum-of-a-sloping-eady-layer):

$$
\boxed{\frac{d}{dt}\int dx\,dy\left[\frac{\psi_z'^2(D)}{2(\Lambda f_0-N_0^2\gamma)}-\frac{\psi_z'^2(0)}{2(\Lambda f_0-N_0^2\alpha)}\right]=0.}
$$

The original PDF uses squared vertical derivatives and the upper slope $\gamma$ in the first denominator; these details are corrupted in the converted TeX. For arbitrary nonzero interior PV the same calculation instead gives $d\mathcal P/dt=(f_0s)^{-1}\int\psi'_xq'\,dV$, which need not vanish. For example, at an instant take $\psi'=\cos kx+(z/D)^2\sin kx$, independent of $y$; the zonal average of $\psi'_xq'$ is $-ks/D^2$. Thus the boundary-only conservation statement also needs the zero-interior-PV qualification.

For an exponentially growing smooth [normal mode](../../../wave-equation.md#normal-mode), this qualification is automatic: the interior equation is $ik(\Lambda z-c)\widehat q=0$, and a [phase speed](../../../wave-equation.md#phase-speed) with nonzero [imaginary part](../../../complex-analysis.md#imaginary-part) cannot equal the real basic [velocity](../../../classical-mechanics.md#velocity). Therefore $\widehat q=0$. If $A_0A_D<0$, the conserved boundary [quadratic form](../../../linear-algebra.md#quadratic-form) is definite, so a nonzero exponentially growing boundary amplitude is impossible. Instability consequently requires

$$
\boxed{\left(1-\frac{N_0^2\gamma}{f_0\Lambda}\right)\left(1-\frac{N_0^2\alpha}{f_0\Lambda}\right)>0,}
$$

for $\Lambda\ne0$. When one $A$ vanishes, the corresponding boundary derivative is simply advected and must vanish for a growing mode. The other boundary then yields a real single-edge-wave speed; if both vanish, the zero-interior-PV Neumann problem has no nonzero growing mode. These degenerate cases are neutral and should not be handled by dividing by zero.

For equal slopes, put $\zeta=z/D$, $C=c/(\Lambda D)$, $M=N_0|k|D/|f_0|$, and $a=N_0^2\alpha/(f_0\Lambda)-1$. The normal-mode interior equation is $\Phi_{\zeta\zeta}-M^2\Phi=0$ for the zero-interior-PV modes. Thus

$$
\Phi=P\cosh(M\zeta)+Q\sinh(M\zeta),\qquad
(\zeta-C)\Phi_\zeta+a\Phi=0\quad\text{at }\zeta=0,1.
$$

The coefficient equations are

$$
aP-CMQ=0,
$$



$$
[(1-C)M\sinh M+a\cosh M]P+[(1-C)M\cosh M+a\sinh M]Q=0.
$$

Setting their determinant to zero, without dividing by $C$ or $a$, gives

$$
C(1-C)M\sinh M+a\cosh M+\frac{a^2}{M}\sinh M=0,
$$

so the [Eady model with parallel sloping boundaries](../../../hydrodynamic-stability.md#eady-model-with-parallel-sloping-boundaries) has

$$
\boxed{C=\frac12\pm\sqrt{\frac14+a\frac{\coth M}{M}+\frac{a^2}{M^2}}.}
$$

For positive $k,f_0$, $M$ is the printed $\mu$, and $a$ is the printed $\widetilde\alpha$. The expression is even in the sign of that vertical scale. For $a\ge0$ the radicand is at least $1/4$, so both speeds are real and **these modes have no exponential growth**. For equal slopes the earlier necessary condition is merely $a^2>0$, which is satisfied in many stable cases and is not sufficient. At $a=0$ the speeds are $0$ and $\Lambda D$; the invariant with nonzero denominators cannot be used, but the determinant still correctly gives neutral modes. No claim excluding transient amplification is needed.

## 4

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $R=\overline{u'v'}$ be the eddy [momentum flux](../../../physics.md#momentum-flux), $F=\overline{\rho'v'}$ the eddy [density](../../../fluid-mechanics.md#density) flux, and $S=d\rho_s/dz<0$. The PDF's hydrostatic equation is $g\overline\rho=-\overline p_z$; the converted TeX mistakenly replaces the [pressure](../../../thermodynamics.md#pressure) derivative by a [density](../../../fluid-mechanics.md#density) derivative. With $N_0^2=-gS/\rho_0$, define

$$
A=F/S,\qquad v^*=\overline v_a-A_z,\qquad w^*=\overline w_a+A_y.
$$

The [residual mean circulation](../../../geophysical-fluid-dynamics.md#residual-mean-circulation) is nondivergent because $v_y^*+w_z^*=\overline v_{ay}+\overline w_{az}$. Substituting in the original mean momentum and [density](../../../fluid-mechanics.md#density) equations gives the [transformed Eulerian mean](../../../geophysical-fluid-dynamics.md#transformed-eulerian-mean) equations

$$
\boxed{\overline u_t-f_0v^*=-R_y+f_0A_z=\partial_y\mathsf F_y+\partial_z\mathsf F_z,}
\qquad
\boxed{\overline\rho_t+Sw^*=0,\quad v_y^*+w_z^*=0,}
$$

with the unchanged geostrophic and hydrostatic balances. Here the [Eliassen–Palm flux](../../../geophysical-fluid-dynamics.md#eliassen-palm-flux) components are

$$
\mathsf F_y=-R,\qquad \mathsf F_z=f_0A
=\frac{f_0\overline{v'b'}}{N_0^2},\qquad b'=-g\rho'/\rho_0.
$$

The [eddy buoyancy flux](../../../geophysical-fluid-dynamics.md#eddy-buoyancy-flux) has been absorbed into the residual transport, while both types of wave forcing enter the momentum equation through the [Eliassen–Palm flux](../../../geophysical-fluid-dynamics.md#eliassen-palm-flux) divergence.

For geostrophic disturbances, the [Taylor identity for quasi-geostrophic flux](../../../geophysical-fluid-dynamics.md#taylor-identity-for-quasi-geostrophic-flux) gives

$$
\nabla\cdot\boldsymbol{\mathsf F}=\overline{v'q'}.
$$

For example, zonal averaging removes $\overline{\psi'_x\psi'_{xx}}$ and converts the remaining horizontal and vertical terms in $\overline{\psi'_xq'}$ into derivatives of $\overline{\psi'_x\psi'_y}$ and $(f_0^2/N_0^2)\overline{\psi'_x\psi'_z}$, giving precisely the displayed fluxes.

Locally, for a basic flow with nonzero meridional PV gradient $Q_y$, the [quasi-geostrophic wave pseudomomentum](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-wave-pseudomomentum) is $\mathcal A=\overline{q'^2}/(2Q_y)$. Multiplying the linear perturbation PV equation by $q'/Q_y$ gives

$$
\mathcal A_t+\nabla\cdot\boldsymbol{\mathsf F}=\frac{\overline{q'\mathcal D}}{Q_y},
$$

where $\mathcal D$ is a PV source or sink. In a locally uniform conservative [Rossby wave](../../../geophysical-fluid-dynamics.md#rossby-wave) packet, $\boldsymbol{\mathsf F}=\mathcal A\mathbf c_g$. Thus the flux tracks [group velocity](../../../wave-equation.md#group-velocity) rather than the generally different [phase velocity](../../../wave-equation.md#phase-velocity), with a signed [wave activity](../../../geophysical-fluid-dynamics.md#wave-activity) if $Q_y<0$.

The [non-acceleration theorem for quasi-geostrophic waves](../../../geophysical-fluid-dynamics.md#non-acceleration-theorem-for-quasi-geostrophic-waves) states that statistically steady conservative waves, with no wave-activity sources, sinks or independent boundary forcing, produce no balanced mean acceleration. Their flux divergence vanishes. In the present stable, impermeable mean-flow problem the homogeneous residual-circulation equation then has the zero solution, so $v^*=w^*=0$ and $\overline u_t=0$. The [Eulerian mean flow](../../../geophysical-fluid-dynamics.md#eulerian-mean-flow) can still circulate because its eddy-induced correction need not vanish. Dissipation, absorption at a critical layer, time-dependent [wave activity](../../../geophysical-fluid-dynamics.md#wave-activity) or boundary forcing produces a nonzero flux divergence and invalidates the non-acceleration conclusion.

<h3 id="4/i">Circulation application</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [Circulation application](#4/i)

Use the [meridional overturning streamfunction](../../../geophysical-fluid-dynamics.md#meridional-overturning-streamfunction) convention

$$
\overline v_a=-\mathcal X_z,\quad\overline w_a=\mathcal X_y,\qquad
v^*=-\mathcal X_z^*,\quad w^*=\mathcal X_y^*,\qquad
\boxed{\mathcal X^*=\mathcal X+F/S.}
$$

Differentiating geostrophic and hydrostatic balance gives the [thermal wind](../../../geophysical-fluid-dynamics.md#thermal-wind) relation $f_0\overline u_z=(g/\rho_0)\overline\rho_y$. Differentiate it in time and use the mean momentum and [density](../../../fluid-mechanics.md#density) equations. The resulting diagnostic [elliptic boundary value problem](../../../elliptic-boundary-value-problem.md) is

$$
\boxed{(f_0^2\partial_z^2+N_0^2\partial_y^2)\mathcal X
=\frac g{\rho_0}F_{yy}-f_0R_{yz}.}
$$

For the transformed circulation it becomes the [Eliassen equation for residual circulation](../../../geophysical-fluid-dynamics.md#eliassen-equation-for-residual-circulation), with signs appropriate to the convention above:

$$
\boxed{(f_0^2\partial_z^2+N_0^2\partial_y^2)\mathcal X^*
=f_0\partial_z\left(-R_y+f_0\partial_z(F/S)\right).}
$$

At the rigid meridional walls, impermeability requires each [streamfunction](../../../fluid-mechanics.md#stream-function) to be constant along each wall. Set those constants to zero, choosing the solution with no imposed net vertical throughflow. Since the prescribed [density](../../../fluid-mechanics.md#density) flux vanishes at both walls, the same conditions apply to $\mathcal X^*$.

There is a genuine data limitation: prescribing $F$ alone does not prescribe $R$. The term $-f_0R_{yz}$ remains in both circulation equations. To give the usual explicit step-flux circulation, assume **vanishing meridional momentum-flux divergence**, $R_y=0$, with no independently imposed circulation. The formulas below are conditional on that assumption, not a unique consequence of the [density](../../../fluid-mechanics.md#density) flux alone.

Let $l=\pi/L$, $\kappa=N_0l/|f_0|$ and $A_0=-1/S>0$, using the flux unit in which its lower plateau is $-1$. The bounded solution has $\mathcal X=\sin(ly)\chi(z)$. Its vertical equation is

$$
\chi''-\kappa^2\chi=-\frac{gl^2}{\rho_0f_0^2}\mathcal F(z).
$$

At vertical infinity require bounded Eulerian flow and vanishing residual flow. Requiring the Eulerian vertical [velocity](../../../classical-mechanics.md#velocity) to vanish also at lower infinity would be inconsistent with the continuing lower-region flux divergence. At $z=0$, continuity of $\chi$ and $\chi'$ follows because the forcing has a step but no delta function. The [step-flux residual circulation in a stratified channel](../../../geophysical-fluid-dynamics.md#step-flux-residual-circulation-in-a-stratified-channel) is therefore

$$
\boxed{\chi(z)=
\begin{cases}
-A_0(1-\tfrac12e^{\kappa z}),&z<0,\\
-\tfrac12A_0e^{-\kappa z},&z>0,
\end{cases}\qquad
\chi^*(z)=
\begin{cases}
\tfrac12A_0e^{\kappa z},&z<0,\\
-\tfrac12A_0e^{-\kappa z},&z>0.
\end{cases}}
$$

Here $\mathcal X^*=\sin(ly)\chi^*$, because $F/S=A_0\sin(ly)$ below zero and vanishes above it. The residual [streamfunction](../../../fluid-mechanics.md#stream-function) decays at both infinities, whereas the Eulerian [streamfunction](../../../fluid-mechanics.md#stream-function) tends to $-A_0\sin(ly)$ below and to zero above.

For $z\ne0$, the Eulerian [velocity](../../../classical-mechanics.md#velocity) is

$$
\overline v_a=-\frac{A_0\kappa}{2}e^{-\kappa|z|}\sin(ly),\qquad
\overline w_a=
\begin{cases}
-A_0l(1-\tfrac12e^{\kappa z})\cos(ly),&z<0,\\
-\tfrac12A_0le^{-\kappa z}\cos(ly),&z>0.
\end{cases}
$$

The flow descends near the $y=0$ wall and rises near $y=L$, with a negative meridional return flow concentrated near $z=0$. Below the dissipation level its vertical flow balances the continuing divergence of eddy [density](../../../fluid-mechanics.md#density) transport. There is no independently added throughflow, but opposing vertical transports at lower infinity are required by this idealized forcing.

Away from the discontinuity the residual meridional [velocity](../../../classical-mechanics.md#velocity) equals the Eulerian value, while

$$
w^*=
\begin{cases}
\tfrac12A_0le^{\kappa z}\cos(ly),&z<0,\\
-\tfrac12A_0le^{-\kappa z}\cos(ly),&z>0.
\end{cases}
$$

Thus the [residual mean circulation](../../../geophysical-fluid-dynamics.md#residual-mean-circulation) forms two oppositely rotating cells, confined within vertical distance $O(1/\kappa)$ of the termination of the wave flux. Its [streamfunction](../../../fluid-mechanics.md#stream-function) jumps by $-A_0\sin(ly)$ at zero. Distributionally this supplies the horizontal return transport

$$
\boxed{v^*=-\frac{A_0\kappa}{2}e^{-\kappa|z|}\sin(ly)+A_0\sin(ly)\delta(z).}
$$

The [Dirac delta](../../../distribution-theory.md#dirac-delta-function) sheet is a consequence of the discontinuous imposed flux, not an extra [boundary condition](../../../differential-equation.md#boundary-condition). Smoothing the flux termination replaces it by a thin finite return current. Streamlines must not be drawn as continuously crossing the jump without that transport.

The physical [Eulerian mean flow](../../../geophysical-fluid-dynamics.md#eulerian-mean-flow) is continuous. In the transformed momentum equation, the sheet contribution to $f_0v^*$ cancels the sheet in the flux divergence, leaving the smooth mean acceleration

$$
\overline u_t=-\frac{f_0A_0\kappa}{2}e^{-\kappa|z|}\sin(ly),\qquad
\int_{-\infty}^{\infty}\overline u_t\,dz=-f_0A_0\sin(ly).
$$

Thus termination of the vertical [Eliassen–Palm flux](../../../geophysical-fluid-dynamics.md#eliassen-palm-flux) produces a finite column-integrated wave drag, redistributed over depth by the [residual mean circulation](../../../geophysical-fluid-dynamics.md#residual-mean-circulation).

<a id="4/i/image-eulerian-and-residual-circulations-for-zero-momentum-flux-divergence-the-residual-flux-termination-sheet-closes-two-opposite-cells"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-73-mean-circulations.png)

**[Figure 2](#4/i/image-eulerian-and-residual-circulations-for-zero-momentum-flux-divergence-the-residual-flux-termination-sheet-closes-two-opposite-cells). Eulerian and residual circulations for zero momentum-flux divergence; the residual flux-termination sheet closes two opposite cells**.

For completeness, the general bounded response can be calculated without setting $R_y$ to zero. Expand $R_{yz}$ in wall-compatible sine modes, with coefficients $B_n(z)$, $l_n=n\pi/L$ and $\kappa_n=N_0l_n/|f_0|$. Add to either displayed [streamfunction](../../../fluid-mechanics.md#stream-function) the same correction

$$
\mathcal X_R(y,z)=\sum_{n\ge1}\sin(l_ny)\frac1{2f_0\kappa_n}
\int_{-\infty}^{\infty}e^{-\kappa_n|z-z'|}B_n(z')\,dz',
$$

for decaying momentum-flux forcing. The [Green function](../../../analysis.md#green-s-function) sign follows from $(\partial_z^2-\kappa_n^2)e^{-\kappa_n|z-z'|}=-2\kappa_n\delta(z-z')$.

An explicit counterexample to uniqueness is the additional [momentum flux](../../../physics.md#momentum-flux) $R=\epsilon[1-\cos(2ly)]e^{-a|z|}$, with $a>0$. It vanishes at both walls and leaves the prescribed [density](../../../fluid-mechanics.md#density) flux unchanged. For $a\ne2\kappa$ it adds

$$
\mathcal X_R=\frac{2l\epsilon a}{f_0(a^2-4\kappa^2)}\sin(2ly)\operatorname{sgn}(z)
\left(e^{-a|z|}-e^{-2\kappa|z|}\right)
$$

to both circulations. This nonzero bounded, wall-impermeable solution verifies that the original mean equations need an additional momentum-flux specification to select a unique sketch.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
