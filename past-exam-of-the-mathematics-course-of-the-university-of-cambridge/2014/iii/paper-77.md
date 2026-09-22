# Paper 77

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_77.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_77.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
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
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
  - [g](#3/g)
    - [Solution](#3/g/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Choose positive tilt towards $+x$, so the rod tangent is $\mathbf t=(\sin\theta,\cos\theta)$ and its normal is $\mathbf n=(\cos\theta,-\sin\theta)$. The opposite angular convention reverses the signed phase optimum later. In [resistive-force theory](../../../mathematical-biology.md#resistive-force-theory), a point with centred arclength $s\in[-L/2,L/2]$ has [velocity](../../../classical-mechanics.md#velocity) $\mathbf u=\dot x\mathbf e_x+s\dot\theta\mathbf n$, and its [force](../../../classical-mechanics.md#force) on the fluid is $\mathbf D\mathbf u$, where $\mathbf D=c_\perp\mathbf I+(c_\parallel-c_\perp)\mathbf t\mathbf t$. The [force](../../../classical-mechanics.md#force) on the rod has the opposite sign.

The pure centred rotational contribution is odd in $s$ and therefore gives zero net [force](../../../classical-mechanics.md#force) instantaneously in either direction. In the combined [oscillating rigid rod in resistive-force theory](../../../mathematical-biology.md#oscillating-rigid-rod-in-resistive-force-theory), however, orientation modulates the translational [force](../../../classical-mechanics.md#force). After half a period, $\dot x\mapsto-\dot x$ and $\theta\mapsto-\theta$. Reflection in the $y$ axis takes one configuration and its forcing into the other. A [force](../../../classical-mechanics.md#force) component in $x$ reverses under this reflection, whereas a component in $y$ does not. Explicitly,

$$
F_x=L[c_\perp+(c_\parallel-c_\perp)\sin^2\theta]\dot x,\qquad
F_y=L(c_\parallel-c_\perp)\sin\theta\cos\theta\,\dot x.
$$

The first is half-period antisymmetric and the second is half-period symmetric. Hence **$\langle F_x\rangle=0$, while symmetry permits $\langle F_y\rangle\ne0$**. The possible mean $y$ [force](../../../classical-mechanics.md#force) comes from the coupled translation and rotation, not from pure centred rotation alone.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In the [oscillating rigid rod in resistive-force theory](../../../mathematical-biology.md#oscillating-rigid-rod-in-resistive-force-theory), $\sin\theta\cos\theta=\theta+O(\epsilon^3)$ and $\dot x=-\epsilon a\omega\sin\omega t$. Since

$$
\langle\theta\dot x\rangle=-\epsilon^2a\omega\langle\cos(\omega t+\phi)\sin\omega t\rangle
=\frac{\epsilon^2a\omega}{2}\sin\phi,
$$

the [mean transverse force from a rocking rod](../../../mathematical-biology.md#mean-transverse-force-from-a-rocking-rod), on the fluid in the tilt convention of part (a), is

$$
\boxed{\langle F_y\rangle=-\frac12(c_\perp-c_\parallel)L\epsilon^2a\omega\sin\phi+O(\epsilon^4).}
$$

The [parallel and perpendicular drag coefficients of a slender filament](../../../mathematical-biology.md#parallel-and-perpendicular-drag-coefficients-of-a-slender-filament) are per unit length here. Their difference is essential: isotropic local drag gives zero transverse [force](../../../classical-mechanics.md#force). The hydrodynamic [force](../../../classical-mechanics.md#force) on the rod is the negative of the displayed answer.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For the usual anisotropy $c_\perp>c_\parallel$ and $a>0$, the maximum positive [mean transverse force from a rocking rod](../../../mathematical-biology.md#mean-transverse-force-from-a-rocking-rod) occurs at

$$
\boxed{\phi=-\pi/2\pmod{2\pi},\qquad
\langle F_y\rangle_{\max}=\tfrac12(c_\perp-c_\parallel)L\epsilon^2a\omega.}
$$

The maximum magnitude has either quadrature phase $\phi=\pm\pi/2$. If positive tilt is defined towards $-x$, the positive-[force](../../../classical-mechanics.md#force) optimum is instead $+\pi/2$. At our optimum $\theta=\epsilon\sin\omega t$ is opposite in sign to $\dot x$: the rod tilts so that the weaker tangential drag and stronger normal drag combine into a positive $y$ [force](../../../classical-mechanics.md#force) on both strokes.

For $\phi=0$ or $\pi$, orientation is a single-valued function of the centre displacement. The configuration retraces its path under time reversal, and [kinematic reversibility of Stokes flow](../../../stokes-flow.md#kinematic-reversibility-of-stokes-flow) makes the [force](../../../classical-mechanics.md#force) impulse cancel. Equivalently, $\langle\theta\dot x\rangle=0$. The enclosed loop in the displacement-orientation plane is largest in quadrature and vanishes for a reciprocal stroke, illustrating the principle behind the [scallop theorem](../../../stokes-flow.md#scallop-theorem).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The instantaneous work on the fluid equals the integral of $\mathbf u\cdot\mathbf D\mathbf u$. For the [oscillating rigid rod in resistive-force theory](../../../mathematical-biology.md#oscillating-rigid-rod-in-resistive-force-theory), $\mathbf u\cdot\mathbf t=\dot x\sin\theta$ and $\mathbf u\cdot\mathbf n=\dot x\cos\theta+s\dot\theta$. Odd terms in $s$ integrate to zero, giving

$$
P=L[c_\parallel\sin^2\theta+c_\perp\cos^2\theta]\dot x^2
+\frac{c_\perp L^3}{12}\dot\theta^2.
$$

Thus the leading [power of a rocking rod](../../../mathematical-biology.md#power-of-a-rocking-rod) is

$$
\boxed{\langle P\rangle=\frac12c_\perp\epsilon^2\omega^2
\left(La^2+\frac{L^3}{12}\right)+O(\epsilon^4).}
$$

Both terms are quadratic in $\epsilon$. Small angle does not make rotation a higher-order contribution: points away from the centre have rotational speed $s\dot\theta=O(\epsilon\omega L)$, just as the translational speed is $O(\epsilon\omega a)$. Their ratio is $L^2/(12a^2)$, controlled by geometry rather than by $\epsilon$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Use the printed [Maxwell-filtered local drag](../../../rheology.md#maxwell-filtered-local-drag) law at fixed material arclength, after transients have decayed to a periodic response. Averaging the [force](../../../classical-mechanics.md#force) equation over a period makes the time-derivative term vanish. Therefore the mean [force](../../../classical-mechanics.md#force) equals the mean instantaneous [resistive-force theory](../../../mathematical-biology.md#resistive-force-theory) driving [force](../../../classical-mechanics.md#force), even though its oscillating part is filtered. In particular,

$$
\boxed{\langle F_y\rangle=-\tfrac12(c_\perp-c_\parallel)L\epsilon^2a\omega\sin\phi+O(\epsilon^4),}
$$

with the same sign convention as before.

At first order the tangent is $\mathbf e_y$ and both [velocity](../../../classical-mechanics.md#velocity) components are single harmonics of frequency $\omega$. The [linear Maxwell fluid](../../../rheology.md#linear-maxwell-fluid) response multiplies their complex [force](../../../classical-mechanics.md#force) amplitudes by $(1+i\omega\lambda)^{-1}$. Only its in-phase real part contributes to the mean work. Consequently

$$
\boxed{\langle P\rangle_{\mathrm M}=\frac{c_\perp\epsilon^2\omega^2}{2[1+(\omega\lambda)^2]}
\left(La^2+\frac{L^3}{12}\right)+O(\epsilon^4).}
$$

The leading power is strictly smaller when $\lambda>0$ and $\omega>0$, and equal in the Newtonian limit. The zero-frequency component generating the mean [force](../../../classical-mechanics.md#force) is unattenuated, whereas elastic storage and phase lag reduce the dissipative harmonic response. This conclusion concerns the specified linear local [force](../../../classical-mechanics.md#force) law and prescribed kinematics; it is not a claim for every nonlinear viscoelastic constitutive model.

## 2

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The Laplacian and the added drag term in the [Brinkman equation](../../../stokes-flow.md#brinkman-equation) must have the same dimensions. Therefore

$$
\boxed{[\alpha]=\mathrm{length}^{-1}.}
$$

The length $\alpha^{-1}$ is a hydrodynamic screening length. When the viscous coefficients are identical in the two terms, the corresponding permeability is $\alpha^{-2}$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Scale time by $\omega^{-1}$, length by $k^{-1}$, [velocity](../../../classical-mechanics.md#velocity) by $\omega/k$, [pressure](../../../thermodynamics.md#pressure) by $\mu\omega$, and [streamfunction](../../../fluid-mechanics.md#stream-function) by $\omega/k^2$. Write $A=\alpha/k$, $\xi=x-t$, and drop stars from dimensionless coordinates. The surface is $y=\epsilon\sin\xi$ and its material [velocity](../../../classical-mechanics.md#velocity) in the sheet frame is $(0,-\epsilon\cos\xi)$. The [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) is therefore

$$
\mathbf u(x,\epsilon\sin\xi,t)=(0,-\epsilon\cos\xi),\qquad
\mathbf u\longrightarrow\mathcal U\mathbf e_x\quad(y\to+\infty),\qquad
\mathcal U=kU/\omega.
$$

The stationary matrix identifies a preferred frame. In the sheet frame it translates with $\mathcal U\mathbf e_x$, so [matrix-relative Brinkman velocity](../../../stokes-flow.md#matrix-relative-brinkman-velocity) gives the consistent equations

$$
\boxed{-\nabla p+\nabla^2\mathbf u=A^2(\mathbf u-\mathcal U\mathbf e_x),\qquad
\nabla\cdot\mathbf u=0.}
$$

Equivalently one may keep the printed right-hand side $A^2\mathbf u$ after defining $\widetilde p=p-A^2\mathcal U x$; then the far-field [pressure](../../../thermodynamics.md#pressure) has the gradient needed to balance that term. Using the printed equation with a uniform far-field flow and no such adjustment is inconsistent. The distinction first matters at second order, since the first-order swimming speed is zero. We solve the upper half-space; the lower half-space is its reflected counterpart.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Taking the curl of the [Brinkman equation](../../../stokes-flow.md#brinkman-equation) eliminates [pressure](../../../thermodynamics.md#pressure) and the constant matrix [velocity](../../../classical-mechanics.md#velocity). With $\mathbf u=(\psi_y,-\psi_x)$ and [vorticity](../../../fluid-mechanics.md#vorticity) $-\nabla^2\psi$, the [Brinkman swimming sheet](../../../stokes-flow.md#brinkman-swimming-sheet) equation is

$$
\boxed{(\nabla^2-A^2)\nabla^2\psi=0.}
$$

The surface conditions are conditions on partial derivatives evaluated on the moving boundary:

$$
\boxed{\psi_y(x,\epsilon\sin\xi,t)=0,\qquad
\psi_x(x,\epsilon\sin\xi,t)=\epsilon\cos\xi.}
$$

At infinity, $\psi_y\to\mathcal U$ and $\psi_x\to0$. The derivative of $\psi$ along the surface also equals $\epsilon\cos\xi$, because $\psi_y=0$ there, so a convenient gauge has $\psi(x,\epsilon\sin\xi,t)=\epsilon\sin\xi$. Decaying perturbations and the [force-free](../../../stokes-flow.md#force-free) condition determine the swimming solution.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Expand $\psi=\epsilon\psi_1+\epsilon^2\psi_2+\cdots$ and $\mathcal U=\epsilon^2\mathcal U_2+\cdots$. The [screened first-order transverse sheet flow](../../../stokes-flow.md#screened-first-order-transverse-sheet-flow) has $\psi_1=f(y)\sin\xi$. Set $s=\sqrt{1+A^2}$. The two decaying roots of the [Brinkman swimming sheet](../../../stokes-flow.md#brinkman-swimming-sheet) operator are $1$ and $s$, and $f(0)=1$, $f'(0)=0$ select

$$
\boxed{f(y)=\frac{s e^{-y}-e^{-sy}}{s-1},\qquad
\mathbf u_1=(f'(y)\sin\xi,-f(y)\cos\xi).}
$$

The physical first-order flow is $\epsilon(\omega/k)\mathbf u_1$ in scaled coordinates. The dimensionless first-order [pressure](../../../thermodynamics.md#pressure), determined from momentum balance, is

$$
\boxed{p_1=-s(s+1)e^{-y}\cos\xi.}
$$

Although the expression for $f$ appears singular at $A=0$, its continuous limit is $f=(1+y)e^{-y}$, the ordinary [transverse mode of a Taylor swimming sheet](../../../stokes-flow.md#transverse-mode-of-a-taylor-swimming-sheet).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

A [Taylor expansion](../../../calculus.md#taylor-expansion) of the tangential [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) gives $u_{2x}(0)=-\sin\xi\,\partial_yu_{1x}(0)$. Since $f''(0)=-s$,

$$
\langle u_{2x}(0)\rangle=s\langle\sin^2\xi\rangle=s/2.
$$

For [matrix-relative Brinkman velocity](../../../stokes-flow.md#matrix-relative-brinkman-velocity), the mean second-order tangential flow is

$$
\overline u_{2x}(y)=\mathcal U_2+C e^{-Ay}.
$$

The mean tangential traction has no first-order geometric remainder: at the surface $\partial_y\sigma_{xy,1}=s(s+1)\sin\xi$ and $\sigma_{xx,1}=s(s+1)\cos\xi$, so the mean displaced-boundary and tilted-normal corrections cancel. Thus the [force-free](../../../stokes-flow.md#force-free) condition gives $\overline u_{2x}'(0)=0$, hence $C=0$. In the $A=0$ limit boundedness likewise excludes mean shear. The [swimming speed of a Brinkman sheet](../../../stokes-flow.md#swimming-speed-of-a-brinkman-sheet) is therefore

$$
\boxed{\mathcal U=\frac{\epsilon^2}{2}\sqrt{1+A^2}+O(\epsilon^4),\qquad
U=\frac{b^2k\omega}{2}\sqrt{1+(\alpha/k)^2}+O\!\left(\frac\omega k\epsilon^4\right).}
$$

It is larger than the simple-fluid speed by $\sqrt{1+(α/k)^2}$ for fixed waveform and frequency. The matrix offers a reaction structure for the transverse stroke and more strongly confines the induced motion; it acts as a footing against which the wave pushes. This is a prescribed-stroke comparison, not a guarantee at fixed motor power. The small-amplitude expansion is at fixed $A$; a large-$A$ use also needs $\epsilon s\ll1$ to control variation across the displaced boundary.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

At the undeformed boundary, the [screened first-order transverse sheet flow](../../../stokes-flow.md#screened-first-order-transverse-sheet-flow) has $v_1=-\cos\xi$ and $\partial_yv_1=-f'(0)\cos\xi=0$. Hence the normal stress is $\sigma_{yy,1}=-p_1=s(s+1)\cos\xi$. The sheet does work on the upper fluid at rate $-\langle\mathbf u_S\cdot\boldsymbol\sigma\mathbf n\rangle$, where $\mathbf n$ points from the sheet into that fluid. To second order only the first-order normal [velocity](../../../classical-mechanics.md#velocity) and stress are needed. The [power of a Brinkman sheet](../../../stokes-flow.md#power-of-a-brinkman-sheet) per projected area on one side is

$$
\boxed{\overline P_+=\mu b^2k\omega^2\frac{s(s+1)}2
+O\!\left(\frac{\mu\omega^2}{k}\epsilon^4\right),\qquad
s=\sqrt{1+(\alpha/k)^2}.}
$$

For fluid on both sides, double this answer. At $\alpha=0$ the one-sided power is $\mu b^2k\omega^2$, so the fixed-stroke cost increases by $s(s+1)/2>1$. The mechanical energy supplied to the fluid accounts for both [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) and work against the matrix drag; the stress still has the printed Newtonian form. Enhanced speed therefore comes with increased energetic cost.

## 3

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [Stokeslet](../../../stokes-flow.md#stokeslet) is the flow produced by a point [force](../../../classical-mechanics.md#force). With $C=1/(8\pi\mu)$, its tensor is $G_{ij}=C(\delta_{ij}/r+r_ir_j/r^3)$. A separated pair of equal and opposite forces has no [force](../../../classical-mechanics.md#force) monopole. Expanding their difference in the separation gives a directional derivative of this tensor. For an axial pair, choose the sign of the strength so that

$$
u_i=-S e_j e_k\partial_kG_{ij}
=\frac S{8\pi\mu}\left[-\frac1{r^3}+3\frac{(\mathbf e\cdot\mathbf r)^2}{r^5}\right]r_i.
$$

The trace part of $\mathbf e\mathbf e$ does not affect the flow because $\partial_jG_{ij}=0$. The remaining symmetric [force](../../../classical-mechanics.md#force)-dipole contribution is the [stresslet](../../../stokes-flow.md#force-dipole-flow), decaying as $r^{-2}$ instead of the [Stokeslet](../../../stokes-flow.md#stokeslet)'s $r^{-1}$. A [force-free](../../../stokes-flow.md#force-free) swimming cell has thrust balanced by drag, so this is typically its leading far field. With $S>0$ it is a [pusher microswimmer](../../../stokes-flow.md#pusher-microswimmer): axial outflow and transverse inflow. It is distinct from the antisymmetric [torque](../../../classical-mechanics.md#torque) singularity, the [rotlet](../../../stokes-flow.md#rotlet).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

On the axis of an identical [stresslet](../../../stokes-flow.md#force-dipole-flow), $\mathbf r=\ell\mathbf e$ gives [velocity](../../../classical-mechanics.md#velocity) $S\mathbf e/(4\pi\mu\ell^2)$, while the point on the opposite axis has its negative. Their identical intrinsic swimming velocities cancel from the relative motion. The [axial repulsion of pusher stresslets](../../../stokes-flow.md#axial-repulsion-of-pusher-stresslets) obeys

$$
\boxed{\dot\ell=\frac S{2\pi\mu\ell^2}>0,\qquad
\ell(t)=\left(\ell_0^3+\frac{3S}{2\pi\mu}t\right)^{1/3}.}
$$

This point-singularity approximation assumes the bodies are separated by distances large compared with their own sizes.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For a flat impermeable [free surface](../../../fluid-mechanics.md#free-surface) with zero tangential stress, the image of a parallel [stresslet](../../../stokes-flow.md#force-dipole-flow) is a [stresslet](../../../stokes-flow.md#force-dipole-flow) of the same strength and parallel orientation at the reflected point. Reflection makes the normal [velocity](../../../classical-mechanics.md#velocity) odd and tangential [velocity](../../../classical-mechanics.md#velocity) even across the plane, enforcing zero normal flow and zero tangential shear. This is the [free-surface image of a force dipole](../../../stokes-flow.md#free-surface-image-of-a-force-dipole); it is not the no-slip-wall image system.

The cell at $z=-h$ lies a distance $2h$ vertically below its image. Since $\mathbf e\cdot\mathbf r=0$ there, its induced vertical [velocity](../../../classical-mechanics.md#velocity) is $S/(32\pi\mu h^2)$ towards the surface. There is no image-induced tangential [velocity](../../../classical-mechanics.md#velocity), [vorticity](../../../fluid-mechanics.md#vorticity) or tangent-normal strain at this point, so a parallel orientation remains parallel in this idealization. Therefore the [finite-time free-surface approach of a point stresslet](../../../stokes-flow.md#finite-time-free-surface-approach-of-a-point-stresslet) is

$$
\boxed{\dot h=-\frac S{32\pi\mu h^2},\qquad
h(t)=\left(h_0^3-\frac{3S}{32\pi\mu}t\right)^{1/3},\qquad
t_* =\frac{32\pi\mu h_0^3}{3S}.}
$$

The trajectory combines its parallel self-propulsion with this normal drift. **Finite-time contact is the point-model prediction for $S>0$**, carried over from part (b). A puller with $S<0$ moves away instead. For a finite cell, the far-field approximation fails before $h$ reaches zero; surface deformation and near-contact physics can change the final encounter.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $C=S/(8\pi\mu)$. The image of the other [stresslet](../../../stokes-flow.md#force-dipole-flow) is at relative vector $(\ell,0,-2h)$, for which $r^2=\ell^2+4h^2$. Summing direct and image interactions gives the [free-surface interaction of two parallel stresslets](../../../stokes-flow.md#free-surface-interaction-of-two-parallel-stresslets)

$$
\dot\ell=\frac{4C}{\ell^2}
+2C\ell\frac{2\ell^2-4h^2}{(\ell^2+4h^2)^{5/2}},
\qquad
\dot h=-\frac C{4h^2}+2Ch\frac{2\ell^2-4h^2}{(\ell^2+4h^2)^{5/2}}.
$$

The direct neighbour gives no vertical [velocity](../../../classical-mechanics.md#velocity). Its image gives a vertical correction of order $Ch/\ell^3$, compared with the own-image attraction of order $C/h^2$. Thus for $h/\ell\ll1$,

$$
\boxed{\dot h=-\frac S{32\pi\mu h^2}\left[1+O((h/\ell)^3)\right],\qquad
\dot\ell=\frac S{\pi\mu\ell^2}\left[1+O((h/\ell)^2)\right].}
$$

The height evolution is unchanged to leading order, while the repulsion is twice the unbounded-fluid value: the neighbouring image lies almost at the same horizontal separation as the real neighbour. At this order $\ell^3=\ell_0^3+3St/(\pi\mu)$ and the height follows part (c). The equality for height is asymptotic, not exact; weak neighbour-induced orientation changes are also neglected in the stated parallel configuration.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [rotlet](../../../stokes-flow.md#rotlet) is the point-[torque](../../../classical-mechanics.md#torque) fundamental solution of [Stokes flow](../../../stokes-flow.md). Its [torque](../../../classical-mechanics.md#torque) strength $\mathbf R$ is an axial vector, and its circulating [velocity](../../../classical-mechanics.md#velocity) decays as $r^{-2}$. A freely swimming cell with no external [torque](../../../classical-mechanics.md#torque) is [torque-free](../../../stokes-flow.md#torque-free). The motor applies opposite internal torques to its body and flagellar apparatus, so the net [torque](../../../classical-mechanics.md#torque) monopole satisfies

$$
\boxed{\mathbf R_{\mathrm{total}}=0.}
$$

Individual body and flagellar torques need not vanish. A spatially separated pair can therefore leave a [rotlet dipole](../../../stokes-flow.md#rotlet-dipole) even though there is no far-field [rotlet](../../../stokes-flow.md#rotlet) monopole.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

A flagellar bundle and the counterrotating body supply oppositely signed axial torques separated along the swimming direction. Their leading [torque](../../../classical-mechanics.md#torque) moments cancel, and the next term is a [rotlet dipole](../../../stokes-flow.md#rotlet-dipole), decaying as $r^{-3}$. For the ideal axisymmetric bacterium the [torque](../../../classical-mechanics.md#torque) vector is parallel or antiparallel to $\mathbf e$.

To fix the sign convention, define a signed dipole strength $D$ with units [torque](../../../classical-mechanics.md#torque) times length and set

$$
\mathbf u_{\mathrm{RD}}=\frac D{8\pi\mu}(\mathbf e\cdot\nabla)
\frac{\mathbf e\times\mathbf r}{r^3}.
$$

Differentiating gives

$$
\boxed{\mathbf u_{\mathrm{RD}}=-\frac{3D}{8\pi\mu}
\frac{(\mathbf e\cdot\mathbf r)(\mathbf e\times\mathbf r)}{r^5}.}
$$

More generally, differentiating $\mathbf R\times\mathbf r/r^3$ gives $\mathbf R\times\mathbf e/r^3-3(\mathbf e\cdot\mathbf r)(\mathbf R\times\mathbf r)/r^5$; the first term vanishes when $\mathbf R\parallel\mathbf e$. A derivative with respect to source position instead of observation position changes the definition of the signed moment. The physical handedness depends on which [torque](../../../classical-mechanics.md#torque) is ahead, so it cannot be fixed without that convention.

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

Take $\mathbf e=\mathbf e_x$ and the surface normal $\mathbf e_z$. Under reflection in the free surface, polar vectors transform by $M=\operatorname{diag}(1,1,-1)$ and an axial [torque](../../../classical-mechanics.md#torque) transforms by $\det(M)M$. A parallel [torque](../../../classical-mechanics.md#torque) therefore reverses sign, while the separation direction $\mathbf e_x$ does not. The [free-surface image of a rotlet dipole](../../../stokes-flow.md#free-surface-image-of-a-rotlet-dipole) is a dipole of strength $-D$ at $z=+h$.

The observation point at the cell is directly below the image, so $\mathbf e\cdot\mathbf r=0$ and the image [velocity](../../../classical-mechanics.md#velocity) vanishes. A symmetry proof of the vanishing normal drift is also useful: reflection in the vertical plane containing $\mathbf e$ reverses the axial dipole moment, preserves the normal component of a polar [velocity](../../../classical-mechanics.md#velocity), and leaves the geometry unchanged. Linearity would make that same component change sign with $D$, forcing it to be zero. Thus **this singularity alone produces no attraction or repulsion**.

Write $X,Y,Z$ relative to the image, so the cell is at $(0,0,-2h)$. The image field is

$$
\mathbf u_{\mathrm{im}}=\frac{3D}{8\pi\mu}
\frac{X(0,-Z,Y)}{(X^2+Y^2+Z^2)^{5/2}}.
$$

Although its value at the cell is zero, its [velocity](../../../classical-mechanics.md#velocity) gradient is not. In particular, the [surface-induced yaw of a rotlet dipole](../../../stokes-flow.md#surface-induced-yaw-of-a-rotlet-dipole) has

$$
\boxed{\omega_z=(\partial_Xu_Y-\partial_Yu_X)_{\mathrm{cell}}
=\frac{3D}{128\pi\mu h^4}\ne0\quad(D\ne0).}
$$

A spherical [torque](../../../classical-mechanics.md#torque)-free body rotates with the local fluid angular [velocity](../../../classical-mechanics.md#velocity) $\Omega_z=\omega_z/2$. Its swimming direction therefore turns in the surface plane and, at fixed height and speed, it traces a circle with radius $V_{\mathrm{swim}}/|\Omega_z|$. The sign of $D$ sets the sense of turning in this convention. An elongated swimmer also responds to strain; its rotation coefficient depends on its shape and need not equal one half of the [vorticity](../../../fluid-mechanics.md#vorticity). When the [stresslet](../../../stokes-flow.md#force-dipole-flow) is included, its changing height produces a changing turning rate rather than an exactly fixed-radius circle.

## 4

↑ **Parent:** [Paper 77](paper-77.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $\mathbf t=(x_s,y_s)$ be the unit tangent of the [inextensible filament](../../../mathematical-biology.md#inextensible-filament). Define

$$
\rho=\frac{c_\parallel}{c_\perp},\qquad
\boxed{\beta=\frac1\Lambda\int_0^\Lambda x_s^2\,ds,\qquad
\delta=\frac1\Lambda\int_0^\Lambda x_sy_s\,ds.}
$$

These quantities are invariant under a shift of the periodic arclength coordinate. Since $x_s^2+y_s^2=1$, the average tangent tensor is $M=\left(\begin{smallmatrix}\beta&\delta\\\delta&1-\beta\end{smallmatrix}\right)$. Also $\int\mathbf t\,ds=\lambda\mathbf e_x$.

For [finite-amplitude propulsion of an inextensible periodic filament](../../../mathematical-biology.md#finite-amplitude-propulsion-of-an-inextensible-periodic-filament), distinguish axial phase speed from tangential material speed. The $V$ in the displayed formula is the axial speed of the travelling pattern relative to the mean filament motion. In the wave frame an inextensible material line slides backwards tangentially at the constant speed $Q=V\Lambda/\lambda$: its mean axial sliding is $Q\lambda/\Lambda=V$. If the filament translates at $-U\mathbf e_x$ in the laboratory, its local fluid-relative [velocity](../../../classical-mechanics.md#velocity) is

$$
\mathbf u=(V-U)\mathbf e_x-Q\mathbf t.
$$

This relation is the [axial and arclength travelling-wave speeds](../../../mathematical-biology.md#axial-and-arclength-travelling-wave-speeds) conversion. It ensures the arclength-averaged material [velocity](../../../classical-mechanics.md#velocity) is $-U\mathbf e_x$, rather than confusing wave propagation with material transport.

Integrating the [resistive-force theory](../../../mathematical-biology.md#resistive-force-theory) hydrodynamic [force](../../../classical-mechanics.md#force) over a period and imposing zero axial [force](../../../classical-mechanics.md#force) gives

$$
0=c_\perp\Lambda(V-U)[1+(\rho-1)\beta]-c_\parallel Q\lambda.
$$

Substitution of $Q\lambda=V\Lambda$ yields

$$
\boxed{\frac UV=\frac{(1-\rho)(1-\beta)}{1+\beta(\rho-1)}.}
$$

For $0<\rho<1$ and $\beta<1$ it is positive: anisotropic drag drives swimming opposite to the wave. A straight waveform has $\beta=1$ and gives no propulsion; isotropic drag $\rho=1$ also gives zero. The denominator $(1-\beta)+\rho\beta$ is positive. If instead $V$ denotes arclength propagation speed, the left-hand ratio acquires the extra factor $\lambda/\Lambda$; the two speeds are not interchangeable.

There is a geometric qualification to the asserted direction. For free swimming strictly along $x$, zero transverse [force](../../../classical-mechanics.md#force) also requires $\delta=0$, which holds for the usual reflection-symmetric waveforms. The periodicity assumptions alone do not imply that symmetry. A general waveform has [cross-resistance of an asymmetric planar waveform](../../../mathematical-biology.md#cross-resistance-of-an-asymmetric-planar-waveform) and can require a transverse translation. If the mean laboratory [velocity](../../../classical-mechanics.md#velocity) is $(-U_x,U_y)$, the full [force-free](../../../stokes-flow.md#force-free) condition is

$$
[I+(\rho-1)M]\binom{V-U_x}{U_y}=\rho V\binom10.
$$

Writing $A_0=1+(\rho-1)\beta$, $B_0=1+(\rho-1)(1-\beta)$ and $\mathcal D=A_0B_0-(\rho-1)^2\delta^2$, one obtains

$$
\boxed{\frac{U_x}V=1-\frac{\rho B_0}{\mathcal D},\qquad
\frac{U_y}V=-\frac{\rho(\rho-1)\delta}{\mathcal D}.}
$$

The printed expression is recovered when $\delta=0$, or as the axial [force](../../../classical-mechanics.md#force)-balance result if transverse motion is externally constrained. For an explicit permitted asymmetric shape, concatenate tangents $(\sqrt3/2,1/2)$ and $(1/2,-\sqrt3/2)$ with arclength fractions $p=\sqrt3/(1+\sqrt3)$ and $1-p$. Their mean vertical tangent is zero, but $\delta=\sqrt3(2p-1)/4\ne0$. Repeating the segments gives a periodic graph; the corners can be smoothed without removing the nonzero cross integral. Thus **pure opposite-to-wave free swimming also needs a zero cross-resistance assumption**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
