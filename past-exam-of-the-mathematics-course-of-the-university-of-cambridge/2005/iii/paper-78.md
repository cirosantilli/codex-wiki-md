# Paper 78

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper78.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper78.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For the [polar decomposition of an invertible real matrix](../../../linear-algebra.md#polar-decomposition-of-an-invertible-real-matrix), start with $C=F^TF$. For nonzero $y$, $y^TCy=|Fy|^2>0$, since $\det F>0$ makes $F$ invertible. The [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) gives an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $n_a$ with $Cn_a=\lambda_a^2n_a$ and $\lambda_a>0$. Define

$$
U=\sum_a\lambda_a n_a\otimes n_a,\qquad R=FU^{-1}.
$$

Then $U$ is a [positive-definite symmetric matrix](../../../linear-algebra.md#symmetric-positive-definite-matrix), $U^2=C$, and

$$
R^TR=U^{-1}F^TFU^{-1}=I,\qquad
\det R=\frac{\det F}{\det U}=1,
$$

because $\det U=\sqrt{\det(F^TF)}=\det F$. Thus $R$ is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) with positive determinant. Set $V=RUR^T$; it too is a [positive-definite symmetric matrix](../../../linear-algebra.md#symmetric-positive-definite-matrix), and $VR=RU=F$. Moreover $V^2=FF^T$. This proves

$$
\boxed{F=RU=VR,\quad U=(F^TF)^{1/2},\quad V=(FF^T)^{1/2},\quad R^TR=I,\quad\det R=1.}
$$

The positive square root is unique: any positive symmetric square root of $C$ commutes with $C$, preserves its eigenspaces and has the positive scalar square root on each of them. Hence $U$, then $R$ and $V$, are unique. These are the [right stretch tensor](../../../continuum-mechanics.md#right-stretch-tensor), rotation and [left stretch tensor](../../../continuum-mechanics.md#left-stretch-tensor) of the [polar decomposition in continuum mechanics](../../../continuum-mechanics.md#polar-decomposition-in-continuum-mechanics).

A standard [spectral strain measure](../../../continuum-mechanics.md#spectral-strain-measure) is

$$
E^f=f(U)=\sum_a f(\lambda_a)n_a\otimes n_a.
$$

Take $f\in C^1(0,\infty)$, $f(1)=0$ and $f'(1)=1$, with $f$ strictly increasing; the customary stronger condition $f'(\lambda)>0$ gives a regular one-to-one parameterization of all positive [principal stretches](../../../continuum-mechanics.md#principal-stretch). The zero condition makes a rigid rotation [strain](../../../continuum-mechanics.md#strain) free, monotonicity distinguishes extension from contraction and prevents nonunit stretch from being [strain](../../../continuum-mechanics.md#strain) free, and the derivative normalization gives the ordinary infinitesimal [strain](../../../continuum-mechanics.md#strain). Indeed, for $F=I+H$,

$$
U=I+\frac{H+H^T}{2}+O(\|H\|^2),\qquad
E^f=\frac{H+H^T}{2}+o(\|H\|).
$$

Under a superposed spatial rotation $F\mapsto QF$, $F^TF$ and hence $E^f$ remain unchanged, giving [material frame indifference](../../../continuum-mechanics.md#material-frame-indifference). Choosing $f(\lambda)=\lambda-1$ satisfies all these conditions and gives the [Biot strain tensor](../../../continuum-mechanics.md#biot-strain-tensor)

$$
\boxed{E^{(1)}=U-I.}
$$

The meaning of [work-conjugate stress and strain](../../../continuum-mechanics.md#work-conjugate-stress-and-strain) here is that a symmetric material [tensor](../../../linear-algebra.md#tensor) $T^f$ satisfies

$$
T^f:\dot E^f=P_{Ii}\dot F_{iI}
$$

for every admissible rate, with both powers measured per reference volume. To keep the nominal-stress index convention explicit, write $M_{iI}=P_{Ii}$, so $M=P^T$ and the power is $M:\dot F$. Differentiating $F=RU$ gives $\dot F=R(\Omega U+\dot U)$, where $\Omega=R^T\dot R$ is skew. [Conservation of angular momentum](../../../classical-mechanics.md#conservation-of-angular-momentum) gives symmetry of $MF^T$, or equivalently of $R^TMU$. Therefore

$$
\begin{aligned}
M:\dot F
&=\operatorname{tr}((R^TM)^T\Omega U)
 +(R^TM):\dot U\\
&=\operatorname{tr}((R^TMU)^T\Omega)
 +\operatorname{sym}(R^TM):\dot U\\
&=\operatorname{sym}(R^TM):\dot U.
\end{aligned}
$$

The first term vanishes because a symmetric [tensor](../../../linear-algebra.md#tensor) has zero contraction with a skew [tensor](../../../linear-algebra.md#tensor). Since $\dot E^{(1)}=\dot U$, the [symmetric Biot stress](../../../continuum-mechanics.md#symmetric-biot-stress) is

$$
\boxed{T^{(1)}=\operatorname{sym}(PR)
=\frac12(PR+R^TP^T).}
$$

If the [nominal stress](../../../continuum-mechanics.md#nominal-stress-tensor) is instead stored spatial-index first as $M$, the same answer is $\operatorname{sym}(R^TM)$. The symmetrization is essential: $PR$ need not itself be symmetric.

## 2

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use $z=\lambda_z>0$. In cylindrical orthonormal bases the [principal stretches](../../../continuum-mechanics.md#principal-stretch) are $r_{,R}$, $r/R$ and $z$. [Incompressibility](../../../fluid-mechanics.md#incompressible-flow) gives

$$
r_{,R}\frac rR z=1,\qquad
\frac{d(r^2)}{dR}=\frac{2R}{z}.
$$

Integrate from the inner surface to obtain the [inflation and extension of an incompressible tube](../../../continuum-mechanics.md#inflation-and-extension-of-an-incompressible-tube) kinematics

$$
r^2=a^2+\frac{R^2-a_0^2}{z},\qquad
\boxed{\lambda=\frac rR=z^{-1/2}
\left(1+\frac{za^2-a_0^2}{R^2}\right)^{1/2}.}
$$

In particular $b^2=a^2+(b_0^2-a_0^2)/z$. The radial [principal stretch](../../../continuum-mechanics.md#principal-stretch) is $1/(z\lambda)$, so the reference-volume [strain energy density](../../../continuum-mechanics.md#strain-energy-density) is $\widehat W(\lambda,z)$ with the three arguments $(1/(z\lambda),\lambda,z)$.

For reference length $L_0$, the stored energy is $L_0\mathcal E$, where

$$
\mathcal E(a,z)=2\pi\int_{a_0}^{b_0}\widehat W(\lambda(R;a,z),z)R\,dR.
$$

Let $N_{\rm wall}$ denote the total axial resultant acting on the material annulus. The work of the inner [pressure](../../../thermodynamics.md#pressure) on the cylindrical wall is $2\pi azL_0p\dot a$, and axial work is $N_{\rm wall}L_0\dot z$. Reversible [virtual work](../../../classical-mechanics.md#virtual-work) therefore says

$$
2\pi azp\dot a+N_{\rm wall}\dot z
=\mathcal E_{,a}\dot a+\mathcal E_{,z}\dot z.
$$

The independent derivatives of the circumferential stretch are

$$
\lambda_{,a}=\frac{a}{\lambda R^2},\qquad
\left.\lambda_{,z}\right|_a
=-\frac{R^2-a_0^2}{2\lambda z^2R^2}.
$$

Equating the coefficients of $\dot a$ and $\dot z$ proves

$$
\boxed{p=\frac1z\int_{a_0}^{b_0}
\widehat W_{,\lambda}\frac{dR}{\lambda R},}
$$

and the corresponding axial resultant is

$$
\boxed{N_{\rm wall}=2\pi\int_{a_0}^{b_0}
\left[\widehat W_{,z}R
-\widehat W_{,\lambda}\frac{R^2-a_0^2}{2\lambda z^2R}\right]dR.}
$$

Here $\widehat W_{,z}$ holds $\lambda$ fixed. If $N$ means the independently applied load on pressurized closed ends, the [pressure](../../../thermodynamics.md#pressure) also does axial end-cap work $\pi a^2pL_0\dot z$. Equivalently its complete work is $p\,d(\pi a^2zL_0)/dt$. In that convention,

$$
\boxed{N=N_{\rm wall}-\pi a^2p.}
$$

If $N$ includes the end-pressure resultant, it is $N_{\rm wall}$ itself. Stating this distinction is necessary because the ends are not specified; the [pressure](../../../thermodynamics.md#pressure) formula is the same in both conventions.

For the specified [Mooney-Rivlin solid](../../../continuum-mechanics.md#mooney-rivlin-solid) convention, differentiating the constrained [strain energy density](../../../continuum-mechanics.md#strain-energy-density) gives

$$
\widehat W_{,\lambda}
=(\mu_1-\mu_2z^2)(\lambda-z^{-2}\lambda^{-3}).
$$

Thus

$$
p=z^{-1}(\mu_1-\mu_2z^2)
\int_{a_0}^{b_0}(1-z^{-2}\lambda^{-4})\frac{dR}{R}.
$$

Put $c=za^2-a_0^2$. If $c\ne0$, $z\lambda^2-1=c/R^2$ yields $dR/R=-z\lambda\,d\lambda/(z\lambda^2-1)$. The factor cancels because

$$
\frac{\lambda(1-z^{-2}\lambda^{-4})}{z\lambda^2-1}
=\frac1{z\lambda}+\frac1{z^2\lambda^3}.
$$

The limits are $\lambda_a=a/a_0$ and $\lambda_b=b/b_0$, so direct integration gives

$$
\boxed{p=(\mu_1z^{-2}-\mu_2)
\left[z\log\frac{\lambda_a}{\lambda_b}
-\frac12(\lambda_a^{-2}-\lambda_b^{-2})\right].}
$$

For $c=0$, all circumferential stretches equal $z^{-1/2}$ and the original integrand vanishes, so this formula still holds, with $p=0$. This also verifies its continuous limiting value without dividing by zero.

## 3

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $v_i=\dot x_i$ and use a fixed arbitrary material subvolume $B_0$ in the [reference configuration](../../../continuum-mechanics.md#reference-configuration), with outward unit normal $N_I$. The reference mass density $\rho_0$ is time independent. The global [momentum conservation](../../../classical-mechanics.md#momentum-conservation) law is

$$
\frac d{dt}\int_{B_0}\rho_0v_i\,dX
=\int_{\partial B_0}P_{Ii}N_I\,dS+\int_{B_0}\rho_0g_i\,dX.
$$

The [divergence theorem](../../../calculus.md#divergence-theorem), differentiation under the integral, and arbitrariness of $B_0$ give

$$
\boxed{\rho_0\dot v_i=P_{Ii,I}+\rho_0g_i.}
$$

The global [conservation of energy](../../../physics.md#conservation-of-energy) law includes both [internal energy](../../../thermodynamics.md#internal-energy) and [kinetic energy](../../../classical-mechanics.md#kinetic-energy):

$$
\frac d{dt}\int_{B_0}\rho_0\left(u+\frac12v_iv_i\right)dX
=\int_{\partial B_0}(P_{Ii}v_i-q_I^0)N_I\,dS
+\int_{B_0}\rho_0(g_iv_i+r)\,dX.
$$

Here $q^0$ is outgoing [heat flux](../../../thermodynamics.md#heat-flux-density) per reference area. Localizing gives

$$
\rho_0\dot u+\rho_0v_i\dot v_i
=P_{Ii,I}v_i+P_{Ii}v_{i,I}-q_{I,I}^0
+\rho_0g_iv_i+\rho_0r.
$$

Subtract the scalar product of the local [momentum conservation](../../../classical-mechanics.md#momentum-conservation) law with $v$. Since $v_{i,I}=\dot F_{iI}$, this proves the [Lagrangian internal energy balance](../../../continuum-mechanics.md#lagrangian-internal-energy-balance)

$$
\boxed{\rho_0\dot u=P_{Ii}\dot F_{iI}+\rho_0r-q_{I,I}^0.}
$$

For positive [temperature](../../../thermodynamics.md#temperature) $\theta$, the global [entropy](../../../thermodynamics.md#entropy) inequality is

$$
\frac d{dt}\int_{B_0}\rho_0\eta\,dX
\geq\int_{B_0}\frac{\rho_0r}{\theta}\,dX
-\int_{\partial B_0}\frac{q_I^0N_I}{\theta}\,dS.
$$

Its local excess is a nonnegative production density $\gamma$. Expanding the divergence of $q^0/\theta$ proves the [Lagrangian entropy inequality](../../../continuum-mechanics.md#lagrangian-entropy-inequality) in the requested equality form:

$$
\boxed{\rho_0\dot\eta
=\frac{\rho_0r-q_{I,I}^0}{\theta}
+\frac{\theta_{,I}q_I^0}{\theta^2}+\gamma,
\qquad\gamma\geq0.}
$$

No constitutive assumption on the [heat flux](../../../thermodynamics.md#heat-flux-density) was needed for these balance identities.

For the [reference-configuration jump balances](../../../continuum-mechanics.md#reference-configuration-jump-balances), make the orientation convention explicit. Write $[a]=a^+-a^-$ and let $n^0$ point from the minus side to the plus side. Let $c$ be the actual interface speed in direction $n^0$. A signed level function $\phi$ with the plus side $\phi>0$ obeys $\phi_t=-c|\nabla_X\phi|$ on the interface. For $a=a^-+[a]H(\phi)$, the singular time derivative is $-c[a]\delta_S$; the singular reference divergence of $b$ is $n_I^0[b_I]\delta_S$. Thus a local conservation law $a_t=\operatorname{Div}b+$ bounded sources has the [Rankine-Hugoniot condition](../../../partial-differential-equation.md#rankine-hugoniot-conditions)

$$
-c[a]=n_I^0[b_I].
$$

This is also the shrinking moving-pillbox calculation of the global law: finite volume supplies have no surviving surface term.

To match the displayed positive-sign momentum jump in the paper, use its speed parameter as $V=-c$, so the interface travels in direction $-Vn^0$. Assuming continuous $\rho_0$ and no surface force or energy supply, the jump laws are then

$$
\boxed{\rho_0V[v_i]=n_I^0[P_{Ii}],}
$$



$$
\boxed{\rho_0V\left[u+\frac12v_iv_i\right]
=n_I^0[P_{Ii}v_i-q_I^0],}
$$

and, from $\partial_t(\rho_0\eta)+\operatorname{Div}(q^0/\theta)\geq\rho_0r/\theta$,

$$
\boxed{\rho_0V[\eta]+n_I^0[q_I^0/\theta]\geq0.}
$$

The last inequality is nonnegative entropy production concentrated on the interface. Temperature and flux in the entropy term are the traces on their respective sides; one cannot take a common temperature outside the jump unless it is continuous.

If $V$ is instead defined as the interface speed in direction $n^0$, all three $V$ terms above acquire a minus sign. In particular the printed positive-sign momentum formula requires the opposite speed convention; changing just the order of the jump does not remove this convention issue. If reference density is discontinuous, replace $\rho_0[a]$ by the jump $[\rho_0a]$ of the complete conserved density.

An equivalent internal-energy jump follows by subtracting the kinetic-energy jump using $[|v|^2/2]=\{v_i\}[v_i]$, where $\{a\}=(a^++a^-)/2$:

$$
\rho_0V[u]=n_I^0\{P_{Ii}\}[v_i]-n_I^0[q_I^0].
$$

The averaged traction appears because $[P_{Ii}v_i]=\{P_{Ii}\}[v_i]+[P_{Ii}]\{v_i\}$; using a one-sided traction would generally be incorrect.

## 4

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [spin tensor](../../../viscous-fluid-flow.md#spin-tensor) $W$ is skew, and $\dot Q Q^T=W$ means $\dot Q=WQ$ and $\dot Q^T=-Q^TW$. Differentiate all factors to obtain the [corotating-frame representation of a Jaumann derivative](../../../rheology.md#corotating-frame-representation-of-a-jaumann-derivative):

$$
\begin{aligned}
\frac d{dt}(Q^TTQ)
&=-Q^TWTQ+Q^T\dot TQ+Q^TTWQ\\
&=Q^T(\dot T-WT+TW)Q.
\end{aligned}
$$

Thus the [Jaumann derivative](../../../rheology.md#jaumann-derivative) is the ordinary derivative of the [tensor](../../../linear-algebra.md#tensor) components in this rotating frame.

Put $S=\sigma^d$, $\Delta\mu=\mu_1-\mu_0$, $A=S-2\mu_0D$ and $\widetilde A=Q^TAQ$, $\widetilde D=Q^TDQ$. The [corotational Jeffreys fluid](../../../rheology.md#corotational-jeffreys-fluid) equation reduces to

$$
\dot{\widetilde A}+\frac1\tau\widetilde A
=\frac{2\Delta\mu}{\tau}\widetilde D.
$$

For $\tau>0$, an [integrating factor](../../../differential-equation.md#integrating-factor) gives the complete finite-initial-time solution

$$
\widetilde A(t)=e^{-(t-t_0)/\tau}\widetilde A(t_0)
+\frac{2\Delta\mu}{\tau}\int_{t_0}^t
 e^{-(t-s)/\tau}\widetilde D(s)\,ds.
$$

The infinite-past constitutive history selects $\lim_{t_0\to-\infty}e^{t_0/\tau}\widetilde A(t_0)=0$, as holds for bounded past [stress](../../../continuum-mechanics.md#stress) histories, and assumes convergence of the integral. Taking that limit and rotating back proves

$$
\boxed{S(t)=2\mu_0D(t)+\frac{2\Delta\mu}{\tau}
\int_{-\infty}^t e^{-(t-s)/\tau}
Q(t)Q^T(s)D(s)Q(s)Q^T(t)\,ds.}
$$

A general initial [stress](../../../continuum-mechanics.md#stress) would retain the displayed homogeneous term. [Incompressibility](../../../fluid-mechanics.md#incompressible-flow) means $\operatorname{tr}D=0$; the [pressure](../../../thermodynamics.md#pressure) reaction is added as $\sigma=S-pI$ and does not affect this [deviatoric stress](../../../continuum-mechanics.md#deviatoric-stress) equation.

For [simple shear deformation](../../../continuum-mechanics.md#simple-shear), direct multiplication gives the [velocity gradient](../../../continuum-mechanics.md#velocity-gradient) and its symmetric and skew parts:

$$
L=\dot FF^{-1}=\begin{pmatrix}0&\dot\gamma\\0&0\end{pmatrix},\qquad
D=\frac{\dot\gamma}{2}\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
W=\frac{\dot\gamma}{2}\begin{pmatrix}0&1\\-1&0\end{pmatrix}.
$$

Use the signed counterclockwise angle $\theta$ with

$$
Q(t)=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix},
\qquad \dot\theta=-\dot\gamma/2.
$$

Thus the material frame rotates clockwise for positive shear rate. This angle convention is necessary for the signs of the sine terms. Set $\delta=\theta(t)-\theta(s)$. With $H=\begin{pmatrix}0&1\\1&0\end{pmatrix}$ and $R_\delta=Q(t)Q^T(s)$, multiplication yields

$$
R_\delta H R_\delta^T
=\begin{pmatrix}-\sin2\delta&\cos2\delta\\
\cos2\delta&\sin2\delta\end{pmatrix}.
$$

Substitution in the history formula proves

$$
\boxed{S(t)=\mu_0\dot\gamma(t)H+
\frac{\Delta\mu}{\tau}\int_{-\infty}^t
 e^{-(t-s)/\tau}\dot\gamma(s)
\begin{pmatrix}-\sin2\delta&\cos2\delta\\
\cos2\delta&\sin2\delta\end{pmatrix}ds.}
$$

The suppressed third row and column are zero for the selected infinite-past history.

For constant shear rate $g=\dot\gamma$, $2\delta=-g(t-s)$. Put $u=t-s\geq0$. The real and imaginary parts of the elementary exponential integral give

$$
\int_0^\infty e^{-u/\tau}\cos(gu)\,du
=\frac\tau{1+g^2\tau^2},\qquad
\int_0^\infty e^{-u/\tau}\sin(gu)\,du
=\frac{g\tau^2}{1+g^2\tau^2}.
$$

The constant-rate [deviatoric stress](../../../continuum-mechanics.md#deviatoric-stress) therefore has components

$$
\boxed{S_{12}=\frac{\mu_1+\mu_0g^2\tau^2}{1+g^2\tau^2}\,g,\qquad
S_{11}=\frac{(\mu_1-\mu_0)g^2\tau}{1+g^2\tau^2},\qquad
S_{22}=-S_{11}.}
$$

The [normal-stress difference](../../../rheology.md#normal-stress-difference) is $2(\mu_1-\mu_0)g^2\tau/(1+g^2\tau^2)$. As checks, the small-rate shear viscosity is $\mu_1$, and $\mu_1=\mu_0$ removes all memory and normal [stresses](../../../continuum-mechanics.md#stress), leaving the Newtonian relation $S=2\mu_0D$.

## 5

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $w=v'-v$ and $D(v)=\operatorname{sym}\nabla v$. The supporting-hyperplane inequality for the convex [viscous dissipation potential](../../../rheology.md#viscous-dissipation-potential) gives

$$
\Omega(D')-\Omega(D)\geq\sigma_{ij}(D'_{ij}-D_{ij}).
$$

The [stress](../../../continuum-mechanics.md#stress) is symmetric because its argument is a symmetric [rate-of-strain tensor](../../../viscous-fluid-flow.md#strain-rate-tensor), so $\sigma_{ij}(D'_{ij}-D_{ij})=\sigma_{ij}w_{i,j}$. Subtracting the two functional values yields

$$
\mathcal F(v')-\mathcal F(v)
\geq\int_{\mathcal D}\sigma_{ij}w_{i,j}\,dx
-\int_{\mathcal D}\rho g_iw_i\,dx
-\int_{S_t}t_i^0w_i\,dS.
$$

[Integration by parts](../../../calculus.md#integration-by-parts) turns the first integral into

$$
\int_{\partial\mathcal D}\sigma_{ij}n_jw_i\,dS
-\int_{\mathcal D}\sigma_{ij,j}w_i\,dx.
$$

Inertialess [force balance](../../../classical-mechanics.md#force-balance) is $\sigma_{ij,j}+\rho g_i=0$. The variation vanishes on $S_v$, and the [traction](../../../continuum-mechanics.md#traction) is $t_i^0$ on $S_t$. Thus both the volume and boundary contributions cancel exactly, proving the [convex viscous potential minimum principle](../../../rheology.md#convex-viscous-potential-minimum-principle)

$$
\boxed{\mathcal F(v')\geq\mathcal F(v)
\quad\text{for every admissible }v'.}
$$

Only convexity, not strict convexity, is required, so no uniqueness follows just from this argument. For [incompressible flow](../../../fluid-mechanics.md#incompressible-flow), admissible trial [velocities](../../../classical-mechanics.md#velocity) must also be divergence free. The [pressure](../../../thermodynamics.md#pressure) term then does no work, because $(-pI):(D'-D)=-p\,\operatorname{div}w=0$; the same proof applies to the deviatoric constitutive law.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For $\dot\gamma=(2D:D)^{1/2}>0$, differentiation in the symmetric [tensor](../../../linear-algebra.md#tensor) space gives $\partial\dot\gamma/\partial D_{ij}=2D_{ij}/\dot\gamma$. Therefore the [Bingham fluid](../../../rheology.md#bingham-plastic) [viscous dissipation potential](../../../rheology.md#viscous-dissipation-potential) gives

$$
\boxed{\sigma'_{ij}
=2\left(\frac{\tau_0}{\dot\gamma}+\mu_0\right)D_{ij}.}
$$

The [deviatoric stress](../../../continuum-mechanics.md#deviatoric-stress) is trace free since $D$ is trace free; an arbitrary [pressure](../../../thermodynamics.md#pressure) reaction completes the [Cauchy stress tensor](../../../continuum-mechanics.md#cauchy-stress-tensor).

At $D=0$ the yield term is not differentiable, and the correct relation is the [subdifferential](../../../convex-optimization.md#subdifferential) condition. A symmetric trace-free [stress](../../../continuum-mechanics.md#stress) $S$ is admissible there if

$$
S:E\leq\tau_0(2E:E)^{1/2}\qquad
\text{for every symmetric trace-free }E.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) shows that this is equivalent to $\|S\|_F\leq\sqrt2\tau_0$; necessity follows by choosing $E$ proportional to $S$. Hence the no-strain-rate restriction is

$$
\boxed{\left(\frac12\sigma'_{ij}\sigma'_{ij}\right)^{1/2}\leq\tau_0.}
$$

The quadratic term has zero derivative at zero and does not change this restriction. This is the unyielded part of the [Bingham plastic](../../../rheology.md#bingham-plastic) law.

For flow along the plates, write $y=x_2$, $v=(u(y),0,0)$ and take $G=-p_{,1}>0$ as the pressure-drop magnitude. The only nonzero [rate-of-strain tensor](../../../viscous-fluid-flow.md#strain-rate-tensor) entries are $D_{12}=D_{21}=u'/2$, so $\dot\gamma=|u'|$ and the yielded [shear stress](../../../viscous-fluid-flow.md#shear-stress) law is

$$
\sigma_{12}=\tau_0\operatorname{sign}u'+\mu_0u'.
$$

[Force balance](../../../classical-mechanics.md#force-balance) gives $G+\sigma_{12,y}=0$. The prescribed odd, continuous shear [stress](../../../continuum-mechanics.md#stress) fixes its integration constant to zero, proving

$$
\boxed{\sigma_{12}(y)=-Gy.}
$$

For $\mu_0>0$ the inverse shear law is

$$
u'(y)=
\begin{cases}
0,&|Gy|\leq\tau_0,\\
(-Gy+\tau_0\operatorname{sign}y)/\mu_0,&|Gy|>\tau_0.
\end{cases}
$$

The original PDF also calls $u$ odd. That assumption is inconsistent with a nonzero flow between identical fixed plates: the inverse shear law makes $u'$ odd, whereas the derivative of an odd $u$ is even. Both can hold only if $u'=0$, and the no-slip wall values then give $u=0$. Thus **with the literal odd-velocity requirement, there is no admissible flowing solution when $Gh>\tau_0$**. The standard pressure-driven [velocity](../../../classical-mechanics.md#velocity) is even; replacing that erroneous parity yields the intended profile below.

If $Gh\leq\tau_0$, the whole gap is unyielded and the fixed no-slip walls force $u=0$. Otherwise let $y_0=\tau_0/G<h$. The [plug flow of a yield-stress fluid](../../../rheology.md#plug-flow-of-a-yield-stress-fluid) occupies $|y|\leq y_0$. In the upper yielded layer $u'=(-Gy+\tau_0)/\mu_0$, and integration from $u(h)=0$ gives

$$
u(y)=\frac G{2\mu_0}\left[(h-y_0)^2-(y-y_0)^2\right]
\qquad(y_0\leq y\leq h).
$$

In the plug the [velocity](../../../classical-mechanics.md#velocity) is the constant $G(h-y_0)^2/(2\mu_0)$, and reflection gives the lower layer. The complete [plane Poiseuille flow of a Bingham fluid](../../../rheology.md#plane-poiseuille-flow-of-a-bingham-fluid) answer is

$$
\boxed{\text{Nonzero flow requires }G>\tau_0/h,\qquad
u(y)=\frac G{2\mu_0}\left[(h-y_0)^2-(|y|-y_0)_+^2\right].}
$$

The profile is continuous with continuous first derivative at the plug boundaries, vanishes at both walls and tends to the ordinary parabolic profile when $\tau_0=0$. If signed [pressure](../../../thermodynamics.md#pressure) gradients of either direction are allowed, the threshold is $|G|h>\tau_0$, and reversing the gradient reverses the [velocity](../../../classical-mechanics.md#velocity).

## 6

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Put $a=\sigma_{13}$, $b=\sigma_{23}$, $w=v_3$, and write $f_a=\partial f/\partial a$, $f_b=\partial f/\partial b$. In [antiplane perfect plasticity](../../../continuum-mechanics.md#antiplane-perfect-plasticity), [force balance](../../../classical-mechanics.md#force-balance) and the fixed [yield surface](../../../rheology.md#yield-surface) give

$$
a_{,1}+b_{,2}=0,\qquad f(a,b)=k.
$$

Differentiate the second relation in $x_2$. Along the proposed [characteristic curve](../../../partial-differential-equation.md#characteristic-curve),

$$
\frac{da}{ds}
=\alpha(-f_ba_{,1}+f_aa_{,2})
=\alpha(f_bb_{,2}+f_aa_{,2})=0.
$$

Similarly, differentiating the yield relation in $x_1$ gives

$$
\frac{db}{ds}
=\alpha(-f_bb_{,1}+f_ab_{,2})
=-\alpha(f_bb_{,1}+f_aa_{,1})=0.
$$

The [associated flow rule](../../../continuum-mechanics.md#associated-flow-rule) and $\dot\epsilon_{i3}=w_{,i}/2$ give $w_{,1}=2\dot\lambda f_a$, $w_{,2}=2\dot\lambda f_b$. Consequently

$$
\frac{dw}{ds}
=2\alpha\dot\lambda(-f_bf_a+f_af_b)=0.
$$

Thus **both shear [stresses](../../../continuum-mechanics.md#stress) and the antiplane [velocity](../../../classical-mechanics.md#velocity) are constant on each characteristic**. Assume a regular yield gradient $(f_a,f_b)\ne0$. Since the [stress](../../../continuum-mechanics.md#stress) is constant on a characteristic, its tangent $(-f_b,f_a)$ has fixed direction, so the curves are straight lines, apart from arbitrary reparameterization by $\alpha$.

In a [centred antiplane plastic fan](../../../continuum-mechanics.md#centred-antiplane-plastic-fan) those lines emanate from the crack tip. Hence

$$
a=a(\phi),\qquad b=b(\phi),\qquad w=w(\phi),
$$

and a radial line at angle $\phi$ from the $x_1$ axis must have

$$
(\cos\phi,\sin\phi)\parallel(-f_b,f_a),\qquad
f_a\cos\phi+f_b\sin\phi=0.
$$

The crack faces have normal in the $x_2$ direction, so traction freedom requires $b=0$ there. The fan joins the adjacent constant crack-face [stress](../../../continuum-mechanics.md#stress) region along the characteristic carrying that [stress](../../../continuum-mechanics.md#stress). Its boundary line therefore satisfies

$$
\boxed{\tan\phi_b=-\frac{f_a}{f_b}\quad\text{at }b=0,}
$$

with the direction interpreted directly when the denominator vanishes. The original PDF reverses this ratio. Its displayed ratio is $dx_1/dx_2$, whereas the tangent of an angle from the $x_1$ axis is $dx_2/dx_1$. The distinction cannot be removed while retaining both its stated characteristic direction and its angle convention.

For the elliptic [yield surface](../../../rheology.md#yield-surface), with $A,B>0$,

$$
f_a=2a/A^2,\qquad f_b=2b/B^2.
$$

On the forward fan $-\pi/2<\phi<\pi/2$, choose the loading branch $b>0$. The radial tangent condition gives $a/A^2=-(b/B^2)\tan\phi$. Substituting in the yield equation and choosing the positive square root gives exactly

$$
\boxed{a=\frac{-A^2\tan\phi}{(B^2+A^2\tan^2\phi)^{1/2}},\qquad
b=\frac{B^2}{(B^2+A^2\tan^2\phi)^{1/2}}.}
$$

For the endpoints, use the equivalent nonsingular expressions

$$
a=-\frac{A^2\sin\phi}{H(\phi)},\qquad
b=\frac{B^2\cos\phi}{H(\phi)},\qquad
H(\phi)=(A^2\sin^2\phi+B^2\cos^2\phi)^{1/2}.
$$

They give $(a,b)=(-A,0)$ on the upper boundary ray and $(A,0)$ on the lower one. The correct boundaries are **$\phi=\pm\pi/2$**, the vertical line through the tip. At either of these [stress](../../../continuum-mechanics.md#stress) states $f_b=0$ and $f_a\ne0$, so the characteristic tangent is vertical. The printed boundary ratio would instead give a horizontal line, providing a concrete counterexample to that intermediate assertion.

Extend the upper and lower rear sectors by the constant [stresses](../../../continuum-mechanics.md#stress) $(-A,0)$ and $(A,0)$ respectively; these satisfy the traction-free crack faces and match the fan [stresses](../../../continuum-mechanics.md#stress) continuously. The reversed loading has all [stresses](../../../continuum-mechanics.md#stress) negated. To check equilibrium within the forward fan, differentiation gives

$$
a_{,\phi}=-\frac{A^2B^2\cos\phi}{H^3},\qquad
b_{,\phi}=-\frac{A^2B^2\sin\phi}{H^3},
$$

and hence $a_{,1}+b_{,2}=(-\sin\phi\,a_{,\phi}+\cos\phi\,b_{,\phi})/r=0$. The yield equation is satisfied identically as well.

<a id="6/image-radial-characteristics-and-vertical-boundaries-of-the-elliptic-antiplane-fan"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-78-plastic-fan.png)

**[Figure 1](#6/image-radial-characteristics-and-vertical-boundaries-of-the-elliptic-antiplane-fan). Radial characteristics and vertical boundaries of the elliptic antiplane fan**.

Finally $\nabla w=w'(\phi)e_\phi/r$, while $(f_a,f_b)=2e_\phi/H$. The [associated flow rule](../../../continuum-mechanics.md#associated-flow-rule) reduces to

$$
\boxed{\dot\lambda=\frac{H(\phi)w'(\phi)}{4r},\qquad w'(\phi)\geq0}
$$

for this [stress](../../../continuum-mechanics.md#stress) branch. Any such angular [velocity](../../../classical-mechanics.md#velocity) field is constant along the rays and has constant values in the adjacent rear sectors. Its magnitude and angular variation require [velocity](../../../classical-mechanics.md#velocity) or loading data beyond the specified traction-free faces; the local [stress](../../../continuum-mechanics.md#stress) fan alone does not determine them.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
