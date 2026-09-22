# Paper 3

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperib_3_2024.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperib_3_2024.pdf)

**Table of contents**

- [1E](#1e)
  - [i](#1e/i)
    - [Solution](#1e/i/solution)
  - [ii](#1e/ii)
    - [Solution](#1e/ii/solution)
  - [iii](#1e/iii)
    - [Solution](#1e/iii/solution)
- [2G](#2g)
  - [Solution](#2g/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
- [6A](#6a)
  - [i](#6a/i)
    - [Solution](#6a/i/solution)
  - [ii](#6a/ii)
    - [Solution](#6a/ii/solution)
  - [iii](#6a/iii)
    - [Solution](#6a/iii/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
- [8H](#8h)
  - [i](#8h/i)
    - [Solution](#8h/i/solution)
  - [ii](#8h/ii)
    - [Solution](#8h/ii/solution)
  - [iii](#8h/iii)
    - [Solution](#8h/iii/solution)
- [9G](#9g)
  - [Solution](#9g/solution)
  - [a](#9g/a)
    - [Solution](#9g/a/solution)
  - [b](#9g/b)
    - [Solution](#9g/b/solution)
  - [c](#9g/c)
    - [Solution](#9g/c/solution)
  - [d](#9g/d)
    - [Solution](#9g/d/solution)
- [10E](#10e)
  - [a](#10e/a)
    - [i](#10e/a/i)
      - [Solution](#10e/a/i/solution)
    - [ii](#10e/a/ii)
      - [Solution](#10e/a/ii/solution)
  - [b](#10e/b)
    - [i](#10e/b/i)
      - [Solution](#10e/b/i/solution)
    - [ii](#10e/b/ii)
      - [Solution](#10e/b/ii/solution)
  - [c](#10e/c)
    - [Solution](#10e/c/solution)
- [11F](#11f)
  - [a](#11f/a)
    - [Solution](#11f/a/solution)
  - [b](#11f/b)
    - [Solution](#11f/b/solution)
- [12E](#12e)
  - [Solution](#12e/solution)
- [13F](#13f)
  - [Solution](#13f/solution)
- [14B](#14b)
  - [Solution](#14b/solution)
- [15C](#15c)
  - [Solution](#15c/solution)
- [16D](#16d)
  - [Solution](#16d/solution)
- [17A](#17a)
  - [Solution](#17a/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
  - [d](#18h/d)
    - [i](#18h/d/i)
      - [Solution](#18h/d/i/solution)
    - [ii](#18h/d/ii)
      - [Solution](#18h/d/ii/solution)
- [19H](#19h)
  - [a](#19h/a)
    - [Solution](#19h/a/solution)
  - [b](#19h/b)
    - [i](#19h/b/i)
      - [Solution](#19h/b/i/solution)
    - [ii](#19h/b/ii)
      - [Solution](#19h/b/ii/solution)

## 1E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1e/i">i</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/i/solution">Solution</h4>

↑ **Parent:** [I](#1e/i)

The [Smith normal form](../../../algebra.md#smith-normal-form) of an integer $m\times n$ [matrix](../../../vector-space.md#matrix) $A$ is a diagonal [matrix](../../../vector-space.md#matrix)

$$
D=\operatorname{diag}(d_1,\ldots,d_r,0,\ldots,0),
\qquad d_i>0,
\qquad d_i\mid d_{i+1},
$$

for which

$$
UAV=D
$$

with $U\in GL_m(\mathbb Z)$ and $V\in GL_n(\mathbb Z)$. It exists and is unique.

The [structure theorem for finitely generated modules over a principal ideal domain](../../../module-theory.md#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain), specialized to $\mathbb Z$, says that every finitely generated abelian [group](../../../group.md) has a unique invariant-factor decomposition

$$
M\cong\mathbb Z^s\oplus
\mathbb Z/d_1\mathbb Z\oplus\cdots\oplus
\mathbb Z/d_r\mathbb Z,
\qquad
1<d_1\mid\cdots\mid d_r.
$$

Equivalently, its finite part is a direct sum of cyclic [groups](../../../group.md) of prime-power order.

<h3 id="1e/ii">ii</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1e/ii)

Integer row and column operations give

$$
\begin{pmatrix}-4&-6\\2&2\end{pmatrix}
\sim
\begin{pmatrix}2&2\\-4&-6\end{pmatrix}
\sim
\begin{pmatrix}2&2\\0&-2\end{pmatrix}
\sim
\begin{pmatrix}2&0\\0&2\end{pmatrix}.
$$

Thus the Smith normal form is

$$
\boxed{\operatorname{diag}(2,2)}.
$$

The two relation [vectors](../../../vector-space.md#vector) are the columns of the displayed [matrix](../../../vector-space.md#matrix), so its cokernel is the presented module. Consequently

$$
\boxed{M\cong\mathbb Z/2\mathbb Z\oplus\mathbb Z/2\mathbb Z}.
$$

<h3 id="1e/iii">iii</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1e/iii)

By the finite case of the structure theorem, a finite abelian [group](../../../group.md) is a direct sum of cyclic [groups](../../../group.md) of prime-power order. If it is indecomposable, this decomposition can have only one nonzero summand, so the [group](../../../group.md) is cyclic of order $p^n$ for some prime $p$.

Conversely, every nontrivial [subgroup](../../../group.md#subgroup) of the cyclic [group](../../../group.md) $C_{p^n}$ contains its unique [subgroup](../../../group.md#subgroup) of order $p$. Hence two nontrivial [subgroups](../../../group.md#subgroup) cannot have trivial intersection. They therefore cannot be the two summands of an internal direct sum. Thus the [indecomposable finite abelian groups](../../../module-theory.md#indecomposable-finite-abelian-groups) are precisely

$$
\boxed{C_{p^n}\quad(n\geq1)}.
$$

## 2G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2g/solution">Solution</h3>

↑ **Parent:** [2G](#2g)

Use the global parametrization

$$
X(u,v)=(u,v,h(u,v)).
$$

Its [tangent vectors](../../../differential-geometry.md#tangent-vector) are

$$
X_u=(1,0,h_u),
\qquad
X_v=(0,1,h_v),
$$

and

$$
X_u\times X_v=(-h_u,-h_v,1)\ne0.
$$

Thus $X$ is a regular parametrization and the graph is a smooth surface.

The [first fundamental form](../../../differential-geometry.md#first-fundamental-form) is

$$
\boxed{
I=(1+h_u^2)\,du^2+2h_uh_v\,du\,dv+(1+h_v^2)\,dv^2}.
$$

Choosing the upward orientation, the [Gauss map](../../../differential-geometry.md#gauss-map) is

$$
\boxed{
N(u,v)=\frac{(-h_u,-h_v,1)}
{\sqrt{1+h_u^2+h_v^2}}}.
$$

## 3B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

The [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) states that if $f$ is holomorphic on a simply connected domain, then its [integral](../../../calculus.md#integral) around every closed piecewise smooth contour in that domain is zero.

Put $q=b-k$. Completing the square gives

$$
-ax^2+iqx
=-a\left(x-\frac{iq}{2a}\right)^2-
\frac{q^2}{4a}.
$$

After the change of variable $z=x-iq/(2a)$, the [integral](../../../calculus.md#integral) runs along the horizontal line $\operatorname{Im}z=-q/(2a)$. The integrand $e^{-az^2}$ is entire. Apply Cauchy's theorem to a rectangle joining this line to the real axis; the two vertical [integrals](../../../calculus.md#integral) tend to zero as their real parts tend to $\pm\infty$, because $a>0$. The contour may therefore be shifted to the real line. Hence the [Fourier transform of a Gaussian](../../../fourier-analysis.md#fourier-transform-of-a-gaussian) gives

$$
\begin{aligned}
\widehat f_{a,b}(k)
&=e^{-q^2/(4a)}\int_{-\infty}^{\infty}e^{-az^2}\,dz\\
&=\boxed{\sqrt{\frac\pi a}
\exp\left[-\frac{(k-b)^2}{4a}\right]}.
\end{aligned}
$$

## 4C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

For a general [Lagrangian](../../../calculus-of-variations.md#lagrangian),

$$
p=\frac{\partial L}{\partial\dot x},
\qquad
H=p\cdot\dot x-L.
$$

Along an Euler-Lagrange trajectory,

$$
\frac{dH}{dt}=-\frac{\partial L}{\partial t},
$$

so energy is conserved when $L$ has no explicit time dependence.

For the given [Lagrangian](../../../calculus-of-variations.md#lagrangian), write $v=|\dot x|$. At points where $v\ne0$,

$$
\boxed{p=mc\frac{\dot x}{v}}.
$$

The Euler-Lagrange equation is therefore

$$
\boxed{
\frac d{dt}\left(mc\frac{\dot x}{|\dot x|}\right)
=-\nabla V(x)}.
$$

In expanded form its left-hand side is

$$
mc\left(
\frac{\ddot x}{v}
-\frac{\dot x(\dot x\cdot\ddot x)}{v^3}
\right).
$$

The [momentum](../../../classical-mechanics.md#momentum) has fixed magnitude,

$$
\boxed{p\cdot p=m^2c^2},
$$

so this is constant without needing to solve the equation of motion. The [Hamiltonian](../../../classical-mechanics.md#hamiltonian) is

$$
\boxed{H=p\cdot\dot x-L=V(x)}.
$$

The [singular Legendre transform of a degree-one velocity Lagrangian](../../../classical-mechanics.md#singular-legendre-transform-of-a-degree-one-velocity-lagrangian) applies here: $p$ determines only the direction of $\dot x$, not its magnitude, and the [velocity](../../../classical-mechanics.md#velocity) Hessian is not invertible. Thus the usual inverse Legendre transform cannot reconstruct the [Lagrangian](../../../calculus-of-variations.md#lagrangian) from this [Hamiltonian](../../../classical-mechanics.md#hamiltonian).

## 5B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

Set $u(r,\theta)=R(r)\Theta(\theta)$. Periodicity and [separation of variables](../../../partial-differential-equation.md#separation-of-variables) give the angular modes $1$, $\cos n\theta$, and $\sin n\theta$. The radial equation is

$$
r^2R''+rR'-n^2R=0,
$$

whose solutions are $r^{\pm n}$ for $n\geq1$; the zero mode has solutions $1$ and $\log r$. Thus a general real harmonic [function](../../../function.md) on the annulus is

$$
\begin{aligned}
u(r,\theta)={}&A_0+B_0\log r\\
&+\sum_{n=1}^{\infty}
\left(A_nr^n+B_nr^{-n}\right)\cos n\theta\\
&+\sum_{n=1}^{\infty}
\left(C_nr^n+D_nr^{-n}\right)\sin n\theta.
\end{aligned}
$$

The boundary data contain only the $n=2$ cosine mode, so write

$$
u=(Ar^2+Br^{-2})\cos2\theta.
$$

The condition at $r=a$ gives $B=-Aa^4$, and the condition at $r=b$ fixes $A$. The [Dirichlet problem on an annulus for one Fourier mode](../../../partial-differential-equation.md#dirichlet-problem-on-an-annulus-for-one-fourier-mode) therefore has solution

$$
\boxed{
u(r,\theta)=
\frac{b^2(r^4-a^4)}{r^2(b^4-a^4)}\cos2\theta}.
$$

## 6A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6a/i">i</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/i/solution">Solution</h4>

↑ **Parent:** [I](#6a/i)

The [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) is

$$
\boxed{[x,p]=i\hbar I}.
$$

<h3 id="6a/ii">ii</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6a/ii)

For a normalized state, the uncertainty of a Hermitian [observable](../../../quantum-mechanics.md#observable) $O$ is

$$
\boxed{
\Delta O=\sqrt{\langle O^2\rangle-\langle O\rangle^2}}.
$$

<h3 id="6a/iii">iii</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6a/iii)

Positivity of the squared norm of the supplied state gives, for every real $s$,

$$
\begin{aligned}
0&\leq\lVert(p-isx)\psi\rVert^2\\
&=\langle(p+isx)(p-isx)\rangle\\
&=\langle p^2\rangle+s^2\langle x^2\rangle
+is\langle[x,p]\rangle\\
&=(\Delta p)^2+s^2(\Delta x)^2-s\hbar,
\end{aligned}
$$

where the stated zero means were used in the last line. This quadratic in $s$ is nonnegative for every real $s$, so its discriminant is nonpositive:

$$
\hbar^2-4(\Delta x)^2(\Delta p)^2\leq0.
$$

This is the [quadratic-norm proof of the Heisenberg uncertainty relation](../../../quantum-theory.md#quadratic-norm-proof-of-the-heisenberg-uncertainty-relation), and proves

$$
\boxed{\Delta x\,\Delta p\geq\frac\hbar2}.
$$

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

The steady [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) are

$$
\rho(u\cdot\nabla)u=-\nabla p-\nabla\chi.
$$

Taking the [scalar](../../../vector-space.md#scalar) product with $u$ and using

$$
u\cdot(u\cdot\nabla u)
=u\cdot\nabla\left(\frac12|u|^2\right)
$$

gives

$$
u\cdot\nabla
\left(\frac12\rho|u|^2+p+\chi\right)=0.
$$

Thus

$$
\boxed{u\cdot\nabla H=0}.
$$

The [Bernoulli function](../../../fluid-mechanics.md#bernoulli-function) $H$ is constant along each [streamline](../../../fluid-mechanics.md#streamline): fluid particles in steady flow exchange [pressure](../../../thermodynamics.md#pressure), kinetic, and [potential energy](../../../classical-mechanics.md#potential-energy) without changing their total mechanical energy density.

Let $y(t)$ be the downward displacement of the free surface from its initial level, and let $U$ be the speed in the tube. Conservation of volume gives

$$
aU=A\dot y.
$$

The free surface and the outlet are both at atmospheric [pressure](../../../thermodynamics.md#pressure), and their vertical separation is $H+h_0-y$. Applying the [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) between them, while retaining the small free-surface speed, gives

$$
\frac12\left(U^2-\dot y^2\right)
=g(H+h_0-y).
$$

Therefore

$$
\dot y=
\sqrt{\frac{2g(H+h_0-y)}{A^2/a^2-1}}.
$$

The surface reaches the upper tube end when $y=h_0$. Hence the [draining time of a uniform tank through a siphon](../../../fluid-mechanics.md#draining-time-of-a-uniform-tank-through-a-siphon) is

$$
\begin{aligned}
t
&=\sqrt{\frac{A^2/a^2-1}{2g}}
\int_0^{h_0}\frac{dy}{\sqrt{H+h_0-y}}\\
&=\boxed{
\sqrt{2}\left(\frac{A^2}{a^2}-1\right)^{1/2}
\frac{\sqrt{H+h_0}-\sqrt H}{\sqrt g}}.
\end{aligned}
$$

## 8H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8h/i">i</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/i/solution">Solution</h4>

↑ **Parent:** [I](#8h/i)

The independent identically distributed [sequence](../../../real-analysis.md#sequence) $(X_n)$ is itself a [Markov chain](../../../markov-process.md#markov-chain), since the conditional law of $X_{n+1}$ is its common marginal law and does not depend on the past.

Also,

$$
S_{n+1}=S_n+X_{n+1}.
$$

Because $X_{n+1}$ is independent of the past, the conditional law of $S_{n+1}$ depends on the history only through $S_n$. Thus the partial sums $(S_n)$ are a Markov chain.

<h3 id="8h/ii">ii</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8h/ii)

The running minima satisfy

$$
L_{n+1}=\min\{L_n,X_{n+1}\}.
$$

Since $X_{n+1}$ is independent of the past, the conditional law of $L_{n+1}$ depends only on $L_n$. Hence $(L_n)$ is a Markov chain. This is the [running minimum of an independent sequence is Markov](../../../markov-process.md#running-minimum-of-an-independent-sequence-is-markov) property.

<h3 id="8h/iii">iii</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8h/iii)

The moving sums $(K_n)$ are not necessarily Markov. For a counterexample, let the $X_n$ be independent Bernoulli variables with parameter $1/2$. On the event

$$
K_n=1,
\qquad K_{n-1}=0,
$$

we must have $X_{n-1}=0$ and $X_n=1$, so

$$
\mathbb P(K_{n+1}=2\mid K_n=1,K_{n-1}=0)=\frac12.
$$

On the other hand, $K_n=1$ and $K_{n-1}=2$ force $X_{n-1}=1$ and $X_n=0$, whence

$$
\mathbb P(K_{n+1}=2\mid K_n=1,K_{n-1}=2)=0.
$$

Both conditioning events have positive probability. Knowledge of $K_n$ alone therefore does not determine the next-step law. The [overlapping moving sum need not be Markov](../../../markov-process.md#overlapping-moving-sum-need-not-be-markov).

## 9G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9g/solution">Solution</h3>

↑ **Parent:** [9G](#9g)

Fix $y\in V$. The map $x\mapsto\theta(x,y)$ is a linear functional, so the finite-dimensional [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem) gives a unique [vector](../../../vector-space.md#vector) $\beta(y)$ such that

$$
\theta(x,y)=\langle x,\beta(y)\rangle
\qquad(x\in V).
$$

For [scalars](../../../vector-space.md#scalar) $\lambda,\mu$,

$$
\begin{aligned}
\langle x,\beta(\lambda y+\mu z)\rangle
&=\theta(x,\lambda y+\mu z)\\
&=\overline\lambda\,\theta(x,y)
 +\overline\mu\,\theta(x,z)\\
&=\langle x,\lambda\beta(y)+\mu\beta(z)\rangle.
\end{aligned}
$$

Uniqueness gives

$$
\boxed{\beta(\lambda y+\mu z)=\lambda\beta(y)+\mu\beta(z)},
$$

so $\beta$ is linear.

For $\alpha\in\operatorname{End}(V)$, apply this result to

$$
\theta(x,y)=\langle\alpha x,y\rangle.
$$

It produces a unique [linear map](../../../vector-space.md#linear-map) $\alpha^*$ satisfying

$$
\boxed{\langle\alpha x,y\rangle=\langle x,\alpha^*y\rangle},
$$

which proves existence and uniqueness of the adjoint.

<h3 id="9g/a">a</h3>

↑ **Parent:** [9G](#9g)

<h4 id="9g/a/solution">Solution</h4>

↑ **Parent:** [A](#9g/a)

Suppose first that $\alpha(U)\subseteq U$. If $y\in U^\perp$ and $u\in U$, then

$$
\langle u,\alpha^*y\rangle
=\langle\alpha u,y\rangle=0.
$$

Thus $\alpha^*(U^\perp)\subseteq U^\perp$.

Conversely, assume that latter inclusion. For $u\in U$ and $y\in U^\perp$,

$$
\langle\alpha u,y\rangle
=\langle u,\alpha^*y\rangle=0.
$$

Hence $\alpha u\in(U^\perp)^\perp=U$. This proves the [adjoint criterion for an invariant orthogonal complement](../../../hilbert-space.md#adjoint-criterion-for-an-invariant-orthogonal-complement):

$$
\boxed{\alpha(U)\subseteq U
\iff \alpha^*(U^\perp)\subseteq U^\perp}.
$$

<h3 id="9g/b">b</h3>

↑ **Parent:** [9G](#9g)

<h4 id="9g/b/solution">Solution</h4>

↑ **Parent:** [B](#9g/b)

Write $B(x,y)=\langle\alpha x,y\rangle$. The hypothesis says $B(x,x)=0$. Expanding at $x+y$ gives

$$
B(x,y)+B(y,x)=0,
$$

whereas expanding at $x+iy$ gives

$$
-iB(x,y)+iB(y,x)=0.
$$

Therefore $B(x,y)=0$ for every $x,y$, so

$$
\boxed{\alpha=0}.
$$

This is the complex [polarization argument for a vanishing quadratic form](../../../linear-algebra.md#polarization-argument-for-a-vanishing-quadratic-form).

The conclusion is false over a real [inner product](../../../linear-algebra.md#inner-product) space. On $\mathbb R^2$, the nonzero operator

$$
J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}
$$

satisfies $\langle Jx,x\rangle=0$ for every $x$.

<h3 id="9g/c">c</h3>

↑ **Parent:** [9G](#9g)

<h4 id="9g/c/solution">Solution</h4>

↑ **Parent:** [C](#9g/c)

For every $x$,

$$
\|\alpha x\|^2=\langle x,\alpha^*\alpha x\rangle,
\qquad
\|\alpha^*x\|^2=\langle x,\alpha\alpha^*x\rangle.
$$

If $\alpha$ is normal, these quantities are equal. Conversely, equality of the norms for all $x$ gives

$$
\langle x,(\alpha^*\alpha-\alpha\alpha^*)x\rangle=0.
$$

The operator in parentheses is self-adjoint, so polarization makes it zero. Therefore

$$
\boxed{\alpha\alpha^*=\alpha^*\alpha
\iff \|\alpha x\|=\|\alpha^*x\|\quad\hbox{for all }x}.
$$

The same equivalence holds over a real [inner product](../../../linear-algebra.md#inner-product) space: for a self-adjoint operator $T$, the real polarization identity

$$
4\langle Tx,y\rangle
=\langle T(x+y),x+y\rangle
-\langle T(x-y),x-y\rangle
$$

shows that a vanishing quadratic form forces $T=0$.

<h3 id="9g/d">d</h3>

↑ **Parent:** [9G](#9g)

<h4 id="9g/d/solution">Solution</h4>

↑ **Parent:** [D](#9g/d)

Proceed by induction on $\dim V$. Over $\mathbb C$, $\alpha$ has an [eigenvector](../../../linear-operator-theory.md#eigenvector) $v$, say $\alpha v=\lambda v$. The normal operator $\alpha-\lambda I$ satisfies the norm equality from part (c), so

$$
\|(\alpha^*-\overline\lambda I)v\|
=\|(\alpha-\lambda I)v\|=0.
$$

Thus $\alpha^*v=\overline\lambda v$. Part (a) now shows that $v^\perp$ is invariant under both $\alpha$ and $\alpha^*$. The restriction of $\alpha$ to $v^\perp$ is normal. By induction it has an orthonormal eigenbasis, and adjoining the normalized [vector](../../../vector-space.md#vector) $v$ proves the finite-dimensional [spectral theorem for normal operators](../../../hilbert-space.md#spectral-theorem-for-normal-operators).

Hence

$$
\boxed{V\text{ has an orthonormal basis of eigenvectors of }\alpha}.
$$

## 10E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10e/a">a</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/a/i">i</h4>

↑ **Parent:** [A](#10e/a)

<h5 id="10e/a/i/solution">Solution</h5>

↑ **Parent:** [I](#10e/a/i)

Suppose $I$ is prime. If

$$
(a+I)(b+I)=0+I,
$$

then $ab\in I$, so $a\in I$ or $b\in I$. Thus one factor is zero and $R/I$ is an [integral](../../../calculus.md#integral) domain.

Conversely, if $R/I$ is an [integral](../../../calculus.md#integral) domain and $ab\in I$, then

$$
(a+I)(b+I)=0+I,
$$

so $a+I=0+I$ or $b+I=0+I$. Therefore $a\in I$ or $b\in I$, and $I$ is prime. This proves the [prime ideal quotient criterion](../../../commutative-algebra.md#prime-ideal-quotient-criterion).

<h4 id="10e/a/ii">ii</h4>

↑ **Parent:** [A](#10e/a)

<h5 id="10e/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10e/a/ii)

In a Boolean [ring](../../../commutative-algebra.md#ring), $(r+1)^2=r+1$. Using $r^2=r$ and $1^2=1$ gives

$$
r+2r+1=r+1,
$$

so

$$
\boxed{2r=0\quad\text{for every }r\in R}.
$$

If $R$ is also a nonzero [integral](../../../calculus.md#integral) domain, then

$$
r(r-1)=r^2-r=0
$$

forces every $r$ to equal $0$ or $1$. Hence $R\cong\mathbb F_2$.

If $I$ is prime in a Boolean [ring](../../../commutative-algebra.md#ring), then $R/I$ is a nonzero Boolean [integral](../../../calculus.md#integral) domain by part (i), and hence is $\mathbb F_2$. Since the quotient is a field,

$$
\boxed{I\text{ is maximal}}.
$$

This is the [prime ideals of a Boolean ring are maximal](../../../commutative-algebra.md#prime-ideals-of-a-boolean-ring-are-maximal) property.

<h3 id="10e/b">b</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/b/i">i</h4>

↑ **Parent:** [B](#10e/b)

<h5 id="10e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#10e/b/i)

Reduce coefficients modulo $I$:

$$
\Phi:R[X]\longrightarrow(R/I)[X],
\qquad
\sum_ka_kX^k\longmapsto\sum_k(a_k+I)X^k.
$$

This is a surjective [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism) and its kernel consists exactly of [polynomials](../../../polynomial.md) all of whose coefficients lie in $I$, namely $I[X]$. The first isomorphism theorem gives the [coefficientwise quotient of a polynomial ring](../../../commutative-algebra.md#coefficientwise-quotient-of-a-polynomial-ring)

$$
\boxed{R[X]/I[X]\cong(R/I)[X]}.
$$

If $I$ is prime, then $R/I$ is an [integral](../../../calculus.md#integral) domain, so $(R/I)[X]$ is an [integral](../../../calculus.md#integral) domain. The quotient criterion therefore shows that $I[X]$ is prime in $R[X]$.

<h4 id="10e/b/ii">ii</h4>

↑ **Parent:** [B](#10e/b)

<h5 id="10e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10e/b/ii)

Take $R=\mathbb Z$ and $I=(2)$. The [ideal](../../../commutative-algebra.md#ideal) $I$ is maximal, but

$$
\mathbb Z[X]/I[X]\cong\mathbb F_2[X]
$$

is not a field, since $X$ is nonzero and not invertible. Therefore

$$
\boxed{I[X]\text{ need not be maximal}}.
$$

<h3 id="10e/c">c</h3>

↑ **Parent:** [10E](#10e)

<h4 id="10e/c/solution">Solution</h4>

↑ **Parent:** [C](#10e/c)

Let $G=\mathbb F_p^\times$, and let $m$ be the least common multiple of the orders of its elements. For every prime power $q^a$ dividing $m$, some element of $G$ has order divisible by $q^a$, and a suitable power of it has order exactly $q^a$. Multiplying these elements over the distinct primes produces, because their orders are coprime, an element of order $m$.

Every element of $G$ is a root of $X^m-1$. A nonzero [polynomial](../../../polynomial.md) of degree $m$ over a field has at most $m$ roots, so $p-1\leq m$. On the other hand, every element order divides $p-1$ by Lagrange's theorem, so $m\leq p-1$. Hence $m=p-1$, and

$$
\boxed{\mathbb F_p^\times\text{ is cyclic}}.
$$

The squaring homomorphism has kernel $\{1,-1\}$ because $p$ is odd. Its image $H$ therefore has order $(p-1)/2$ and index two. If $p=3$, then $3=0$ is already a square. Otherwise $2,3\in G$. In the two-element quotient $G/H$, either $2H=H$, or $3H=H$, or both are the nontrivial coset, in which case $6H=H$. Thus one of $2,3,6$ is a square modulo $p$.

Finally,

$$
f(x)=(x^2-2)(x^2-3)(x^2-6).
$$

Whichever of $2,3,6$ is a square supplies a root, so

$$
\boxed{f\text{ has a root in }\mathbb F_p}.
$$

This is the [index-two square-class argument for three related residues](../../../algebra.md#index-two-square-class-argument-for-three-related-residues).

## 11F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11f/a">a</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/a/solution">Solution</h4>

↑ **Parent:** [A](#11f/a)

A [function](../../../function.md) $f:(X,d_X)\to(Y,d_Y)$ is uniformly continuous if for every $\varepsilon>0$ there is $\delta>0$ such that

$$
d_X(x,x')<\delta
\implies d_Y(f(x),f(x'))<\varepsilon
$$

for all $x,x'\in X$.

Suppose $f_n\to f$ uniformly and every $f_n$ is uniformly continuous. Given $\varepsilon>0$, choose $N$ such that

$$
d_Y(f_N(x),f(x))<\varepsilon/3
$$

for every $x$. Uniform continuity of $f_N$ supplies $\delta>0$ such that $d_X(x,x')<\delta$ implies

$$
d_Y(f_N(x),f_N(x'))<\varepsilon/3.
$$

The triangle inequality then gives $d_Y(f(x),f(x'))<\varepsilon$. Thus the [uniform limit theorem for uniformly continuous functions](../../../topological-analysis.md#uniform-limit-theorem-for-uniformly-continuous-functions) proves that $f$ is uniformly continuous.

[Pointwise convergence](../../../real-analysis.md#pointwise-convergence) is insufficient. On $[0,1]$, the uniformly [continuous functions](../../../calculus.md#continuous-function) $f_n(x)=x^n$ converge pointwise to

$$
f(x)=\begin{cases}0,&0\leq x<1,\\1,&x=1,\end{cases}
$$

which is discontinuous and therefore not uniformly continuous.

<h3 id="11f/b">b</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/b/solution">Solution</h4>

↑ **Parent:** [B](#11f/b)

The inequalities imply

$$
B_{d_1}(x,r/\beta)\subseteq B_{d_2}(x,r)
\quad\text{and}\quad
B_{d_2}(x,\alpha r)\subseteq B_{d_1}(x,r).
$$

Thus the two metrics induce the same [open sets](../../../topology.md#open-set) and are equivalent.

The converse fails. On $\mathbb R$, let

$$
d_1(x,y)=|x-y|,
\qquad
d_2(x,y)=|\arctan x-\arctan y|.
$$

The metrics are equivalent because $\arctan:\mathbb R\to(-\pi/2,\pi/2)$ is a homeomorphism, but

$$
\frac{d_2(0,n)}{d_1(0,n)}\longrightarrow0,
$$

so no positive lower comparison constant exists. This is an [equivalent metrics need not be bi-Lipschitz equivalent](../../../topological-analysis.md#equivalent-metrics-need-not-be-bi-lipschitz-equivalent) example.

Equivalent metrics on the codomain also need not give the same [uniform convergence](../../../real-analysis.md#uniform-convergence). Take $X=\mathbb N$, $Y=\mathbb R$, and use the two metrics above. Define

$$
f(k)=k,
\qquad
f_n(k)=\begin{cases}2n,&k=n,\\k,&k\ne n.
\end{cases}
$$

Then

$$
\sup_kd_2(f_n(k),f(k))
=\arctan(2n)-\arctan n\longrightarrow0,
$$

so $f_n\to f$ uniformly for $d_2$, whereas

$$
\sup_kd_1(f_n(k),f(k))=n,
$$

so convergence is not uniform for $d_1$. This is the [equivalent codomain metrics need not preserve uniform convergence](../../../topological-analysis.md#equivalent-codomain-metrics-need-not-preserve-uniform-convergence) phenomenon.

## 12E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12e/solution">Solution</h3>

↑ **Parent:** [12E](#12e)

In polar coordinates the metric is

$$
ds^2=\frac{4(dr^2+r^2d\theta^2)}{(1-r^2)^2}.
$$

Along a radius, the hyperbolic distance from the origin to Euclidean radius $r$ is therefore

$$
R=\int_0^r\frac{2\,dt}{1-t^2}
=\log\frac{1+r}{1-r},
$$

so $r=\tanh(R/2)$. The Riemannian area element is

$$
dA=\frac{4r}{(1-r^2)^2}\,dr\,d\theta.
$$

Consequently a hyperbolic disc of radius $R$ has area

$$
\begin{aligned}
A(R)
&=\int_0^{2\pi}\int_0^{\tanh(R/2)}
\frac{4r}{(1-r^2)^2}\,dr\,d\theta\\
&=4\pi\sinh^2(R/2)
=2\pi(\cosh R-1).
\end{aligned}
$$

This proves the [area of a hyperbolic disc](../../../geometry-and-topology.md#area-of-a-hyperbolic-disc) formula from the metric.

For area $\pi/2$ we get $\cosh R=5/4$. Hence $\sinh R=3/4$ and $e^R=2$, so $R=\log2$. Tangent equal discs have centers at distance $2R$. Since the centers lie successively on the same radial geodesic,

$$
d(O,c_n)=2nR=n\log4.
$$

If $r_n$ is the Euclidean coordinate of $c_n$, the radial distance formula gives

$$
\frac{1+r_n}{1-r_n}=4^n.
$$

Therefore the [radial chain of equal hyperbolic discs](../../../geometry-and-topology.md#radial-chain-of-equal-hyperbolic-discs) has

$$
\boxed{r_n=\frac{4^n-1}{4^n+1}}.
$$

**No such isometry to the stated upper-half-plane configuration exists for $n\geq3$.** The centers $c_0,\ldots,c_n$ lie on one hyperbolic geodesic, so their images under an isometry would also lie on one geodesic. In the upper-half-plane model, geodesics are vertical lines or semicircles orthogonal to the real axis. Neither type can contain three distinct points of the horizontal line $y=1$, while the centers of the distinct discs $D'_0,\ldots,D'_n$ all lie on that line. This is the [geodesic obstruction for a horizontal chain of hyperbolic discs](../../../geometry-and-topology.md#geodesic-obstruction-for-a-horizontal-chain-of-hyperbolic-discs).

## 13F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="13f/solution">Solution</h3>

↑ **Parent:** [13F](#13f)

For a closed piecewise [smooth curve](../../../differential-geometry.md#smooth-curve) $\gamma$ avoiding $w$, its [winding number](../../../complex-analysis.md#winding-number) about $w$ is

$$
\boxed{
\operatorname{wind}(\gamma,w)
=\frac1{2\pi i}\int_\gamma\frac{dz}{z-w}}.
$$

The [argument principle](../../../complex-analysis.md#argument-principle) says that if a positively oriented closed curve $\gamma$ bounds a domain $U$, and a meromorphic [function](../../../function.md) $F$ has no zeros or poles on $\gamma$, then

$$
\boxed{
\frac1{2\pi i}\int_\gamma\frac{F'(z)}{F(z)}\,dz
=N_U(F)-P_U(F)},
$$

where zeros and poles are counted with multiplicity.

Suppose $F$ and $G$ are holomorphic on a neighbourhood of $\overline U$ and

$$
|G(z)|<|F(z)|
\qquad(z\in\gamma).
$$

For $0\leq t\leq1$, $F+tG$ has no boundary zero, because a zero would imply $|F|=t|G|<|F|$. Its argument-principle count is integer-valued and continuous in $t$, hence constant. Thus [Rouché's theorem](../../../complex-analysis.md#rouche-s-theorem) states that

$$
\boxed{F\text{ and }F+G\text{ have the same number of zeros in }U}.
$$

Now let $w_0=f(z_0)$. Since $|w_0|<1\leq|f|$ on the unit circle, Rouché's theorem shows that $f$ and $f-w_0$ have the same number of zeros in the unit disc. The latter has the zero $z_0$, so $f$ has at least one zero there. For any $w$ with $|w|<1$, the same boundary inequality shows that $f-w$ has the same positive number of zeros as $f$. Therefore

$$
\boxed{\mathbb D\subseteq f(\mathbb D)}.
$$

This is the [unit-disc image from a boundary modulus lower bound](../../../complex-analysis.md#unit-disc-image-from-a-boundary-modulus-lower-bound).

Finally, take a sufficiently small positively oriented circle $C$ around zero. The residue

$$
k=\operatorname{res}_{0}\frac{g'}g
=\frac1{2\pi i}\int_C\frac{g'}g\,dz
$$

is the winding number of $g(C)$ around zero, so $k\in\mathbb Z$. The pole is simple, hence its residue is nonzero and $k\ne0$. For

$$
h(z)=z^{-k}g(z)
$$

we have

$$
\frac{h'}h=\frac{g'}g-\frac{k}{z}.
$$

The second term cancels the complete principal part at zero, so the [integer residue of a logarithmic derivative](../../../complex-analysis.md#integer-residue-of-a-logarithmic-derivative) proves that $h'/h$ has a removable singularity there.

## 14B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="14b/solution">Solution</h3>

↑ **Parent:** [14B](#14b)

Separation $y=T(t)X(x)$ and the fixed-end conditions give

$$
X_n(x)=\sin(n\pi x),
\qquad
T_n''+T_n'+n^2\pi^2T_n=0.
$$

Put

$$
\omega_n=\sqrt{n^2\pi^2-\frac14}.
$$

The initial displacement and zero initial [velocity](../../../classical-mechanics.md#velocity) then give the [separated solution of the damped string equation](../../../wave-equation.md#separated-solution-of-the-damped-string-equation)

$$
\boxed{
y(t,x)=\sum_{n=1}^{\infty}a_ne^{-t/2}
\left(
\cos(\omega_nt)+\frac{\sin(\omega_nt)}{2\omega_n}
\right)\sin(n\pi x)}.
$$

For the triangular initial displacement,

$$
\begin{aligned}
a_n
&=2\int_0^1y(0,x)\sin(n\pi x)\,dx\\
&=\boxed{\frac{4\sin(n\pi/2)}{n^2\pi^2}}.
\end{aligned}
$$

Thus the even coefficients vanish and the odd ones alternate in sign.

Let

$$
T_n(t)=a_ne^{-t/2}
\left(\cos(\omega_nt)+\frac{\sin(\omega_nt)}{2\omega_n}\right).
$$

Then

$$
T_n'(t)=-a_ne^{-t/2}
\frac{n^2\pi^2}{\omega_n}\sin(\omega_nt).
$$

Orthogonality of the sine and cosine modes, equivalently the [Parseval identity](../../../fourier-analysis.md#parseval-identity), gives

$$
\boxed{
E(t)=\frac14\sum_{n=1}^{\infty}a_n^2e^{-t}
\left[
\frac{n^4\pi^4}{\omega_n^2}\sin^2(\omega_nt)
+n^2\pi^2
\left(\cos(\omega_nt)+
\frac{\sin(\omega_nt)}{2\omega_n}\right)^2
\right]}.
$$

The sign of its [derivative](../../../calculus.md#derivative) is clearest directly from the equation. Integration by parts, using $y_t=0$ at the fixed endpoints, yields

$$
\begin{aligned}
E'(t)
&=\int_0^1(y_ty_{tt}+y_xy_{xt})\,dx\\
&=\int_0^1y_t(y_{tt}-y_{xx})\,dx
=-\int_0^1y_t^2\,dx\leq0.
\end{aligned}
$$

This is the [energy dissipation identity for a linearly damped string](../../../wave-equation.md#energy-dissipation-identity-for-a-linearly-damped-string).

## 15C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="15c/solution">Solution</h3>

↑ **Parent:** [15C](#15c)

In electrostatic equilibrium, a nonzero [electric field](../../../electromagnetism.md#electric-field) inside a conductor would move its free charges. Hence $E=0$ in the conducting material and the potential is constant throughout each connected conductor. Immediately outside its surface the tangential [electric field](../../../electromagnetism.md#electric-field) is zero. A Gaussian pillbox across the surface gives

$$
(E_{\rm out}-E_{\rm in})\cdot n=\frac\sigma{\epsilon_0}.
$$

Since $E_{\rm in}=0$, the [electrostatic boundary conditions at a conductor](../../../electromagnetism.md#electrostatic-boundary-conditions-at-a-conductor) give

$$
\boxed{\sigma=\epsilon_0E_{\rm out}\cdot n}.
$$

For the widely separated shells, let their charges be $Q_1,Q_2$. Their common potential requires

$$
\frac{Q_1}{4\pi\epsilon_0R_1}
=\frac{Q_2}{4\pi\epsilon_0R_2},
\qquad Q_1+Q_2=Q.
$$

Thus the [charge sharing between distant connected spheres](../../../electromagnetism.md#charge-sharing-between-distant-connected-spheres) is

$$
\boxed{
Q_1=\frac{R_1}{R_1+R_2}Q,
\qquad
Q_2=\frac{R_2}{R_1+R_2}Q}.
$$

For the [charge on connected concentric spherical shells](../../../electromagnetism.md#charge-on-connected-concentric-spherical-shells), the potentials at the two radii are

$$
\Phi(R_1)=\frac1{4\pi\epsilon_0}
\left(\frac{Q_1}{R_1}+\frac{Q_2}{R_2}\right),
\qquad
\Phi(R_2)=\frac{Q_1+Q_2}{4\pi\epsilon_0R_2}.
$$

Equality forces $Q_1=0$. Hence

$$
\boxed{Q_1=0,
\qquad Q_2=Q},
$$

so all charge lies on the exterior of the outer shell.

For the neutral sphere in the uniform field, the far-field condition gives $\alpha=-E$. Constancy of the potential on $r=R$ gives $\beta=ER^3$. Therefore

$$
\boxed{
\Phi(r,\theta)=-E\left(r-\frac{R^3}{r^2}\right)\cos\theta}.
$$

The outward normal field at the surface is

$$
E_r(R,\theta)
=-\left.\frac{\partial\Phi}{\partial r}\right|_{r=R}
=3E\cos\theta.
$$

The [induced charge on a conducting sphere in a uniform electric field](../../../electromagnetism.md#induced-charge-on-a-conducting-sphere-in-a-uniform-electric-field) is consequently

$$
\boxed{\sigma(\theta)=3\epsilon_0E\cos\theta}.
$$

Finally,

$$
\int_{S^2}\sigma\,dA
=6\pi\epsilon_0ER^2\int_0^\pi
\cos\theta\sin\theta\,d\theta=0,
$$

confirming neutrality.

## 16D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="16d/solution">Solution</h3>

↑ **Parent:** [16D](#16d)

Take the sphere to move in the positive $z$-direction and use spherical coordinates centred on it. An axisymmetric harmonic potential that decays at infinity has the dipole form $A\cos\theta/r^2$. The no-penetration condition in the laboratory frame is

$$
\left.\frac{\partial\phi}{\partial r}\right|_{r=a}
=U\cos\theta.
$$

It fixes $A=-Ua^3/2$, so the [potential flow around a translating sphere](../../../fluid-mechanics.md#potential-flow-around-a-translating-sphere) is

$$
\boxed{
\phi(r,\theta)=-\frac{Ua^3}{2r^2}\cos\theta}.
$$

The laboratory-frame [velocity](../../../classical-mechanics.md#velocity) components are

$$
\boxed{
u_r=\frac{Ua^3}{r^3}\cos\theta,
\qquad
u_\theta=\frac{Ua^3}{2r^3}\sin\theta,
\qquad
u_\varphi=0}.
$$

The fluid [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is

$$
\begin{aligned}
K_f
&=\frac\rho2\int_a^\infty\int_{S^2}
\frac{U^2a^6}{r^6}
\left(\cos^2\theta+\frac14\sin^2\theta\right)
r^2\,d\Omega\,dr\\
&=\boxed{\frac{\pi}{3}\rho a^3U^2}
=\frac12\left(\frac12\rho V\right)U^2,
\end{aligned}
$$

where $V=4\pi a^3/3$. Thus the [added mass of a sphere](../../../physics.md#added-mass-of-a-sphere) is $\rho V/2$.

When the sphere falls, replacing fluid of density $\rho$ by material of density $\rho_s$ lowers the gravitational [potential energy](../../../classical-mechanics.md#potential-energy) at rate

$$
\boxed{\dot P=-(\rho_s-\rho)VgU}.
$$

The total [kinetic energy](../../../classical-mechanics.md#kinetic-energy) of sphere and fluid is

$$
K=\frac12\left(\rho_s+\frac\rho2\right)VU^2.
$$

Conservation of total energy gives

$$
\left(\rho_s+\frac\rho2\right)VU\frac{dU}{dt}
-(\rho_s-\rho)VgU=0.
$$

For $U\ne0$, the [acceleration of a freely falling sphere with added mass](../../../physics.md#acceleration-of-a-freely-falling-sphere-with-added-mass) is

$$
\boxed{
\frac{dU}{dt}=\frac{\rho_s-\rho}{\rho_s+\rho/2}\,g}.
$$

The same formula holds at release by continuity.

## 17A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="17a/solution">Solution</h3>

↑ **Parent:** [17A](#17a)

If the bound is to hold with finite $c$, the error functional must vanish on every [polynomial](../../../polynomial.md) whose fourth [derivative](../../../calculus.md#derivative) is zero. Thus the scheme must be exact for degrees zero through three. Applying it to powers of $t=x+1$ gives

$$
\begin{aligned}
a_{-1}+a_0+a_1+a_2&=0,\\
a_0+2a_1+3a_2&=0,\\
a_0+4a_1+9a_2&=2,\\
a_0+8a_1+27a_2&=0.
\end{aligned}
$$

Solving,

$$
\boxed{a_{-1}=2,
\qquad a_0=-5,
\qquad a_1=4,
\qquad a_2=-1}.
$$

This is the [four-point one-sided second-derivative formula](../../../numerical-analysis.md#four-point-one-sided-second-derivative-formula).

The [Peano kernel theorem](../../../numerical-analysis.md#peano-kernel-theorem) says that if a linear functional $L$ annihilates all [polynomials](../../../polynomial.md) of degree below $r$, then for $f\in C^r[a,b]$,

$$
L(f)=\int_a^bK(t)f^{(r)}(t)\,dt,
\qquad
K(t)=L\left(\frac{(x-t)_+^{r-1}}{(r-1)!}\right).
$$

Here $r=4$ and $L=e$. Under the stated nonnegativity assumption,

$$
|e(f)|\leq
\left(\int_{-1}^2K(t)\,dt\right)
\max_{[-1,2]}|f^{(4)}|.
$$

The [integral](../../../calculus.md#integral) equals $e(q)$ for $q(x)=(x+1)^4/24$, since $q^{(4)}=1$. Now $q''(-1)=0$ and

$$
\eta(q)=\frac{-5+4\cdot16-81}{24}=-\frac{11}{12}.
$$

Therefore

$$
\int_{-1}^2K(t)\,dt=e(q)=\frac{11}{12}.
$$

Equality is attained by $q$, so the [sharp Peano-kernel constant for the four-point endpoint second derivative](../../../numerical-analysis.md#sharp-peano-kernel-constant-for-the-four-point-endpoint-second-derivative) is

$$
\boxed{c=\frac{11}{12}}.
$$

## 18H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

Under $H_0$,

$$
\sqrt n\,\overline X\sim N(0,1).
$$

Let $z_{1-\alpha/2}=\Phi^{-1}(1-\alpha/2)$. The standard two-sided level-$\alpha$ test rejects exactly when

$$
\boxed{|\sqrt n\,\overline X|>z_{1-\alpha/2}}.
$$

For the observed value $\overline X=\overline x$, its [two-sided Gaussian p-value](../../../statistical-modelling.md#two-sided-gaussian-p-value) is

$$
\boxed{
p(\overline x)=2\left[1-\Phi(\sqrt n\,|\overline x|)\right]}.
$$

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

Conditionally on $\mu$,

$$
\overline X\mid\mu\sim N\left(\mu,\frac1n\right),
$$

so

$$
\boxed{
f(\overline x\mid\mu)
=\sqrt{\frac n{2\pi}}
\exp\left[-\frac n2(\overline x-\mu)^2\right]}.
$$

Under the continuous half of the prior, write $\overline X=\mu+Z$ with independent

$$
\mu\sim N(0,\tau^2),
\qquad
Z\sim N(0,1/n).
$$

Thus $\overline X\sim N(0,\tau^2+1/n)$ there. Mixing this density with the point-null density gives the [marginal likelihood for a Gaussian point-null mixture](../../../statistical-inference.md#marginal-likelihood-for-a-gaussian-point-null-mixture)

$$
\boxed{
\begin{aligned}
m(\overline x)={}&\frac12\sqrt{\frac n{2\pi}}
 e^{-n\overline x^2/2}\\
&+\frac1{2\sqrt{2\pi(\tau^2+1/n)}}
 \exp\left[-\frac{\overline x^2}{2(\tau^2+1/n)}\right].
\end{aligned}}
$$

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

Bayes' formula divides the point-null contribution to the mixture density by the full marginal density:

$$
q(\overline x)
=\frac{\phi_{1/n}(\overline x)}
{\phi_{1/n}(\overline x)+
 \phi_{\tau^2+1/n}(\overline x)}.
$$

Since

$$
\frac{\phi_{\tau^2+1/n}(\overline x)}
{\phi_{1/n}(\overline x)}
=\frac1{\sqrt{1+n\tau^2}}
\exp\left[
\frac{n^2\tau^2\overline x^2}{2(1+n\tau^2)}
\right],
$$

the [posterior probability of a Gaussian point null](../../../statistical-inference.md#posterior-probability-of-a-gaussian-point-null) is

$$
\boxed{
q(\overline x)=
\left\{
1+\frac1{\sqrt{1+n\tau^2}}
\exp\left[
\frac{n^2\tau^2\overline x^2}{2(1+n\tau^2)}
\right]
\right\}^{-1}}.
$$

<h3 id="18h/d">d</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/d/i">i</h4>

↑ **Parent:** [D](#18h/d)

<h5 id="18h/d/i/solution">Solution</h5>

↑ **Parent:** [I](#18h/d/i)

For $n=100$ and $\tau=1$,

$$
p(0)=1,
\qquad
q(0)=\frac1{1+1/\sqrt{101}}<1.
$$

Both are continuous, so when $|\overline x|$ is sufficiently small,

$$
\boxed{p(\overline x)>q(\overline x)}.
$$

<h4 id="18h/d/ii">ii</h4>

↑ **Parent:** [D](#18h/d)

<h5 id="18h/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#18h/d/ii)

For large $|\overline x|$, the supplied normal-tail approximation gives

$$
p(\overline x)
\sim\frac1{5\sqrt{2\pi}\,|\overline x|}
 e^{-50\overline x^2}.
$$

Meanwhile,

$$
q(\overline x)
\sim\sqrt{101}
\exp\left(-\frac{5000}{101}\overline x^2\right).
$$

Since $5000/101<50$, the posterior point-null probability decays more slowly. Therefore, for sufficiently large $|\overline x|$,

$$
\boxed{q(\overline x)>p(\overline x)}.
$$

This reversal is the [Jeffreys-Lindley paradox for a Gaussian point null](../../../statistical-inference.md#jeffreys-lindley-paradox-for-a-gaussian-point-null).

## 19H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="19h/a">a</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/a/solution">Solution</h4>

↑ **Parent:** [A](#19h/a)

A feasible flow assigns $f_{ij}$ to each directed edge so that

$$
0\leq f_{ij}\leq C_{ij}
$$

and inflow equals outflow at every vertex other than the source and sink. Its value $|f|$ is the net outflow from the source. For a set $S$ containing the source but not the sink, the associated cut has capacity

$$
C(S,V\setminus S)
=\sum_{i\in S,\,j\notin S}C_{ij}.
$$

The [max-flow min-cut theorem](../../../graph-theory.md#max-flow-min-cut-theorem) states

$$
\boxed{
\max_f|f|=\min_{S\ni s,\,t\notin S}C(S,V\setminus S)}.
$$

For every flow and cut, conservation at vertices inside $S$ gives

$$
|f|=f(S,V\setminus S)-f(V\setminus S,S)
\leq C(S,V\setminus S).
$$

This proves the weak inequality.

A maximum flow exists because the feasible-flow polytope is nonempty, closed, and bounded. Form its residual graph: a forward edge has residual capacity $C_{ij}-f_{ij}$, and a reverse edge has residual capacity $f_{ij}$. If the residual graph contained a source-to-sink path, augmenting by the smallest positive residual capacity on that path would increase the flow, contradicting maximality.

Let $S$ be the vertices reachable from the source in the residual graph. The sink is not in $S$. Every original edge from $S$ to its complement is saturated, and every original edge from the complement into $S$ carries zero flow; otherwise the appropriate residual edge would make its other endpoint reachable. Hence

$$
|f|=f(S,V\setminus S)-f(V\setminus S,S)
=C(S,V\setminus S).
$$

The maximum flow therefore equals the capacity of this cut, completing the proof.

<h3 id="19h/b">b</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/b/i">i</h4>

↑ **Parent:** [B](#19h/b)

<h5 id="19h/b/i/solution">Solution</h5>

↑ **Parent:** [I](#19h/b/i)

Label the seven black intermediate vertices, from left to right and top to bottom within each column, by $a,b,c,d,e,f,g$: thus $a$ is directly below $r$, $b$ is the lower-left vertex, $c,d$ are the next upper and lower vertices, $e$ is the middle-right vertex, and $f,g$ are the upper-right and lower-right vertices.

For $x=4$, the following nonzero edge flows are feasible:

$$
\begin{array}{c|cccccccccc}
\text{edge}&sr&rc&cf&ft&sb&bd&de&et&dg&gt\\ \hline
\text{flow}&4&4&4&4&5&5&3&3&2&2.
\end{array}
$$

Their value is $9$. The cut with source side $\{s\}$ has capacity

$$
C(\{s\},V\setminus\{s\})=x+5=9.
$$

By the max-flow min-cut theorem,

$$
\boxed{\delta^*(4)=9}.
$$

<h4 id="19h/b/ii">ii</h4>

↑ **Parent:** [B](#19h/b)

<h5 id="19h/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#19h/b/ii)

Two cuts give the upper bounds

$$
\delta^*(x)\leq x+5
$$

from the source cut, and

$$
\delta^*(x)\leq14
$$

from the cut whose source side is

$$
S=\{s,r,a,b,c,d,f\}.
$$

The latter cut crosses the edges $ce,de,dg,ft$, of respective capacities $3,3,2,6$.

At $x=0$, a flow of value $5$ is

$$
sb=bd=5,
\qquad de=et=3,
\qquad dg=gt=2.
$$

At $x=9$, a flow of value $14$ is given by

$$
\begin{array}{c|rrrrrrrrrrrrr}
\text{edge}&sr&sb&rc&ra&ac&bd&cf&ce&de&dg&et&ft&gt\\ \hline
\text{flow}&9&5&6&3&3&5&6&3&3&2&6&6&2.
\end{array}
$$

For $0\leq x\leq9$, take the convex combination of these two flows with weights $1-x/9$ and $x/9$. It is feasible at capacity $x$ and has value $5+x$. For $x\geq9$, the second flow remains feasible and has value $14$. The two cut bounds are therefore attained, and the [parametric maximum flow with one source capacity](../../../graph-theory.md#parametric-maximum-flow-with-one-source-capacity) is

$$
\boxed{
\delta^*(x)=\min\{x+5,14\}
=\begin{cases}
x+5,&0\leq x\leq9,\\
14,&x\geq9.
\end{cases}}
$$

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
