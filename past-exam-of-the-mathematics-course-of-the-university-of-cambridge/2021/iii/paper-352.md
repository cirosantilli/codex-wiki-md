# Paper 352

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_352.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_352.pdf)

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

## 1

↑ **Parent:** [Paper 352](paper-352.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let

$$
\mathbf D=\frac12\left(\nabla\mathbf u+(\nabla\mathbf u)^T\right)
$$

be the [rate-of-strain tensor](../../../viscous-fluid-flow.md#strain-rate-tensor) and let $\dot{\boldsymbol\gamma}=2\mathbf D$. The invariant magnitude convention that reproduces the ordinary scalar rate in [simple shear flow](../../../viscous-fluid-flow.md#simple-shear-flow) is

$$
\boxed{\dot\gamma
=\left(\frac12\dot{\boldsymbol\gamma}:
\dot{\boldsymbol\gamma}\right)^{1/2}
=\left(2\mathbf D:\mathbf D\right)^{1/2}}.
$$

The tensor contraction makes this definition independent of a rigid rotation of coordinates.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [generalized Newtonian fluid](../../../rheology.md#generalized-newtonian-fluid) responds instantaneously with stress determined only by the current scalar [shear rate](../../../viscous-fluid-flow.md#shear-rate). It therefore cannot represent [viscoelasticity](../../../rheology.md#viscoelasticity), including stress relaxation, elastic recoil, memory, and rate-dependent normal stresses. It also cannot represent [thixotropy](../../../rheology.md#thixotropy), in which microstructure and viscosity evolve with the duration and history of shearing. Other omitted effects include hysteresis and genuine finite-time yielding.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put $G=\Delta p/L>0$, with flow in the positive $z$ direction, so $dp/dz=-G$. Balancing pressure forces and wall shear on a cylindrical fluid volume of radius $R$ and length $L$ gives

$$
\Delta p\,\pi R^2=2\pi RL\,\tau_R,
\qquad
\boxed{\tau_R=\frac{\Delta p\,R}{2L}=\frac{GR}{2}}.
$$

Thus the wall stress is fixed before any [constitutive equation](../../../continuum-mechanics.md#constitutive-equation) is specified.

For fully developed [pipe flow](../../../viscous-fluid-flow.md#pipe-flow), the axial Cauchy equation reduces to

$$
-G=\frac1r\frac d{dr}(r\tau_{rz}).
$$

Regularity at the axis removes the $1/r$ integration constant, so

$$
\boxed{\tau_{rz}(r)=-\frac{Gr}{2}
=-\tau_R\frac rR}.
$$

Its magnitude rises linearly from zero at the axis to $\tau_R$ at the wall.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The axial velocity $u(r)$ decreases toward the wall, so $\dot\gamma=-du/dr\geq0$. For a [power-law fluid](../../../rheology.md#power-law-fluid), the stress magnitude is

$$
K\dot\gamma^n=\frac{Gr}{2}.
$$

Hence

$$
\boxed{\dot\gamma(r)=
\left(\frac{Gr}{2K}\right)^{1/n}}.
$$

Integrating inward from the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) $u(R)=0$ gives

$$
\boxed{u(r)=\frac n{n+1}
\left(\frac G{2K}\right)^{1/n}
\left(R^{1+1/n}-r^{1+1/n}\right)}.
$$

For $n=1$ this reduces to the parabolic Hagen--Poiseuille profile.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The [volumetric flow rate](../../../fluid-mechanics.md#volumetric-flow-rate) is $Q=2\pi\int_0^R u(r)r\,dr$. [Integration by parts](../../../calculus.md#integration-by-parts), using finite $u(0)$ and $u(R)=0$, gives

$$
Q=-\pi\int_0^Rr^2\frac{du}{dr}\,dr
=\boxed{\pi\int_0^R\dot\gamma(r)r^2\,dr}.
$$

Because the stress magnitude is $\tau=\tau_Rr/R$, change variables from $r$ to $\tau$:

$$
\boxed{Q=\frac{\pi R^3}{\tau_R^3}
\int_0^{\tau_R}\dot\gamma(\tau)\tau^2\,d\tau}.
$$

Therefore the required power is $n=3$. The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) gives the pipe form of the [Weissenberg–Rabinowitsch equation](../../../rheology.md#weissenberg-rabinowitsch-equation):

$$
\boxed{\dot\gamma_R
=\frac1{\pi R^3\tau_R^2}
\frac d{d\tau_R}(Q\tau_R^3)
=\frac{3Q+\tau_R,dQ/d\tau_R}{\pi R^3}}.
$$

Finally $\eta(\dot\gamma_R)=\tau_R/\dot\gamma_R$, so

$$
\boxed{\eta(\dot\gamma_R)
=\frac{\pi R^3\tau_R}
{3Q+\tau_R,dQ/d\tau_R}}.
$$

A measured pressure-drop--flow-rate curve therefore recovers the wall viscosity without assuming a constitutive form.

## 2

↑ **Parent:** [Paper 352](paper-352.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

In the [Giesekus model](../../../rheology.md#giesekus-model), $\lambda$ is the [viscoelastic relaxation time](../../../rheology.md#viscoelastic-relaxation-time): after deformation stops, polymeric stress relaxes on that timescale. The parameter $\eta$ has dimensions of [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) and is the model's zero-rate viscosity scale. Since $\lambda\boldsymbol\tau^2/\eta$ already has dimensions of stress, $\alpha$ is dimensionless.

The symbol $\overset{\triangledown}{\boldsymbol\tau}$ is the [upper-convected derivative](../../../rheology.md#upper-convected-derivative)

$$
\boxed{
\overset{\triangledown}{\boldsymbol\tau}
=\frac{D\boldsymbol\tau}{Dt}
-(\nabla\mathbf u)\boldsymbol\tau
-\boldsymbol\tau(\nabla\mathbf u)^T}.
$$

The convective and velocity-gradient terms account for translation, rotation, and affine stretching of material elements. They make the constitutive law objective under time-dependent rigid changes of observer.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Setting $\alpha=0$ gives the [Upper-convected Maxwell model](../../../rheology.md#upper-convected-maxwell-model)

$$
\boldsymbol\tau+\lambda
\overset{\triangledown}{\boldsymbol\tau}
=\eta\dot{\boldsymbol\gamma}.
$$

In steady incompressible uniaxial extension of rate $\dot\epsilon$, its tensile and transverse stresses give

$$
\eta_E
=\frac{\tau_{zz}-\tau_{xx}}{\dot\epsilon}
=\frac{2\eta}{1-2\lambda\dot\epsilon}
+\frac{\eta}{1+\lambda\dot\epsilon}.
$$

The [extensional viscosity](../../../rheology.md#extensional-viscosity) rises above the [Trouton ratio](../../../rheology.md#trouton-ratio) value $3\eta$ and diverges at $\lambda\dot\epsilon=1/2$, the ideal model's extensional catastrophe. An extensional rheometer can locate that rapid growth and estimate $\lambda\simeq1/(2\dot\epsilon_c)$. More robustly, impose a small deformation, stop the flow, and fit the exponential stress decay $\tau\propto e^{-t/\lambda}$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Write $g=\dot\gamma$ and

$$
\mathbf L=\nabla\mathbf u
=\begin{pmatrix}0&g&0\\0&0&0\\0&0&0\end{pmatrix},
\qquad
\boldsymbol\tau=
\begin{pmatrix}
\tau_{xx}&\tau_{xy}&0\\
\tau_{xy}&\tau_{yy}&0\\
0&0&\tau_{zz}
\end{pmatrix}.
$$

The flow and stresses are steady and homogeneous, so the material derivative vanishes. Direct multiplication gives

$$
\boxed{
\overset{\triangledown}{\boldsymbol\tau}
=-\mathbf L\boldsymbol\tau
-\boldsymbol\tau\mathbf L^T
=\begin{pmatrix}
-2g\tau_{xy}&-g\tau_{yy}&0\\
-g\tau_{yy}&0&0\\
0&0&0
\end{pmatrix}}
$$

and

$$
\boxed{
\boldsymbol\tau^2=
\begin{pmatrix}
\tau_{xx}^2+\tau_{xy}^2&
\tau_{xy}(\tau_{xx}+\tau_{yy})&0\\
\tau_{xy}(\tau_{xx}+\tau_{yy})&
\tau_{xy}^2+\tau_{yy}^2&0\\
0&0&\tau_{zz}^2
\end{pmatrix}}.
$$

Since $\dot\gamma_{xy}=\dot\gamma_{yx}=g$, the four independent component equations are

$$
\boxed{\tau_{xx}-2\lambda g\tau_{xy}
+\frac{\alpha\lambda}{\eta}(\tau_{xx}^2+\tau_{xy}^2)=0},
$$



$$
\boxed{\tau_{xy}-\lambda g\tau_{yy}
+\frac{\alpha\lambda}{\eta}
\tau_{xy}(\tau_{xx}+\tau_{yy})=\eta g},
$$



$$
\boxed{\tau_{yy}
+\frac{\alpha\lambda}{\eta}
(\tau_{xy}^2+\tau_{yy}^2)=0},
\qquad
\boxed{\tau_{zz}
+\frac{\alpha\lambda}{\eta}\tau_{zz}^2=0}.
$$

The branch continuous from equilibrium has $\tau_{zz}=0$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

At order $\alpha^0$, the preceding equations give

$$
\boxed{\tau_{xy}^0=\eta g,
\qquad \tau_{xx}^0=2\eta\lambda g^2,
\qquad \tau_{yy}^0=\tau_{zz}^0=0}.
$$

At order $\alpha^1$, the quadratic term is evaluated on $\boldsymbol\tau^0$. Solving first the $yy$ equation, then $xy$, then $xx$, gives

$$
\boxed{\tau_{yy}^1=-\eta\lambda g^2,
\qquad
\tau_{xy}^1=-3\eta\lambda^2g^3},
$$



$$
\boxed{\tau_{xx}^1
=-\eta\lambda g^2-10\eta\lambda^3g^4,
\qquad \tau_{zz}^1=0}.
$$

Thus the apparent [shear viscosity](../../../fluid-mechanics.md#dynamic-viscosity) is

$$
\boxed{\eta_{\rm app}(g)=\frac{\tau_{xy}}g
=\eta\left[1-3\alpha(\lambda g)^2\right]
+O(\alpha^2)},
$$

so positive $\alpha$ produces [shear thinning](../../../rheology.md#shear-thinning). The expansion requires $\alpha\ll1$ and $\alpha(\lambda g)^2\ll1$; it cannot describe arbitrarily high shear rates even when $\alpha$ is numerically small.

Using the [normal-stress difference](../../../rheology.md#normal-stress-difference) definitions

$$
N_1=\tau_{xx}-\tau_{yy}=\Psi_1g^2,
\qquad
N_2=\tau_{yy}-\tau_{zz}=\Psi_2g^2,
$$

we find

$$
\boxed{\Psi_1
=2\eta\lambda\left[1-5\alpha(\lambda g)^2\right]
+O(\alpha^2),
\qquad
\Psi_2=-\alpha\eta\lambda+O(\alpha^2)}.
$$

In the low-rate limit, $-2\Psi_2/\Psi_1=\alpha+O(\alpha^2)$. A cone-and-plate or parallel-plate rheometer can measure shear stress and normal thrust over a low-rate range; combining $\Psi_1$ and $\Psi_2$ then estimates $\alpha$ independently of the viscosity scale.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
