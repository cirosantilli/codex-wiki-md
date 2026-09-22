# Paper 4

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperib_4_2025.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2025/paperib_4_2025.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2G](#2g)
  - [Solution](#2g/solution)
- [3E](#3e)
  - [Solution](#3e/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5B](#5b)
  - [Solution](#5b/solution)
- [6A](#6a)
  - [a](#6a/a)
    - [Solution](#6a/a/solution)
  - [b](#6a/b)
    - [Solution](#6a/b/solution)
- [7H](#7h)
  - [a](#7h/a)
    - [Solution](#7h/a/solution)
  - [b](#7h/b)
    - [Solution](#7h/b/solution)
- [8F](#8f)
  - [Solution](#8f/solution)
- [9E](#9e)
  - [a](#9e/a)
    - [i](#9e/a/i)
      - [Solution](#9e/a/i/solution)
    - [ii](#9e/a/ii)
      - [Solution](#9e/a/ii/solution)
  - [b](#9e/b)
    - [i](#9e/b/i)
      - [Solution](#9e/b/i/solution)
    - [ii](#9e/b/ii)
      - [Solution](#9e/b/ii/solution)
    - [iii](#9e/b/iii)
      - [Solution](#9e/b/iii/solution)
- [10G](#10g)
  - [Solution](#10g/solution)
- [11E](#11e)
  - [a](#11e/a)
    - [Solution](#11e/a/solution)
  - [b](#11e/b)
    - [Solution](#11e/b/solution)
- [12A](#12a)
  - [a](#12a/a)
    - [Solution](#12a/a/solution)
  - [b](#12a/b)
    - [Solution](#12a/b/solution)
  - [c](#12a/c)
    - [Solution](#12a/c/solution)
- [13C](#13c)
  - [Solution](#13c/solution)
- [14D](#14d)
  - [Solution](#14d/solution)
- [15C](#15c)
  - [i](#15c/i)
    - [Solution](#15c/i/solution)
  - [ii](#15c/ii)
    - [Solution](#15c/ii/solution)
- [16D](#16d)
  - [Solution](#16d/solution)
- [17H](#17h)
  - [a](#17h/a)
    - [Solution](#17h/a/solution)
  - [b](#17h/b)
    - [Solution](#17h/b/solution)
  - [c](#17h/c)
    - [Solution](#17h/c/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
  - [d](#18h/d)
    - [Solution](#18h/d/solution)

## 1F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

The dual space $V^*$ is the [vector space](../../../vector-space.md) of [linear maps](../../../vector-space.md#linear-map) $V\to\mathbb F$. If $B=(v_1,\ldots,v_n)$, its dual family satisfies $v_i^*(v_j)=\delta_{ij}$. Every functional $f$ obeys

$$
f=\sum_i f(v_i)v_i^*,
$$

so the family spans; evaluation on each $v_j$ proves linear independence. Thus it is a [basis](../../../vector-space.md#basis) without any prior dimension argument.

For $p=a+bt+ct^2$,

$$
f_0(p)=a,\quad f_1(p)=a+b/2+c/3,\quad f_2(p)=a-b/2+c/3.
$$

The [basis](../../../vector-space.md#basis) dual to $(f_0,f_1,f_2)$ is

$$
p_0=1-3t^2,\qquad p_1=t+\frac32t^2,\qquad p_2=-t+\frac32t^2,
$$

as direct substitution gives $f_i(p_j)=\delta_{ij}$. Hence the three functionals form a [basis](../../../vector-space.md#basis) of $P_2^*$.

## 2G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2g/solution">Solution</h3>

↑ **Parent:** [2G](#2g)

A contraction satisfies $d(Tx,Ty)\le qd(x,y)$ for some $0\le q<1$. Starting from $x_0$, define $x_{k+1}=Tx_k$. The geometric bound on successive distances makes $(x_k)$ Cauchy, so completeness gives a [limit](../../../calculus.md#limit-of-a-function) $x$. Continuity of $T$ gives $Tx=x$. If $Ty=y$, then $d(x,y)\le qd(x,y)$, hence $x=y$. This is the [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem).

If $T^n$ is a contraction, it has a unique fixed point $x$. Since $T^n(Tx)=T(T^nx)=Tx$, the point $Tx$ is also fixed by $T^n$, so uniqueness gives $Tx=x$. Every fixed point of $T$ is fixed by $T^n$, so it too must equal $x$. Thus $T$ has exactly one fixed point.

## 3E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3e/solution">Solution</h3>

↑ **Parent:** [3E](#3e)

The local [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) says that if $|f|$ has a local maximum at an interior point of a connected domain, then $f$ is constant. On a small circle about the maximum, the mean-value property and

$$
|f(z_0)|\le\frac1{2\pi}\int|f(z_0+re^{it})|dt\le|f(z_0)|
$$

force equality everywhere. Equality in the triangle inequality makes the boundary values identical; Cauchy's formula then makes $f$ constant locally, and the identity theorem makes it constant on the domain.

Write $f=u+iv$. The hypothesis gives $u-v\le0$. Therefore

$$
|e^{(1+i)f(z)}|=e^{u-v}\le1,
$$

with equality at zero. The local maximum [modulus](../../../complex-analysis.md#modulus) principle makes the exponential constant. [Differentiation](../../../calculus.md#differentiation) then gives $f'=0$, so $f$ is constant; since $f(0)=0$, it is identically zero.

## 4C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

Separation with Dirichlet walls gives

$$
\Psi_{n_xn_yn_z}=\sin\frac{n_x\pi x}{a}\sin\frac{n_y\pi y}{b}\sin\frac{n_z\pi z}{c},
$$



$$
E_{n_xn_yn_z}=\frac{\hbar^2\pi^2}{2m}\left(\frac{n_x^2}{a^2}+\frac{n_y^2}{b^2}+\frac{n_z^2}{c^2}\right),\qquad n_x,n_y,n_z\ge1.
$$

For $a<b<c$, the [ground state](../../../quantum-mechanics.md#ground-state) $(1,1,1)$ has a [nondegenerate](../../../quantum-mechanics.md#nondegenerate-energy-eigenvalue) energy. The cheapest [excitation](../../../quantum-mechanics.md#excited-state) changes the [quantum number](../../../quantum-mechanics.md#quantum-number) in the longest direction, so the [first excited state](../../../quantum-mechanics.md#first-excited-state) $(1,1,2)$ also has a nondegenerate energy.

If $a<b=c$, the ground-state energy remains [nondegenerate](../../../quantum-mechanics.md#nondegenerate-energy-eigenvalue), but $(1,2,1)$ and $(1,1,2)$ have equal first-excited energy, giving [degeneracy](../../../statistical-physics.md#state-degeneracy) two.

## 5B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5b/solution">Solution</h3>

↑ **Parent:** [5B](#5b)

In vacuum, curl [Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) and use $\nabla\cdot E=0$ and the [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) to obtain

$$
\nabla^2E-\frac1{c^2}\partial_t^2E=0,\qquad c=(\mu_0\varepsilon_0)^{-1/2}.
$$

The plane wave solves this when $\omega=c|k|$ and $k\cdot E_0=0$. [Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) gives

$$
B=\operatorname{Re}\left(\frac{k\times E_0}{\omega}e^{i(k\cdot x-\omega t)}\right).
$$

For the stated wave, propagation is along $+x$ and polarization is $(0,1,1)/\sqrt2$. Thus

$$
B=\frac{E_0}{c}(0,-1,1)\frac{\cos(kx-\omega t)}{\sqrt2},
$$



$$
S=\frac{E_0^2}{\mu_0c}\cos^2(kx-\omega t)e_x,\qquad
\langle S\rangle=\frac{E_0^2}{2\mu_0c}e_x.
$$

The [Poynting vector](../../../electromagnetism.md#poynting-vector) is electromagnetic energy flux, and its average is the wave intensity.

## 6A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6a/a">a</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/a/solution">Solution</h4>

↑ **Parent:** [A](#6a/a)

Exactness for $1$ and $x$ gives

$$
a_0+a_1=\frac12,\qquad a_0x_0+a_1x_1=\frac13.
$$

Hence

$$
\boxed{a_0=\frac{x_1/2-1/3}{x_1-x_0},\qquad
a_1=\frac{1/3-x_0/2}{x_1-x_0}.}
$$

<h3 id="6a/b">b</h3>

↑ **Parent:** [6A](#6a)

<h4 id="6a/b/solution">Solution</h4>

↑ **Parent:** [B](#6a/b)

A two-node Gaussian rule is exact through degree three, the maximal degree $2n-1$. Its nodes are the zeros of the monic quadratic orthogonal to $1,x$ for weight $x$ on $[0,1]$. Writing it as $p=x^2+ux+v$ gives

$$
\int_0^1px\,dx=0,\qquad\int_0^1px^2\,dx=0,
$$

so $u=-6/5$, $v=3/10$. Therefore

$$
\boxed{x_0=\frac35-\frac{\sqrt6}{10},\qquad
x_1=\frac35+\frac{\sqrt6}{10}.}
$$

## 7H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7h/a">a</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/a/solution">Solution</h4>

↑ **Parent:** [A](#7h/a)

The communicating classes are $\{1,3\}$ and $\{2,4\}$. The first is open because state 3 can enter 4 and cannot return; the second is closed.

<h3 id="7h/b">b</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/b/solution">Solution</h4>

↑ **Parent:** [B](#7h/b)

On the closed class, the transition [matrix](../../../vector-space.md#matrix) is

$$
\begin{pmatrix}1/3&2/3\\1/4&3/4\end{pmatrix}.
$$

Its [stationary distribution](../../../markov-process.md#stationary-distribution) is $(3/11,8/11)$. The class is irreducible and aperiodic because of its self-loops, while the other class is transient and enters it almost surely. Hence

$$
\lim_{n\to\infty}P^n=
\begin{pmatrix}
0&3/11&0&8/11\\0&3/11&0&8/11\\0&3/11&0&8/11\\0&3/11&0&8/11
\end{pmatrix}.
$$

## 8F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8f/solution">Solution</h3>

↑ **Parent:** [8F](#8f)

The symmetric bilinear form associated with a real [quadratic form](../../../linear-algebra.md#quadratic-form) $Q$ is obtained by [polarization identity](../../../linear-algebra.md#polarization-identity):

$$
phi(u,v)=\frac12\bigl(Q(u+v)-Q(u)-Q(v)\bigr).
$$

In coordinates $Q(x)=x^TAx$, replacing $A$ by its symmetric part does not change $Q$, and the formula gives $phi(u,v)=u^TAv$; this proves existence. A symmetric form is positive semidefinite when $phi(v,v)\geq0$ for every $v$, and positive definite when the inequality is strict for every $v\ne0$.

The diagonalization theorem for real quadratic forms says that some [basis](../../../vector-space.md#basis) puts any symmetric form into

$$
x_1^2+\cdots+x_p^2-y_1^2-\cdots-y_q^2,
$$

with $r$ further zero coordinates. [Sylvester's law of inertia](../../../linear-algebra.md#sylvester-s-law-of-inertia) says that $(p,q,r)$ is independent of the diagonalizing [basis](../../../vector-space.md#basis). To prove this, let $P$ be the span of the positive coordinate [vectors](../../../vector-space.md#vector) and let $N\oplus Z$ be the span of the negative and zero [vectors](../../../vector-space.md#vector). If $P'$ is positive definite for another diagonalization and $\dim P'>p$, then

$$
\dim P'+\dim(N\oplus Z)>(p+q+r),
$$

so the two spaces intersect nontrivially. A [vector](../../../vector-space.md#vector) in the intersection would have both positive and nonpositive square, a contradiction. Thus $p'\leq p$; symmetry gives $p=p'$. Applying the same argument to $-\phi$ gives $q=q'$, and then $r=r'$.

For the [nondegenerate form](../../../linear-algebra.md#nondegenerate-bilinear-form) on $V$, write its [inertia](../../../linear-algebra.md#inertia-of-a-bilinear-form) as $(p,q,0)$, so $p+q=2n$. The restriction vanishes identically on $E$: [polarization](../../../linear-algebra.md#polarization-identity) gives $phi(u,v)=0$ for $u,v\in E$. Projection of $E$ to the positive coordinate space is [injective](../../../algebra.md#injective-function), since a [vector](../../../vector-space.md#vector) with zero positive projection cannot be [isotropic](../../../linear-algebra.md#isotropic-vector) unless it is zero. Hence $k\leq p$; projection to the negative space likewise gives $k\leq q$. Therefore $k\leq\min(p,q)\leq n$.

The [matrix](../../../vector-space.md#matrix) of $l^2$ is $ll^T$. If $l\ne0$, it has rank one and inertia $(1,0,n-1)$, hence signature one; if $l=0$, its rank and signature are zero. The coefficientwise product $(l^2,s^2)$ has [matrix](../../../vector-space.md#matrix) $tt^T$, where $t_i=l_is_i$, so it has the same rank-one conclusion when $t\ne0$ and is zero otherwise.

Finally, diagonalization writes every positive semidefinite form as a sum of squares, say $f=\sum_a l_a^2$ and $g=\sum_b s_b^2$. Bilinearity of coefficientwise multiplication gives

$$
 (f,g)=\sum_{a,b}(l_a^2,s_b^2),
$$

a sum of positive semidefinite rank-at-most-one forms. Thus $(f,g)$ is positive semidefinite.

## 9E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9e/a">a</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/a/i">i</h4>

↑ **Parent:** [A](#9e/a)

<h5 id="9e/a/i/solution">Solution</h5>

↑ **Parent:** [I](#9e/a/i)

If $M$ is irreducible and $m\ne0$, the image $Rm$ is a nonzero submodule, hence $Rm=M$ and the map is onto. Conversely, if every nonzero $m$ is cyclic and $N\leq M$ is nonzero, choose $m\in N\setminus\{0\}$. Then $M=Rm\subseteq N$, so $N=M$ and $M$ is irreducible.

<h4 id="9e/a/ii">ii</h4>

↑ **Parent:** [A](#9e/a)

<h5 id="9e/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9e/a/ii)

The annihilator $I=\operatorname{Ann}_R(M)$ is an [ideal](../../../commutative-algebra.md#ideal). For $r\notin I$, choose $m$ with $rm\ne0$. Irreducibility and part (i) give $s\in R$ such that $srm=m$. The element $(sr-1)$ therefore kills the generator $m$, and hence all of $M$; thus $sr-1\in I$. Every nonzero class in $R/I$ consequently has an inverse, so $R/I$ is a field.

<h3 id="9e/b">b</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/b/i">i</h4>

↑ **Parent:** [B](#9e/b)

<h5 id="9e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9e/b/i)

Make $V$ a $k[x]$-module by $xv=\varphi(v)$. The structure theorem over the Euclidean domain $k[x]$ decomposes its torsion module as

$$
V\cong\bigoplus_\alpha k[x]/(p_\alpha^{e_\alpha}),
$$

where the $p_\alpha$ are monic irreducibles. Each summand is indecomposable: its submodules form a chain, so two nonzero submodules cannot form a direct sum. This is the desired decomposition into invariant indecomposable subspaces.

The [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is

$$
\chi_\varphi(x)=\prod_\alpha p_\alpha(x)^{e_\alpha},
$$

whereas the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) is the least common multiple

$$
\boxed{m_\varphi(x)=\operatorname{lcm}_\alpha p_\alpha(x)^{e_\alpha}.}
$$

<h4 id="9e/b/ii">ii</h4>

↑ **Parent:** [B](#9e/b)

<h5 id="9e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9e/b/ii)

The prime [ideals](../../../commutative-algebra.md#ideal) of $\mathbb R[x]$ are $(0)$ and the maximal [ideals](../../../commutative-algebra.md#ideal) generated by the monic irreducibles

$$
x-a\quad(a\in\mathbb R),\qquad (x-a)^2+b^2\quad(a\in\mathbb R, b>0).
$$

For a nonzero prime $I=(p)$, use the residue classes of $1,x,\ldots,x^{N-1}$, where $N=n\deg p$. Multiplication by $x$ on $\mathbb R[x]/(p^n)$ is represented by the [companion matrix](../../../linear-operator-theory.md#companion-matrix) of the monic [polynomial](../../../polynomial.md) $p^n$. In particular, for $p=x-a$ this may equivalently be written as one size-$n$ [Jordan block](../../../linear-operator-theory.md#jordan-block) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $a$. The [ideal](../../../commutative-algebra.md#ideal) $(0)$ does not give a finite-dimensional quotient.

<h4 id="9e/b/iii">iii</h4>

↑ **Parent:** [B](#9e/b)

<h5 id="9e/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#9e/b/iii)

The upper-left block has characteristic and minimal [polynomial](../../../polynomial.md) $(x^2+1)^2$, while the lower-right block has characteristic and minimal [polynomial](../../../polynomial.md) $x^2+1$. Hence the corresponding module is

$$
\mathbb R[x]/((x^2+1)^2)\oplus\mathbb R[x]/(x^2+1).
$$

In the power [bases](../../../vector-space.md#basis) from part (ii), an explicit normal form is

$$
\begin{pmatrix}
0&0&0&-1&0&0\\
1&0&0&0&0&0\\
0&1&0&-2&0&0\\
0&0&1&0&0&0\\
0&0&0&0&0&-1\\
0&0&0&0&1&0
\end{pmatrix},
$$

the direct sum of the companion [matrices](../../../vector-space.md#matrix) of $(x^2+1)^2$ and $x^2+1$.

## 10G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10g/solution">Solution</h3>

↑ **Parent:** [10G](#10g)

A map $f:\mathbb R^n\to\mathbb R^m$ is [differentiable](../../../analysis.md#differentiable-function) at $x$ if there is a [linear map](../../../vector-space.md#linear-map) $L$ such that

$$
f(x+h)=f(x)+Lh+o(\lVert h\rVert);
$$

then $Df|_x=L$. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) says that if $f$ is continuously [differentiable](../../../analysis.md#differentiable-function) near $x$ and $Df|_x$ is invertible, then $f$ restricts to a $C^1$ diffeomorphism between neighborhoods of $x$ and $f(x)$.

Since $F(A)=A^TA$ is [polynomial](../../../polynomial.md),

$$
DF|_A(H)=H^TA+A^TH.
$$

Thus $\ker DF|_I=T$, the space of skew-symmetric [matrices](../../../vector-space.md#matrix).

Define

$$
\Phi(A)=A^TA+A-A^T-I.
$$

Then $D\Phi|_I(H)=2H$, so the inverse [function](../../../function.md) theorem supplies open neighborhoods $I\in U$, $0\in V$ on which $\Phi:U\to V$ is a $C^1$ diffeomorphism. Its symmetric part is $A^TA-I$ and its skew part is $A-A^T$. Consequently

$$
\Phi(A)\in T\iff A^TA=I,
$$

and therefore $\Phi(U\cap\mathcal O)=V\cap T$.

For any $R\in\mathcal O$, left multiplication $A\mapsto R^TA$ is a homeomorphism preserving $\mathcal O$ and carrying $R$ to $I$. Transporting the preceding chart gives a neighborhood of $R$ in $\mathcal O$ homeomorphic to an open subset of $T$.

## 11E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11e/a">a</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/a/solution">Solution</h4>

↑ **Parent:** [A](#11e/a)

The disc model is

$$
D=\{z:|z|<1\},\qquad g_D=\frac{4|dz|^2}{(1-|z|^2)^2},
$$

and the upper half-plane model is

$$
\mathfrak h=\{x+iy:y>0\},\qquad g_{\mathfrak h}=\frac{dx^2+dy^2}{y^2}.
$$

The Cayley map

$$
C(z)=i\frac{1+z}{1-z}
$$

maps $D$ bijectively to $\mathfrak h$. Since $C'(z)=2i/(1-z)^2$ and $\operatorname{Im}C(z)=(1-|z|^2)/|1-z|^2$, direct substitution gives $C^*g_{\mathfrak h}=g_D$.

Representing $C$ by $K=\begin{pmatrix}i&i\\-1&1\end{pmatrix}$, the disc isometry corresponding to $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ is represented, up to a nonzero [scalar](../../../vector-space.md#scalar), by

$$
K^{-1}gK=\frac12\begin{pmatrix}
a+d+i(b-c)&a-d-i(b+c)\\
a-d+i(b+c)&a+d-i(b-c)
\end{pmatrix}.
$$

<h3 id="11e/b">b</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/b/solution">Solution</h4>

↑ **Parent:** [B](#11e/b)

A [hyperbolic triangle](../../../geometry-and-topology.md#hyperbolic-triangle) is bounded by three hyperbolic geodesic segments or rays. Its vertices may lie in the hyperbolic plane; an [ideal vertex](../../../geometry-and-topology.md#ideal-vertex) is their endpoint on the boundary at infinity. Every [ideal](../../../commutative-algebra.md#ideal) angle is zero. [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) with curvature $-1$ gives

$$
\operatorname{area}(\Delta)=\pi-(\alpha+\beta+\gamma),
$$

so an all-ideal triangle has area $\pi$.

For fixed admissible angles, hyperbolic trigonometry determines all three side lengths from the angles, for example

$$
\cosh a=\frac{\cos\alpha+\cos\beta\cos\gamma}{\sin\beta\sin\gamma}.
$$

Thus two such triangles are congruent. An orientation-preserving isometry can send one chosen vertex and oriented tangent to the corresponding data of the other, and the determined side lengths and angles then send the entire triangle to it. Since the orientation-preserving isometry [group](../../../group.md) is $PSL_2(\mathbb R)$, represented by $SL_2(\mathbb R)$, the stated action is transitive.

## 12A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12a/a">a</h3>

↑ **Parent:** [12A](#12a)

<h4 id="12a/a/solution">Solution</h4>

↑ **Parent:** [A](#12a/a)

The Heaviside factor restricts the [integral](../../../calculus.md#integral) to $t\geq\alpha$. With $u=t-\alpha$,

$$
\boxed{\mathcal L\{f(t-\alpha)H(t-\alpha)\}(s)
=\int_\alpha^\infty e^{-st}f(t-\alpha)dt
=e^{-\alpha s}\int_0^\infty e^{-su}f(u)du
=e^{-\alpha s}F(s).}
$$

<h3 id="12a/b">b</h3>

↑ **Parent:** [12A](#12a)

<h4 id="12a/b/solution">Solution</h4>

↑ **Parent:** [B](#12a/b)

Split the transform into periods and translate each interval:

$$
\mathcal L\{g\}(s)=\sum_{j=0}^\infty\int_{jT}^{(j+1)T}e^{-st}g(t)dt
=\sum_{j=0}^\infty e^{-sjT}\int_0^T e^{-su}g(u)du.
$$

Summing the [geometric series](../../../real-analysis.md#geometric-series) yields

$$
\boxed{\mathcal L\{g\}(s)=\frac{\mathcal L\{g_T\}(s)}{1-e^{-sT}}.}
$$

<h3 id="12a/c">c</h3>

↑ **Parent:** [12A](#12a)

<h4 id="12a/c/solution">Solution</h4>

↑ **Parent:** [C](#12a/c)

For one period,

$$
\int_0^{2\pi}e^{-st}h(t)dt=\int_0^\pi e^{-st}\sin t\,dt
=\frac{1+e^{-\pi s}}{s^2+1}.
$$

Part (b), followed by cancellation of $1+e^{-\pi s}$, gives

$$
\boxed{\mathcal L\{h\}(s)=\frac{1}{(s^2+1)(1-e^{-\pi s})}.}
$$

## 13C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="13c/solution">Solution</h3>

↑ **Parent:** [13C](#13c)

The Euler--Lagrange equation is

$$
2ma^2(1-\cos\phi)\ddot\phi+ma^2\sin\phi\,\dot\phi^2-mga\sin\phi=0.
$$

Putting $u=\cos(\phi/2)$ and simplifying gives

$$
\ddot u+\omega^2u=0,\qquad \omega^2=\frac{g}{4a}.
$$

Since $1-\cos\phi=2(1-u^2)$, $1+\cos\phi=2u^2$, and $\dot u^2=(1-u^2)\dot\phi^2/4$, the transformed functional is

$$
\widehat S[u]=\int_0^T(8ma^2\dot u^2-2mga u^2)dt.
$$

Its Euler--Lagrange equation is $\ddot u+(g/4a)u=0$, exactly the preceding equation.

For endpoint-vanishing $\eta$, the [second variation](../../../calculus-of-variations.md#second-variation) is

$$
\delta^2\widehat S(\eta)=16ma^2\int_0^T(\dot\eta^2-\omega^2\eta^2)dt.
$$

Writing $\eta=\sum_{n\geq1}c_ne_n$ and using orthonormality gives

$$
\delta^2\widehat S=16ma^2\sum_{n\geq1}\left[\left(\frac{n\pi}{T}\right)^2-\omega^2\right]c_n^2.
$$

It is positive definite when $T<\pi/\omega$ and has a negative $e_1$ direction when $T>\pi/\omega$. Therefore

$$
\boxed{t_0=\frac\pi\omega=2\pi\sqrt{\frac ag}.}
$$

## 14D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="14d/solution">Solution</h3>

↑ **Parent:** [14D](#14d)

Spatial Fourier transformation gives

$$
\widetilde u_{tt}+c^2k^2\widetilde u=0,\qquad
\widetilde u(k,0)=\sqrt\pi e^{-k^2/4},\qquad
\widetilde u_t(k,0)=0.
$$

Hence

$$
\widetilde u(k,t)=\sqrt\pi e^{-k^2/4}\cos(ckt).
$$

Inverting and splitting the cosine into exponentials, or applying [D'Alembert formula](../../../wave-equation.md#d-alembert-s-formula), yields

$$
u(x,t)=\frac12\left(e^{-(x-ct)^2}+e^{-(x+ct)^2}\right).
$$

**Thus the initial Gaussian separates into two half-amplitude Gaussian pulses travelling without distortion at speeds $c$ and $-c$.**

## 15C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="15c/i">i</h3>

↑ **Parent:** [15C](#15c)

<h4 id="15c/i/solution">Solution</h4>

↑ **Parent:** [I](#15c/i)

Here $L_3=-i\hbar(x_1\partial_{x_2}-x_2\partial_{x_1})$. The radial factor and $x_3^n$ are annihilated by the angular [derivative](../../../calculus.md#derivative), while

$$
L_3(x_1+ix_2)=\hbar(x_1+ix_2).
$$

The product rule therefore gives

$$
L_3\chi_{m,n}=m\hbar\chi_{m,n}.
$$

Replacing $i$ by $-i$ gives [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-m\hbar$ for $(x_1-ix_2)^mx_3^nf(r)$.

<h3 id="15c/ii">ii</h3>

↑ **Parent:** [15C](#15c)

<h4 id="15c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#15c/ii)

Set $\xi_j=\sqrt{m\omega/\hbar}\,x_j$. Separation into three one-dimensional oscillators gives

$$
\Psi_{n_1n_2n_3}=h_{n_1}(\xi_1)h_{n_2}(\xi_2)h_{n_3}(\xi_3)e^{-m\omega r^2/(2\hbar)},
$$



$$
E_N=\hbar\omega\left(N+\frac32\right),\qquad N=n_1+n_2+n_3.
$$

The ground state is

$$
E_0=\frac32\hbar\omega,\qquad \Psi_0=e^{-m\omega r^2/(2\hbar)}.
$$

The number of triples of nonnegative integers summing to $N$ is

$$
\binom{N+2}{2},
$$

which is the degeneracy of $E_N$.

Finally,

$$
\chi=(x_1+ix_2)^2e^{-m\omega r^2/(2\hbar)}
$$

is a pure level-$N=2$ oscillator state: the constant terms in the two degree-two Hermite contributions cancel. Part (i) gives $L_3\chi=2\hbar\chi$, while $N=2$ gives $H\chi=(7/2)\hbar\omega\chi$.

## 16D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="16d/solution">Solution</h3>

↑ **Parent:** [16D](#16d)

In the fluid region $y>\eta(x)$, incompressibility and [potential flow](../../../fluid-mechanics.md#potential-flow) give

$$
\nabla^2\phi=0,\qquad \nabla\phi\to0\quad(y\to\infty).
$$

No penetration through the exact surface gives

$$
(-\eta_x,1)\mathbin\cdot(U+\phi_x,\phi_y)=0,\qquad
\phi_y=(U+\phi_x)\eta_x\quad(y=\eta).
$$

The condition $hk\ll1$ says the hill slope is small; $|\nabla\phi|\ll U$ says the disturbance [velocity](../../../classical-mechanics.md#velocity) is small compared with the background wind. Dropping the product $\phi_x\eta_x$ and Taylor-shifting the boundary from $y=\eta$ to $y=0$ therefore gives

$$
\phi_y(x,0)=U\eta_x=-Uhk\sin kx.
$$

The decaying solution is

$$
\phi=Uh e^{-ky}\sin kx.
$$

Bernoulli's equation is

$$
p+\rho gy+\frac12\rho|Ue_x+\nabla\phi|^2=\text{constant}.
$$

To first order on the surface,

$$
p=\text{constant}-\rho g\eta-\rho U\phi_x,\qquad
\phi_x(x,0)=Uhk\cos kx.
$$

Thus

$$
p_{\rm trough}-p_{\rm crest}=2\rho h(g+kU^2).
$$

Equivalently, crest minus trough is the negative of this. For $kU^2/g\ll1$, hydrostatic elevation dominates; for $kU^2/g\gg1$, the Bernoulli [pressure](../../../thermodynamics.md#pressure) drop caused by faster crest flow dominates.

## 17H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="17h/a">a</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/a/solution">Solution</h4>

↑ **Parent:** [A](#17h/a)

The unrestricted maximum-likelihood estimates are $(\bar X,\bar Y)$, while the null fixes both means at zero. Hence

$$
-2\log\Lambda=m\bar X^2+n\bar Y^2.
$$

Under the null this is $\chi^2_2$, so the size-$\alpha$ [generalized likelihood-ratio test](../../../statistical-modelling.md#generalized-likelihood-ratio-test) rejects exactly when

$$
\boxed{m\bar X^2+n\bar Y^2>F_2^{-1}(1-\alpha).}
$$

<h3 id="17h/b">b</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/b/solution">Solution</h4>

↑ **Parent:** [B](#17h/b)

Under the null the common-mean estimate is $(m\bar X+n\bar Y)/(m+n)$. Completing squares gives

$$
-2\log\Lambda=\frac{mn}{m+n}(\bar X-\bar Y)^2=Z^2,
$$

where

$$
Z=\sqrt{\frac{mn}{m+n}}(\bar X-\bar Y)\sim N(0,1)
$$

under the null. The test rejects when

$$
|Z|>\Phi^{-1}(1-\alpha/2).
$$

<h3 id="17h/c">c</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/c/solution">Solution</h4>

↑ **Parent:** [C](#17h/c)

Put $u=\sqrt m\bar X$ and $v=\sqrt n\bar Y$. Test (a) accepts inside the disc

$$
u^2+v^2\leq q_2,\qquad q_2=F_2^{-1}(1-\alpha),
$$

whereas $Z$ is the projection of $(u,v)$ onto the unit [vector](../../../vector-space.md#vector)

$$
\left(\sqrt{\frac n{m+n}},-\sqrt{\frac m{m+n}}\right).
$$

If $q_1=[\Phi^{-1}(1-\alpha/2)]^2$, then $q_1$ is the corresponding $\chi^2_1$ quantile. Since a $\chi^2_2$ variable is stochastically larger than a $\chi^2_1$ variable, $q_2>q_1$. Choose a point on that unit-vector line with squared radius strictly between $q_1$ and $q_2$. A whole open neighborhood then makes (b) reject while (a) accepts. The joint normal density of $(\bar X,\bar Y)$ is strictly positive everywhere for every true $(\lambda,\mu)$, so this neighborhood always has positive probability.

## 18H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

Introduce unrestricted row and column potentials $u_i,v_j$. The dual is

$$
\text{maximize }\sum_i u_is_i+\sum_jv_jd_j
\quad\text{subject to }u_i+v_j\leq c_{ij}.
$$

Primal and dual feasible solutions are optimal precisely when [complementary slackness](../../../mathematical-optimization.md#complementary-slackness) holds:

$$
x_{ij}>0\implies u_i+v_j=c_{ij}.
$$

Indeed, the primal--dual objective gap is $\sum_{ij}x_{ij}(c_{ij}-u_i-v_j)$, a sum of nonnegative terms.

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

One of the $m+n$ balance equations is redundant, and the remaining $m+n-1$ have full rank. A nondegenerate [basic feasible solution](../../../mathematical-optimization.md#basic-feasible-solution) therefore has exactly $m+n-1$ positive variables. Equivalently, its positive cells form a spanning tree of the complete bipartite row--column graph.

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

The northwest-corner rule constructs an initial basic feasible solution: fill the current cell with the smaller remaining supply and demand, delete the exhausted row or column, and continue.

For a current spanning-tree [basis](../../../vector-space.md#basis), solve $u_i+v_j=c_{ij}$ on its occupied cells, fixing one potential to zero. The [reduced cost](../../../mathematical-optimization.md#reduced-cost) of an unoccupied cell is

$$
\bar c_{ij}=c_{ij}-u_i-v_j.
$$

If all reduced costs are nonnegative, part (a) proves optimality. Otherwise choose a cell with negative reduced cost. Adding its edge to the tree creates a unique even cycle. Mark its cells alternately $+$ and $-$, starting with $+$ at the entering cell, and set

$$
\theta=\min\{x_{ij}: (i,j)\text{ is a }-\text{ cell}\}.
$$

Add $\theta$ on the plus cells and subtract it on the minus cells. Row and column totals are unchanged, the entering cell becomes positive, and a minimizing minus cell leaves the [basis](../../../vector-space.md#basis). In the nondegenerate case the objective decreases strictly. There are finitely many [bases](../../../vector-space.md#basis), so no [basis](../../../vector-space.md#basis) repeats and the algorithm terminates at a [basis](../../../vector-space.md#basis) with no negative reduced cost, which is optimal.

<h3 id="18h/d">d</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/d/solution">Solution</h4>

↑ **Parent:** [D](#18h/d)

With integer supplies and demands, every northwest-corner allocation is integer. At each pivot, $\theta$ is the minimum of finitely many current allocations on the minus cells, so it remains integer; adding and subtracting it preserves integrality. The algorithm therefore reaches an integer-valued optimal solution.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
