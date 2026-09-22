# Paper 331

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_331.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_331.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [a](#1/i/a)
      - [Solution](#1/i/a/solution)
    - [b](#1/i/b)
      - [Solution](#1/i/b/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
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

## 1

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/a">a</h4>

↑ **Parent:** [I](#1/i)

<h5 id="1/i/a/solution">Solution</h5>

↑ **Parent:** [A](#1/i/a)

Write the [Rayleigh equation for inviscid shear flow](../../../hydrodynamic-stability.md#rayleigh-equation-for-inviscid-shear-flow) as

$$
\phi''-\alpha^2\phi-
\frac{U''}{U-c}\phi=0,
\qquad \phi(0)=\phi(1)=0.
$$

Multiply by $\phi^*$, integrate, and use [integration by parts](../../../calculus.md#integration-by-parts):

$$
\int_0^1(|\phi'|^2+\alpha^2|\phi|^2)\,dz
+\int_0^1\frac{U''(U-c^*)}{|U-c|^2}|\phi|^2\,dz=0.
$$

Its imaginary part is

$$
c_i\int_0^1\frac{U''}{|U-c|^2}|\phi|^2\,dz=0.
$$

For an unstable mode $c_i>0$, the integral can vanish only if $U''$ changes sign somewhere in the flow. Thus the velocity profile must have an inflection point. This is [Rayleigh's inflection-point theorem](../../../hydrodynamic-stability.md#rayleigh-s-inflection-point-theorem); it is necessary, not sufficient, for inviscid instability.

<h4 id="1/i/b">b</h4>

↑ **Parent:** [I](#1/i)

<h5 id="1/i/b/solution">Solution</h5>

↑ **Parent:** [B](#1/i/b)

Put $\phi=(U-c)F$. The [Rayleigh equation for inviscid shear flow](../../../hydrodynamic-stability.md#rayleigh-equation-for-inviscid-shear-flow) becomes

$$
[(U-c)^2F']'-\alpha^2(U-c)^2F=0.
$$

Multiplication by $F^*$ and integration gives

$$
\int_0^1(U-c)^2Q\,dz=0,
\qquad
Q=|F'|^2+\alpha^2|F|^2\geq0.
$$

For $c_i>0$, its real and imaginary parts imply

$$
c_r=\frac{\int UQ\,dz}{\int Q\,dz},
\qquad
c_i^2=\frac{\int(U-c_r)^2Q\,dz}{\int Q\,dz}.
$$

Thus $c_r$ is a weighted mean of $U$ and $c_i^2$ is its weighted [variance](../../../variance.md). If $U_-\leq U\leq U_+$, the sharp bounded-variable variance estimate gives

$$
c_i^2\leq(U_+-c_r)(c_r-U_-).
$$

Completing the square proves [Howard's semicircle theorem](../../../hydrodynamic-stability.md#howard-s-semicircle-theorem):

$$
\boxed{
\left(c_r-\frac{U_++U_-}{2}\right)^2+c_i^2
\leq\left(\frac{U_+-U_-}{2}\right)^2}.
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Away from $z=0,\pm1$, the base profile is linear or constant, so $U''=0$ and $\phi''-\alpha^2\phi=0$. Across a corner $z=z_0$, integration of the Rayleigh equation gives the jump condition

$$
(U(z_0)-c)[\phi']=[U']\phi.
$$

For the even mode, at $z=0$ this gives

$$
\phi'(0^+)=-\frac{\phi(0)}{1-c}.
$$

For $0<z<1$, therefore,

$$
\phi(z)=A\left[
\cosh(\alpha z)-
\frac{\sinh(\alpha z)}{\alpha(1-c)}
\right].
$$

For $z>1$, decay requires $\phi\propto e^{-\alpha(z-1)}$. The jump at $z=1$, where $[U']=1$, gives

$$
\phi'(1^-)=\left(\frac1c-\alpha\right)\phi(1).
$$

Substitution and elementary simplification yield

$$
\boxed{
2\alpha^2c^2+\alpha(1-2\alpha-e^{-2\alpha})c
-[1-\alpha-(1+\alpha)e^{-2\alpha}]=0}.
$$

The coefficients are real, so instability occurs when the quadratic discriminant is negative. At $\alpha=1$ it is

$$
(1+e^{-2})^2-16e^{-2}<0,
$$

whereas at $\alpha=2$, using $e^{-4}\simeq1/55$, it is positive. By continuity there is a first threshold $1<\alpha_s<2$ at which the discriminant vanishes. Hence one conjugate root has $c_i>0$ for

$$
\boxed{1\leq\alpha<\alpha_s<2}.
$$

## 2

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The energy is

$$
E(t)=c_1^2e^{-2\lambda_1t}
+c_2^2e^{-2\lambda_2t}
+2\alpha c_1c_2e^{-(\lambda_1+\lambda_2)t}.
$$

Thus

$$
E'(0)=-2[\lambda_1c_1^2+\lambda_2c_2^2
+(\lambda_1+\lambda_2)\alpha c_1c_2].
$$

This quadratic form can be negative for positive $c_1,c_2$ precisely when

$$
\boxed{\alpha<-\frac{2\sqrt{\lambda_1\lambda_2}}
{\lambda_1+\lambda_2}}.
$$

The decaying vectors must therefore be sufficiently nonorthogonal and oppositely directed. This is [transient growth from non-normal modes](../../../hydrodynamic-stability.md#transient-growth-from-non-normal-modes).

With $c_2=1$ and $\mu=c_1/c_2$, maximizing $E'(0)$ gives

$$
2\lambda_1\mu+(\lambda_1+\lambda_2)\alpha=0,
$$

so

$$
\boxed{\mu_{\rm opt}
=-\frac{(\lambda_1+\lambda_2)\alpha}{2\lambda_1}}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Dot the momentum equation with $\mathbf u$, multiply the temperature equation by $\sigma\operatorname{Ra}\theta$, and integrate over $V$. The pressure term vanishes by incompressibility, while [skew-symmetry of incompressible transport](../../../viscous-fluid-flow.md#skew-symmetry-of-incompressible-transport) removes both nonlinear advection terms. Integration by parts and the boundary conditions give

$$
\boxed{
\frac{dE}{dt}=\sigma\int_V
[2\operatorname{Ra}w\theta-|\nabla\mathbf u|^2
-\operatorname{Ra}|\nabla\theta|^2],dV},
$$

where

$$
E=\frac12\int_V
(|\mathbf u|^2+\sigma\operatorname{Ra}\theta^2)\,dV.
$$

For $\operatorname{Ra}=0$, this reduces to

$$
\frac{dE}{dt}=-\sigma\int_V|\nabla\mathbf u|^2\,dV\leq0,
$$

so viscosity monotonically dissipates kinetic energy.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Vary the integral on the right-hand side, imposing $\nabla\mathbin\cdot\mathbf u=0$ with multiplier $2p$. After integration by parts, independent variations of $\mathbf u$, $\theta$, and $p$ give

$$
\boxed{
0=-\nabla p+\sigma\operatorname{Ra}\theta\widehat{\mathbf z}
+\sigma\nabla^2\mathbf u,
\qquad
0=w+\nabla^2\theta,
\qquad
\nabla\mathbin\cdot\mathbf u=0}.
$$

Dot the first equation with $\mathbf u$ and the second with $\sigma\operatorname{Ra}\theta$, then integrate. Their sum says exactly that the energy-production functional is zero. Hence any nonzero stationary point is a perturbation whose energy initially neither grows nor decays.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

The linear normal-mode problem is

$$
\lambda\mathbf u=-\nabla p+sigma\operatorname{Ra}\theta\widehat{\mathbf z}
+\sigma\nabla^2\mathbf u,
\qquad
\lambda\theta=w+\nabla^2\theta,
\qquad
\nabla\mathbin\cdot\mathbf u=0.
$$

At $\lambda=0$ it is exactly the variational Euler--Lagrange system from part ii. Therefore the [energy-stability threshold](../../../hydrodynamic-stability.md#energy-stability-threshold) coincides with the stated linear neutral threshold $\operatorname{Ra}_{\rm crit}$. Below it the quadratic production functional is negative for every nonzero perturbation, so there is no transient energy growth; at the threshold a neutral perturbation exists, and above it the leading real eigenvalue produces exponential growth.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

After the pressure enforces incompressibility, let $L$ denote the displayed linear operator. Integration by parts gives

$$
\langle\Phi_i,L\Phi_j\rangle
=-\sigma\int_V\nabla\mathbf u_i:\nabla\mathbf u_j\,dV
-\sigma\operatorname{Ra}\int_V\nabla\theta_i\mathbin\cdot\nabla\theta_j\,dV
+\sigma\operatorname{Ra}\int_V(w_i\theta_j+\theta_iw_j)\,dV.
$$

The pressure terms vanish by incompressibility and the boundary conditions. The expression is symmetric under $i\leftrightarrow j$, so

$$
\boxed{\langle\Phi_i,L\Phi_j\rangle
=\langle L\Phi_i,\Phi_j\rangle}.
$$

**Thus $L$ is a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) in the energy inner product and hence a [normal operator](../../../hilbert-space.md#normal-operator). Its orthogonal eigenmodes cannot generate non-normal transient growth.**

## 3

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Substitute the stated scales and divide the momentum equation by $2\Omega V$. The ratio of inertial to Coriolis acceleration is the [Rossby number](../../../geophysical-fluid-dynamics.md#rossby-number)

$$
\operatorname{Ro}=\frac{V}{2\Omega L},
$$

while the dimensionless buoyancy coefficient is

$$
\frac{\alpha g\Delta\theta}{2\Omega V}
=\frac{B}{\operatorname{Ro}},
\qquad
B=\frac{\alpha g\Delta\theta}{4\Omega^2L}.
$$

Thus

$$
\boxed{
\operatorname{Ro}(\mathbf u_t+\mathbf u\mathbin\cdot\nabla\mathbf u)
+\widehat{\mathbf z}\times\mathbf u
=-\nabla p+\frac{B}{\operatorname{Ro}}\theta\widehat{\mathbf z}},
$$



$$
\boxed{\theta_t+\mathbf u\mathbin\cdot\nabla\theta=0,
\qquad\nabla\mathbin\cdot\mathbf u=0}.
$$

The dimensionless $B$ is the [Burgers number](../../../geophysical-fluid-dynamics.md#burgers-number) for this rotating stratified flow.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For

$$
\mathbf U=z\widehat{\mathbf x},
\qquad
\Theta=z-\frac{\operatorname{Ro}}B y,
$$

both material derivatives vanish because the fields are independent of $x$. Since $\widehat{\mathbf z}\times\mathbf U=z\widehat{\mathbf y}$, steady momentum balance requires

$$
P_y=-z,
\qquad
P_z=\frac B{\operatorname{Ro}}z-y.
$$

These derivatives are compatible and integrate to

$$
\boxed{P=-yz+\frac{B}{2\operatorname{Ro}}z^2+\text{constant}}.
$$

The cross-stream temperature gradient and vertical stratification are in [thermal-wind balance](../../../geophysical-fluid-dynamics.md#thermal-wind) with the vertical shear.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $D=\partial_t+z\partial_x$. Retaining terms linear in the primed fields gives

$$
\boxed{
\operatorname{Ro}(Du'+\operatorname{Ro}w')-v'=-p'_x},
$$



$$
\boxed{\operatorname{Ro}Dv'+u'=-p'_y},
$$



$$
\boxed{\operatorname{Ro}^2Dw'=-p'_z+B\theta'},
$$



$$
\boxed{D\theta'+w'-\frac1Bv'=0},
\qquad
\boxed{u'_x+v'_y+\operatorname{Ro}w'_z=0}.
$$

The terms $\operatorname{Ro}^2w'$ and $-v'/B$ respectively arise from perturbation advection of the velocity and temperature gradients in the basic state.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Differentiate the $y$-momentum equation with respect to $x$, subtract the $y$ derivative of the $x$-momentum equation, and use incompressibility. With vertical perturbation vorticity

$$
\zeta'=v'_x-u'_y,
$$

one obtains

$$
\operatorname{Ro}D\zeta'
-\operatorname{Ro}w'_z-\operatorname{Ro}^2w'_y=0.
$$

Therefore

$$
\boxed{
\left(\frac\partial{\partial t}+z\frac\partial{\partial x}\right)
\left(\frac{\partial v'}{\partial x}
-\frac{\partial u'}{\partial y}\right)
=\frac{\partial w'}{\partial z}
+\operatorname{Ro}\frac{\partial w'}{\partial y}}.
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

At leading order as $\operatorname{Ro}\to0$, horizontal [geostrophic balance](../../../physics.md#geostrophic-balance) and vertical hydrostatic balance give

$$
v'=p'_x,
\qquad
u'=-p'_y,
\qquad
\theta'=\frac1B p'_z.
$$

The temperature equation gives

$$
Bw'=p'_x-Dp'_z.
$$

Meanwhile $\zeta'=p'_{xx}+p'_{yy}$. The leading vertical-vorticity equation is $D\zeta'=w'_z$. Since derivatives in $z$ do not commute with $D$,

$$
(Dp'_z)_z=Dp'_{zz}+p'_{xz}.
$$

The $p'_{xz}$ terms therefore cancel, leaving the conserved [three-dimensional quasi-geostrophic potential vorticity](../../../geophysical-fluid-dynamics.md#three-dimensional-quasi-geostrophic-potential-vorticity)

$$
\boxed{
D\left[p'_{zz}+B(p'_{xx}+p'_{yy})\right]=0}.
$$

No normal flow at $y=0,1$ means $v'=p'_x=0$. At $z=0,1$, $w'=0$, so

$$
\boxed{
p'_x=0\quad(y=0,1),
\qquad
Dp'_z=p'_x\quad(z=0,1)}.
$$

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Insert

$$
p'=p(z)\sin(n\pi y)e^{i\alpha(x-ct)}.
$$

The side-wall condition is automatic, and the potential-vorticity equation gives

$$
p''-B(\alpha^2+n^2\pi^2)p=0.
$$

Define

$$
\lambda=\frac12\sqrt{B(\alpha^2+n^2\pi^2)}.
$$

Then

$$
p=A\cosh[2\lambda(z-	frac12)]
+C\sinh[2\lambda(z-	frac12)].
$$

The top and bottom conditions become

$$
-cp'(0)=p(0),
\qquad
(1-c)p'(1)=p(1).
$$

Setting the determinant of these two homogeneous equations for $A,C$ to zero and simplifying gives

$$
\boxed{
c=\frac12\pm
\frac1{2\lambda}
\sqrt{(\lambda\coth\lambda-1)
(\lambda\tanh\lambda-1)}}.
$$

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

For every $\lambda>0$, $\tanh\lambda<\lambda$, so

$$
\lambda\coth\lambda>1.
$$

The radicand in part f is therefore negative precisely when its second factor is negative. The two wave speeds are then complex conjugates, one with positive imaginary part and exponential growth. Hence

$$
\boxed{\text{instability occurs exactly when }
\lambda\tanh\lambda<1}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
