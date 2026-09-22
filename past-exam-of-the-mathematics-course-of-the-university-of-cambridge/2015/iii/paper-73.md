# Paper 73

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_73.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_73.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

One convention for the [Papkovich–Neuber representation](../../../stokes-flow.md#papkovich-neuber-representation) uses a harmonic vector potential $\boldsymbol\Phi$ and a harmonic scalar potential $\chi$:

$$
\boxed{2\mu\mathbf u=\nabla(\mathbf r\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi,\qquad p=\nabla\cdot\boldsymbol\Phi,\qquad\nabla^2\boldsymbol\Phi=0,\quad\nabla^2\chi=0.}
$$

These are [harmonic functions](../../../partial-differential-equation.md#harmonic-function) away from any singular [force](../../../classical-mechanics.md#force) point. Since $\nabla^2(\mathbf r\cdot\boldsymbol\Phi)=2\nabla\cdot\boldsymbol\Phi$, the representation gives $\nabla\cdot\mathbf u=0$ and $\mu\nabla^2\mathbf u=\nabla p$, the equations of homogeneous [Stokes flow](../../../stokes-flow.md).

Place the point [force](../../../classical-mechanics.md#force) at the origin. A [velocity](../../../classical-mechanics.md#velocity) linear in $\mathbf F$, decaying as $r^{-1}$ and having the rotational symmetry of a point [force](../../../classical-mechanics.md#force) is obtained from $\boldsymbol\Phi=c\mathbf F/r$, $\chi=0$. The vector components are [harmonic functions](../../../partial-differential-equation.md#harmonic-function) for $r>0$; scalar dipole potentials would instead generate higher-order decaying singularities. The [force](../../../classical-mechanics.md#force) normalization fixes $c=-1/(4\pi)$. Indeed, substitution gives the [Stokeslet](../../../stokes-flow.md#stokeslet):

$$
\boxed{\mathbf u(\mathbf r)=\frac1{8\pi\mu}\left(\frac{\mathbf F}{r}+\frac{(\mathbf F\cdot\mathbf r)\mathbf r}{r^3}\right),\qquad p(\mathbf r)=\frac{\mathbf F\cdot\mathbf r}{4\pi r^3}.}
$$

To verify its strength, the [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) is $\sigma_{ij}=-3(\mathbf F\cdot\mathbf r)r_i r_j/(4\pi r^5)$. Its outward traction integrated over any [sphere](../../../geometry-and-topology.md#sphere) surrounding the origin is $-\mathbf F$, because $\int\mathbf n\mathbf n\,d\Omega=(4\pi/3)I$. Thus the localized [force](../../../classical-mechanics.md#force) applied to the fluid is $\mathbf F$, as required. Translation of the origin gives the same [Stokeslet](../../../stokes-flow.md#stokeslet) centered at any prescribed [force](../../../classical-mechanics.md#force) point.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $\mathbf n=\mathbf X/R$, $\zeta=6\pi\mu a$, and let

$$
\mathsf G(\mathbf r)=\frac{I+\widehat{\mathbf r}\widehat{\mathbf r}}{8\pi\mu r},\qquad\mathsf A=\zeta\mathsf G(\mathbf X)=\frac{3a}{4R}(I+\mathbf n\mathbf n).
$$

Use the [method of reflections for Stokes flow](../../../stokes-flow.md#method-of-reflections-for-stokes-flow). At the fixed [sphere](../../../geometry-and-topology.md#sphere), the first [sphere](../../../geometry-and-topology.md#sphere) produces the incident [Stokeslet](../../../stokes-flow.md#stokeslet) [velocity](../../../classical-mechanics.md#velocity) $\mathbf u_\infty(0)=\mathsf A\mathbf V$ to leading order. In [Faxén translation law](../../../stokes-flow.md#faxen-s-first-law), set the second [sphere](../../../geometry-and-topology.md#sphere)'s translational [velocity](../../../classical-mechanics.md#velocity) to zero. The applied holding [force](../../../classical-mechanics.md#force) is therefore

$$
\boxed{\mathbf F_2=-\frac{9\pi\mu a^2}{2R}\left[\mathbf V+(\mathbf V\cdot\mathbf n)\mathbf n\right]+O\left(\frac{\mu Va^4}{R^3}\right).}
$$

The first [sphere](../../../geometry-and-topology.md#sphere)'s finite-radius [potential dipole](../../../fluid-mechanics.md#potential-dipole) adds $O(Va^3/R^3)$ to the incident [velocity](../../../classical-mechanics.md#velocity), as does the [Laplacian](../../../calculus.md#laplacian) term in [Faxén translation law](../../../stokes-flow.md#faxen-s-first-law) at the fixed [sphere](../../../geometry-and-topology.md#sphere). Multiplying by $\zeta$ gives the stated next correction. There is no intermediate $O(\mu Va^3/R^2)$ term. This is the [holding force and torque for a sphere in a distant Stokeslet](../../../stokes-flow.md#holding-force-and-torque-for-a-sphere-in-a-distant-stokeslet).

The [vorticity](../../../fluid-mechanics.md#vorticity) of a [Stokeslet](../../../stokes-flow.md#stokeslet) at displacement $\mathbf r$ is $\mathbf F\times\mathbf r/(4\pi\mu r^3)$. At the fixed [sphere](../../../geometry-and-topology.md#sphere), $\mathbf r=-\mathbf X$, so

$$
\boldsymbol\omega_\infty(0)=-\frac{3a}{2R^3}\mathbf V\times\mathbf X.
$$

Set its [angular velocity](../../../classical-mechanics.md#angular-velocity) to zero in [Faxén rotation law](../../../stokes-flow.md#faxen-s-rotational-law). The applied holding couple is

$$
\boxed{\mathbf G_2=-4\pi\mu a^3\boldsymbol\omega_\infty(0)=\frac{6\pi\mu a^4}{R^3}\mathbf V\times\mathbf X+O\left(\frac{\mu Va^6}{R^4}\right).}
$$

The displayed sign is the external couple needed to oppose the ambient rotation, rather than the hydrodynamic couple on the [sphere](../../../geometry-and-topology.md#sphere).

The leading reflected flow at the first [sphere](../../../geometry-and-topology.md#sphere) is $\mathsf G(\mathbf X)\mathbf F_2=-\mathsf A^2\mathbf V$. Apply [Faxén translation law](../../../stokes-flow.md#faxen-s-first-law) there with its prescribed [force](../../../classical-mechanics.md#force) $\mathbf F=\zeta\mathbf V$. Since $(I+\mathbf n\mathbf n)^2=I+3\mathbf n\mathbf n$, the [mobility correction from a fixed distant sphere](../../../stokes-flow.md#mobility-correction-from-a-fixed-distant-sphere) is

$$
\boxed{\dot{\mathbf X}=\mathbf V-\frac{9a^2}{16R^2}\left[\mathbf V+3(\mathbf V\cdot\mathbf n)\mathbf n\right]+O\left(\frac{Va^4}{R^4}\right).}
$$

The next correction comes from finite-radius terms in the incident/reflected flow and in [Faxén translation law](../../../stokes-flow.md#faxen-s-first-law), together with the fixed [sphere](../../../geometry-and-topology.md#sphere)'s induced [stresslet](../../../stokes-flow.md#force-dipole-flow) and holding-couple [rotlet](../../../stokes-flow.md#rotlet). Each gives $O(Va^4/R^4)$ at the first [sphere](../../../geometry-and-topology.md#sphere). The symbol $\mathbf V$ is its isolated-sphere [velocity](../../../classical-mechanics.md#velocity) scale, not its actual [velocity](../../../classical-mechanics.md#velocity) in the two-sphere problem.

The first [sphere](../../../geometry-and-topology.md#sphere) has no applied couple. Its [angular velocity](../../../classical-mechanics.md#angular-velocity) follows from [Faxén rotation law](../../../stokes-flow.md#faxen-s-rotational-law) and the reflected [Stokeslet](../../../stokes-flow.md#stokeslet):

$$
\boldsymbol\Omega_1=\frac{\mathbf F_2\times\mathbf X}{8\pi\mu R^3}+O\left(\frac{Va^4}{R^5}\right)=\boxed{-\frac{9a^2}{16}\frac{\mathbf V\times\mathbf X}{R^4}+O\left(\frac{Va^4}{R^5}\right).}
$$

The component of $\mathbf F_2$ parallel to $\mathbf X$ contributes no [vorticity](../../../fluid-mechanics.md#vorticity). The next reflected [rotlet](../../../stokes-flow.md#rotlet) and [stresslet](../../../stokes-flow.md#force-dipole-flow) give the stated error order.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [mobility correction from a fixed distant sphere](../../../stokes-flow.md#mobility-correction-from-a-fixed-distant-sphere) gives

$$
\dot Y=-\frac{27Va^2}{16}\frac{XY}{(X^2+Y^2)^2},\qquad\dot X=V\left[1+O(a^2/R^2)\right].
$$

Taking their ratio and keeping the first nonzero transverse correction yields

$$
\boxed{\frac{dY}{dX}=-\frac{27a^2}{16}\frac{XY}{R^4}}
$$

to the stated leading order. Set $b=Y_\infty\gg a$. The deflection is $O(a^2/b)$, so replacing $Y$ by $b$ on the right introduces only higher-order errors. Integrating from $X=-\infty$ gives

$$
Y(X)-b=\frac{27a^2b}{32(X^2+b^2)}+O(a^4/b^3).
$$

The maximum occurs at $X=0$, and the [deflection and spin in a distant sphere encounter](../../../stokes-flow.md#deflection-and-spin-in-a-distant-sphere-encounter) are

$$
\boxed{\max(Y-Y_\infty)=\frac{27a^2}{32Y_\infty}+O(a^4/Y_\infty^3).}
$$

For the rotation, use $dt=dX/V$ and $Y=b$ to leading order in the [angular velocity](../../../classical-mechanics.md#angular-velocity) from part (b). Its signed angle about the positive $z$ axis is

$$
\Delta\vartheta=-\frac{9a^2b}{16}\int_{-\infty}^{\infty}\frac{dX}{(X^2+b^2)^2}+O(a^4/b^4)=\boxed{-\frac{9\pi a^2}{32Y_\infty^2}+O(a^4/Y_\infty^4).}
$$

Thus the rotation is clockwise when viewed from positive $z$, with the magnitude of the displayed leading term.

The deflection tends back to zero downstream: **$Y(+\infty)=Y_\infty$**. More generally, [kinematic reversibility of Stokes flow](../../../stokes-flow.md#kinematic-reversibility-of-stokes-flow) combined with reflection in the plane $X=0$ makes a passing trajectory fore-aft symmetric. One can see this without using the distant-sphere approximation: the relevant translational [hydrodynamic mobility matrix](../../../stokes-flow.md#hydrodynamic-mobility-matrix) has the form $m_\perp(R)I+[m_\parallel(R)-m_\perp(R)]\mathbf n\mathbf n$. Hence $\dot X$ is even in $X$ and $\dot Y$ is odd in $X$. Uniqueness of the trajectory through $X=0$ then gives $Y(X)=Y(-X)$.

For $Y_\infty=a/100$, the numerical deflection and spin approximations above are invalid: the encounter enters a narrow gap and requires [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory). However, **the same return to the incoming offset holds for an ideal passing encounter of perfectly smooth [spheres](../../../geometry-and-topology.md#sphere) in [Stokes flow](../../../stokes-flow.md)**. [Lubrication resistance](../../../viscous-fluid-flow.md#lubrication-resistance) prevents finite-time contact under a bounded [force](../../../classical-mechanics.md#force), and does not itself destroy [kinematic reversibility of Stokes flow](../../../stokes-flow.md#kinematic-reversibility-of-stokes-flow). Contact, surface roughness or nonhydrodynamic [forces](../../../classical-mechanics.md#force) could change that conclusion; they are additional physics, not part of the ideal model. This distinction is the [fore-aft symmetry of a sedimenting-sphere encounter](../../../stokes-flow.md#fore-aft-symmetry-of-a-sedimenting-sphere-encounter).

## 2

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Take $z$ positive upwards and let $f$ denote axial [body force](../../../fluid-mechanics.md#body-force) per unit volume. With inertia and [surface tension](../../../fluid-mechanics.md#surface-tension) omitted, the [extensional equations for a slender Newtonian column](../../../rheology.md#extensional-equations-for-a-slender-newtonian-column) are

$$
\boxed{\partial_t(a^2)+\partial_z(a^2w)=0,\qquad\frac{3\mu}{a^2}\partial_z(a^2\partial_z w)=\partial_zp_{\mathrm{ext}}-f.}
$$

[Mass conservation](../../../continuum-mechanics.md#mass-conservation) gives the first equation. The second uses the [Trouton ratio](../../../rheology.md#trouton-ratio) three: the leading radial [velocity](../../../classical-mechanics.md#velocity) is $u_r=-r w_z/2$, the radial normal traction gives $p=p_{\mathrm{ext}}-\mu w_z$, and the axial [stress](../../../continuum-mechanics.md#stress) is $-p_{\mathrm{ext}}+3\mu w_z$. An axial [control volume](../../../fluid-mechanics.md#control-volume) balance then gives the displayed equation. The approximation requires a slender column and slowly varying radius.

Let $h=R-a$. Since the container base is closed, the total [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) at every section is zero. The column carries flux $\pi a^2w$, so the annulus carries $-\pi a^2w$ and has mean speed of order $a|w|/h$. Its interfacial [shear stress](../../../viscous-fluid-flow.md#shear-stress) is therefore of order $\lambda\mu a|w|/h^2$. Transmitting this [stress](../../../continuum-mechanics.md#stress) through the core produces an axial [velocity](../../../classical-mechanics.md#velocity) variation of order $\lambda a^2|w|/h^2$. The [plug-flow criterion for a column in a low-viscosity annulus](../../../rheology.md#plug-flow-criterion-for-a-column-in-a-low-viscosity-annulus) is consequently

$$
\boxed{\frac{\delta w}{|w|}=O\left(\frac{\lambda a^2}{h^2}\right)\ll1\quad\text{when}\quad\lambda\ll\frac{h^2}{a^2}.}
$$

Use modified [pressure](../../../thermodynamics.md#pressure) $P=p_{\mathrm{ext}}+\rho gz$, removing the annular fluid's [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure). In a local planar gap, with $y=0$ at the column and $y=h$ at the container wall, [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) gives

$$
v(y)=w\left(1-\frac yh\right)+\frac{P_z}{2\lambda\mu}y(y-h),\qquad q_g=\frac{wh}{2}-\frac{h^3P_z}{12\lambda\mu}.
$$

The required return flux per unit circumference is $q_g=-aw/2$ to leading order in $h/a$. Its pressure-driven component is larger than the Couette component by $a/h$, so the [annular return flow around a slumping column](../../../rheology.md#annular-return-flow-around-a-slumping-column) gives

$$
\boxed{P_z=\frac{6\lambda\mu a}{h^3}w\,[1+O(h/a)].}
$$

The annular shear contribution to the integrated axial [force](../../../classical-mechanics.md#force) is smaller than this pressure-gradient term by $h/a$. Retaining the leading terms and substituting $f=-(\rho+\Delta\rho)g$ gives the dimensional equations

$$
\boxed{\partial_t(a^2)+\partial_z(a^2w)=0,\qquad\frac1{a^2}\partial_z(a^2w_z)=\frac{\Delta\rho g}{3\mu}+\frac{2\lambda a}{(R-a)^3}w.}
$$

The boundary conditions are $w(0,t)=0$ at the base and $w_z(L(t),t)=0$ at the free upper end; the latter expresses zero excess axial extensional [stress](../../../continuum-mechanics.md#stress).

For $\lambda=0$ and initially constant $a=a_0$, put $G=\Delta\rho g/(3\mu)$. Then $w_{zz}=G$, so

$$
w(z,0)=G\left(\frac{z^2}{2}-L_0z\right),\qquad\boxed{w(L_0,0)=-\frac{\Delta\rho gL_0^2}{6\mu}.}
$$

For $\lambda>0$, define

$$
\phi=\frac{a^2}{R^2},\qquad\alpha(\phi)=\frac{2\sqrt\phi}{(1-\sqrt\phi)^3},\qquad\phi_0=\frac{a_0^2}{R^2},\quad\alpha_0=\alpha(\phi_0).
$$

This function records the leading thin-annulus resistance; differences from curvature and the Couette term enter at the already neglected relative order $h/a$. Choose the [extensional screening length of a slumping column](../../../rheology.md#extensional-screening-length-of-a-slumping-column) and the associated scales as

$$
\boxed{\widehat z=\frac{R}{\sqrt{\lambda\alpha_0}}=\sqrt{\frac{h_0^3}{2\lambda a_0}},\qquad\widehat w=G\widehat z^2,\qquad\widehat t=\frac{\widehat z}{\widehat w}=\frac{3\mu}{\Delta\rho g\widehat z}.}
$$

Here $h_0=R-a_0$ denotes the initial annular gap in this question. With $Z=z/\widehat z$, $T=t/\widehat t$ and $W=w/\widehat w$, the dimensional equations reduce to

$$
\boxed{\frac1\phi\partial_Z(\phi W_Z)=1+\frac{\alpha(\phi)}{\alpha_0}W,\qquad\phi_T+\partial_Z(\phi W)=0.}
$$

Initially $\phi=\phi_0$ and $\Lambda_0=L_0/\widehat z$, so $W_{ZZ}=1+W$, with $W(0)=0$ and $W_Z(\Lambda_0)=0$. The [initial velocity profile of an annularly confined column](../../../rheology.md#initial-velocity-profile-of-an-annularly-confined-column) is

$$
\boxed{W(Z,0)=\frac{\cosh(\Lambda_0-Z)}{\cosh\Lambda_0}-1,\qquad\phi_T(Z,0)=\phi_0\frac{\sinh(\Lambda_0-Z)}{\cosh\Lambda_0}.}
$$

The column thickens everywhere below its stress-free top, while that initial thickening rate is zero at the top.

For a tall column, $\Lambda_0\gg1$, the limiting forms away from exponentially small end corrections are

$$
W\simeq e^{-Z}-1,\qquad\phi_T\simeq\phi_0e^{-Z}.
$$

The bulk falls at approximately $-\widehat w$, where excess weight balances annular hydraulic resistance. Extensional [stresses](../../../continuum-mechanics.md#stress) adjust this [velocity](../../../classical-mechanics.md#velocity) to zero in a basal [boundary layer](../../../continuum-mechanics.md#boundary-layer) of thickness $\widehat z$; almost all thickening occurs there.

For a short column on this scale, $\Lambda_0\ll1$, while still slender, the limits are

$$
W\simeq\frac{Z^2}{2}-\Lambda_0Z,\qquad\phi_T\simeq\phi_0(\Lambda_0-Z).
$$

The annular-resistance term $W$ is small, so excess weight is balanced predominantly by extensional viscous [stress](../../../continuum-mechanics.md#stress). The top speed is $-\widehat w\Lambda_0^2/2$, recovering the zero-annular-viscosity result. Thus $\widehat z$ is the vertical distance over which extensional [stress](../../../continuum-mechanics.md#stress) communicates the basal constraint before annular resistance screens it. The sketches below use separate natural normalizations for the two limits.

<a id="2/image-initial-velocity-and-thickening-profiles-of-long-and-short-annularly-confined-viscous-columns"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-73-column-limits.png)

**[Figure 1](#2/image-initial-velocity-and-thickening-profiles-of-long-and-short-annularly-confined-viscous-columns). Initial velocity and thickening profiles of long and short annularly confined viscous columns**.

## 3

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

At leading order in the [lubrication approximation](../../../viscous-fluid-flow.md#lubrication-theory), surface arclength is horizontal distance. An [insoluble surfactant](../../../fluid-mechanics.md#insoluble-surfactant) is transported by the surface [velocity](../../../classical-mechanics.md#velocity), without bulk exchange or diffusion. [Conservation of insoluble surfactant on a moving interface](../../../fluid-mechanics.md#conservation-of-insoluble-surfactant-on-a-moving-interface) therefore becomes

$$
\boxed{C_t+\partial_x(Cu_s)=0,\qquad u_s=u(x,h,t).}
$$

The local [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) and capillary normal [stress](../../../continuum-mechanics.md#stress) give

$$
p_x=\rho g h_x-\partial_x(\gamma h_{xx}).
$$

Solve $\mu u_{zz}=p_x$ with [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) at $z=0$ and [Marangoni stress](../../../fluid-mechanics.md#marangoni-effect) $\mu u_z(h)=\gamma_x=-AC_x$. The [velocity](../../../classical-mechanics.md#velocity), surface [velocity](../../../classical-mechanics.md#velocity) and [volume flux per unit width](../../../fluid-mechanics.md#volume-flux-per-unit-width) are

$$
\begin{aligned}
u(z)&=\frac{p_x}{2\mu}(z^2-2hz)+\frac{\gamma_x}{\mu}z,\\
u_s&=-\frac{h^2p_x}{2\mu}-\frac{AhC_x}{\mu},\\
q&=-\frac{h^3p_x}{3\mu}-\frac{Ah^2C_x}{2\mu}.
\end{aligned}
$$

[Mass conservation](../../../continuum-mechanics.md#mass-conservation), $h_t+q_x=0$, yields the [thin-film equations with insoluble surfactant](../../../viscous-fluid-flow.md#thin-film-equations-with-insoluble-surfactant):

$$
\boxed{h_t=\frac{A}{2\mu}\partial_x(h^2C_x)+\frac{\rho g}{3\mu}\partial_x(h^3h_x)-\frac1{3\mu}\partial_x\left[h^3\partial_x(\gamma h_{xx})\right],}
$$

and the corresponding [surfactant](../../../fluid-mechanics.md#surfactant) equation is

$$
\boxed{C_t=\frac{A}{\mu}\partial_x(hCC_x)+\frac{\rho g}{2\mu}\partial_x(Ch^2h_x)-\frac1{2\mu}\partial_x\left[Ch^2\partial_x(\gamma h_{xx})\right].}
$$

The hydrostatic and capillary terms thus affect both the film flux and the surface transport, with different coefficients.

For [finite-mass Marangoni spreading on a liquid film](../../../viscous-fluid-flow.md#finite-mass-marangoni-spreading-on-a-liquid-film), first neglect both pressure-gradient terms. If the spread has size $\ell$, then $C\sim M/\ell$ and $C_x\sim M/\ell^2$, giving surface speed $u_s\sim AMh_0/(\mu\ell^2)$. Equating $\ell/t$ to this speed gives

$$
\boxed{\ell(t)\sim\left(\frac{AMh_0t}{\mu}\right)^{1/3}.}
$$

Set $\ell=(AMh_0t/\mu)^{1/3}$ exactly as a similarity scale, and write

$$
\eta=x/\ell,\qquad h=h_0H(\eta),\qquad C=(M/\ell)\Gamma(\eta).
$$

On the positive half of the pool, substitution produces two [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation):

$$
\boxed{-\frac23\eta H'=(H^2\Gamma')',\qquad-\frac13(\eta\Gamma)'=(H\Gamma\Gamma')'.}
$$

Symmetry fixes the flux integration constant in the second equation to zero, giving $H\Gamma'=-\eta/3$ wherever $\Gamma>0$. Substitution into the first equation gives $\eta H'=H$. Thus the [linear similarity profiles for surfactant spreading](../../../viscous-fluid-flow.md#linear-similarity-profiles-for-surfactant-spreading) have the form

$$
H=k\eta,\qquad\Gamma=\frac{\eta_N-\eta}{3k},\qquad0\leq\eta\leq\eta_N.
$$

The concentration vanishes at the moving front. The two integral constraints are total [surfactant](../../../fluid-mechanics.md#surfactant) mass and conservation of the fluid volume relative to the undisturbed layer:

$$
\boxed{2\int_0^{\eta_N}\Gamma\,d\eta=1,\qquad\int_0^{\eta_N}(H-1)\,d\eta=0.}
$$

The first gives $k=\eta_N^2/3$; the second gives $k\eta_N=2$. Therefore $\eta_N^3=6$. In physical variables, the solution is

$$
\boxed{x_N=\left(\frac{6AMh_0t}{\mu}\right)^{1/3},\quad h=\frac{2h_0|x|}{x_N},\quad C=\frac{M}{x_N}\left(1-\frac{|x|}{x_N}\right)\quad(|x|<x_N).}
$$

Outside the pool the leading outer solution has $h=h_0$, $C=0$. In particular, **$h(x_{N-},t)=2h_0$**: the subscript means the one-sided limit just behind the front. As a consistency check, the surface speed there is $x_N/(3t)=\dot x_N$ and the fluid jump satisfies the moving-front [mass conservation](../../../continuum-mechanics.md#mass-conservation) condition. This ideal outer solution has a height jump from $2h_0$ to $h_0$.

That jump cannot persist in a physical interface with nonzero gravity or [surface tension](../../../fluid-mechanics.md#surface-tension). Across a smoothing region of width $\Delta$, $h$ changes by $O(h_0)$. The Marangoni flux scales as $AMh_0^2/(\mu x_N^2)$. At $g=0$, its balance with the capillary flux $\gamma_0h_0^4/(\mu\Delta^3)$ gives [capillary smoothing of a Marangoni front](../../../viscous-fluid-flow.md#capillary-smoothing-of-a-marangoni-front):

$$
\boxed{\Delta\sim\left(\frac{\gamma_0h_0^2x_N^2}{AM}\right)^{1/3}\propto t^{2/9}.}
$$

Here the [surface tension](../../../fluid-mechanics.md#surface-tension) approaches $\gamma_0$ at the surfactant-free edge. The assumed concentration-gradient scale is $M/x_N^2$ even inside the smoothing region.

When gravity dominates capillarity, the hydrostatic flux is $\rho gh_0^4/(\mu\Delta)$. The same balance gives [gravity smoothing of a Marangoni front](../../../viscous-fluid-flow.md#gravity-smoothing-of-a-marangoni-front):

$$
\boxed{\Delta\sim\frac{\rho gh_0^2x_N^2}{AM}\propto t^{2/3}.}
$$

The gravity-dominated condition is $\Delta^2\gg\gamma_0/(\rho g)$, the square of the [capillary length](../../../fluid-mechanics.md#capillary-length). **The printed condition omits $\rho$; the expression above restores dimensional consistency.**

This width grows faster than $x_N$. It becomes comparable with the pool size when

$$
\boxed{x_N^*\sim\frac{AM}{\rho gh_0^2},\qquad t^*\sim\frac{\mu(AM)^2}{(\rho g)^3h_0^7}.}
$$

The time is a scaling estimate, so numerical factors cannot be fixed by the width balance. For $t\gg t^*$, the sharp-front similarity profile no longer describes the film: [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) levels the layer over the whole pool, and its thickness tends towards $h_0$ with an increasingly small depression beneath the [surfactant](../../../fluid-mechanics.md#surfactant). The surface can still spread by [Marangoni stress](../../../fluid-mechanics.md#marangoni-effect) while a hydrostatic-pressure-driven return flow nearly cancels the net film flux. In this [gravity-levelled surfactant film](../../../viscous-fluid-flow.md#gravity-levelled-surfactant-film), $q\simeq0$ gives $h_x\simeq-3AC_x/(2\rho gh_0)$, so the fractional height variation is of order $AM/(\rho gh_0^2x_N)\ll1$.

## 4

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use [pressure](../../../thermodynamics.md#pressure) with the ambient [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) removed, and let $\Delta P$ be the [pressure](../../../thermodynamics.md#pressure) below the falling [sphere](../../../geometry-and-topology.md#sphere) minus that above it. Away from the [sphere](../../../geometry-and-topology.md#sphere) the tube flow is [Hagen-Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation). The upper and lower clear lengths add to $L$ to leading order in $a/L$, so their [pressure](../../../thermodynamics.md#pressure) drops add:

$$
\boxed{Q=\frac{\pi a^4\Delta P}{8\mu L}.}
$$

The large exterior reservoir returns this flux with negligible [pressure](../../../thermodynamics.md#pressure) loss compared with the long narrow tube. The [sphere](../../../geometry-and-topology.md#sphere) is assumed far enough from the ends that entrance effects and its occupied length give only lower-order corrections.

Now use a frame translating downwards with the [sphere](../../../geometry-and-topology.md#sphere), and take $z$ positive upwards from its center. The [sphere](../../../geometry-and-topology.md#sphere) is stationary and the tube wall moves upwards with speed $U$. The narrow gap is

$$
h(z)=a-\sqrt{a^2(1-\epsilon/2)^2-z^2}\simeq\frac a2\left[\epsilon+(z/a)^2\right].
$$

It has axial length scale $a\sqrt\epsilon$, making [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) appropriate. The [sphere-frame flux in a tube](../../../viscous-fluid-flow.md#sphere-frame-flux-in-a-tube) is constant: the upward relative flux through the whole section is $\pi a^2U-Q$, so its flux per unit circumference is

$$
\boxed{q=\frac{\pi a^2U-Q}{2\pi a}.}
$$

With $y=0$ on the [sphere](../../../geometry-and-topology.md#sphere) and $y=h$ on the wall, [Couette-Poiseuille flow in a thin gap](../../../viscous-fluid-flow.md#couette-poiseuille-flow-in-a-thin-gap) gives

$$
u(y)=\frac{p_z}{2\mu}y(y-h)+\frac{Uy}{h},\qquad q=-\frac{h^3p_z}{12\mu}+\frac{Uh}{2},\qquad p_z=\frac{6\mu U}{h^2}-\frac{12\mu q}{h^3}.
$$

Since $\Delta P=-\int p_z\,dz$, the pressure-jump relation is

$$
\boxed{\frac{\Delta P}{6\mu}=2qI_3-UI_2,\qquad I_n=\int_{-\infty}^{\infty}\frac{dz}{h(z)^n}.}
$$

The parabolic inner gap can be extended to infinite $z$ because these integrals are dominated by $|z|=O(a\sqrt\epsilon)$. The [lubrication resistance integrals for a nearly occluding sphere](../../../viscous-fluid-flow.md#lubrication-resistance-integrals-for-a-nearly-occluding-sphere) are

$$
I_n=2^n a^{1-n}\epsilon^{1/2-n}J_n,\qquad J_n=\int_{-\infty}^{\infty}(1+\xi^2)^{-n}\,d\xi.
$$

Setting $\xi=\tan\theta$ evaluates $J_1=\pi$, $J_2=\pi/2$, $J_3=3\pi/8$, hence

$$
\boxed{I_1=2\pi\epsilon^{-1/2},\quad I_2=\frac{2\pi}{a}\epsilon^{-3/2},\quad I_3=\frac{3\pi}{a^2}\epsilon^{-5/2}.}
$$

For the [force](../../../classical-mechanics.md#force), enclose the fluid between sections just above and below the [sphere](../../../geometry-and-topology.md#sphere), including the annular layer. The net upward [pressure](../../../thermodynamics.md#pressure) [force](../../../classical-mechanics.md#force) is $\pi a^2\Delta P$. The tube wall exerts upward shear traction $\mu u_y(h)$ on this fluid; the [sphere](../../../geometry-and-topology.md#sphere) exerts a downward [force](../../../classical-mechanics.md#force) equal to the upward hydrodynamic [force](../../../classical-mechanics.md#force) $F$ on itself. From the gap solution,

$$
u_y(h)=\frac{p_zh}{2\mu}+\frac Uh=\frac{4U}{h}-\frac{6q}{h^2}.
$$

The axial [control volume](../../../fluid-mechanics.md#control-volume) [force](../../../classical-mechanics.md#force) balance therefore gives the [control-volume drag formula for a sphere in a tube](../../../viscous-fluid-flow.md#control-volume-drag-formula-for-a-sphere-in-a-tube):

$$
\boxed{F=\pi a^2\Delta P+2\pi a\mu(4UI_1-6qI_2).}
$$

Using a [control volume](../../../fluid-mechanics.md#control-volume) avoids having to integrate the curved-sphere normal [pressure](../../../thermodynamics.md#pressure) and tangential shear separately.

With $Q^*=Q/(\pi a^2U)$, $\Delta P^*=a\Delta P/(6\mu U)$, $q^*=2q/(aU)$, $F^*=F/(6\pi\mu aU)$, $I_n^*=a^{n-1}I_n$ and $L^*=4L/(3a)$, the three flux/[pressure](../../../thermodynamics.md#pressure) equations become

$$
Q^*=\frac{\Delta P^*}{L^*},\qquad\Delta P^*=q^*I_3^*-I_2^*,\qquad q^*=1-Q^*.
$$

Solving these linear relations gives

$$
\boxed{Q^*=\frac{I_3^*-I_2^*}{L^*+I_3^*},\qquad q^*=\frac{L^*+I_2^*}{L^*+I_3^*},\qquad\Delta P^*=\frac{L^*(I_3^*-I_2^*)}{L^*+I_3^*}.}
$$

The [force](../../../classical-mechanics.md#force) relation is $F^*=\Delta P^*+\tfrac43I_1^*-q^*I_2^*$. Substitution first yields

$$
F^*=\frac{L^*I_3^*-2L^*I_2^*+\tfrac43L^*I_1^*+\tfrac43I_1^*I_3^*-(I_2^*)^2}{L^*+I_3^*}.
$$

Because $I_2^*/I_3^*=2\epsilon/3$ and $I_1^*/I_3^*=2\epsilon^2/3$, the terms $-2L^*I_2^*$ and $\tfrac43L^*I_1^*$ are lower order than $L^*I_3^*$. Keeping the uniformly relevant leading terms gives

$$
\boxed{F^*\simeq\frac{L^*I_3^*+\tfrac43I_1^*I_3^*-(I_2^*)^2}{L^*+I_3^*}=\frac{3\pi L^*\epsilon^{-5/2}+4\pi^2\epsilon^{-3}}{L^*+3\pi\epsilon^{-5/2}}.}
$$

The squared $I_2^*$ is essential; replacing it by $I_2^*I_3^*$ would give the wrong sign and scaling. This establishes the [three drag regimes for a nearly occluding sphere](../../../viscous-fluid-flow.md#three-drag-regimes-for-a-nearly-occluding-sphere).

For $L^*\ll\epsilon^{-1/2}$,

$$
\boxed{F^*\sim\frac{4\pi}{3}\epsilon^{-1/2},\quad Q^*\sim1,\quad q^*\sim\frac23\epsilon,\quad\Delta P^*\sim L^*,\quad\frac{F^*}{\Delta P^*}\gg1.}
$$

The [sphere](../../../geometry-and-topology.md#sphere) nearly carries the tube's fluid down with it: the far-field flux is close to the piston displacement rate. The relative annular leakage is small in total volume, and the dominant [force](../../../classical-mechanics.md#force) comes from the local annular shear term. The [pressure](../../../thermodynamics.md#pressure) [force](../../../classical-mechanics.md#force) associated with the overall tube resistance is smaller.

For $\epsilon^{-1/2}\ll L^*\ll\epsilon^{-5/2}$,

$$
\boxed{F^*\sim L^*,\quad\Delta P^*\sim L^*,\quad Q^*\sim1,\quad q^*\simeq\frac23\epsilon+\frac{L^*\epsilon^{5/2}}{3\pi}\ll1,\quad\frac{F^*}{\Delta P^*}\sim1.}
$$

The flow remains approximately piston-like, but the dominant [force](../../../classical-mechanics.md#force) is now the [pressure](../../../thermodynamics.md#pressure) needed to drive [Hagen-Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation) through the long clear tube. Both displayed terms in $q^*$ are retained because their relative size changes inside this regime without producing an additional leading drag regime.

For $L^*\gg\epsilon^{-5/2}$,

$$
\boxed{F^*\sim\Delta P^*\sim3\pi\epsilon^{-5/2},\quad Q^*\sim\frac{3\pi\epsilon^{-5/2}}{L^*}\ll1,\quad q^*\sim1,\quad\frac{F^*}{\Delta P^*}\sim1.}
$$

The large tube resistance makes its net through-flow negligible. The [sphere](../../../geometry-and-topology.md#sphere)'s displaced fluid instead passes upwards relative to it through the thin annular gap, with gap [velocity](../../../classical-mechanics.md#velocity) of order $U/\epsilon$. Its [pressure](../../../thermodynamics.md#pressure) drop and resulting [pressure](../../../thermodynamics.md#pressure) [force](../../../classical-mechanics.md#force) dominate.

Finally consider two identical co-moving [spheres](../../../geometry-and-topology.md#sphere), with nonoverlapping lubrication regions and the same total clear-tube length to leading order. The common through-flux is not doubled. In the middle regime it is still approximately $\pi a^2U$, so the same total tube [pressure](../../../thermodynamics.md#pressure) drop is shared equally between the two identical [spheres](../../../geometry-and-topology.md#sphere). The [load sharing between co-moving spheres in a tube](../../../viscous-fluid-flow.md#load-sharing-between-co-moving-spheres-in-a-tube) gives **half the single-sphere [force](../../../classical-mechanics.md#force) on each [sphere](../../../geometry-and-topology.md#sphere) in regime (ii)**. In regime (i), drag is set locally by the nearly pressure-balanced annular shear and is unchanged on each [sphere](../../../geometry-and-topology.md#sphere). In regime (iii), each [sphere](../../../geometry-and-topology.md#sphere) must pass essentially its own displacement flux through its annular gap, giving the same local [pressure](../../../thermodynamics.md#pressure) drag as before; adding another [pressure](../../../thermodynamics.md#pressure) jump changes the already small tube flux but not either leading drag. **The [force](../../../classical-mechanics.md#force) is unchanged in regimes (i) and (iii).**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
