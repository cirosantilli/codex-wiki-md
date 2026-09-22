# Paper 40

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper40.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper40.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use the [instantaneous recycling approximation](../../../galaxy.md#instantaneous-recycling-approximation) and treat the [interstellar medium](../../../galaxy.md#interstellar-medium) as well mixed. If [star formation](../../../stellar-astrophysics.md#star-formation) initially consumes mass $dM$, returning a fraction $\beta$ leaves locked stellar mass $ds=(1-\beta)dM$. The original metal mass removed from the [interstellar medium](../../../galaxy.md#interstellar-medium) is $Z_i\,dM$. Of this original material, $\beta fZ_i\,dM$ returns and remains in the [galaxy](../../../galaxy.md). In addition, the [stellar yield](../../../galaxy.md#stellar-yield) produces fresh metal mass $y_i\,ds$, of which the retained part is $fy_i\,ds$. Therefore metal accounting gives

$$
d(gZ_i)=-Z_i\,dM+\beta fZ_i\,dM+fy_i\,ds,
\qquad
\boxed{\frac{d(gZ_i)}{ds}=-\frac{1-\beta f}{1-\beta}Z_i+y_if.}
$$

This is the [retained-ejecta chemical evolution](../../../galaxy.md#retained-ejecta-chemical-evolution) equation. It assumes that the same retention fraction applies to original and newly synthesized metals. Pristine [galactic gas inflow](../../../galaxy.md#galactic-gas-inflow) can change $g$ without contributing to $d(gZ_i)$; enriched [galactic gas inflow](../../../galaxy.md#galactic-gas-inflow) would require an additional metal source. Here $0\leq\beta<1$, and $0\leq f\leq1$.

A [star](../../../stellar-astrophysics.md#star) inherits the [gas-phase metallicity](../../../galaxy.md#gas-phase-metallicity) at its birth. Suppose enrichment is monotone and a fixed [initial mass function](../../../stellar-astrophysics.md#initial-mass-function), with an appropriate surviving tracer selection, produces $\kappa$ observable [stars](../../../stellar-astrophysics.md#star) per unit locked mass. For two birth abundances $Z_a<Z_b$, the relative count is

$$
N(Z_a<Z_i<Z_b)=\kappa\,[s(Z_b)-s(Z_a)],
\qquad
\boxed{\frac{dN}{dZ_i}=\kappa\frac{ds}{dZ_i}.}
$$

Thus $s(Z_i)$ is proportional to the cumulative [metallicity distribution function](../../../galaxy.md#metallicity-distribution-function); its derivative gives the differential [metallicity distribution function](../../../galaxy.md#metallicity-distribution-function). The normalized distribution after final locked mass $s_\infty$ is $s_\infty^{-1}ds/dZ_i$. For logarithmic abundances, the [logarithmic metallicity distribution](../../../galaxy.md#logarithmic-metallicity-distribution) instead has $dN/d\log_{10}Z_i=(\ln10)Z_i\,dN/dZ_i$.

The fixed [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) and survival selection matter: a mass distribution is not automatically the number distribution of every presently observable [star](../../../stellar-astrophysics.md#star). If enrichment is nonmonotone, add the contributions $\kappa|ds/dZ_i|$ from all birth-time branches attaining that abundance, rather than using one inverse.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The independent dimensionless variable is $S=s/s_\infty$. Since $gZ_i=s_\infty GZ_i$ and $dS/ds=1/s_\infty$, the chain rule gives $d(gZ_i)/ds=d(GZ_i)/dS$. The derivative in the normalized equation must consequently be with respect to $S$. Substituting the gas history in the [retained-ejecta chemical evolution](../../../galaxy.md#retained-ejecta-chemical-evolution) equation yields

$$
\frac{d(GZ_i)}{dS}+\frac{1-\beta f}{(1-\beta)S(1-S)}GZ_i=y_if.
$$

This step allows a varying retention fraction $f(S)$; no derivative of $f$ is needed because $f$ enters the instantaneous metal source and loss terms.

Set $H=GZ_i$ and now take $f=S$. The coefficient in this first-order [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) decomposes as

$$
\frac{1-\beta S}{(1-\beta)S(1-S)}=\frac1{(1-\beta)S}+\frac1{1-S}.
$$

Hence an [integrating factor](../../../differential-equation.md#integrating-factor) is $\mu(S)=S^{1/(1-\beta)}/(1-S)$. With $q=1+1/(1-\beta)=(2-\beta)/(1-\beta)$, multiplication by this [integrating factor](../../../differential-equation.md#integrating-factor) gives

$$
\mu H=S^qZ_i,
\qquad
\frac d{dS}(S^qZ_i)=\frac{y_iS^q}{1-S}.
$$

The general solution has an additional term $C/S^q$. Finite initial [gas-phase metallicity](../../../galaxy.md#gas-phase-metallicity) rules it out. Consequently, for $0<S<1$,

$$
\boxed{Z_i(S)=\frac{y_i}{S^q}\int_0^S\frac{u^q}{1-u}\,du.}
$$

The upper limit is the dimensionless $S$, not the unnormalized stellar mass. On each compact subinterval of $0\leq S<1$, the [geometric series](../../../real-analysis.md#geometric-series) $1/(1-u)=\sum_{k\geq0}u^k$ converges uniformly, permitting integration term by term. Thus

$$
Z_i=\frac{y_i}{S^q}\sum_{k=0}^{\infty}\frac{S^{q+k+1}}{q+k+1}
=\boxed{y_i\sum_{n=1}^{\infty}\frac{S^n}{q+n}.}
$$

In particular $Z_i\sim y_iS/(q+1)$ at small $S$. For positive [stellar yield](../../../galaxy.md#stellar-yield), the series is strictly increasing, so the inverse needed for the [metallicity distribution function](../../../galaxy.md#metallicity-distribution-function) exists. Differentiating either representation gives $Z_i'=y_i/(1-S)-qZ_i/S>0$. It diverges logarithmically as gas exhaustion approaches; the trace-metal approximation eventually becomes inadequate.

The [quadratic gas-history enrichment model](../../../galaxy.md#quadratic-gas-history-enrichment-model) is not a closed gas reservoir: its gas mass initially increases. This can be made consistent with the metal equation by pristine [galactic gas inflow](../../../galaxy.md#galactic-gas-inflow). Indeed gas accounting gives $dg/ds=-(1-\beta f)/(1-\beta)+dM_{\rm in}/ds$. Since $dg/ds=1-2S$ and $f=S$, the required inflow is $dM_{\rm in}/ds=q(1-S)\geq0$. It adds no metals and therefore leaves the preceding derivation intact.

## 2

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [pressure tensor](../../../thermodynamics.md#pressure-tensor) has Cartesian components $p_{ab}=\int f(v_a-u_a)(v_b-u_b)\,d^3v$. With zero mean [velocity](../../../classical-mechanics.md#velocity) and an isotropic [galactic distribution function](../../../galaxy.md#galactic-distribution-function), off-diagonal components vanish by reflection symmetry and diagonal components are equal by rotational symmetry. Therefore

$$
p_{ab}=p\delta_{ab},\qquad p=\frac13\int f|\mathbf v|^2\,d^3v=n\langle v_a^2\rangle.
$$

Here $p$ is a tracer number-weighted random-motion stress, rather than thermodynamic pressure per volume. Its tensor [divergence](../../../calculus.md#divergence) is $(\operatorname{div}\mathbf p)_a=\partial_b(p\delta_{ab})=\partial_ap$. The time-independent, nonstreaming [Jeans equation](../../../galaxy.md#jeans-equation) consequently reduces to

$$
\boxed{\nabla p=n\nabla\psi.}
$$

The [gravitational acceleration](../../../classical-mechanics.md#gravitational-acceleration) convention is $\nabla\psi$: this $\psi$ differs by a sign from the usual [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) $\Phi$.

Let $z$ measure distance along the [line of sight](../../../astrophysics.md#line-of-sight). [Spherical density projection](../../../galaxy.md#spherical-density-projection) gives

$$
N(R)=\int_{-\infty}^{\infty}n(\sqrt{R^2+z^2})\,dz
=2\int_R^\infty\frac{n(r)r}{\sqrt{r^2-R^2}}\,dr.
$$

Because isotropy makes the local second [stellar velocity moment](../../../galaxy.md#stellar-velocity-moment) along every [line of sight](../../../astrophysics.md#line-of-sight) equal to $p/n$, and because there is no streaming motion, the projected moment is

$$
N(R)\sigma^2(R)=\int_{-\infty}^{\infty}p(\sqrt{R^2+z^2})\,dz
=2\int_R^\infty\frac{p(r)r}{\sqrt{r^2-R^2}}\,dr.
$$

This is the forward relation for [isotropic stellar pressure deprojection](../../../galaxy.md#isotropic-stellar-pressure-deprojection).

Both inversions follow from one [Abel transform](../../../functional-analysis.md#abel-transform) calculation. Write $F(u)=N(\sqrt u)$ and $a(v)=n(\sqrt v)$, so $F(u)=\int_u^\infty a(v)(v-u)^{-1/2}\,dv$. Compose the transforms, using [Tonelli's theorem](../../../measure-theory.md#tonelli-theorem) for nonnegative densities, or absolute convergence for signed profiles:

$$
\begin{aligned}
J(x)&=\int_x^\infty\frac{F(u)}{\sqrt{u-x}}\,du\\
&=\int_x^\infty a(v)\left[\int_x^v\frac{du}{\sqrt{(u-x)(v-u)}}\right]dv
=\pi\int_x^\infty a(v)\,dv.
\end{aligned}
$$

Assume sufficient decay to make these integrals finite and sufficient regularity for the last derivative. Then $J'(x)=-\pi a(x)$. Setting $x=r^2$ gives the [spherical Abel deprojection](../../../galaxy.md#spherical-abel-deprojection)

$$
\boxed{n(r)=-\frac1{2\pi r}\frac d{dr}\int_{r^2}^\infty\frac{N(\sqrt u)}{\sqrt{u-r^2}}\,du.}
$$

Replacing $F(u)$ by $N(\sqrt u)\sigma^2(\sqrt u)$ and $a(v)$ by $p(\sqrt v)$ proves

$$
\boxed{p(r)=-\frac1{2\pi r}\frac d{dr}\int_{r^2}^\infty\frac{N(\sqrt u)\sigma^2(\sqrt u)}{\sqrt{u-r^2}}\,du.}
$$

These are the requested expressions, with $u=R^2$. The composed-transform argument avoids an invalid separate differentiation of a divergent lower-end kernel.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For the [spherical Abel deprojection](../../../galaxy.md#spherical-abel-deprojection), put $A_r=r^2+b^2$ and $s=(R^2+b^2)/A_r$. Then $dR^2=A_r\,ds$ and $\sqrt{R^2-r^2}=A_r^{1/2}\sqrt{s-1}$. Consequently the integral appearing in the reconstruction of $n$ is

$$
J_n(r)=N_0b^5 A_r^{-2}I_{5/2},\qquad
I_\alpha=\int_1^\infty s^{-\alpha}(s-1)^{-1/2}\,ds.
$$

Differentiate before substituting the numerical value of $I_{5/2}$:

$$
n(r)=-\frac{J_n'(r)}{2\pi r}=\frac{2N_0b^5}{\pi A_r^3}I_{5/2}
=\boxed{\frac{8N_0b^5}{3\pi(r^2+b^2)^3}.}
$$

For the projected second [stellar velocity moment](../../../galaxy.md#stellar-velocity-moment), $N\sigma^2=N_0\sigma_0^2b^6(R^2+b^2)^{-3}$. The identical substitution in [isotropic stellar pressure deprojection](../../../galaxy.md#isotropic-stellar-pressure-deprojection) gives

$$
J_p=N_0\sigma_0^2b^6A_r^{-5/2}I_3,\qquad
p(r)=\frac{5N_0\sigma_0^2b^6}{2\pi A_r^{7/2}}I_3
=\boxed{\frac{15N_0\sigma_0^2b^6}{16(r^2+b^2)^{7/2}}.}
$$

For completeness, setting $t=1/s$ yields $I_\alpha=B(1/2,\alpha-1/2)$, where $B$ is the [Euler beta function](../../../complex-analysis.md#beta-function). The [Gamma function recurrence](../../../complex-analysis.md#gamma-function-recurrence) gives $I_{5/2}=4/3$ and $I_3=3\pi/8$. This also checks the normalization of the [power-law spherical projection kernel](../../../galaxy.md#power-law-spherical-projection-kernel).

The radial [Jeans equation](../../../galaxy.md#jeans-equation) is $p'=n\psi'$. Since $p'=-105N_0\sigma_0^2b^6r/(16A_r^{9/2})$, division by the tracer [number density](../../../statistical-physics.md#number-density) gives

$$
\psi'(r)=-\frac{315\pi}{128}\frac{\sigma_0^2br}{(r^2+b^2)^{3/2}}.
$$

Writing $A=315\pi\sigma_0^2b/128$, the total [gravitational acceleration](../../../classical-mechanics.md#gravitational-acceleration) is therefore

$$
\boxed{\nabla\psi=-\frac{A\mathbf r}{(r^2+b^2)^{3/2}}.}
$$

To find all gravitating [mass density](../../../fluid-mechanics.md#density), apply the [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity), with the same sign convention:

$$
\rho_{\rm tot}(r)=-\frac1{4\pi G r^2}\frac d{dr}(r^2\psi')
=\frac{3Ab^2}{4\pi G(r^2+b^2)^{5/2}}
=\boxed{\frac{945\sigma_0^2b^3}{512G(r^2+b^2)^{5/2}}.}
$$

Equivalently, the enclosed [mass](../../../classical-mechanics.md#mass) is $M(r)=Ar^3/[G(r^2+b^2)^{3/2}]$, and $\rho_{\rm tot}=M'/(4\pi r^2)$. The inferred total [mass](../../../classical-mechanics.md#mass) is $A/G$ and its [relative potential](../../../galaxy.md#relative-potential) is $A/\sqrt{r^2+b^2}$, a [Plummer model](../../../galaxy.md#plummer-model). The tracer [number density](../../../statistical-physics.md#number-density) has a different radial exponent from this total [mass density](../../../fluid-mechanics.md#density). One must not multiply $n$ by an arbitrary stellar mass and identify it with all matter: the inferred field can include unobserved [stars](../../../stellar-astrophysics.md#star), gas, and [dark matter](../../../cosmology.md#dark-matter).

## 3

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use [gravitational acceleration](../../../classical-mechanics.md#gravitational-acceleration) $\mathbf g=\nabla\psi$. Through the plane with upward unit normal, the signed gravitational flux per unit area of the point mass is

$$
g_z(R,0)=\left.\partial_z\psi\right|_{z=0}=-\frac{Gmb}{(R^2+b^2)^{3/2}}.
$$

Thus its downward flux magnitude is $Gmb/(R^2+b^2)^{3/2}$. Subtracting a constant from the [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass) does not change this flux.

The [Kuzmin reflection method](../../../astrophysics.md#kuzmin-reflection-method) gives the even [relative potential](../../../galaxy.md#relative-potential) $\psi=Gm/\sqrt{R^2+(|z|+b)^2}$. It is harmonic above and below the plane because the corresponding point masses lie outside the respective half-spaces. At the plane the derivative jump is

$$
\partial_z\psi(R,0^+)-\partial_z\psi(R,0^-)
=-\frac{2Gmb}{(R^2+b^2)^{3/2}}.
$$

Integrating the [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) $\nabla^2\psi=-4\pi G\Sigma(R)\delta(z)$ through a thin layer, with $\delta$ the [Dirac delta](../../../distribution-theory.md#dirac-delta-function), equates this jump to $-4\pi G\Sigma$. Therefore

$$
\boxed{\Sigma(R)=\frac{mb}{2\pi(R^2+b^2)^{3/2}}.}
$$

This is a [Kuzmin disk](../../../astrophysics.md#kuzmin-disk). As a check, its total [mass](../../../classical-mechanics.md#mass) is $2\pi\int_0^\infty R\Sigma(R)\,dR=m$.

Replace the point mass by $dm=\mu(b)\,db$ and superpose the [Kuzmin disks](../../../astrophysics.md#kuzmin-disk). Linearity of the [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) gives, whenever the force integral converges,

$$
\boxed{\Sigma(R)=\frac1{2\pi}\int_0^\infty\frac{b\mu(b)}{(R^2+b^2)^{3/2}}\,db.}
$$

Both choices of potential reference give this same [surface density](../../../astrophysics.md#surface-density-of-a-disk). If the unreferenced potential diverges, perform the reference subtraction in each component before taking the integral limit; the force and the [surface density](../../../astrophysics.md#surface-density-of-a-disk) may still be finite.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The exponent of the point-mass weight is $\beta$, with $0<\beta<1$. At the origin the unreferenced [relative potential](../../../galaxy.md#relative-potential) has integrand $GBb^{\beta-1}$, whose integral diverges at its upper endpoint. In the origin-referenced potential the two terms cancel pointwise there. More generally, first form their difference at finite cutoffs and then pass to the limit. For any fixed nonzero $(R,z)$, the small-$b$ singular term is $-b^{\beta-1}$, which is integrable because $\beta>0$. At large $b$,

$$
\frac1{\sqrt{R^2+(|z|+b)^2}}-\frac1b
=-\frac{|z|}{b^2}+O(b^{-3}),
$$

so the weighted difference is integrable because $\beta<1$. Hence the referenced potential is well defined, and **its value at the origin is zero**. It is a potential difference for an infinite [astrophysical disk](../../../astrophysics.md#astrophysical-disk), not a potential with zero at infinity. In fact rescaling all lengths shows $\psi_{II}(\lambda R,\lambda z)=\lambda^\beta\psi_{II}(R,z)$; its finite values approach zero at the origin even though its force is singular there.

For $R>0$, differentiation under the convergent force integral in the plane gives

$$
\partial_R\psi_{II}=-GBR\int_0^\infty\frac{b^\beta}{(R^2+b^2)^{3/2}}\,db.
$$

Use $b=R\sqrt{t/(1-t)}$, for which $db=(R/2)t^{-1/2}(1-t)^{-3/2}\,dt$. The powers of $R$, $t$, and $1-t$ then give

$$
\partial_R\psi_{II}=-\frac{GB}{2}R^{\beta-1}\int_0^1t^{(\beta-1)/2}(1-t)^{-\beta/2}\,dt
=\boxed{-CR^{\beta-1}},
$$

where the [Euler beta function](../../../complex-analysis.md#beta-function) evaluates the constant as

$$
C=\frac{GB}{2}B\left(\frac{1+\beta}{2},1-\frac\beta2\right)
=\frac{GB}{2}\frac{\Gamma((1+\beta)/2)\Gamma(1-\beta/2)}{\Gamma(3/2)}.
$$

The first [gamma function](../../../complex-analysis.md#gamma-function) argument is $(1+\beta)/2$: it follows from adding one to the exponent of $t$. Both [Euler beta function](../../../complex-analysis.md#beta-function) arguments are positive in the stated range.

For a [circular orbit](../../../classical-mechanics.md#circular-orbit) in the plane, $V^2/R=-\partial_R\psi_{II}$. The prescribed [circular speed](../../../galaxy.md#circular-speed) therefore fixes $C=K^2$ and

$$
B=\frac{2K^2\Gamma(3/2)}{G\Gamma((1+\beta)/2)\Gamma(1-\beta/2)}.
$$

Independently, the [Kuzmin reflection method](../../../astrophysics.md#kuzmin-reflection-method) gives

$$
\Sigma(R)=\frac{B}{2\pi}\int_0^\infty\frac{b^{\beta+1}}{(R^2+b^2)^{3/2}}\,db
=\frac{BR^{\beta-1}}{4\pi}B\left(1+\frac\beta2,\frac{1-\beta}{2}\right).
$$

Here the power of $b$ is one larger than in the force integral, so its [Euler beta function](../../../complex-analysis.md#beta-function) arguments differ. Substituting the normalization fixed by the [circular speed](../../../galaxy.md#circular-speed) yields

$$
\boxed{\Sigma(R)=\frac{K^2}{2\pi G}R^{\beta-1}
\frac{\Gamma(1+\beta/2)\Gamma((1-\beta)/2)}{\Gamma((1+\beta)/2)\Gamma(1-\beta/2)}.}
$$

This [scale-free Kuzmin superposition](../../../astrophysics.md#scale-free-kuzmin-superposition) has nonnegative [surface density](../../../astrophysics.md#surface-density-of-a-disk), finite central enclosed [mass](../../../classical-mechanics.md#mass), and infinite total [mass](../../../classical-mechanics.md#mass). Its force and [surface density](../../../astrophysics.md#surface-density-of-a-disk) approach the [Mestel disk](../../../astrophysics.md#mestel-disk) values as $\beta\downarrow0$; that limiting disk requires a different potential reference at the origin.

## 4

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Let $\mathcal G$ be the outward [viscous torque in an accretion disk](../../../astrophysics.md#viscous-torque-in-an-accretion-disk). For a declining [angular velocity](../../../classical-mechanics.md#angular-velocity), the vertically integrated viscous shear stress gives

$$
\mathcal G=-2\pi\nu\Sigma r^3\Omega'(r)>0.
$$

In a steady [accretion disk](../../../astrophysics.md#accretion-disk) without radiated [angular momentum](../../../classical-mechanics.md#angular-momentum), the net inward [angular-momentum flux](../../../classical-mechanics.md#angular-momentum-flux) $Fh-\mathcal G$ is constant and equals the swallowed flux $Fh_0$. Thus [conservation of angular momentum](../../../classical-mechanics.md#conservation-of-angular-momentum) gives $F(h-h_0)=\mathcal G$. Substituting $F=2\pi r\Sigma u$ cancels the [surface density](../../../astrophysics.md#surface-density-of-a-disk) and proves

$$
\boxed{u=\frac{\nu r^2[-\Omega'(r)]}{h-h_0}.}
$$

This uses the stipulated phenomenological viscous shear law; it does not replace it by a different fully relativistic stress prescription.

For the orbital calculation let a dot denote a derivative with respect to [proper time](../../../special-relativity.md#proper-time). Substituting the geodesic energy and [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) first integrals into the timelike normalization in [Schwarzschild spacetime](../../../general-relativity.md#schwarzschild-spacetime) gives

$$
\dot r^2=\frac{\epsilon^2}{c^2}-\left(1-\frac{2m}{r}\right)\left(c^2+\frac{h^2}{r^2}\right).
$$

Differentiate with $h$ and $\epsilon$ constant along the [geodesic](../../../riemannian-geometry.md#geodesic). Where $\dot r\ne0$, division by $2\dot r$ gives

$$
\ddot r=-\frac12\frac d{dr}\left[\left(1-\frac{2m}{r}\right)\left(c^2+\frac{h^2}{r^2}\right)\right]
=\boxed{-\frac{mc^2}{r^2}+\frac{h^2}{r^3}\left(1-\frac{3m}{r}\right).}
$$

This equation also holds at turning points and on [circular orbits](../../../classical-mechanics.md#circular-orbit). To justify that without dividing by zero, put $A=1-2m/r$ in the equatorial geodesic [Lagrangian](../../../calculus-of-variations.md#lagrangian) $L=(Ac^2\dot t^2-A^{-1}\dot r^2-r^2\dot\phi^2)/2$. Its radial [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is $\ddot r=(A'/2A)\dot r^2-AA'c^2\dot t^2/2+Ar\dot\phi^2$. Substitution of the timelike normalization cancels the $\dot r^2$ terms and yields $\ddot r=-A'c^2/2+(A/r-A'/2)h^2/r^2$, exactly the displayed radial equation, including when $\dot r=0$.

A [circular orbit](../../../classical-mechanics.md#circular-orbit) requires $\ddot r=\dot r=0$. Therefore

$$
h^2=\frac{mc^2r^2}{r-3m},\qquad
\boxed{h(r)=rc\sqrt{\frac m{r-3m}}},\qquad r>3m,
$$

choosing the positive sense of rotation. Differentiating the square is simpler than differentiating $h$:

$$
\frac d{dr}h^2=mc^2\frac{r(r-6m)}{(r-3m)^2}.
$$

It is negative for $3m<r<6m$ and positive for $r>6m$, so the global minimum over timelike [circular orbits](../../../classical-mechanics.md#circular-orbit) is

$$
\boxed{r_0=6m,\qquad h_0=\sqrt{12}\,mc.}
$$

As a stability check, the second radial derivative of $W=(1-2m/r)(c^2+h^2/r^2)$ at a [circular orbit](../../../classical-mechanics.md#circular-orbit), holding $h$ fixed for the perturbation, is $W''=2mc^2(r-6m)/[r^3(r-3m)]$. Thus the exterior branch is stable, and $6m$ is the [innermost stable circular orbit](../../../astrophysics.md#innermost-stable-circular-orbit). It is the natural matching radius for the idealized [zero-torque inner boundary condition](../../../astrophysics.md#zero-torque-inner-boundary-condition).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Take constant [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) $\nu$ and the inner [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) found above. The [Angular velocity of a circular Schwarzschild geodesic](../../../general-relativity.md#angular-velocity-of-a-circular-schwarzschild-geodesic) gives $-\Omega'=3c\sqrt m/(2r^{5/2})$. Hence the inward radial component of [four-velocity](../../../special-relativity.md#four-velocity) in the stated viscous model is

$$
u=\frac{3\nu/2}{\sqrt r\,[r/\sqrt{r-3m}-\sqrt{12m}]}.
$$

To convert [proper time](../../../special-relativity.md#proper-time) to [Schwarzschild time](../../../general-relativity.md#schwarzschild-time), neglect $\dot r^2$ in the normalization as prescribed and insert the circular value of $h$. One obtains

$$
\frac{dt}{d\tau}\simeq\sqrt{\frac{1+h^2/(c^2r^2)}{1-2m/r}}
=\sqrt{\frac r{r-3m}}.
$$

The change in observed [Schwarzschild time](../../../general-relativity.md#schwarzschild-time) equals this coordinate-time change when differential light travel time is neglected. Since $dr/d\tau=-u$,

$$
\Delta t=\int_{6m}^{r_1}\frac{dt/d\tau}{u}\,dr
=\boxed{\frac2{3\nu}\int_{6m}^{r_1}\left[r-\sqrt{12m(r-3m)}\right]\frac r{r-3m}\,dr.}
$$

This time is nonnegative: $r^2-12m(r-3m)=(r-6m)^2\geq0$ on the integration interval.

Put $x=r/(3m)$ and $X=r_1/(3m)$. The integral becomes

$$
\Delta t=\frac{6m^2}{\nu}\int_2^X\left[\frac{x^2}{x-1}-\frac{2x}{\sqrt{x-1}}\right]dx.
$$

Polynomial division gives $x^2/(x-1)=x+1+1/(x-1)$. Separately, writing $y=x-1$ gives $\int2x/\sqrt{x-1}\,dx=(4/3)(x-1)^{3/2}+4\sqrt{x-1}$. Therefore the antiderivative inside the integral is

$$
\frac{x^2}{2}+x+\log(x-1)-\frac43(x-1)^{3/2}-4\sqrt{x-1}.
$$

Its value at $x=2$ is $-4/3$. Subtracting this lower endpoint yields the [formal viscous inspiral time in Schwarzschild spacetime](../../../astrophysics.md#formal-viscous-inspiral-time-in-schwarzschild-spacetime)

$$
\boxed{\Delta t=\frac{m^2}{\nu}\left[3X^2+6X+6\log(X-1)-8(X-1)^{3/2}-24\sqrt{X-1}+8\right].}
$$

**The logarithm has a positive coefficient.** The minus sign in the printed final expression is inconsistent with its preceding integral. Differentiating the corrected bracket gives $6X[X-2\sqrt{X-1}]/(X-1)$, precisely the positive integrand after rescaling. The bracket vanishes at $X=2$; replacing $+6\log(X-1)$ by its negative would give derivative $-12$ there and a negative elapsed time for $X$ just above $2$. This is a sign error, not a choice of potential or time convention.

The result assumes constant [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity); if $\nu$ varies with radius it remains inside the time integral. There is also a physical limitation to the stipulated approximation: $h-h_0$ vanishes quadratically at $6m$, so its formal $u$ diverges and eventually violates the neglected-radial-motion condition. The finite integral is the formal extrapolation of the nearly circular viscous model. A real [accretion disk](../../../astrophysics.md#accretion-disk) must instead match to its [plunging region of a black-hole accretion disk](../../../astrophysics.md#plunging-region-of-a-black-hole-accretion-disk); this approximation cannot describe that transition arbitrarily closely.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
