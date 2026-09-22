# Paper 3

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperib_3_2022.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperib_3_2022.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2F](#2f)
  - [a](#2f/a)
    - [Solution](#2f/a/solution)
  - [b](#2f/b)
    - [Solution](#2f/b/solution)
- [3A](#3a)
  - [Solution](#3a/solution)
- [4D](#4d)
  - [Solution](#4d/solution)
- [5A](#5a)
  - [Solution](#5a/solution)
- [6B](#6b)
  - [a](#6b/a)
    - [Solution](#6b/a/solution)
  - [b](#6b/b)
    - [Solution](#6b/b/solution)
  - [c](#6b/c)
    - [Solution](#6b/c/solution)
- [7C](#7c)
  - [a](#7c/a)
    - [Solution](#7c/a/solution)
  - [b](#7c/b)
    - [Solution](#7c/b/solution)
- [8H](#8h)
  - [a](#8h/a)
    - [Solution](#8h/a/solution)
  - [b](#8h/b)
    - [Solution](#8h/b/solution)
- [9F](#9f)
  - [a](#9f/a)
    - [Solution](#9f/a/solution)
  - [b](#9f/b)
    - [Solution](#9f/b/solution)
  - [c](#9f/c)
    - [i](#9f/c/i)
      - [Solution](#9f/c/i/solution)
    - [ii](#9f/c/ii)
      - [Solution](#9f/c/ii/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
- [11G](#11g)
  - [Solution](#11g/solution)
- [12F](#12f)
  - [a](#12f/a)
    - [Solution](#12f/a/solution)
  - [b](#12f/b)
    - [Solution](#12f/b/solution)
- [13G](#13g)
  - [Solution](#13g/solution)
- [14A](#14a)
  - [a](#14a/a)
    - [Solution](#14a/a/solution)
  - [b](#14a/b)
    - [i](#14a/b/i)
      - [Solution](#14a/b/i/solution)
    - [ii](#14a/b/ii)
      - [Solution](#14a/b/ii/solution)
    - [iii](#14a/b/iii)
      - [Solution](#14a/b/iii/solution)
    - [iv](#14a/b/iv)
      - [Solution](#14a/b/iv/solution)
- [15D](#15d)
  - [a](#15d/a)
    - [Solution](#15d/a/solution)
  - [b](#15d/b)
    - [Solution](#15d/b/solution)
  - [c](#15d/c)
    - [Solution](#15d/c/solution)
- [16C](#16c)
  - [a](#16c/a)
    - [Solution](#16c/a/solution)
  - [b](#16c/b)
    - [Solution](#16c/b/solution)
  - [c](#16c/c)
    - [Solution](#16c/c/solution)
  - [d](#16c/d)
    - [Solution](#16c/d/solution)
  - [e](#16c/e)
    - [Solution](#16c/e/solution)
- [17C](#17c)
  - [a](#17c/a)
    - [Solution](#17c/a/solution)
  - [b](#17c/b)
    - [Solution](#17c/b/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
  - [d](#18h/d)
    - [Solution](#18h/d/solution)
- [19H](#19h)
  - [a](#19h/a)
    - [Solution](#19h/a/solution)
  - [b](#19h/b)
    - [Solution](#19h/b/solution)

## 1E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

The [first isomorphism theorem for rings](../../../commutative-algebra.md#first-isomorphism-theorem-for-rings) states that a ring homomorphism $\phi:R\to S$ induces an isomorphism

$$
R/\ker\phi\cong\operatorname{im}\phi.
$$

Because $J$ is an [ideal](../../../commutative-algebra.md#ideal), sums and products of elements of $R+J$ remain in $R+J$, so it is a subring. The surjective homomorphism

$$
R\longrightarrow(R+J)/J,
\qquad r\longmapsto r+J
$$

has kernel $R\cap J$. The theorem gives

$$
\boxed{R/(R\cap J)\cong(R+J)/J}.
$$

Evaluation at $-2$ gives

$$
\mathbb Q[X]/(X+2)\cong\mathbb Q,
$$

so this quotient is a [field](../../../algebra.md#field) of [characteristic](../../../algebra.md#characteristic-of-a-field) zero. The other quotient is

$$
\mathbb Z[X]/(3,X^2+X+1)
\cong\mathbb F_3[X]/((X-1)^2).
$$

It has characteristic $3$ but is not a field, since the nonzero class of $X-1$ is [nilpotent](../../../commutative-algebra.md#nilpotent).

## 2F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2f/a">a</h3>

↑ **Parent:** [2F](#2f)

<h4 id="2f/a/solution">Solution</h4>

↑ **Parent:** [A](#2f/a)

Let

$$
F(x,y,z)=x^2+y^2+z^3+az+b.
$$

By the [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem), $F^{-1}(0)$ is a smooth surface wherever $\nabla F\ne0$. A critical point on the level set would satisfy

$$
x=y=0,
\qquad a=-3z^2,
\qquad b=2z^3.
$$

These equations imply $4a^3+27b^2=0$. Therefore

$$
\boxed{4a^3+27b^2\ne0\Longrightarrow S_{a,b}\text{ is a smooth surface}.}
$$

<h3 id="2f/b">b</h3>

↑ **Parent:** [2F](#2f)

<h4 id="2f/b/solution">Solution</h4>

↑ **Parent:** [B](#2f/b)

If $4a^3+27b^2=0$ and $(a,b)\ne(0,0)$, there is a nonzero real number $r$ such that

$$
a=-3r^2,
\qquad b=2r^3.
$$

Then $(0,0,r)$ is singular and

$$
z^3+az+b=(z-r)^2(z+2r).
$$

For $r>0$, the singular point is locally isolated because all terms in

$$
x^2+y^2+(z-r)^2(z+2r)=0
$$

are nonnegative nearby. For $r<0$, the surface is locally a double cone with vertex at that point. Neither neighbourhood is homeomorphic to an open disc, so

$$
\boxed{S_{a,b}\text{ is not a smooth surface when }4a^3+27b^2=0.}
$$

## 3A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3a/solution">Solution</h3>

↑ **Parent:** [3A](#3a)

With the stated [Fourier transform](../../../analysis.md#fourier-transform) convention, [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
f(x)=\frac1{2\pi}\int_{-\infty}^{\infty}
\frac{-2ik}{p^2+k^2}e^{ikx},dk.
$$

For $x>0$, close the contour in the upper half-plane. [Jordan lemma](../../../complex-analysis.md#jordan-s-lemma) removes the semicircle contribution, and the only enclosed pole is $k=ip$. Its residue is

$$
\operatorname{Res}_{k=ip}
\frac{-2ik e^{ikx}}{(k-ip)(k+ip)}=-i e^{-px}.
$$

The [residue theorem](../../../analysis.md#residue-theorem) therefore yields

$$
\boxed{f(x)=e^{-px},\qquad x>0}.
$$

## 4D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4d/solution">Solution</h3>

↑ **Parent:** [4D](#4d)

At a regular constrained stationary point of $F$ on $G=0$, the [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) method solves

$$
\nabla F=\lambda\nabla G,
\qquad G=0.
$$

For the first problem, substitute $z=1+xy$ to obtain

$$
F=x^2+y^2+(1+xy)^2.
$$

Its stationary equations imply either $x=y$ or $xy=0$, and in either case the only real stationary point is $x=y=0$, $z=1$. Coercivity ensures that the minimum is attained, so

$$
\boxed{\min(x^2+y^2+z^2)=1}
$$

at $(0,0,1)$.

For the second problem, the [arithmetic-geometric mean inequality](../../../mathematical-optimization.md#arithmetic-geometric-mean-inequality) gives

$$
-xy\leq\frac{x^2+y^2}{2}=\frac{1-z^2}{2}.
$$

Consequently

$$
z-xy\leq z+\frac{1-z^2}{2}
=1-\frac{(z-1)^2}{2}\leq1.
$$

Equality occurs at $(0,0,1)$, and hence

$$
\boxed{\max_{x^2+y^2+z^2=1}(z-xy)=1}.
$$

## 5A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5a/solution">Solution</h3>

↑ **Parent:** [5A](#5a)

Differentiate the [Legendre differential equation](../../../differential-equation.md#legendre-differential-equation) and put $Q_n=P_n'$. This gives

$$
(1-x^2)Q_n''-4xQ_n'+(n-1)(n+2)Q_n=0.
$$

Multiplication by $1-x^2$ puts it in the [self-adjoint form](../../../analysis.md#sturm-liouville-theory)

$$
\boxed{
\frac d{dx}\left((1-x^2)^2Q_n'\right)
 +(n-1)(n+2)(1-x^2)Q_n=0}.
$$

The boundary term vanishes at $x=\pm1$. Distinct eigenvalues are therefore orthogonal with weight $1-x^2$:

$$
\boxed{
\int_{-1}^{1}(1-x^2)Q_n(x)Q_m(x),dx=0,
\qquad n\ne m.}
$$

## 6B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6b/a">a</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/a/solution">Solution</h4>

↑ **Parent:** [A](#6b/a)

For a free particle, the [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) is

$$
H=-\frac{\hbar^2}{2m}\frac{d^2}{dx^2}.
$$

Since $\chi''=-k^2\chi$,

$$
H\chi=\frac{\hbar^2k^2}{2m}\chi.
$$

Thus

$$
\boxed{E=\frac{\hbar^2k^2}{2m}\geq0,
\qquad p=\hbar k},
$$

where the momentum follows because $-i\hbar\,d\chi/dx=\hbar k\chi$.

<h3 id="6b/b">b</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/b/solution">Solution</h4>

↑ **Parent:** [B](#6b/b)

The [probability density](../../../quantum-mechanics.md#probability-density) and [probability current](../../../quantum-mechanics.md#probability-current) are

$$
\rho=|\psi|^2,
\qquad
J=\frac{\hbar}{2mi}
\left(\psi^*\frac{\partial\psi}{\partial x}
-\psi\frac{\partial\psi^*}{\partial x}\right).
$$

For a [stationary state](../../../quantum-mechanics.md#stationary-state), $\psi(x,t)=\chi(x)e^{-iEt/\hbar}$, so $\rho=|\chi|^2$ is independent of time. The [continuity equation](../../../physics.md#continuity-equation) then gives $\partial J/\partial x=0$. Hence

$$
\boxed{J\text{ is independent of }x}.
$$

<h3 id="6b/c">c</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/c/solution">Solution</h4>

↑ **Parent:** [C](#6b/c)

A plane wave $Ae^{ikx}$ carries current $(\hbar k/m)|A|^2$. The incident, reflected, and transmitted currents are therefore

$$
J_{\rm in}=\frac{\hbar k}{m},
\qquad
J_{\rm ref}=-\frac{\hbar k}{m}|R|^2,
\qquad
J_{\rm tr}=\frac{\hbar k}{m}|T|^2.
$$

Spatial constancy of the current gives

$$
J_{\rm in}+J_{\rm ref}=J_{\rm tr},
$$

and hence

$$
\boxed{|R|^2+|T|^2=1}.
$$

This is conservation of probability flux: every incident particle is either reflected or transmitted.

## 7C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7c/a">a</h3>

↑ **Parent:** [7C](#7c)

<h4 id="7c/a/solution">Solution</h4>

↑ **Parent:** [A](#7c/a)

Choose the polar axis along $\mathbf d$ and write $d=|\mathbf d|$. Since

$$
\mathbf d=d(\cos\theta\,\mathbf e_r-\sin\theta\,\mathbf e_\theta),
$$

the velocity components are

$$
u_r=\frac{d\cos\theta}{r^2},
\qquad
u_\theta=\frac{d\sin\theta}{r^2}.
$$

Their [divergence](../../../calculus.md#divergence) is

$$
\nabla\cdot\mathbf u
=\frac1r\frac{\partial}{\partial r}(ru_r)
 +\frac1r\frac{\partial u_\theta}{\partial\theta}
=-\frac{d\cos\theta}{r^3}
 +\frac{d\cos\theta}{r^3}=0.
$$

**Thus the flow is [incompressible](../../../fluid-mechanics.md#incompressible-flow) for $r\ne0$.**

<h3 id="7c/b">b</h3>

↑ **Parent:** [7C](#7c)

<h4 id="7c/b/solution">Solution</h4>

↑ **Parent:** [B](#7c/b)

For a two-dimensional incompressible flow, the [stream function](../../../fluid-mechanics.md#stream-function) convention

$$
u_r=\frac1r\frac{\partial\psi}{\partial\theta},
\qquad
u_\theta=-\frac{\partial\psi}{\partial r}
$$

is satisfied by

$$
\boxed{\psi(r,\theta)=\frac{d\sin\theta}{r}+C}.
$$

## 8H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8h/a">a</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/a/solution">Solution</h4>

↑ **Parent:** [A](#8h/a)

Expand according to the hitting time and use [detailed balance](../../../markov-process.md#detailed-balance) to reverse each finite path:

$$
\begin{aligned}
\mathbb P_\pi(X_{T_A}=z)
&=\sum_{n\geq0}
\sum_{x_0,\ldots,x_{n-1}\notin A}
\pi(x_0)P(x_0,x_1)\cdots P(x_{n-1},z)\\
&=\pi(z)\sum_{n\geq0}
\mathbb P_z(X_1,\ldots,X_n\notin A).
\end{aligned}
$$

The event in the final probability is $\{T_A^+>n\}$. The tail-sum formula for a nonnegative integer-valued random variable gives

$$
\sum_{n\geq0}\mathbb P_z(T_A^+>n)=\mathbb E_zT_A^+.
$$

Therefore

$$
\boxed{\mathbb P_\pi(X_{T_A}=z)=\pi(z)\mathbb E_zT_A^+}.
$$

<h3 id="8h/b">b</h3>

↑ **Parent:** [8H](#8h)

<h4 id="8h/b/solution">Solution</h4>

↑ **Parent:** [B](#8h/b)

Sum the identity from part (a) over $z\in A$. Since $X_{T_A}\in A$ almost surely under positive recurrence,

$$
1=\sum_{z\in A}\pi(z)\mathbb E_zT_A^+.
$$

Using the conditional stationary law $\pi_A(z)=\pi(z)/\pi(A)$ gives

$$
\mathbb E_{\pi_A}T_A^+
=\frac1{\pi(A)}
\sum_{z\in A}\pi(z)\mathbb E_zT_A^+.
$$

Hence the [return-time identity](../../../probability-and-statistics.md#kac-s-lemma)

$$
\boxed{\mathbb E_{\pi_A}T_A^+=\frac1{\pi(A)}}.
$$

## 9F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9f/a">a</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/a/solution">Solution</h4>

↑ **Parent:** [A](#9f/a)

The [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) $m_\alpha$ is the unique monic polynomial of least positive degree such that $m_\alpha(\alpha)=0$. The [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) says that $\alpha$ satisfies its characteristic polynomial, so such polynomials exist. Dividing any two monic candidates of least degree shows uniqueness.

If $m_\alpha(x)=x^m$, then $\alpha^m=0$ but $\alpha^{m-1}\ne0$. The least $r$ for which $(\alpha^3)^r=0$ is the least integer satisfying $3r\geq m$. Hence

$$
\boxed{m_{\alpha^3}(x)=x^{\lceil m/3\rceil}}.
$$

<h3 id="9f/b">b</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/b/solution">Solution</h4>

↑ **Parent:** [B](#9f/b)

If $\alpha v=\lambda v$ for nonzero $v$, then

$$
\alpha^3v=\lambda^3v,
$$

so $\lambda^3$ is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue). Let $\omega=e^{2\pi i/3}$. Since $\lambda\ne0$, the three factors of

$$
x^3-\lambda^3=(x-\lambda)(x-\omega\lambda)(x-\omega^2\lambda)
$$

are pairwise coprime. The [kernel decomposition for coprime polynomials](../../../linear-operator-theory.md#kernel-decomposition-for-coprime-polynomials) therefore gives

$$
\boxed{
E_{\lambda^3}(\alpha^3)
=E_\lambda(\alpha)\oplus E_{\omega\lambda}(\alpha)
\oplus E_{\omega^2\lambda}(\alpha)},
$$

where an absent eigenspace is interpreted as zero.

<h3 id="9f/c">c</h3>

↑ **Parent:** [9F](#9f)

<h4 id="9f/c/i">i</h4>

↑ **Parent:** [C](#9f/c)

<h5 id="9f/c/i/solution">Solution</h5>

↑ **Parent:** [I](#9f/c/i)

Set

$$
q(x)=\prod_{i=1}^k(x-\lambda_i^3)^{c_i}.
$$

For every $i$,

$$
\alpha^3-\lambda_i^3I
=(\alpha-\lambda_iI)
(\alpha^2+\lambda_i\alpha+\lambda_i^2I).
$$

Consequently $q(\alpha^3)$ contains $m_\alpha(\alpha)$ as a polynomial factor and is zero. By the divisibility property of the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial),

$$
\boxed{m_{\alpha^3}(x)\mid
\prod_{i=1}^k(x-\lambda_i^3)^{c_i}}.
$$

<h4 id="9f/c/ii">ii</h4>

↑ **Parent:** [C](#9f/c)

<h5 id="9f/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9f/c/ii)

If the nonzero $\lambda_i$ are real and distinct, their cubes are also distinct. Suppose the multiplicity of $x-\lambda_i^3$ in $m_{\alpha^3}$ were $d_i<c_i$. Since

$$
m_{\alpha^3}(\alpha^3)=0,
$$

minimality makes $m_\alpha(x)$ divide $m_{\alpha^3}(x^3)$. At $x=\lambda_i$, the factor $x^3-\lambda_i^3$ has a simple zero because its derivative is $3\lambda_i^2\ne0$. Thus $m_{\alpha^3}(x^3)$ has multiplicity only $d_i$ there, contradicting the multiplicity $c_i$ in $m_\alpha$. Every exponent is therefore $c_i$, and

$$
\boxed{m_{\alpha^3}(x)=
\prod_{i=1}^k(x-\lambda_i^3)^{c_i}}.
$$

## 10E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

Matrices over a [Euclidean domain](../../../commutative-algebra.md#euclidean-domain) are equivalent when $B=PAQ$ for invertible matrices $P,Q$, equivalently when one can pass between them by invertible elementary row and column operations.

For a nonzero matrix, move a nonzero entry to the top left and use Euclidean division and row or column operations to replace it by any nonzero remainder. Repeating terminates with an entry $d_1$ dividing every entry; otherwise adding an offending entry into its row would permit one more strict Euclidean reduction. Clear its row and column, then apply induction to the remaining submatrix. This proves equivalence to a diagonal matrix. It is in [Smith normal form](../../../algebra.md#smith-normal-form) when, up to units,

$$
d_1\mid d_2\mid\cdots\mid d_r.
$$

Applying these operations over $\mathbb Z$ does not change the isomorphism type of the quotient. If the Smith form of $A$ is $\operatorname{diag}(d_1,\ldots,d_n)$, then

$$
\mathbb Z^n/M\cong\bigoplus_i\mathbb Z/d_i\mathbb Z.
$$

It is finite exactly when every $d_i$ is nonzero, equivalently $\det A\ne0$, and then

$$
\boxed{|\mathbb Z^n/M|=\prod_i|d_i|=|\det A|}.
$$

Both displayed matrices have determinant of absolute value $8$. For $A_1$, the gcds of the entries and of the $2$ by $2$ minors are both $1$, giving Smith invariants

$$
(1,1,8),
\qquad G_1\cong\mathbb Z/8\mathbb Z.
$$

For $A_2$, those gcds are $1$ and $2$, giving

$$
(1,2,4),
\qquad G_2\cong\mathbb Z/2\mathbb Z\oplus\mathbb Z/4\mathbb Z.
$$

The first group has an element of order eight and the second does not, so

$$
\boxed{G_1\not\cong G_2}.
$$

## 11G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11g/solution">Solution</h3>

↑ **Parent:** [11G](#11g)

A map $T:X\to Y$ between metric spaces is a [contraction mapping](../../../analysis.md#contraction-mapping-theorem) if some $q<1$ satisfies $d(Tx,Ty)\leq qd(x,y)$ for all $x,y$.

The [Banach fixed-point theorem](../../../analysis.md#contraction-mapping-theorem) states that a contraction from a nonempty complete metric space to itself has a unique fixed point. Indeed, for $x_{n+1}=Tx_n$,

$$
d(x_{n+1},x_n)\leq q^nd(x_1,x_0),
$$

so the geometric-series estimate makes $(x_n)$ Cauchy. Completeness gives a limit $x_*$, continuity gives $Tx_*=x_*$, and

$$
d(x_*,y_*)\leq qd(x_*,y_*)
$$

proves uniqueness.

Every solution of $x=\cos x$ lies in $[-1,1]$. The cosine maps this complete interval into itself and, by the [mean value theorem](../../../calculus.md#mean-value-theorem), has Lipschitz constant at most $\sin1<1$ there. It therefore has exactly one real fixed point.

The [mean value inequality](../../../calculus.md#mean-value-inequality) says that on a convex domain, a uniform derivative bound $\lVert Df\rVert\leq M$ implies $\lVert f(x)-f(y)\rVert\leq M\lVert x-y\rVert$. Equip $\mathbb R^2$ with the maximum norm and take

$$
D=[0,1/2]\times[-1/2,1/2].
$$

For $(x,y)\in D$, elementary cosine bounds give

$$
f_1(x,y)\in[\cos(1/2)-1/2,1/2],
\qquad |f_2(x,y)|\leq1-\cos(1/2)<1/2,
$$

so $f(D)\subseteq D$. The maximum absolute row sum of

$$
Df=
\begin{pmatrix}
-\tfrac12\sin x&-\tfrac12\sin y\\
-\sin x&\sin y
\end{pmatrix}
$$

is at most $2\sin(1/2)<1$. The mean value inequality makes $f$ a contraction on the complete set $D$, so it has a fixed point.

## 12F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12f/a">a</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/a/solution">Solution</h4>

↑ **Parent:** [A](#12f/a)

A [topological surface](../../../topology.md#topological-surface) is a Hausdorff, second-countable space in which every point has a neighbourhood homeomorphic to an open subset of $\mathbb R^2$.

For $S_1$, interior points and points in the interiors of paired edges plainly have disc neighbourhoods. The corner identifications form two classes; in each class two quarter-discs are glued to make a half-disc, and the adjacent identified edge neighbourhoods complete a disc. Equivalently, this polygon is a cell decomposition of the [real projective plane](../../../differential-geometry.md#real-projective-plane), hence a quotient of $S^2$ by the antipodal group. Thus $S_1$ is a topological surface.

In $S_2$, three distinct sides labelled $a$ are identified. A point in the interior of their common image has a neighbourhood made from three half-discs meeting along their diameters. Removing the common diameter leaves three local sides rather than two, so this neighbourhood is not a disc or half-disc. Therefore

$$
\boxed{S_2\text{ is not a topological surface}.}
$$

<h3 id="12f/b">b</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/b/solution">Solution</h4>

↑ **Parent:** [B](#12f/b)

Cut the octagon for $S_3$ along a diagonal joining the appropriate two vertex classes. The two resulting polygons can be reattached along that diagonal in the opposite order. Reading the new boundary word gives the square word

$$
e f^{-1} e f,
$$

which is exactly the edge identification displayed for $S_4$. The cut-and-paste map is affine on the two pieces and respects every paired edge, so it descends to a [homeomorphism](../../../topology.md#homeomorphism) $S_3\cong S_4$. Both are the [Klein bottle](../../../topology.md#klein-bottle).

After deleting an open disc, the punctured Klein bottle can be realized as a boundary connected sum of two embedded [Möbius strips](../../../topology.md#mobius-band), and hence embeds in $\mathbb R^3$. The closed Klein bottle cannot embed: every connected closed surface embedded in $\mathbb R^3$ is two-sided and therefore orientable, by the [Jordan-Brouwer separation theorem](../../../geometry-and-topology.md#jordan-brouwer-separation-theorem), whereas the Klein bottle is nonorientable. Thus

$$
\boxed{S_4\setminus D^2\text{ embeds in }\mathbb R^3,
\qquad S_4\text{ does not}.}
$$

## 13G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="13g/solution">Solution</h3>

↑ **Parent:** [13G](#13g)

Uniform convergence on compact subsets makes $f$ continuous. For every triangle whose closure lies in $U$, uniform convergence on its boundary permits passage through the contour integral:

$$
\int_{\partial\Delta}f(z),dz
=\lim_{n\to\infty}\int_{\partial\Delta}f_n(z),dz=0.
$$

[Morera's theorem](../../../complex-analysis.md#morera-s-theorem) implies that $f$ is holomorphic. If a compact set $K\Subset U$ is surrounded by a finite union of contours at positive distance from $K$, the [Cauchy integral formula for derivatives](../../../complex-analysis.md#cauchy-derivative-formula) gives

$$
f_n'(z)-f'(z)
=\frac1{2\pi i}\int_\Gamma
\frac{f_n(\zeta)-f(\zeta)}{(\zeta-z)^2},d\zeta.
$$

The uniform bound on the surrounding compact set proves that $f_n'\to f'$ uniformly on $K$.

If $f$ had distinct zeros $c$ and $d$, choose disjoint small closed discs around them whose boundary contains no zero of $f$. Uniform convergence and [Rouché's theorem](../../../complex-analysis.md#rouche-s-theorem) imply that, for large $n$, $f_n$ has a zero in each disc, contradicting uniqueness of $c_n$. Thus $f$ has at most one zero.

For an example on the unit disc, take

$$
f_n(z)=z-(1-1/n),
\qquad c_n=1-1/n.
$$

Then $f_n\to f(z)=z-1$, which has no zero in the open disc. In general, [Hurwitz's theorem](../../../complex-analysis.md#hurwitz-s-theorem) shows that $f$ is zero-free exactly when the unique zeros escape every compact subset of $U$:

$$
\boxed{
\text{for every compact }K\Subset U,
\quad c_n\notin K\text{ eventually}.}
$$

Indeed, an interior accumulation point of $c_n$ is a zero of $f$, while a zero of $f$ forces the unique $c_n$ into each of its sufficiently small neighbourhoods.

## 14A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="14a/a">a</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/a/solution">Solution</h4>

↑ **Parent:** [A](#14a/a)

Apply [Green second identity](../../../partial-differential-equation.md#green-second-identity) to $u$ and the free-space [Green function](../../../analysis.md#green-s-function) $G_{fs}$ on $V$ with a small ball about $\mathbf r_0$ removed. Both functions are harmonic there, so only boundary terms remain. The contribution from the small sphere tends to $u(\mathbf r_0)$ because

$$
G_{fs}(\mathbf r;\mathbf r_0)=-\frac1{4\pi|\mathbf r-\mathbf r_0|}
$$

has unit delta source, while the remaining small-sphere term vanishes. Taking the radius to zero gives [Green's third identity](../../../partial-differential-equation.md#green-s-third-identity)

$$
\boxed{
u(\mathbf r_0)=
\int_S\left(u\frac{\partial G_{fs}}{\partial n}
-G_{fs}\frac{\partial u}{\partial n}\right)dS}.
$$

<h3 id="14a/b">b</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/b/i">i</h4>

↑ **Parent:** [B](#14a/b)

<h5 id="14a/b/i/solution">Solution</h5>

↑ **Parent:** [I](#14a/b/i)

Integrate $\nabla^2u=0$ over a large half-ball and apply the [divergence theorem](../../../calculus.md#divergence-theorem). The hemispherical contribution vanishes by the assumed decay. On $z=0$, the outward normal is $-\mathbf e_z$, so $\partial u/\partial n=-p$. Hence compatibility requires

$$
\boxed{\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}
p(x,y)\,dx\,dy=0}.
$$

This is the usual solvability condition for the [Neumann problem](../../../differential-equation.md#neumann-boundary-condition).

<h4 id="14a/b/ii">ii</h4>

↑ **Parent:** [B](#14a/b)

<h5 id="14a/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#14a/b/ii)

Reflect the source point $\mathbf r_0=(x_0,y_0,z_0)$ across the plane to $\mathbf r_0^*=(x_0,y_0,-z_0)$. Equal-sign source and image make the normal derivatives cancel on the plane. Thus the [method of images](../../../mathematics.md#method-of-images) gives the Neumann Green function

$$
\boxed{
G(\mathbf r;\mathbf r_0)
=-\frac1{4\pi}
\left(\frac1{|\mathbf r-\mathbf r_0|}
+\frac1{|\mathbf r-\mathbf r_0^*|}\right)},
\qquad
\left.\frac{\partial G}{\partial z}\right|_{z=0}=0.
$$

<h4 id="14a/b/iii">iii</h4>

↑ **Parent:** [B](#14a/b)

<h5 id="14a/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#14a/b/iii)

Green's identity with $\partial G/\partial n=0$ leaves only the prescribed normal derivative. Since $\partial u/\partial n=-p$ and, on the plane,

$$
G=-\frac1{2\pi\sqrt{(x-x_0)^2+(y-y_0)^2+z_0^2}},
$$

the decaying solution is

$$
\boxed{
u(x_0,y_0,z_0)
=-\frac1{2\pi}\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}
\frac{p(x,y)}{\sqrt{(x-x_0)^2+(y-y_0)^2+z_0^2}},dx,dy}.
$$

Thus

$$
\boxed{f(X,Y,z_0)=-\frac1{2\pi\sqrt{X^2+Y^2+z_0^2}}.}
$$

<h4 id="14a/b/iv">iv</h4>

↑ **Parent:** [B](#14a/b)

<h5 id="14a/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#14a/b/iv)

Use the large-$z_0$ expansion

$$
\frac1{\sqrt{z_0^2+R^2}}
=\frac1{z_0}-\frac{R^2}{2z_0^3}+O(z_0^{-5}).
$$

The first term vanishes by the compatibility condition. For the given $p$, symmetry leaves

$$
\int p(x,y)\bigl((x-x_0)^2+(y-y_0)^2\bigr),dx,dy
=-2x_0\left(\int_{-\pi/2}^{\pi/2}x\sin x\,dx\right)\pi
=-4\pi x_0.
$$

Consequently

$$
\boxed{
u(x_0,y_0,z_0)
=-\frac{x_0}{z_0^3}+O(z_0^{-5})}.
$$

## 15D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="15d/a">a</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/a/solution">Solution</h4>

↑ **Parent:** [A](#15d/a)

For $X^\mu=(ct,x,y,z)$, the stated [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) gives

$$
\boxed{
t'=\gamma\left(t-\frac{vx}{c^2}\right),
\qquad x'=\gamma(x-vt),
\qquad y'=y,
\qquad z'=z}.
$$

<h3 id="15d/b">b</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/b/solution">Solution</h4>

↑ **Parent:** [B](#15d/b)

Transforming the [electromagnetic field tensor](../../../electromagnetism.md#electromagnetic-field-tensor) by $F'=\Lambda F\Lambda^T$ and reading off its components gives

$$
\boxed{
\begin{aligned}
&E_1'=E_1,
&&E_2'=\gamma(E_2-vB_3),
&&E_3'=\gamma(E_3+vB_2),\\
&B_1'=B_1,
&&B_2'=\gamma\left(B_2+\frac{vE_3}{c^2}\right),
&&B_3'=\gamma\left(B_3-\frac{vE_2}{c^2}\right).
\end{aligned}}
$$

These are the parallel and transverse [field transformation laws](../../../electromagnetism.md#lorentz-transformation-of-electromagnetic-fields) for a boost in the $x$ direction.

<h3 id="15d/c">c</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/c/solution">Solution</h4>

↑ **Parent:** [C](#15d/c)

Take the wire along the $x$-axis and let $r$ be perpendicular distance from it. [Gauss's law](../../../electromagnetism.md#gauss-s-law) and cylindrical symmetry give

$$
\mathbf E=\frac{\lambda}{2\pi\varepsilon_0r}\,\mathbf e_r,
\qquad \mathbf B=0.
$$

For an observer boosted parallel to the wire,

$$
\boxed{
\mathbf E'=\gamma\frac{\lambda}{2\pi\varepsilon_0r}\,\mathbf e_r,
\qquad
\mathbf B'=-\frac{\gamma}{c^2}\mathbf v\times\mathbf E}.
$$

The moving observer sees length contraction and hence line density $\lambda'=\gamma\lambda$, together with current $I'=-\gamma\lambda v$. The transformed magnetic field is exactly

$$
B'=\frac{\mu_0|I'|}{2\pi r},
$$

with the direction prescribed by the current. This is [Ampère's law](../../../electromagnetism.md#ampere-s-circuital-law) for the current seen in the moving frame.

## 16C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="16c/a">a</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/a/solution">Solution</h4>

↑ **Parent:** [A](#16c/a)

Axisymmetry and [incompressibility](../../../fluid-mechanics.md#incompressible-flow) give

$$
0=\nabla\cdot\mathbf u
=\frac1r\frac{d}{dr}(ru_r).
$$

Thus $ru_r=C$. Finiteness at the origin forces $C=0$, so

$$
\boxed{u_r=0}.
$$

<h3 id="16c/b">b</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/b/solution">Solution</h4>

↑ **Parent:** [B](#16c/b)

Using the polar-coordinate [curl](../../../calculus.md#curl) with $u_\theta=r\Omega(r)$ gives

$$
\boxed{
\boldsymbol\omega=\nabla\times\mathbf u
=\left(2\Omega+r\frac{d\Omega}{dr}\right)\mathbf e_z}.
$$

<h3 id="16c/c">c</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/c/solution">Solution</h4>

↑ **Parent:** [C](#16c/c)

Take the curl of the [Navier-Stokes equation](../../../viscous-fluid-flow.md#navier-stokes-equation). The pressure term disappears, curl commutes with the Laplacian, and the incompressible vector identity

$$
\nabla\times((\mathbf u\cdot\nabla)\mathbf u)
=(\mathbf u\cdot\nabla)\boldsymbol\omega
-(\boldsymbol\omega\cdot\nabla)\mathbf u
$$

gives

$$
\frac{\partial\boldsymbol\omega}{\partial t}
 +(\mathbf u\cdot\nabla)\boldsymbol\omega
=(\boldsymbol\omega\cdot\nabla)\mathbf u
 +\nu\nabla^2\boldsymbol\omega.
$$

Therefore the [material derivative](../../../continuum-mechanics.md#material-derivative) form is

$$
\boxed{
\frac{D\boldsymbol\omega}{Dt}
=(\boldsymbol\omega\cdot\nabla)\mathbf u
+\nu\nabla^2\boldsymbol\omega}.
$$

<h3 id="16c/d">d</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/d/solution">Solution</h4>

↑ **Parent:** [D](#16c/d)

The vorticity is normal to the plane, so the stretching term vanishes. Axisymmetry also makes angular advection vanish, and part (a) gives no radial advection. Hence the scalar [vorticity equation](../../../physics.md#vorticity-equation) is the radial [diffusion equation](../../../diffusion-equation.md)

$$
\boxed{
\frac{\partial\omega}{\partial t}
=\nu\left(\frac{\partial^2\omega}{\partial r^2}
 +\frac1r\frac{\partial\omega}{\partial r}\right)}.
$$

<h3 id="16c/e">e</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/e/solution">Solution</h4>

↑ **Parent:** [E](#16c/e)

Set the [similarity variable](../../../partial-differential-equation.md#similarity-variable)

$$
\xi=\frac r{\sqrt{\nu t}},
\qquad \omega(r,t)=W(\xi).
$$

Then

$$
\omega_t=-\frac{\xi}{2t}W',
\qquad
\nu\left(\omega_{rr}+\frac1r\omega_r\right)
=\frac1t\left(W''+\frac1\xi W'\right).
$$

The factors of $t$ cancel, leaving the self-similar ordinary differential equation

$$
\boxed{W''+\left(\frac1\xi+\frac\xi2\right)W'=0}.
$$

## 17C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="17c/a">a</h3>

↑ **Parent:** [17C](#17c)

<h4 id="17c/a/solution">Solution</h4>

↑ **Parent:** [A](#17c/a)

Insert the exact data $y(t)=P(t)$ into the [linear multistep method](../../../numerical-analysis.md#linear-multistep-method). Its local residual is the linear functional

$$
\mathcal L_h[P]
=\sum_{k=0}^s\rho_kP(t_{n+k})
-h\sum_{k=0}^s\sigma_kP'(t_{n+k}).
$$

Taylor expansion about $t_n$ shows that a method has order $p$ exactly when this functional annihilates the monomials $1,t,\ldots,t^p$; by linearity this is equivalent to annihilating every polynomial of degree at most $p$. This is precisely

$$
\boxed{
\sum_{k=0}^s\rho_kP(t_{n+k})
=h\sum_{k=0}^s\sigma_kP'(t_{n+k})}.
$$

<h3 id="17c/b">b</h3>

↑ **Parent:** [17C](#17c)

<h4 id="17c/b/solution">Solution</h4>

↑ **Parent:** [B](#17c/b)

The [Dahlquist equivalence theorem](../../../numerical-analysis.md#dahlquist-equivalence-theorem) says that a consistent linear multistep method is convergent exactly when it is zero-stable. Here

$$
\rho(z)=z^3+(2a-3)z^2-(2a-3)z-1
=(z-1)\bigl(z^2+2(a-1)z+1\bigr).
$$

The consistency conditions hold for every $a$. The two quadratic roots have product one. They are distinct and on the unit circle exactly when $0<a<2$; at $a=2$ the root $-1$ is repeated, while outside this interval one root has modulus greater than one. The [root condition for a multistep method](../../../numerical-analysis.md#root-condition-for-a-multistep-method) therefore gives

$$
\boxed{\text{convergence exactly for }0<a<2}.
$$

The polynomial exactness conditions hold through degree two, while the degree-three residual is $6-a$. Every convergent member thus has

$$
\boxed{\text{order }2}.
$$

(The exceptional value $a=6$ has formal order four but is not zero-stable.)

## 18H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

The log likelihood, up to constants, is

$$
-\frac n2\log\sigma^2
-\frac1{2\sigma^2}(Y-X\beta)^T\Sigma_0^{-1}(Y-X\beta).
$$

Differentiation gives the [generalized least squares estimator](../../../statistical-modelling.md#generalized-least-squares)

$$
\boxed{
\widehat\beta=(X^T\Sigma_0^{-1}X)^{-1}X^T\Sigma_0^{-1}Y},
$$

and maximizing over the scale gives

$$
\boxed{
\widehat\sigma^2
=\frac1n(Y-X\widehat\beta)^T\Sigma_0^{-1}(Y-X\widehat\beta)}.
$$

The divisor $n$ is appropriate for maximum likelihood rather than unbiased estimation.

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

The estimator is an affine transformation of the [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution). Its mean is $\beta$, and direct covariance calculation gives

$$
\boxed{
\widehat\beta\sim
N_p\left(\beta,
\sigma^2(X^T\Sigma_0^{-1}X)^{-1}\right)}.
$$

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

Write $\widehat\beta=AY$, where

$$
A=(X^T\Sigma_0^{-1}X)^{-1}X^T\Sigma_0^{-1},
\qquad AX=I.
$$

Any other linear unbiased estimator is $CY$ with $CX=I$, so $C=A+D$ and $DX=0$. The cross covariance vanishes because

$$
A\Sigma_0D^T
=(X^T\Sigma_0^{-1}X)^{-1}X^TD^T=0.
$$

Therefore

$$
\operatorname{Cov}(CY)-\operatorname{Cov}(AY)
=\sigma^2D\Sigma_0D^T\succeq0.
$$

By the [Gauss-Markov theorem](../../../statistical-modelling.md#gauss-markov-theorem),

$$
\boxed{\widehat\beta\text{ is the best linear unbiased estimator of }\beta}.
$$

<h3 id="18h/d">d</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/d/solution">Solution</h4>

↑ **Parent:** [D](#18h/d)

Let $\nu=n/2-p$. Under $H_0$, the two residual sums of squares are independent and satisfy

$$
\frac{\lVert Y_i-X_i(X_i^TX_i)^{-1}X_i^TY_i\rVert^2}{\sigma^2}
\sim\chi^2_\nu,
\qquad i=1,2.
$$

Hence

$$
\boxed{T\sim F_{\nu,\nu}\quad\text{under }H_0}.
$$

Under $H_1$, the numerator is scaled by the smaller variance, so small values provide evidence against the null. If $F^{-1}_{\nu,\nu}(\alpha)$ denotes the lower $\alpha$ quantile, a size-$\alpha$ test rejects when

$$
\boxed{T<F^{-1}_{\nu,\nu}(\alpha)}.
$$

## 19H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="19h/a">a</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/a/solution">Solution</h4>

↑ **Parent:** [A](#19h/a)

A [transportation problem](../../../mathematical-optimization.md#transportation-problem) chooses nonnegative shipments $x_{ij}$ from $n$ suppliers to $m$ consumers so that row sums equal supplies and column sums equal demands, while minimizing $\sum c_{ij}x_{ij}$.

The north-west corner rule gives

$$
X_{NW}=
\begin{pmatrix}
3&3&0&0\\
0&2&2&0\\
0&0&5&3
\end{pmatrix}.
$$

It has $3+4-1=6$ positive cells and its support contains no cycle, so it is a nondegenerate [basic feasible solution](../../../mathematical-optimization.md#basic-feasible-solution).

A degenerate basic feasible solution is

$$
\boxed{
X_D=
\begin{pmatrix}
3&0&3&0\\
0&0&4&0\\
0&5&0&3
\end{pmatrix}}.
$$

Its five positive cells form a forest with two balanced components; adding one zero cell that joins the components completes a basis of six cells. Thus at least one basic variable is zero.

<h3 id="19h/b">b</h3>

↑ **Parent:** [19H](#19h)

<h4 id="19h/b/solution">Solution</h4>

↑ **Parent:** [B](#19h/b)

The stated plan is

$$
X=
\begin{pmatrix}
3&0&3&0\\
0&4&0&0\\
0&1&4&3
\end{pmatrix}.
$$

Its six positive cells form a spanning tree of the supplier--consumer bipartite graph, so it is basic and feasible. Taking $u_1=0$, the basic-cell equations $u_i+v_j=c_{ij}$ give

$$
u=(0,-4,-3),
\qquad v=(1,5,4,4).
$$

The complete matrix of [reduced costs](../../../mathematical-optimization.md#reduced-cost) $\bar c_{ij}=c_{ij}-u_i-v_j$ is

$$
\overline C=
\begin{pmatrix}
0&-2&0&2\\
4&0&2&4\\
6&0&0&0
\end{pmatrix}.
$$

The negative entry $\bar c_{12}=-2$ proves that the plan is not optimal.

Enter cell $(1,2)$. The alternating cycle is

$$
(1,2)^+,(1,3)^-,(3,3)^+,(3,2)^-,
$$

and the step is $\theta=\min(3,1)=1$. The new plan is

$$
X'=
\begin{pmatrix}
3&1&2&0\\
0&4&0&0\\
0&0&5&3
\end{pmatrix},
$$

whose cost is $26$, down from $28$. New potentials are

$$
u=(0,-2,-3),
\qquad v=(1,3,4,4),
$$

and the reduced-cost matrix is

$$
\overline C'=
\begin{pmatrix}
0&0&0&2\\
2&0&0&2\\
6&2&0&0
\end{pmatrix}.
$$

Every reduced cost is nonnegative, so the [transportation optimality criterion](../../../mathematical-optimization.md#transportation-problem) shows that

$$
\boxed{X'\text{ is optimal, with total cost }26}.
$$

The zero reduced cost in cell $(2,3)$ also indicates an alternative optimum.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
