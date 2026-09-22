# Paper 335

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_335.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_335.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
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
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)

## 1

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Define

$$
A=\partial_x,
\qquad
B=\left(n^2+k_0^{-2}\partial_z^2\right)^{1/2}.
$$

If $A$ and $B$ commute, the [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) operator factorizes as

$$
A^2+k_0^2B^2
=(A+ik_0B)(A-ik_0B).
$$

When $n$ varies with $x$, the exact product also contains the [commutator](../../../lie-algebra.md#commutator) $[A,B]$; neglecting it assumes longitudinal changes are slow. The forward-propagating factor is

$$
(A-ik_0B)\psi=0,
$$

because it admits $e^{ik_0x}$ in a uniform medium.

Put $\psi=Ee^{ik_0x}$. The one-way equation becomes

$$
E_x=ik_0(B-1)E.
$$

For

$$
Q=n^2-1+k_0^{-2}\partial_z^2,
$$

the [Taylor expansion](../../../calculus.md#taylor-expansion) $(1+Q)^{1/2}=1+Q/2+O(Q^2)$ gives

$$
E_x=\frac{i}{2k_0}E_{zz}
+\frac{ik_0}{2}(n^2-1)E.
$$

Thus the [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation) is

$$
\boxed{
2ik_0E_x+E_{zz}
+k_0^2(n^2-1)E=0}.
$$

The expansion is accurate under the [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation): transverse wavenumbers satisfy $|k_z|/k_0\ll1$, the envelope varies slowly on the carrier scale, the refractive-index contrast is weak enough for $Q^2$ to be negligible, and $n$ varies slowly in $x$ so $[A,B]$ is small. The one-way factor discards backward propagation and reflection; the square-root expansion additionally discards large-angle and higher-order diffraction, and it does not accurately represent strongly evanescent components or abrupt longitudinal interfaces.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

With

$$
D=\frac{i}{2k_0}\partial_z^2,
\qquad
S=\frac{ik_0}{2}(n^2-1),
$$

the [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation) is $E_x=(D+S)E$. Freeze $S$ at $x_0$, or preferably at the step midpoint. Over a short distance $\Delta x$, [Lie-Trotter splitting](../../../numerical-analysis.md#lie-product-formula) gives

$$
\boxed{
E(x_0+\Delta x)
\simeq e^{\Delta xD}e^{\Delta xS_0}E(x_0)}.
$$

The reversed ordering has the same first-order accuracy, while symmetric half-steps in $S$ give the more accurate Strang form.

The [commutator](../../../lie-algebra.md#commutator) can be displayed explicitly. If $q=n^2-1$, then

$$
[D,S]E
=-\frac14\left(q_{zz}E+2q_zE_z\right).
$$

The splitting assumption requires $\Delta x^2[D,S]E$ to be small relative to $E$. It is favored by a short range step, a transversely smooth refractive index, and a field without unresolved large transverse wavenumbers. Freezing $S$ also requires $\Delta x\,S_x$ to be small. These conditions supplement the one-way and [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation) already used in part i.

The phase-screen substep is pointwise:

$$
e^{\Delta xS_0}E(x_0,z)
=\exp\left[
\frac{ik_0\Delta x}{2}
(n^2(x_0,z)-1)
\right]E(x_0,z).
$$

Define

$$
\boxed{
\widetilde E_0(x_0,z)
=e^{\Delta xS_0}E(x_0,z)}.
$$

Then solve the free-diffraction initial-value problem

$$
E_x=DE,
\qquad
E(x_0,z)=\widetilde E_0(x_0,z),
$$

to $x_0+\Delta x$. In transverse [Fourier transform](../../../analysis.md#fourier-transform) variables, this substep is simply

$$
\widehat E(x_0+\Delta x,k_z)
=e^{-ik_z^2\Delta x/(2k_0)}
\widehat{\widetilde E}_0(k_z).
$$

This is the [split-step Fourier method](../../../partial-differential-equation.md#split-step-fourier-method).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Partition the range into planes $x_j=x_0+j\Delta x$. At each step, evaluate the refractive-index phase screen at $x_j$ or the midpoint, multiply the current envelope by $e^{\Delta xS_j}$, transform in $z$, multiply each transverse Fourier component by the diffraction phase $e^{-ik_z^2\Delta x/(2k_0)}$, and apply the inverse [Fourier transform](../../../analysis.md#fourier-transform). Repeating this [split-step Fourier method](../../../partial-differential-equation.md#split-step-fourier-method) $m$ times produces $E(x_m,z)$ from $E(x_0,z)$. The step size must continue to resolve both longitudinal medium variation and the [Lie-Trotter splitting](../../../numerical-analysis.md#lie-product-formula) error.

## 2

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use the sign convention in the question,

$$
V(\mathbf r)=k_0^2[n^2(\mathbf r)-1].
$$

Then the total field satisfies

$$
(\nabla^2+k_0^2)\psi=-V\psi.
$$

The outgoing free-space [Green function](../../../analysis.md#green-s-function) is

$$
G_0(\mathbf r-\mathbf r')
=\frac{e^{ik_0|\mathbf r-\mathbf r'|}}
{4\pi|\mathbf r-\mathbf r'|},
$$

with $(\nabla^2+k_0^2)G_0=-\delta$. Hence the [Lippmann-Schwinger equation](../../../quantum-mechanics.md#lippmann-schwinger-equation) is

$$
\psi(\mathbf r)=\psi_i(\mathbf r)
+\int_DG_0(\mathbf r-\mathbf r')
V(\mathbf r')\psi(\mathbf r')\,d^3r'.
$$

Replacing the unknown interior total field by the incident field gives the first [Born approximation](../../../quantum-theory.md#born-approximation)

$$
\boxed{
\psi_B(\mathbf r)=\psi_i(\mathbf r)
+\int_DG_0(\mathbf r-\mathbf r')
V(\mathbf r')\psi_i(\mathbf r')\,d^3r'}.
$$

For the [Rytov approximation](../../../inverse-problem.md#rytov-approximation), put $\psi=\psi_i e^\phi$. After division by $\psi$, the wave equation gives

$$
\nabla^2\phi+(\nabla\phi)^2
+2\nabla\log\psi_i\mathbin\cdot\nabla\phi
=-V.
$$

Neglecting the quadratic term $(\nabla\phi)^2$ makes $\psi_i\phi$ obey the same inhomogeneous equation as the first Born scattered field. Thus

$$
\phi_1(\mathbf r)
=\frac1{\psi_i(\mathbf r)}
\int_DG_0(\mathbf r-\mathbf r')
V(\mathbf r')\psi_i(\mathbf r')\,d^3r',
$$

and

$$
\boxed{
\psi_R(\mathbf r)=\psi_i(\mathbf r)e^{\phi_1(\mathbf r)}}.
$$

Its [power series](../../../real-analysis.md#power-series) begins

$$
\psi_R=\psi_i(1+\phi_1+O(\phi_1^2))
=\psi_B+O(V^2),
$$

so the two approximations agree through first order in the [scattering potential](../../../inverse-problem.md#scattering-potential).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let the incident plane wave be

$$
\psi_i(\mathbf r)
=e^{ik_0\widehat{\mathbf r}_0\cdot\mathbf r},
$$

and define the scattering vector

$$
\mathbf q=k_0
(\widehat{\mathbf r}-\widehat{\mathbf r}_0).
$$

For $r$ much larger than the diameter of $D$, the [far-field pattern](../../../inverse-problem.md#far-field-pattern) follows from

$$
G_0(\mathbf r-\mathbf r')
\sim\frac{e^{ik_0r}}{4\pi r}
e^{-ik_0\widehat{\mathbf r}\cdot\mathbf r'}.
$$

Writing

$$
\widetilde V(\mathbf q)
=\int_DV(\mathbf r')e^{-i\mathbf q\cdot\mathbf r'}\,d^3r',
$$

the Born result is

$$
\boxed{
\psi_B(\mathbf r)
\sim e^{ik_0\widehat{\mathbf r}_0\cdot\mathbf r}
+\frac{e^{ik_0r}}{4\pi r}
\widetilde V(\mathbf q)}.
$$

The corresponding Rytov logarithmic perturbation is

$$
\phi_1(\mathbf r)
\sim a(\mathbf r)\widetilde V(\mathbf q),
\qquad
a(\mathbf r)=
\frac{e^{ik_0(r-\widehat{\mathbf r}_0\cdot\mathbf r)}}
{4\pi r}.
$$

Therefore

$$
\boxed{
\psi_R(\mathbf r)
\sim e^{ik_0\widehat{\mathbf r}_0\cdot\mathbf r}
\exp\left[a(\mathbf r)\widetilde V(\mathbf q)\right]}.
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Since $n=1+W$ with small variance,

$$
V=k_0^2(2W+W^2)
=2k_0^2W+O(W^2).
$$

To leading order, $V$ is therefore a centered [stationary Gaussian random field](../../../stochastic-process.md#stationary-gaussian-random-field). Let its [autocorrelation function of a random field](../../../stochastic-process.md#autocorrelation-function-of-a-random-field) be

$$
C_V(\mathbf s)
=\left\langle
V(\mathbf r')V(\mathbf r'+\mathbf s)
\right\rangle.
$$

The $W^2$ contribution gives higher-order mean and non-Gaussian corrections and is consistently omitted at this order.

The far-field [Rytov approximation](../../../inverse-problem.md#rytov-approximation) from part ii has unit incident intensity and

$$
I(\mathbf r)
=\left\langle
e^{\phi_1+\phi_1^*}
\right\rangle,
\qquad
\phi_1=a\widetilde V(\mathbf q).
$$

The real random variable $X=\phi_1+\phi_1^*$ is centered Gaussian. Its [moment-generating function](../../../probability-theory.md#moment-generating-function) gives

$$
I=\exp\left(\frac12\langle X^2\rangle\right).
$$

Define

$$
J_-(\mathbf q)
=\int_D\int_D
C_V(\mathbf r_1-\mathbf r_2)
e^{-i\mathbf q\cdot(\mathbf r_1-\mathbf r_2)}
\,d^3r_1d^3r_2,
$$



$$
J_+(\mathbf q)
=\int_D\int_D
C_V(\mathbf r_1-\mathbf r_2)
e^{-i\mathbf q\cdot(\mathbf r_1+\mathbf r_2)}
\,d^3r_1d^3r_2.
$$

Then

$$
\langle|\phi_1|^2\rangle=|a|^2J_-,
\qquad
\langle\phi_1^2\rangle=a^2J_+,
$$

and hence

$$
\boxed{
I(\mathbf r)
=\exp\left\{
|a(\mathbf r)|^2J_-(\mathbf q)
+\operatorname{Re}
\left[a(\mathbf r)^2J_+(\mathbf q)\right]
\right\}}.
$$

This expression depends only on the two-point autocorrelation of the [scattering potential](../../../inverse-problem.md#scattering-potential). In the weak-fluctuation expansion it becomes

$$
\boxed{I=1+|a|^2J_-
+\operatorname{Re}(a^2J_+)
+O(C_V^2).}
$$

## 3

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $(\sigma_j,u_j,v_j)$ be a [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator) $A:X\to Y$, so

$$
Av_j=\sigma_ju_j,
\qquad
A^*u_j=\sigma_jv_j,
\qquad
\sigma_j>0.
$$

The [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) has domain

$$
\mathcal D(A^\dagger)
=\operatorname{ran}A\mathbin\oplus
(\operatorname{ran}A)^\perp
$$

and acts by

$$
\boxed{
A^\dagger y
=\sum_j\frac{\langle y,u_j\rangle}{\sigma_j}v_j},
$$

with the orthogonal component of $y$ sent to zero. Equivalently, its domain consists of the data satisfying the [Picard criterion](../../../inverse-problem.md#picard-criterion). It obeys

$$
AA^\dagger y=P_{\overline{\operatorname{ran}A}}y,
\qquad
A^\dagger Ax=P_{(\ker A)^\perp}x.
$$

If $Ax=y$ is exactly solvable, every solution is $x^\dagger+z$ with $z\in\ker A$, and

$$
\boxed{x^\dagger=A^\dagger y}
$$

is the unique [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution). It recovers the component of the original $x$ orthogonal to the null space; no data can determine the null-space component.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) is

$$
A^*Ax=A^*y.
$$

[Landweber iteration](../../../inverse-problem.md#landweber-iteration) is the stationary iteration

$$
\boxed{
x_{n+1}=x_n+\gamma A^*(y-Ax_n)
=(I-\gamma A^*A)x_n+\gamma A^*y}.
$$

A sufficient step-size condition is

$$
\boxed{0<\gamma<\frac2{\lVert A\rVert^2}}.
$$

If $y\in\mathcal D(A^\dagger)$ and $x_0\in(\ker A)^\perp$, then

$$
\boxed{x_n\longrightarrow A^\dagger y}.
$$

For an arbitrary initial iterate, its null-space component is unchanged and the limit is

$$
\boxed{A^\dagger y+P_{\ker A}x_0.}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For

$$
J(x)=\frac12\lVert Ax-y\rVert^2,
$$

the [Fréchet derivative](../../../calculus.md#frechet-derivative) in direction $h$ is

$$
J'(x)h
=\operatorname{Re}
\langle Ax-y,Ah\rangle_Y
=\operatorname{Re}
\langle A^*(Ax-y),h\rangle_X.
$$

Thus the Hilbert-space [gradient](../../../calculus.md#gradient) is

$$
\boxed{\nabla J(x)=A^*(Ax-y)}.
$$

The [gradient descent](../../../numerical-analysis.md#gradient-descent) update with step size $\gamma$ is consequently

$$
x_{n+1}=x_n-\gamma\nabla J(x_n)
=x_n+\gamma A^*(y-Ax_n),
$$

which is exactly [Landweber iteration](../../../inverse-problem.md#landweber-iteration). Its stationary points solve the normal equation and minimize the convex quadratic functional $J$.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Set

$$
B=I-\gamma A^*A.
$$

Starting from $x_0=0$, repeated substitution in [Landweber iteration](../../../inverse-problem.md#landweber-iteration) gives

$$
\boxed{
x_{n+1}
=\gamma\sum_{k=0}^{n}
(I-\gamma A^*A)^kA^*y}.
$$

This is the finite partial sum of a [Neumann series](../../../banach-algebra.md#neumann-series). Whenever $A^*A$ is boundedly invertible on the relevant subspace and $\lVert I-\gamma A^*A\rVert<1$,

$$
\boxed{
(A^*A)^{-1}
=\gamma\sum_{k=0}^{\infty}
(I-\gamma A^*A)^k},
$$

so

$$
x_{n+1}\longrightarrow
(A^*A)^{-1}A^*y=A^\dagger y.
$$

For a genuinely compact operator on an infinite-dimensional space, nonzero singular values can accumulate at zero, so this inverse is generally unbounded and the Neumann series need not converge in operator norm. Under the condition in part ii it nevertheless converges componentwise on admissible data to the [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator); stopping after finitely many terms suppresses poorly determined small-singular-value components and acts as a [regularization of an inverse problem](../../../inverse-problem.md#regularization-of-an-inverse-problem).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
