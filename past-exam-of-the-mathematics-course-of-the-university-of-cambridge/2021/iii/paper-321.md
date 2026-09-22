# Paper 321

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_321.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_321.pdf)

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
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)

## 1

↑ **Parent:** [Paper 321](paper-321.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Inside the [innermost stable circular orbit](../../../astrophysics.md#innermost-stable-circular-orbit), nearly circular motion is unstable and gas enters the [plunging region of a black-hole accretion disk](../../../astrophysics.md#plunging-region-of-a-black-hole-accretion-disk). Its inflow time becomes shorter than the time on which internal stress can communicate [angular momentum](../../../classical-mechanics.md#angular-momentum) back to the disk, motivating the [zero-torque inner boundary condition](../../../astrophysics.md#zero-torque-inner-boundary-condition) at $r_{\rm ISCO}$.

In a [steady state](../../../dynamical-systems.md#steady-state), the given diffusion equation implies

$$
r^{1/2}\frac d{dr}\left(r^{1/2}\bar\nu\Sigma\right)=C.
$$

The constant mass supply fixes $C=\dot M/(6\pi)$, and a second integration gives

$$
\bar\nu\Sigma=\frac{\dot M}{3\pi}
\left[1-C_0r^{-1/2}\right].
$$

Zero torque means $\bar\nu\Sigma=0$ at $r=r_{\rm ISCO}$, so $C_0=r_{\rm ISCO}^{1/2}$. Thus the [Keplerian accretion disk](../../../astrophysics.md#keplerian-accretion-disk) relation is

$$
\boxed{\bar\nu\Sigma=\dot M f(r)},
\qquad
\boxed{f(r)=\frac1{3\pi}
\left[1-\left(\frac{r_{\rm ISCO}}r\right)^{1/2}\right]}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Vertical [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) is established by sound waves over the [disk scale height](../../../astrophysics.md#disk-scale-height), so

$$
t_{\rm vert}\sim\frac H{c_s}\sim\Omega^{-1}.
$$

The local heating-cooling balance is established on the thermal time

$$
t_{\rm th}\sim(\alpha\Omega)^{-1}.
$$

The [surface density of a disk](../../../astrophysics.md#surface-density-of-a-disk) evolves only as angular momentum is redistributed, on the viscous time

$$
t_\nu\sim\frac{r^2}{\bar\nu}
\sim\frac1{\alpha\Omega}\left(\frac rH\right)^2.
$$

For a [thin disk](../../../astrophysics.md#thin-disk), $H/r\ll1$, so $t_{\rm vert}\lesssim t_{\rm th}\ll t_\nu$. The vertical and thermal equations can therefore be treated as local equilibria while $\Sigma$ evolves.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Write $K=11a/12$, so $P=KT^4$. With $\rho\sim\Sigma/H$, vertical balance gives

$$
\frac PH\sim\rho\Omega^2H,
\qquad
\boxed{H\sim\frac{KT^4}{\Sigma\Omega^2}}.
$$

At fixed $\Sigma$ and radius, the volumetric viscous heating is

$$
C_+=\frac94\Omega^2\mu
=\frac94\alpha\Omega P\propto T^4.
$$

The neutrino cooling is

$$
C_-=A\rho T^{1/\beta}
\sim A\frac{\Sigma}{H}T^{1/\beta}
\propto T^{1/\beta-4}.
$$

[Thermal stability of an accretion disk](../../../astrophysics.md#thermal-stability-of-an-accretion-disk) requires the cooling rate to have the larger logarithmic temperature slope:

$$
\frac1\beta-4>4.
$$

Since $\beta>0$, the stable range is

$$
\boxed{0<\beta<\frac18}.
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Local thermal equilibrium gives

$$
A\rho T^{1/\beta}
=\frac94\alpha\Omega KT^4,
$$

so

$$
\boxed{\rho=\frac{9\alpha\Omega K}{4A}
T^{4-1/\beta}}.
$$

Substitute this into $dP/dz=-z\Omega^2\rho$ and use $P=KT^4$. The result integrates to

$$
T^{1/\beta}=T_0^{1/\beta}
\left(1-\frac{z^2}{H^2}\right),
$$

with

$$
\boxed{H=\left(\frac{32A\beta T_0^{1/\beta}}
{9\alpha\Omega^3}\right)^{1/2}}.
$$

Therefore, for $|z|\leq H$,

$$
\boxed{T=T_0g^\beta},
\qquad
\boxed{\rho=\rho_0g^{4\beta-1}},
\qquad
\boxed{P=P_0g^{4\beta}},
\qquad
\boxed{g(z/H)=1-\frac{z^2}{H^2}}.
$$

The exponent requested for the temperature is $m=\beta$, and the midplane relations are

$$
\boxed{P_0=KT_0^4=\frac{11}{12}aT_0^4},
\qquad
\boxed{\rho_0=\frac{9\alpha\Omega K}{4A}
T_0^{4-1/\beta}}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For $\beta=1/2$, the exact profiles are

$$
T=T_0(1-x^2)^{1/2},
\qquad
\rho=\rho_0(1-x^2),
\qquad
P=P_0(1-x^2)^2,
\qquad x=\frac zH.
$$

Integration through both disk faces gives

$$
\boxed{\Sigma=\rho_0H\int_{-1}^1(1-x^2)\,dx
=\frac43\rho_0H}.
$$

Since $\mu=\alpha P/\Omega$ and $\bar\nu\Sigma=\int\mu\,dz$,

$$
\boxed{\bar\nu\Sigma
=\frac{\alpha P_0H}{\Omega}
\int_{-1}^1(1-x^2)^2\,dx
=\frac{16}{15}\frac{\alpha P_0H}{\Omega}}.
$$

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

For $\beta=1/2$, part (b) gives

$$
H\propto T_0\Omega^{-3/2},
\qquad
P_0\propto T_0^4,
\qquad
\rho_0\propto\Omega T_0^2.
$$

Parts (a) and (c)(i) imply $P_0H/\Omega\propto\dot M f$. With constant $\dot M$,

$$
T_0^5\Omega^{-5/2}\propto f.
$$

For [Keplerian rotation](../../../astrophysics.md#keplerian-disk), $\Omega\propto r^{-3/2}$, and consequently

$$
\boxed{T_0\propto f^{1/5}r^{-3/4}}.
$$

It follows that

$$
\boxed{H\propto T_0\Omega^{-3/2}
\propto f^{1/5}r^{3/2}},
$$

and

$$
\boxed{\Sigma\propto\rho_0H
\propto\Omega^{-1/2}T_0^3
\propto f^{3/5}r^{-3/2}}.
$$

## 2

↑ **Parent:** [Paper 321](paper-321.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The three terms represent competing physical effects:

- $\Omega^2$ is the stabilizing [epicyclic motion](../../../astrophysics.md#epicyclic-motion) of a radially displaced fluid element in a [Keplerian disk](../../../astrophysics.md#keplerian-disk).
- $-2\pi G\Sigma|k|$ is the destabilizing self-gravity of a surface-density perturbation, obtained from the [razor-thin disk Poisson kernel](../../../astrophysics.md#razor-thin-disk-poisson-kernel).
- $c_s^2k^2$ is the stabilizing pressure response, strongest at short wavelength.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Without self-gravity and for $k>0$,

$$
\omega^2=\Omega^2+c_s^2k^2.
$$

The [phase velocity and group velocity](../../../wave-equation.md#phase-velocity-and-group-velocity) are

$$
c_p=\frac\omega k,
\qquad
c_g=\frac{d\omega}{dk}=\frac{c_s^2k}{\omega},
$$

so

$$
\boxed{c_pc_g=c_s^2}.
$$

With self-gravity restored,

$$
c_g=\frac{c_s^2k-\pi G\Sigma}{\omega},
\qquad
\boxed{c_pc_g=c_s^2-\frac{\pi G\Sigma}{k}}.
$$

The product changes sign at

$$
\boxed{k_{\rm crit}=\frac{\pi G\Sigma}{c_s^2}
=\frac1{QH}}.
$$

For $k>k_{\rm crit}$, crests and a localized [wave packet](../../../wave-equation.md#wave-packet) travel in the same radial direction. For $k<k_{\rm crit}$, the [group velocity](../../../wave-equation.md#group-velocity) and [phase velocity](../../../wave-equation.md#phase-velocity) have opposite signs: the envelope and its wave energy propagate opposite to the individual crests. At $k_{\rm crit}$ the group velocity vanishes and neighboring wave components cause the packet to spread.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Put $x=kH$, with $H=c_s/\Omega$ and $Q=c_s\Omega/(\pi G\Sigma)$. The dispersion relation becomes

$$
\frac{\omega^2}{\Omega^2}=1-\frac{2x}{Q}+x^2.
$$

The two neutral roots are

$$
\boxed{k_{1,2}=\frac1{QH}
\left(1\mp\sqrt{1-Q^2}\right)}.
$$

Real roots enclosing a range with $\omega^2<0$ exist precisely when

$$
\boxed{Q<1},
$$

which is the [Toomre stability criterion](../../../gravitational-instability-of-an-astrophysical-disk.md#toomre-s-stability-criterion) for axisymmetric instability. For $Q\ll1$, the [Taylor expansion](../../../calculus.md#taylor-expansion) of the square root gives

$$
\boxed{k_1\simeq\frac{Q}{2H},
\qquad
k_2\simeq\frac{2}{QH}}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The longest unstable disturbance has mixing length $\ell\sim k_1^{-1}$ and grows on the orbital timescale $\Omega^{-1}$. Its characteristic turbulent velocity is therefore $u_{\rm turb}\sim\Omega\ell$, so the [gravitoturbulent viscosity](../../../gravitational-instability-of-an-astrophysical-disk.md#gravitoturbulent-viscosity) estimate is

$$
\bar\nu\sim u_{\rm turb}\ell
\sim k_1^{-2}\Omega.
$$

For $Q\ll1$,

$$
k_1\sim\frac QH
=\frac{\Omega^2}{\pi G\Sigma},
$$

up to an unimportant numerical factor. Hence

$$
\bar\nu\sim\frac{G^2\Sigma^2}{\Omega^3}
\propto r^{9/2}\Sigma^2
$$

in a [Keplerian disk](../../../astrophysics.md#keplerian-disk).

For a disk of characteristic radius $R$ and mass $M_D$, $\Sigma\sim M_D/R^2$. The [viscous timescale](../../../astrophysics.md#viscous-timescale) is

$$
t_\nu\sim\frac{R^2}{\bar\nu}
\sim\frac{R^6\Omega^3}{G^2M_D^2}.
$$

Using $\Omega^2=GM_*/R^3$ gives

$$
\boxed{t_\nu\sim
\left(\frac{M_*}{M_D}\right)^2\Omega^{-1}}.
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The specific angular momentum of a circular [Keplerian orbit](../../../classical-mechanics.md#kepler-orbit) is $\sqrt{GM_*r}$. Therefore the disk angular momentum is

$$
J=\int_0^R\sqrt{GM_*r}\,\Sigma\,2\pi r\,dr
=\sqrt{GM_*}\,B,
$$

where

$$
\boxed{B=\int_0^Rr^{1/2}\Sigma\,2\pi r\,dr}.
$$

The absence of an external or inner-boundary torque makes $J$, and hence $B$, constant.

From $\bar\nu=Ar^{9/2}\Sigma^2$,

$$
[A]=L^{3/2}M^{-2}T^{-1},
\qquad
[B]=ML^{1/2}.
$$

The combination $AB^2t$ has dimension $L^{5/2}$. [Dimensional analysis](../../../physics.md#dimensional-analysis) therefore gives

$$
\boxed{R\propto(AB^2t)^{2/5}\propto t^{2/5}}.
$$

For the supplied [similarity solution](../../../partial-differential-equation.md#similarity-solution), put $\tau=t/t_0$ and $u=\sqrt{r/R(t)}$. Then $r=Ru^2$ and $dr=2Ru\,du$. The total mass is

$$
\begin{aligned}
M_D
&=2\pi\int_0^R\Sigma r\,dr\\
&=4\pi\Sigma_0R_0^{3/2}\tau^{-2/5}R^{1/2}
\int_0^1(1-u)^{1/2}\,du\\
&=\frac{8\pi}{3}\Sigma_0R_0^{3/2}
\tau^{-2/5}R^{1/2}.
\end{aligned}
$$

Since $R^{1/2}=R_0^{1/2}\tau^{1/5}$,

$$
\boxed{M_D=\frac{8\pi}{3}\Sigma_0R_0^2
\left(\frac t{t_0}\right)^{-1/5}}.
$$

## 3

↑ **Parent:** [Paper 321](paper-321.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For the [Keplerian shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#keplerian-shearing-sheet) velocity $\mathbf U=-(3/2)\Omega x\mathbf e_y$, its material acceleration vanishes because $\mathbf U\cdot\nabla\mathbf U=0$. The $x$ component of the [Coriolis acceleration](../../../physics.md#coriolis-acceleration) is $-3\Omega^2x$, which is cancelled by $-\nabla\Phi_t=+3\Omega^2x\mathbf e_x$ with the signs in the stated equation; constant $P_0$ supplies no force. The flow is also incompressible.

Let $\mathbf u=\mathbf U+\mathbf u'$ and $h'=P'/\rho$. Axisymmetry removes $\mathbf U\cdot\nabla\mathbf u'$, while $\mathbf u'\cdot\nabla\mathbf U=-(3/2)\Omega u_x'\mathbf e_y$. Keeping first-order terms gives

$$
\boxed{\partial_tu_x'=-\partial_xh'+2\Omega u_y'},
\qquad
\boxed{\partial_tu_y'=-\frac12\Omega u_x'},
$$



$$
\boxed{\partial_tu_z'=-\partial_zh'},
\qquad
\boxed{\partial_xu_x'+\partial_zu_z'=0}.
$$

Differentiate the momentum equations in time and use incompressibility to eliminate $h'$. The radial velocity obeys

$$
\boxed{\partial_t^2(\nabla^2u_x')
+\Omega^2\partial_z^2u_x'=0}.
$$

For a plane wave proportional to $e^{i(k_xx+k_zz-\omega t)}$, this gives the [inertial wave](../../../geophysical-fluid-dynamics.md#inertial-wave) dispersion relation

$$
\boxed{\omega^2=\Omega^2
\frac{k_z^2}{k_x^2+k_z^2}}.
$$

When $k_x=0$ and $k_z\ne0$, incompressibility forces $u_z'=0$, and the vertical momentum equation then forces $h'=0$. The remaining motion has $\omega=\pm\Omega$ and satisfies $u_y'=\mp i u_x'/2$: each horizontal layer executes an [epicyclic motion](../../../astrophysics.md#epicyclic-motion), with the phase varying vertically but no pressure or vertical-velocity perturbation.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write the vortex aspect ratio as $\chi$ to distinguish it from cylindrical radius. The [Kida vortex](../../../gravitational-instability-of-an-astrophysical-disk.md#kida-vortex) core flow is

$$
u_x=\frac{3\Omega}{2\chi(\chi-1)}y,
\qquad
u_y=-\frac{3\Omega\chi}{2(\chi-1)}x.
$$

As $\chi\to\infty$, $u_x\to0$ and $u_y\to-(3/2)\Omega x$, recovering [Keplerian shear](../../../planetary-science.md#keplerian-shear).

For a fluid particle,

$$
\ddot x=-\left[\frac{3\Omega}{2(\chi-1)}\right]^2x.
$$

It therefore circulates around an ellipse with angular frequency $3\Omega/[2(\chi-1)]$ and period

$$
\boxed{T_{\rm vort}=\frac{4\pi(\chi-1)}{3\Omega}}.
$$

For a perturbation depending only on $z,t$, horizontal pressure gradients vanish. Linearization gives

$$
\boxed{\partial_tu_x'
=\Omega\left[2-\frac{3}{2\chi(\chi-1)}\right]u_y'},
$$



$$
\boxed{\partial_tu_y'
=-\Omega\left[2-\frac{3\chi}{2(\chi-1)}\right]u_x'}.
$$

Taking $\mathbf u'\propto e^{-i\omega t}$ yields

$$
\boxed{\omega^2=\Omega^2
\left[2-\frac{3}{2\chi(\chi-1)}\right]
\left[2-\frac{3\chi}{2(\chi-1)}\right]}.
$$

The first bracket is positive for $\chi>3/2$, while the second is negative for $1<\chi<4$. Their product is therefore negative, so $\omega$ is imaginary and the mode grows precisely when

$$
\boxed{\frac32<\chi<4}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
