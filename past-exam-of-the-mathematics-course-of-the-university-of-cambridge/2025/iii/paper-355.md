# Paper 355

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_355.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_355.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 355](paper-355.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write the reaction terms as

$$
f(u,v)=u(1+u-\gamma v),\qquad
g(u,v)=v(\beta u-v).
$$

A nonzero homogeneous equilibrium satisfies $v_*=\beta u_*$ and $1+u_*-\gamma v_*=0$, hence

$$
\boxed{u_*=\frac1{\beta\gamma-1},\qquad
v_*=\frac{\beta}{\beta\gamma-1}}.
$$

For physically positive populations it exists exactly when

$$
\boxed{\beta\gamma>1}.
$$

The reaction [Jacobian matrix](../../../calculus.md#jacobian-matrix) at this equilibrium is

$$
J=u_*
\begin{pmatrix}
1&-\gamma\\
\beta^2&-\beta
\end{pmatrix}.
$$

Its trace and determinant are

$$
\operatorname{tr}J=u_*(1-\beta),\qquad
\det J=u_*^2\beta(\beta\gamma-1)>0.
$$

The equilibrium is therefore stable to spatially uniform perturbations when

$$
\boxed{\beta>1,\qquad\beta\gamma>1}.
$$

For a spatial [Fourier mode](../../../fourier-analysis.md#fourier-mode) of wavenumber $k$, put $q=k^2$. The linearized [reaction–diffusion system](../../../diffusion-equation.md#reaction-diffusion-system) has matrix

$$
J_q=J-q\begin{pmatrix}1&0\\0&d\end{pmatrix}.
$$

Its trace is smaller than $\operatorname{tr}J$, while

$$
\det J_q
=dq^2-u_*(d-\beta)q
+u_*^2\beta(\beta\gamma-1).
$$

The [two-species diffusion-driven instability criterion](../../../diffusion-equation.md#two-species-diffusion-driven-instability-criterion) says that this upward-opening quadratic becomes negative for some $q>0$ precisely when

$$
d>\beta,\qquad
(d-\beta)^2>4d\beta(\beta\gamma-1).
$$

Combining all conditions, a [Turing instability](../../../diffusion-equation.md#turing-instability) may occur in the region

$$
\boxed{
\beta>1,\qquad d>\beta,\qquad
\frac1\beta<\gamma<
\frac1\beta+\frac{(d-\beta)^2}{4d\beta^2}}.
$$

At onset the discriminant vanishes, and the double root is

$$
q_c=\frac{u_*(d-\beta)}{2d}.
$$

The threshold relation gives

$$
\beta\gamma-1=\frac{(d-\beta)^2}{4d\beta},
\qquad
u_*=\frac{4d\beta}{(d-\beta)^2},
$$

so the critical wavenumber is

$$
\boxed{k_c=\left(\frac{2\beta}{d-\beta}\right)^{1/2}}.
$$

If $d=1$, uniform stability requires $\beta>1$ whereas diffusion-driven instability requires $d>\beta$. These inequalities are incompatible, so the Turing region vanishes.

## 2

↑ **Parent:** [Paper 355](paper-355.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Take $z$ upward along the straight rod. The part above height $z$ has weight $\lambda g(L-z)$, so, with tensile force positive, the internal tension is compressive:

$$
\boxed{\sigma(z)=-\lambda g(L-z)}.
$$

For a small transverse displacement $X(z)$, the quadratic bending and gravitational energies are

$$
\mathcal E[X]
=\frac A2\int_0^L(X'')^2\,dz
-\frac{\lambda g}{2}\int_0^L(L-z)(X')^2\,dz.
$$

The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) for this functional is

$$
AX''''+\bigl[\lambda g(L-z)X'\bigr]'=0,
$$

which is exactly

$$
\boxed{AX_{zzzz}-(\sigma X_z)_z=0}.
$$

Clamping at the bottom fixes displacement and slope:

$$
X(0)=0,\qquad X'(0)=0.
$$

At the free upper end, bending moment and transverse force vanish:

$$
AX''(L)=0,\qquad AX'''(L)-\sigma(L)X'(L)=0.
$$

Since $\sigma(L)=0$, the four boundary conditions are

$$
\boxed{X(0)=X'(0)=0,\qquad X''(L)=X'''(L)=0}.
$$

Set $u=X'$. Integrating the field equation once and using the free-end shear condition gives

$$
Au''-\sigma u=0,
$$

or, with $s=L-z$,

$$
u_{ss}+\frac{\lambda g}{A}s\,u=0.
$$

Introduce the dimensionless similarity coordinate

$$
\eta=\frac23\left(\frac{\lambda g}{A}s^3\right)^{1/2}
$$

and write $u=\eta^{1/3}F(\eta)$. Direct substitution reduces the equation to

$$
\eta^2F''+\eta F'
+\left(\eta^2-\frac19\right)F=0.
$$

This is the [Bessel differential equation](../../../analysis.md#bessel-differential-equation) of order $1/3$, so

$$
\boxed{
u=\eta^{1/3}\left[aJ_{-1/3}(\eta)+bJ_{1/3}(\eta)\right]}.
$$

The free-moment condition is $u'(L)=0$. As $\eta\to0$,

$$
\eta^{1/3}J_{-1/3}(\eta)\sim\text{constant},
\qquad
\eta^{1/3}J_{1/3}(\eta)\sim\eta^{2/3}\propto s.
$$

The second term has nonzero limiting $z$ derivative, so the free-end condition forces $b=0$. The free-shear condition $u''(L)=0$ then follows from the differential equation. At the clamp, $u(0)=0$, giving

$$
J_{-1/3}(\eta_0)=0,\qquad
\eta_0=\frac23\left(\frac{\lambda gL^3}{A}\right)^{1/2}.
$$

Let $j_{-1/3,1}$ be the smallest positive zero of this [Bessel function](../../../analysis.md#bessel-function). The first [self-buckling threshold](../../../mathematical-biology.md#self-buckling-of-a-vertical-rod) is

$$
\boxed{
\frac23\left(\frac{\lambda gL^3}{A}\right)^{1/2}
=j_{-1/3,1}},
$$

or equivalently

$$
\boxed{\frac{\lambda gL^3}{A}
=\frac94j_{-1/3,1}^2}.
$$

## 3

↑ **Parent:** [Paper 355](paper-355.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

At large separation, the finite-thickness van der Waals combination has the expansion

$$
\frac1{d^2}-\frac2{(d+\delta)^2}
+\frac1{(d+2\delta)^2}
=\frac{6\delta^2}{d^4}+O(d^{-5}).
$$

Thus the attraction governed by the [Hamaker constant](../../../mathematical-biology.md#hamaker-constant) decays as

$$
V_{\rm vdW}\sim-\frac{A_H\delta^2}{2\pi d^4},
$$

and the screened electrostatic term decays exponentially on the [Debye–Hückel screening length](../../../mathematical-biology.md#debye-huckel-screening-length). The [Helfrich repulsion](../../../mathematical-biology.md#helfrich-repulsion), however, decays only as

$$
V_{\rm rep}\sim\frac{c(k_BT)^2}{k_cd^2}>0.
$$

Consequently the total interaction approaches its unbound value zero from above as $d\to\infty$.

A finite bound minimum must have nonpositive energy to beat the state at infinity. Because the large-$d$ interaction is positive, such a minimum cannot move continuously to infinity while remaining globally stable. At the transition it instead becomes degenerate with the $d=\infty$ state at a finite spacing and then loses global stability. The equilibrium spacing therefore jumps from finite $d_*$ to infinity, making this a discontinuous, first-order unbinding transition.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a dilute stack, the membrane number per unit normal length is $1/d=\phi/\delta$. Dividing the fluctuation repulsion per area by the repeat distance gives its [free-energy density](../../../statistical-physics.md#free-energy-density)

$$
f_{\rm rep}
=\frac{c(k_BT)^2}{k_cd^3}
=\frac{c(k_BT)^2}{k_c\delta^3}\phi^3.
$$

The short-range electrostatic repulsion and long-range van der Waals attraction enter at second-virial order. In general, for an effective pair energy $U_{A_H}(\Gamma)$ over relative configurations $\Gamma$, the [second virial coefficient](../../../statistical-physics.md#second-virial-coefficient) has the Mayer-integral form

$$
\boxed{
B_2(A_H)=\frac12\int
\left[1-e^{-U_{A_H}(\Gamma)/(k_BT)}\right]d\Gamma},
$$

with a fixed normalization by the microscopic membrane thickness making $B_2$ dimensionless here. The mean-field contribution is quadratic in membrane concentration. The required two-power free energy can therefore be written

$$
\boxed{
f(\phi)=
\frac{k_BT}{\delta^3}B_2(A_H)\phi^2
+\frac{c(k_BT)^2}{k_c\delta^3}\phi^3,
\qquad \phi\geq0}.
$$

Changes of microscopic normalization merely rescale $B_2$ by a positive constant and do not affect the transition.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Write the pair energy as

$$
U_{A_H}(\Gamma)=U_{\rm rep}(\Gamma)-A_HW(\Gamma),
\qquad W(\Gamma)>0.
$$

At $A_H=0$ the interaction is repulsive, so the Mayer integrand and hence $B_2$ are positive. Increasing $A_H$ strengthens attraction and

$$
\frac{dB_2}{dA_H}
=-\frac1{2k_BT}\int
W(\Gamma)e^{-U_{A_H}(\Gamma)/(k_BT)}\,d\Gamma<0.
$$

For sufficiently strong attraction, negative configurations dominate and $B_2<0$. Continuity therefore gives a critical $A_H^*$ with $B_2(A_H^*)=0$. The [Taylor theorem](../../../calculus.md#taylor-theorem) gives

$$
\boxed{
B_2(A_H)
=B_2'(A_H^*)(A_H-A_H^*)+\cdots
\sim r(A_H^*-A_H)},
$$

where $r=-B_2'(A_H^*)>0$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Write the free energy as

$$
f(\phi)=a\phi^3+bB_2\phi^2,
\qquad
a=\frac{c(k_BT)^2}{k_c\delta^3}>0,
\qquad
b=\frac{k_BT}{\delta^3}>0.
$$

When $A_H<A_H^*$, $B_2>0$ and the global minimum on $\phi\geq0$ is $\phi_*=0$, corresponding to an unbound stack. When $A_H>A_H^*$, $B_2<0$, and minimization gives

$$
f'(\phi)=\phi(3a\phi+2bB_2)=0,
\qquad
\boxed{\phi_*=-\frac{2bB_2}{3a}}.
$$

Using $B_2\sim-r(A_H-A_H^*)$ yields

$$
\phi_*\sim A_H-A_H^*.
$$

Since $d_*=\delta/\phi_*$,

$$
\boxed{
d_*\sim(A_H-A_H^*)^{-1}},
$$

so the continuous [membrane unbinding transition](../../../mathematical-biology.md#membrane-unbinding-transition) has exponent

$$
\boxed{\nu=1}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
