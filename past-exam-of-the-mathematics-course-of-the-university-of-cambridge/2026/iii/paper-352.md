# Paper 352

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20352.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20352.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
    - [v](#1/b/v)
      - [Solution](#1/b/v/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)

## 1

↑ **Parent:** [Paper 352](paper-352.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $z\in[0,h]$ measure distance through the thin [Bingham plastic](../../../rheology.md#bingham-plastic) layer, with a stationary wall at $z=0$ and large-scale velocity $u_b$ at $z=h$. To leading lubrication order the shear stress $\tau_b$ is uniform across the layer. If $|\tau_b|\leq\tau_c$, the material is unyielded and the no-slip wall makes the entire layer stationary. After yield,

$$
\frac{du}{dz}=\frac1\mu
\left(\tau_b-\tau_c\operatorname{sgn}\tau_b\right).
$$

Integrating across the depth gives the [Bingham sliding law](../../../rheology.md#bingham-sliding-law)

$$
\boxed{u_b=\frac h\mu
\left(|\tau_b|-\tau_c\right)_+
\operatorname{sgn}\tau_b}.
$$

Equivalently, for nonzero sliding,

$$
\boxed{\tau_b=\tau_c\operatorname{sgn}u_b+\frac\mu h u_b}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Write $\tau_d=\rho gH\sin\theta$. For unidirectional velocity $\mathbf u=(u(y,z),0,0)$, the nontrivial force balances are

$$
\frac{\partial\tau_{xy}}{\partial y}
+\frac{\partial\tau_{xz}}{\partial z}
+\rho g\sin\theta=0,
\qquad
\frac{\partial p}{\partial y}=0,
\qquad
\frac{\partial p}{\partial z}=-\rho g\cos\theta.
$$

For the [power-law fluid](../../../rheology.md#power-law-fluid),

$$
\tau_{xy}=K|\dot\gamma|^{n-1}u_y,
\qquad
\tau_{xz}=K|\dot\gamma|^{n-1}u_z,
\qquad
|\dot\gamma|=(u_y^2+u_z^2)^{1/2}.
$$

At the free surface $z=H$, $p=p_{\rm atm}$ and $\tau_{xz}=0$. At the bed $z=0$, continuity of tangential velocity and traction gives the local sliding condition

$$
u(y,0)=\frac h\mu[\tau_b(y)-\tau_c(y)],
\qquad
\tau_b(y)=\tau_{xz}(y,0),
$$

because the stated inequalities keep the downhill bed yielded. The velocity and horizontal shear traction are continuous across $y=0$, and the flow tends to uniform states as $y\to\pm\infty$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

When horizontal shear dominates, $u=U(y)+O(\epsilon)$ and

$$
\tau_{xy}=K|U'|^{n-1}U'+O(\epsilon).
$$

Integrating downhill momentum through $0<z<H$ gives

$$
\tau_b=\tau_d+HK\frac d{dy}
\left(|U'|^{n-1}U'\right).
$$

The [Bingham sliding law](../../../rheology.md#bingham-sliding-law) then yields the ODE

$$
\boxed{HK\frac d{dy}\left(|U'|^{n-1}U'\right)
-\frac\mu hU+\tau_d-\tau_c(y)=0}.
$$

Define

$$
U_-:=\frac h\mu(\tau_d-\tau_1),
\qquad
U_+:=\frac h\mu(\tau_d-\tau_2).
$$

Then

$$
\boxed{U(-\infty)=U_->U_+=U(+\infty)}.
$$

The speed decreases monotonically across the material transition, with a smooth margin layer centered at $y=0$.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

In either half-plane, let $U_\infty$ denote its far-field value. Multiplying the ODE by $U'$ and integrating from the far field gives

$$
HK\frac n{n+1}|U'|^{n+1}
=\frac\mu{2h}(U-U_\infty)^2.
$$

Since the profile decreases,

$$
\boxed{U'=-A|U-U_\infty|^{2/(n+1)}},
\qquad
A=\left[\frac{\mu(n+1)}{2hHKn}\right]^{1/(n+1)}.
$$

Continuity of $U'$ at $y=0$ gives

$$
U(0)=U_0=\frac{U_-+U_+}{2}.
$$

For $n=1$, let $\ell=A^{-1}=\sqrt{hHK/\mu}$ and $\Delta U=U_--U_+$. Then

$$
\boxed{
U(y)=
\begin{cases}
U_--\dfrac{\Delta U}{2}e^{y/\ell},&y<0,\\
U_++\dfrac{\Delta U}{2}e^{-y/\ell},&y>0.
\end{cases}}
$$

The Newtonian disturbance therefore has exponential tails.

For $n<1$ and $y>0$, put $W=U-U_+$. Integration gives

$$
\boxed{U(y)=U_++
\left[
(U_0-U_+)^{-(1-n)/(n+1)}
+\frac{1-n}{n+1}Ay
\right]^{-(n+1)/(1-n)}}.
$$

The corresponding expression on $y<0$ follows by reflection about $(0,U_0)$. A [shear thinning](../../../rheology.md#shear-thinning) power-law material has algebraic rather than exponential margin tails. Measurements of how rapidly an ice-stream speed approaches its far-field values could therefore distinguish an approximately Newtonian rheology from power-law shear thinning and estimate $n$.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

If $\delta$ is the cross-stream transition width and $\Delta U$ its speed change, dominant horizontal shear requires

$$
\frac{\Delta U}{\delta}\gg |u_z|.
$$

Balancing the two terms in the reduced ODE gives the scale

$$
\delta^{n+1}\sim\frac{HKh}{\mu}(\Delta U)^{n-1}.
$$

The approximation is strongest in the margin where $U'$ is large, for a thin basal layer $h\ll H$ and parameters making this lateral scale short compared with the scale on which vertical shear changes the plug velocity. It fails sufficiently far into either uniform region because $U'\to0$ while the $O(\epsilon)$ vertical shear needed to transmit the driving stress remains. It can also fail in narrow neighborhoods where neglected free-surface, bed-transition, or three-dimensional effects vary on the same scale.

<h4 id="1/b/v">v</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/v/solution">Solution</h5>

↑ **Parent:** [V](#1/b/v)

For $n>1$, the exponent $m=2/(n+1)$ in $U'=-A|U-U_\infty|^m$ is below one. Its integral reaches $U=U_\infty$ at a finite distance, after which the constant far-field solution can be attached. The ideal power law therefore predicts a compactly supported transition with finite-width edges rather than the algebraic tails found for $n<1$. Near those edges horizontal shear vanishes and the neglected vertical or regularizing physics becomes important, so the sharp termination should not be interpreted literally.

## 2

↑ **Parent:** [Paper 352](paper-352.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A plain [material derivative](../../../continuum-mechanics.md#material-derivative) of the [conformation tensor](../../../rheology.md#conformation-tensor) is not an [objective time derivative](../../../rheology.md#objective-time-derivative): an observer undergoing a time-dependent rigid rotation would infer a different constitutive response, and even rigid-body rotation could appear to change polymer deformation. The [upper-convected derivative](../../../rheology.md#upper-convected-derivative) subtracts deformation and rotation carried by the velocity gradient and is frame indifferent.

The [Oldroyd-B model](../../../rheology.md#oldroyd-b-model) is often inadequate because its Hookean dumbbells are infinitely extensible. It predicts constant shear viscosity rather than shear thinning, zero second [normal-stress difference](../../../rheology.md#normal-stress-difference), and an unbounded extensional viscosity at a finite extension rate. Real polymer chains have finite extensibility and commonly exhibit shear thinning, bounded extensional stress, multiple relaxation times, and nonlinear solvent or concentration effects.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let $a=\lambda\dot\gamma$. For simple shear, the steady conformation equation is

$$
F\mathbf C-\mathbf I
=\lambda[(\nabla\mathbf u)\mathbf C
+\mathbf C(\nabla\mathbf u)^T].
$$

Its nonzero components are

$$
C_{yy}=C_{zz}=\frac1F,
\qquad
C_{xy}=\frac a{F^2},
\qquad
C_{xx}=\frac1F+\frac{2a^2}{F^3}.
$$

Since $\boldsymbol\tau=\eta_s\dot{\boldsymbol\gamma}+(\eta_p/\lambda)(F\mathbf C-\mathbf I)$,

$$
\boxed{\tau_{xy}=\left(\eta_s+\frac{\eta_p}{F}\right)\dot\gamma},
$$



$$
\boxed{\tau_{xx}=\frac{2\eta_p\lambda\dot\gamma^2}{F^2}},
\qquad
\tau_{yy}=\tau_{zz}=0.
$$

Thus the [FENE-P model](../../../rheology.md#fene-p-model) has

$$
\boxed{N_1=\frac{2\eta_p\lambda\dot\gamma^2}{F^2}>0,
\qquad N_2=0}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The trace is

$$
T=\frac3F+\frac{2a^2}{F^3}.
$$

Substituting it into $F=(L^2-3)/(L^2-T)$ gives

$$
\boxed{F^2(F-1)=\beta},
\qquad
\boxed{\beta=\frac{2\lambda^2\dot\gamma^2}{L^2}}.
$$

For $\beta\ll1$, $F=1+\beta+O(\beta^2)$. For $\beta\gg1$, $F\sim\beta^{1/3}$. The effective shear viscosity is therefore

$$
\eta_{\rm eff}=\eta_s+\frac{\eta_p}{F}
\sim
\begin{cases}
\eta_s+\eta_p,&\lambda|\dot\gamma|\ll L,\\
\eta_s+\eta_p
\left(\dfrac{L^2}{2\lambda^2\dot\gamma^2}\right)^{1/3},
&\lambda|\dot\gamma|\gg L.
\end{cases}
$$

The FENE-P curve decreases from $\eta_s+\eta_p$ toward the solvent plateau $\eta_s$, displaying [shear thinning](../../../rheology.md#shear-thinning). Oldroyd-B has $F=1$ and remains at the constant value $\eta_s+\eta_p$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

For uniaxial extension,

$$
\mathbf u=\left(-\frac{\dot\epsilon x}{2},
-\frac{\dot\epsilon y}{2},\dot\epsilon z\right),
\qquad a=\lambda\dot\epsilon.
$$

The diagonal steady conformation tensor is

$$
\boxed{C_{xx}=C_{yy}=\frac1{F+a},
\qquad C_{zz}=\frac1{F-2a}},
$$

where physical solutions require $F>2a$. The [extensional viscosity](../../../rheology.md#extensional-viscosity) is

$$
\boxed{\eta_{\rm ext}
=\frac{\tau_{zz}-\tau_{xx}}{\dot\epsilon}
=3\eta_s+\eta_p\left[
\frac2{F-2a}+\frac1{F+a}
\right]}.
$$

The implicit closure is

$$
\boxed{T=\frac2{F+a}+\frac1{F-2a},
\qquad
F=\frac{L^2-3}{L^2-T}}.
$$

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

As $\dot\epsilon\to0$, $a\to0$, $F\to1$, and

$$
\boxed{\eta_{\rm ext}(0)=3(\eta_s+\eta_p)}.
$$

The [Trouton ratio](../../../rheology.md#trouton-ratio) is therefore three. This is also the small-rate Oldroyd-B result because finite extensibility is irrelevant while polymer deformation remains small.

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

For FENE-P at $a\gg1$, write $F=2a+\delta$. The trace constraint approaches the finite maximum $T\to L^2$, so $C_{zz}=1/\delta\to L^2$ and $\delta\to L^{-2}$ to leading order. Hence

$$
\boxed{\eta_{\rm ext}\longrightarrow
3\eta_s+2\eta_pL^2}
$$

up to corrections that vanish as $a^{-1}$. Its extensional viscosity rises from the Newtonian plateau and saturates at a finite-extensibility plateau.

For Oldroyd-B, $F=1$ and

$$
\eta_{\rm ext}^{\rm OB}
=3\eta_s+\eta_p\left[
\frac2{1-2\lambda\dot\epsilon}
+\frac1{1+\lambda\dot\epsilon}
\right].
$$

It diverges as $\lambda\dot\epsilon\uparrow1/2$ and has no physical steady homogeneous branch beyond that point. This extensional catastrophe is removed by finite chain extensibility.

## 3

↑ **Parent:** [Paper 352](paper-352.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Define the [viscous number](../../../rheology.md#viscous-number)

$$
I_v=\frac{\eta|\dot\gamma|}{p_s}.
$$

The pressure relation gives

$$
\frac\phi{\phi_m-\phi}=I_v^{-1/2},
\qquad
\boxed{\phi=\frac{\phi_m}{1+\sqrt{I_v}}}.
$$

Using $\eta\widehat\mu\phi^2|\dot\gamma|/(\phi_m-\phi)^2=\widehat\mu p_s$, the shear stress at imposed pressure is

$$
\boxed{\tau=\eta\dot\gamma
+\widehat\mu p_s\operatorname{sgn}\dot\gamma}.
$$

The material therefore behaves as a pressure-dependent [Bingham plastic](../../../rheology.md#bingham-plastic) with yield stress $\widehat\mu p_s$, while its steady concentration dilates as shear rate increases.

After a step in shear rate, the particles must rearrange and undergo [shear-induced dilation](../../../rheology.md#shear-induced-dilation) or compaction. Because the sample is saturated, that volume change requires pore fluid to migrate through the packing, so pore pressure and effective particle pressure relax over a finite poro-viscous time. Measuring the transient stress can therefore constrain the permeability, and with an independently known permeability can constrain the suspension's compressibility or dilatancy law.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Let

$$
G=\frac{\Delta P}{L}>0.
$$

Axial momentum balance gives shear-stress magnitude $|\tau_{rz}|=Gr/2$. The wall stress must exceed the pressure-dependent yield stress, so motion requires

$$
\boxed{\Delta P>\Delta P_{\min}
=\frac{2L\widehat\mu p_s}{R}}.
$$

When this holds, define the plug radius

$$
a=\frac{2\widehat\mu p_s}{G}<R.
$$

The no-slip solid velocity is

$$
\boxed{
w_s(r)=
\begin{cases}
\dfrac{G}{4\eta}(R-a)^2,&0\leq r\leq a,\\[4pt]
\dfrac{G}{4\eta}(R^2-r^2)
-\dfrac{\widehat\mu p_s}{\eta}(R-r),&a<r\leq R.
\end{cases}}
$$

In the sheared annulus,

$$
|w_s'|=\frac{G(r-a)}{2\eta},
\qquad
I_v=\frac{G(r-a)}{2p_s},
$$

so

$$
\boxed{
\phi(r)=
\begin{cases}
\phi_m,&0\leq r\leq a,\\[2pt]
\dfrac{\phi_m}{1+\sqrt{G(r-a)/(2p_s)}},&a<r\leq R.
\end{cases}}
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The volume flux carried with the particle skeleton is

$$
Q_0=2\pi\int_0^Rw_s(r)r\,dr
=\boxed{\frac{\pi G(R-a)^2(3R^2+2Ra+a^2)}{24\eta}}.
$$

By [Darcy law](../../../porous-media-flow.md#darcy-law), the fluid moves relative to the solids at $kG/\eta$. The total mixture-volume flux is therefore

$$
\boxed{Q_T=Q_0+
\frac{2\pi kG}{\eta}
\int_0^R[1-\phi(r)]r\,dr}.
$$

This is explicit because $\phi(r)$ is given above. For example, if

$$
c=\frac{G}{2p_s},
\qquad
T=\sqrt{c(R-a)},
$$

then

$$
\int_0^R\phi r\,dr
=\phi_m\left\{
\frac{a^2}{2}
+\frac{2a}{c}[T-\log(1+T)]
+\frac{2}{c^2}
\left[\frac{T^3}{3}-\frac{T^2}{2}+T-\log(1+T)\right]
\right\}.
$$

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

At fixed $G=\Delta P/L$, increasing $p_s$ increases the plug radius and lowers both the particle velocity and porosity. The total flux decreases from a nearly particle-free Poiseuille value toward a nonzero Darcy seepage flux through a jammed packing. Particles stop when $a=R$, namely at

$$
\boxed{p_s^*=\frac{GR}{2\widehat\mu}
=\frac{\Delta P\,R}{2\widehat\mu L}}.
$$

Put $\delta=1-p_s/p_s^*=1-a/R$. As $\delta\downarrow0$, almost the whole cross-section is a plug at concentration $\phi_m$ and speed $G(R-a)^2/(4\eta)$. The particle flux is therefore

$$
\boxed{Q_p\sim
\frac{\pi\phi_mGR^4}{4\eta}
\left(1-\frac{p_s}{p_s^*}\right)^2}.
$$

The jammed seepage flux is approximately

$$
Q_{\rm seep}^*=\frac{\pi R^2kG}{\eta}(1-\phi_m).
$$

It appreciably changes the total flux when $Q_p\lesssim Q_{\rm seep}^*$, or

$$
\boxed{1-\frac{p_s}{p_s^*}
\lesssim2\sqrt{\frac{1-\phi_m}{\phi_m}}
\frac{\sqrt k}{R}}.
$$

Because $k\ll R^2$, seepage matters principally in a narrow pressure interval just below jamming.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/b/iv)

At fixed $Q_T$, the pressure gradient is no longer fixed. As $p_s\to0$, the constitutive law gives a dilute particle fraction and hence $Q_p\to0$. Raising $p_s$ first adds particles and increases their flux. At high $p_s$, the packing becomes dense and nearly jammed; maintaining $Q_T$ then requires a large pressure gradient that sends most of the liquid through the packing by Darcy seepage, while $Q_p$ falls back toward zero. Thus $Q_p(p_s)$ has an interior maximum, and every particle flux below that maximum occurs at two solid pressures.

On the low-$p_s$ branch the suspension is dilute, shear is distributed broadly, particle motion carries much of the total volume, and the required $\Delta P$ is relatively small. On the high-$p_s$ branch the suspension contains a large nearly jammed plug, particles move slowly, seepage carries a substantial fraction of $Q_T$, and a much larger $\Delta P$ is required. Equal particle flux therefore does not imply equal concentration, flow structure, or pumping cost.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
