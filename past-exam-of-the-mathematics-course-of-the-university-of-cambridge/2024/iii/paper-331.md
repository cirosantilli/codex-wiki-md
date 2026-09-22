# Paper 331

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_331.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_331.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [a](#1/iii/a)
      - [Solution](#1/iii/a/solution)
    - [b](#1/iii/b)
      - [Solution](#1/iii/b/solution)
    - [c](#1/iii/c)
      - [Solution](#1/iii/c/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [a](#3/iii/a)
      - [Solution](#3/iii/a/solution)
    - [b](#3/iii/b)
      - [Solution](#3/iii/b/solution)
    - [c](#3/iii/c)
      - [Solution](#3/iii/c/solution)
    - [d](#3/iii/d)
      - [Solution](#3/iii/d/solution)

## 1

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The steady radial equation first gives the base-pressure gradient

$$
\frac{dp_0}{dr}=r\Omega^2.
$$

For the stated [normal mode](../../../wave-equation.md#normal-mode), put

$$
D(r)=\sigma+im\Omega(r).
$$

Retaining terms linear in the disturbance in the [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) gives

$$
\boxed{Du'-2\Omega v'+\frac{dp'}{dr}=0},
$$



$$
\boxed{Dv'+(2\Omega+r\Omega')u'
+\frac{im}{r}p'=0},
$$



$$
\boxed{Dw'+ikp'=0},
$$

together with [incompressible flow](../../../fluid-mechanics.md#incompressible-flow)

$$
\boxed{\frac1r\frac d{dr}(ru')
+\frac{im}{r}v'+ikw'=0}.
$$

The $-2\Omega v'$ and $(2\Omega+r\Omega')u'$ terms are the linearized centrifugal and angular-momentum couplings of the swirling base flow.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The centrifugal criterion concerns axisymmetric disturbances, so set $m=0$. The azimuthal equation gives

$$
v'=-\frac{2\Omega+r\Omega'}{\sigma}u'.
$$

Eliminating $w'$ with incompressibility and then $p'$ with the axial equation yields

$$
\boxed{
\frac d{dr}\left[\frac1r\frac d{dr}(ru')\right]
-k^2\left(1+\frac{\Phi(r)}{\sigma^2}\right)u'=0},
$$

where the [Rayleigh discriminant](../../../hydrodynamic-stability.md#rayleigh-discriminant) is

$$
\boxed{
\Phi(r)=2\Omega(2\Omega+r\Omega')
=\frac1{r^3}\frac d{dr}(r^4\Omega^2)}.
$$

Impermeability at the two solid walls gives $u'(r_i)=u'(r_o)=0$.

Multiply the equation by $r\overline{u'}$, integrate between the walls, and use [integration by parts](../../../calculus.md#integration-by-parts). The boundary terms vanish and one obtains

$$
\sigma^2
=-\frac{k^2\displaystyle\int_{r_i}^{r_o}
r\Phi|u'|^2\,dr}
{\displaystyle\int_{r_i}^{r_o}
\frac{|(ru')'|^2}{r}\,dr
+k^2\displaystyle\int_{r_i}^{r_o}r|u'|^2\,dr}.
$$

The denominator is positive. Therefore $\Phi\geq0$ throughout the annulus excludes positive real $\sigma^2$ and gives centrifugal stability. Since $r^4\Omega^2=(r^2\Omega)^2$ is the square of the [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum), [Rayleigh's circulation criterion](../../../hydrodynamic-stability.md#rayleigh-s-circulation-criterion) is

$$
\boxed{
\frac d{dr}(r^2\Omega)^2\geq0
\quad\text{for centrifugal stability}}.
$$

An outward decrease of squared specific angular momentum permits an axisymmetric centrifugal instability.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/a">a</h4>

↑ **Parent:** [Iii](#1/iii)

<h5 id="1/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#1/iii/a)

The displaced sheet is the material surface $r=R_0+\xi(\theta,t)$. Its [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) equates the radial velocity on each side to the material velocity of the sheet. To linear order,

$$
\boxed{
\xi_t=\left.\frac{\partial\phi_1}{\partial r}\right|_{R_0}},
$$



$$
\boxed{
\xi_t+\Omega_0\xi_\theta
=\left.\frac{\partial\phi_2}{\partial r}\right|_{R_0}},
\qquad
\Omega_0=\frac{\Gamma_0}{R_0^2}.
$$

For a mode $e^{\sigma t+im\theta}$ these become

$$
\boxed{\sigma\xi=\phi_1'(R_0),
\qquad
(\sigma+im\Omega_0)\xi=\phi_2'(R_0).}
$$

<h4 id="1/iii/b">b</h4>

↑ **Parent:** [Iii](#1/iii)

<h5 id="1/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#1/iii/b)

The inner base flow is at rest, so its linearized [Unsteady Bernoulli equation](../../../fluid-mechanics.md#unsteady-bernoulli-equation) gives $p_1'=-\sigma\phi_1$. The outer base potential is $\Gamma_0\theta$, hence its cross term with the perturbation gives

$$
p_2'=-\sigma\phi_2
-\frac{im\Gamma_0}{R_0^2}\phi_2.
$$

The base outer pressure satisfies $dp_{20}/dr=\Gamma_0^2/r^3$, whereas the inner base pressure is constant. Expanding [pressure continuity](../../../fluid-mechanics.md#pressure-continuity) on the displaced sheet therefore gives

$$
p_1'-p_2'-\frac{\Gamma_0^2}{R_0^3}\xi=0.
$$

After multiplication by $-1$ this is

$$
\boxed{
\sigma(\phi_1-\phi_2)
-\frac{im\Gamma_0}{R_0^2}\phi_2
+\frac{\Gamma_0^2}{R_0^3}\xi=0}.
$$

An additive function of time in Bernoulli appears as the stated constant; it vanishes for every nonaxisymmetric Fourier mode.

<h4 id="1/iii/c">c</h4>

↑ **Parent:** [Iii](#1/iii)

<h5 id="1/iii/c/solution">Solution</h5>

↑ **Parent:** [C](#1/iii/c)

Away from the [cylindrical vortex sheet](../../../fluid-mechanics.md#cylindrical-vortex-sheet), the disturbance is both incompressible and irrotational, so its potential is harmonic. Regularity at the axis and decay at infinity select

$$
\phi_1=A r^m e^{\sigma t+im\theta},
\qquad
\phi_2=B r^{-m}e^{\sigma t+im\theta}
$$

for a positive integer $m$. The kinematic conditions give their values on the sheet:

$$
\phi_1(R_0)=\frac{R_0\sigma}{m}\xi,
\qquad
\phi_2(R_0)=-\frac{R_0}{m}
(\sigma+im\Omega_0)\xi.
$$

Substitution into the dynamical condition gives the [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\sigma^2+im\Omega_0\sigma
+\frac{m(1-m)}2\Omega_0^2=0.
$$

Thus

$$
\boxed{
\sigma=\frac{\Omega_0}{2}
\left[-im\pm\sqrt{m^2-2m}\right]}.
$$

For every $m\geq3$, one root has positive real part. The cylindrical sheet is therefore subject to a [Kelvin-Helmholtz instability](../../../fluid-mechanics.md#kelvin-helmholtz-instability).

## 2

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Linearization about $w=0$ removes the quadratic term and gives

$$
w_t=\Delta^3w-R\Delta_1w.
$$

The three homogeneous boundary conditions select the vertical [normal modes](../../../wave-equation.md#normal-mode)

$$
\boxed{W_j(z)=A_j\sin(j\pi z)},
\qquad j=1,2,\ldots.
$$

Take a horizontal [Laplacian eigenfunction](../../../partial-differential-equation.md#laplacian-eigenfunction) satisfying

$$
\Delta_1f+a^2f=0.
$$

On $W_jf$, the full Laplacian has eigenvalue $-(a^2+j^2\pi^2)$. The [growth rate](../../../wave-equation.md#growth-rate) is consequently

$$
\boxed{s(a,R,j)=Ra^2-(a^2+j^2\pi^2)^3}.
$$

Neutrality occurs at

$$
R_{c,j}(a)=\frac{(a^2+j^2\pi^2)^3}{a^2}.
$$

For fixed nonzero $a$, this increases strictly with $j$, so the first unstable vertical mode is $j=1$ and

$$
\boxed{R_c(a)=\frac{(a^2+\pi^2)^3}{a^2}}.
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

At criticality choose the fundamental mode

$$
w_1=A\cos(ax)\sin(\pi z).
$$

Its quadratic self-interaction satisfies

$$
\frac12\partial_z^3(w_1^2)
=-A^2\pi^3[1+\cos(2ax)]\sin(2\pi z).
$$

The critical linear operator has eigenvalues $-64\pi^6$ on $\sin(2\pi z)$ and $-60(a^2+\pi^2)^3$ on $\cos(2ax)\sin(2\pi z)$. The slaved second-order correction is therefore

$$
w_2=A^2[d_0+d_1\cos(2ax)]\sin(2\pi z),
$$

where

$$
d_0=\frac1{64\pi^3},
\qquad
d_1=\frac{\pi^3}{60(a^2+\pi^2)^3}.
$$

Introduce a [slow time](../../../differential-equation.md#slow-time) $\tau$ and project the next-order equation onto the fundamental mode. Detuning $R-R_c$ contributes $a^2(R-R_c)A$, while the interaction of $w_1$ with $w_2$ has fundamental component

$$
-\frac14\pi^3(2d_0+d_1)A^3.
$$

The solvability condition is the [Landau amplitude equation](../../../dynamical-systems.md#landau-amplitude-equation)

$$
\boxed{
\frac{dA}{d\tau}
=a^2(R-R_c)A
-\frac14\pi^3(2d_0+d_1)A^3}.
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Set

$$
g=\frac14\pi^3(2d_0+d_1)>0,
\qquad
\mu=a^2(R-R_c).
$$

The amplitude equation is $\dot A=\mu A-gA^3$. Its equilibria are

$$
A=0
$$

for every $R$, and, when $R>R_c$,

$$
\boxed{A_\pm=\pm\sqrt{\frac{a^2(R-R_c)}g}}.
$$

For $R<R_c$, the zero branch is stable and every sufficiently small amplitude decays to zero. At $R=R_c$ it loses stability. For $R>R_c$, zero is unstable and the two nonzero branches are stable; positive initial amplitudes approach $A_+$ and negative ones approach $A_-$. The bifurcation diagram is therefore a [supercritical pitchfork](../../../dynamical-systems.md#pitchfork-bifurcation-normal-form).

## 3

↑ **Parent:** [Paper 331](paper-331.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

A matrix is [non-normal](../../../linear-operator-theory.md#non-normal-matrix) when it does not commute with its [adjoint matrix](../../../linear-operator-theory.md#conjugate-transpose):

$$
LL^\dagger\ne L^\dagger L.
$$

Nonorthogonal decaying eigenmodes can interfere constructively and produce [transient growth](../../../linear-operator-theory.md#transient-growth). For example,

$$
L=\begin{pmatrix}-1&10\\0&-2\end{pmatrix}
$$

has two negative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) but is non-normal. Starting from $x(0)=(0,1)^T$ gives

$$
x(t)=\begin{pmatrix}10(e^{-t}-e^{-2t})\\e^{-2t}\end{pmatrix}.
$$

At $t=\log2$, its squared [Euclidean norm](../../../functional-analysis.md#euclidean-norm) is $2.5^2+0.25^2>1=|x(0)|^2$. The energy grows transiently even though both eigenmodes eventually decay.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Because $L$ is diagonalizable, write

$$
L=V\Lambda V^{-1},
$$

where every diagonal entry of $\Lambda$ has negative real part. Define the equivalent norm

$$
\boxed{\|x\|_V=\|V^{-1}x\|_2}.
$$

Then

$$
\|e^{tL}x\|_V
=\|e^{t\Lambda}V^{-1}x\|_2
\leq\|V^{-1}x\|_2
=\|x\|_V
$$

for every $t\geq0$. Equivalently, this norm comes from the positive-definite inner-product matrix $H=V^{-\dagger}V^{-1}$. Thus stable eigenvalues always admit a norm with no growth, even though the standard Euclidean norm may show transient amplification.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/a">a</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#3/iii/a)

The first component obeys $\dot x_1=\lambda_1x_1$, so $x_1(t)=e^{\lambda_1t}x_1(0)$. Variation of constants in

$$
\dot x_2=x_1+\lambda_2x_2
$$

then gives

$$
x_2(t)=e^{\lambda_2t}x_2(0)
+\frac{e^{\lambda_1t}-e^{\lambda_2t}}
{\lambda_1-\lambda_2}x_1(0).
$$

Hence the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) is

$$
\boxed{
A=e^{tL}
=\begin{pmatrix}
e^{\lambda_1t}&0\\
\dfrac{e^{\lambda_1t}-e^{\lambda_2t}}
{\lambda_1-\lambda_2}&e^{\lambda_2t}
\end{pmatrix}}.
$$

<h4 id="3/iii/b">b</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#3/iii/b)

Write

$$
a=e^{\lambda_1t},
\qquad
b=\frac{e^{\lambda_1t}-e^{\lambda_2t}}
{\lambda_1-\lambda_2},
\qquad
c=e^{\lambda_2t}.
$$

The extremal squared amplification factors are the largest and smallest [singular values](../../../linear-algebra.md#singular-value) of $A$ squared, equivalently the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $G$ of

$$
A^TA=\begin{pmatrix}a^2+b^2&bc\\bc&c^2\end{pmatrix}.
$$

Since its trace is $a^2+b^2+c^2$ and its determinant is $a^2c^2$, the requested quadratic is

$$
\boxed{
G^2-(a^2+b^2+c^2)G+a^2c^2=0}.
$$

<h4 id="3/iii/c">c</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/c/solution">Solution</h5>

↑ **Parent:** [C](#3/iii/c)

As $\lambda_1\to\lambda_2=\lambda$, [L'Hôpital's rule](../../../calculus.md#l-hopital-s-rule) gives $b\to te^{\lambda t}$, so

$$
A=e^{\lambda t}
\begin{pmatrix}1&0\\t&1\end{pmatrix}.
$$

The quadratic becomes

$$
G^2-e^{2\lambda t}(t^2+2)G+e^{4\lambda t}=0.
$$

For $t\geq0$, its maximum root is

$$
\boxed{
G_+(t)=\frac{e^{2\lambda t}}2
\left[t^2+2+t\sqrt{t^2+4}\right]
=e^{2\lambda t}
\left(\frac{t+\sqrt{t^2+4}}2\right)^2}.
$$

<h4 id="3/iii/d">d</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/d/solution">Solution</h5>

↑ **Parent:** [D](#3/iii/d)

For $-1/2<\lambda<0$, logarithmic differentiation gives

$$
\frac d{dt}\log G_+(t)
=2\lambda+\frac2{\sqrt{t^2+4}}.
$$

The unique maximizing time is therefore

$$
\boxed{t_m=\sqrt{\lambda^{-2}-4}}.
$$

Writing $\alpha=-\lambda>0$ and $q=\sqrt{1-4\alpha^2}$, the maximum is

$$
\boxed{
G_+(t_m)
=e^{-2q}\left(\frac{1+q}{2\alpha}\right)^2}.
$$

Consequently, as $\lambda\to0^-$,

$$
\boxed{
t_m\sim\frac1{|\lambda|},
\qquad
G_+(t_m)\sim\frac1{e^2\lambda^2}}.
$$

At $\lambda=0$ exactly there is no finite maximizing time: the Jordan-block shear produces unbounded quadratic growth. The formulas describe how the optimal transient moves to later times and becomes larger as the damping tends to zero.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
