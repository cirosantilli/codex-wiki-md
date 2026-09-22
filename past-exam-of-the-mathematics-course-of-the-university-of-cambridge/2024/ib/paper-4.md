# Paper 4

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperib_4_2024.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperib_4_2024.pdf)

**Table of contents**

- [1G](#1g)
  - [Solution](#1g/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
- [5C](#5c)
  - [Solution](#5c/solution)
- [6D](#6d)
  - [Solution](#6d/solution)
- [7H](#7h)
  - [a](#7h/a)
    - [Solution](#7h/a/solution)
  - [b](#7h/b)
    - [i](#7h/b/i)
      - [Solution](#7h/b/i/solution)
    - [ii](#7h/b/ii)
      - [Solution](#7h/b/ii/solution)
- [8G](#8g)
  - [a](#8g/a)
    - [Solution](#8g/a/solution)
  - [b](#8g/b)
    - [Solution](#8g/b/solution)
- [9E](#9e)
  - [a](#9e/a)
    - [Solution](#9e/a/solution)
  - [b](#9e/b)
    - [i](#9e/b/i)
      - [Solution](#9e/b/i/solution)
    - [ii](#9e/b/ii)
      - [Solution](#9e/b/ii/solution)
- [10F](#10f)
  - [Solution](#10f/solution)
- [11G](#11g)
  - [a](#11g/a)
    - [Solution](#11g/a/solution)
  - [b](#11g/b)
    - [Solution](#11g/b/solution)
  - [c](#11g/c)
    - [Solution](#11g/c/solution)
- [12B](#12b)
  - [i](#12b/i)
    - [Solution](#12b/i/solution)
  - [ii](#12b/ii)
    - [Solution](#12b/ii/solution)
  - [iii](#12b/iii)
    - [Solution](#12b/iii/solution)
- [13C](#13c)
  - [Solution](#13c/solution)
- [14B](#14b)
  - [i](#14b/i)
    - [Solution](#14b/i/solution)
  - [ii](#14b/ii)
    - [Solution](#14b/ii/solution)
  - [iii](#14b/iii)
    - [Solution](#14b/iii/solution)
- [15A](#15a)
  - [i](#15a/i)
    - [Solution](#15a/i/solution)
  - [ii](#15a/ii)
    - [Solution](#15a/ii/solution)
  - [iii](#15a/iii)
    - [Solution](#15a/iii/solution)
  - [iv](#15a/iv)
    - [Solution](#15a/iv/solution)
- [16D](#16d)
  - [Solution](#16d/solution)
- [17H](#17h)
  - [a](#17h/a)
    - [Solution](#17h/a/solution)
  - [b](#17h/b)
    - [Solution](#17h/b/solution)
  - [c](#17h/c)
    - [Solution](#17h/c/solution)
  - [d](#17h/d)
    - [Solution](#17h/d/solution)
  - [e](#17h/e)
    - [Solution](#17h/e/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)

## 1G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1g/solution">Solution</h3>

↑ **Parent:** [1G](#1g)

The [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) theorem says that every complex square [matrix](../../../vector-space.md#matrix) is similar to a direct sum of Jordan blocks, uniquely up to their order. For an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$, if its blocks have sizes $n_1,\ldots,n_r$, then its [algebraic multiplicity](../../../linear-operator-theory.md#algebraic-multiplicity) and [geometric multiplicity](../../../linear-operator-theory.md#geometric-multiplicity) are

$$
a_\lambda=\sum_{j=1}^r n_j,
\qquad
g_\lambda=r,
$$

and its contribution to the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) is $(t-\lambda)^{\max_j n_j}$. Thus

$$
m_\alpha(t)=\prod_\lambda(t-\lambda)^{s_\lambda},
$$

where $s_\lambda$ is the largest $\lambda$-block size.

For the given [matrix](../../../vector-space.md#matrix),

$$
\det(tI-A)=(t-2)(t+1)^2.
$$

Moreover,

$$
\dim\ker(A-2I)=1,
\qquad
\dim\ker(A+I)=1.
$$

Hence

$$
\boxed{a_2=g_2=1,
\qquad a_{-1}=2,
\qquad g_{-1}=1}.
$$

The [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-1$ therefore has one Jordan block of size two, so

$$
\boxed{m_\alpha(t)=(t-2)(t+1)^2}.
$$

## 2F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

A subset $A\subseteq X$ is connected if it cannot be written as $A=U\cup V$, where $U,V$ are disjoint, nonempty sets open in the subspace topology on $A$.

If $f(X)$ were disconnected as $U\cup V$, continuity would make $f^{-1}(U)$ and $f^{-1}(V)$ a disconnection of $X$. Thus the [continuous image of a connected space](../../../geometry-and-topology.md#continuous-image-of-a-connected-space) is connected.

For $Y=\{0,1\}$ with the discrete topology, a nonconstant continuous $h:X\to Y$ gives the disconnection

$$
X=h^{-1}(\{0\})\cup h^{-1}(\{1\}).
$$

Conversely, a disconnection $X=U\cup V$ defines a continuous nonconstant [function](../../../function.md) by assigning $0$ on $U$ and $1$ on $V$. Hence $X$ is connected exactly when every such $h$ is constant.

Finally suppose $C$ is connected but $\operatorname{Cl}(C)=U\cup V$ is a disconnection. The intersections $C\cap U$ and $C\cap V$ cannot both be nonempty, so, after interchanging $U,V$, we have $C\subseteq U$. For any $v\in V$, the relatively open neighbourhood $V$ of $v$ in $\operatorname{Cl}(C)$ is disjoint from $C$, contradicting $v\in\operatorname{Cl}(C)$. Therefore the [closure of a connected set](../../../geometry-and-topology.md#closure-of-a-connected-set) is connected.

## 3F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

A [function](../../../function.md) $f:U\to\mathbb C$ is holomorphic when it is complex [differentiable](../../../analysis.md#differentiable-function) at every point of the open connected set $U$. [Morera's theorem](../../../complex-analysis.md#morera-s-theorem) states that a [continuous function](../../../calculus.md#continuous-function) on a domain is holomorphic if its [integral](../../../calculus.md#integral) around every triangle whose interior lies in the domain is zero.

The integrand $e^{tz}/(1+t^2)$ is continuous jointly in $(t,z)$ on $[0,1]\times\mathbb C$, so the displayed [integral](../../../calculus.md#integral) defines a [continuous function](../../../calculus.md#continuous-function). For any triangle $T$, Fubini's theorem and the Cauchy [integral](../../../calculus.md#integral) theorem give

$$
\int_{\partial T}f(z)\,dz
=\int_0^1\frac1{1+t^2}
\left(\int_{\partial T}e^{tz}\,dz\right)dt
=0.
$$

Morera's theorem therefore proves that $f$ is entire.

The [function](../../../function.md) $1/z$ is holomorphic on $\mathbb C\setminus\{0\}$ but has no antiderivative there, because an antiderivative would integrate to zero around every closed curve whereas

$$
\int_{|z|=1}\frac{dz}{z}=2\pi i.
$$

This is the standard [period obstruction to a holomorphic antiderivative](../../../complex-analysis.md#period-obstruction-to-a-holomorphic-antiderivative).

## 4A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

The time-independent [Schrödinger equation](../../../physics.md#schrodinger-equation) is

$$
-\frac{\hbar^2}{2m}\psi''(x)+V(x)\psi(x)=E\psi(x).
$$

Integrating it over $(a-\varepsilon,a+\varepsilon)$ and letting $\varepsilon\to0$ shows that $\psi'$ has no jump because $V$ is finite. A jump in $\psi$ would create a delta term in $\psi'$ and hence a [derivative](../../../calculus.md#derivative) of a delta in $\psi''$, so $\psi$ is also continuous.

For a [bound state](../../../quantum-mechanics.md#bound-state) $-V_0<E<0$, define

$$
\eta^2=-\frac{2mE}{\hbar^2},
\qquad
k^2=\frac{2m(E+V_0)}{\hbar^2}.
$$

Then the proposed even [wavefunction](../../../quantum-mechanics.md#wave-function) solves the equation away from the interfaces, and

$$
\boxed{k^2+\eta^2=\frac{2mV_0}{\hbar^2}}.
$$

Continuity at $x=a$ gives $B\cos(ka)=Ae^{-\eta a}$, while continuity of the [derivative](../../../calculus.md#derivative) gives $-Bk\sin(ka)=-A\eta e^{-\eta a}$. Dividing yields the second required relation

$$
\boxed{\eta=k\tan(ka)}.
$$

**Thus the lowest even state of the [finite square well](../../../quantum-mechanics.md#finite-square-well) is the first-quadrant intersection, with $0<ka<\pi/2$, of the circle $k^2+\eta^2=2mV_0/\hbar^2$ and the curve $\eta=k\tan(ka)$.**

## 5C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5c/solution">Solution</h3>

↑ **Parent:** [5C](#5c)

[Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) is

$$
\mathcal E=\oint_C\mathbf E\cdot d\mathbf l
=-\frac{d\Phi_B}{dt},
\qquad
\Phi_B=\int_S\mathbf B\cdot d\mathbf S.
$$

Choose the positive [circulation](../../../fluid-mechanics.md#circulation-physics) to be anticlockwise as viewed from $+z$. Since $\Phi_B=\pi Br^2$,

$$
\boxed{I=\frac{\mathcal E}{R}
=-\frac{2\pi Br\dot r}{R}}.
$$

If $\dot r>0$, the current is clockwise and its field points in the $-z$ direction, reducing the field inside the loop. Since $d\mathbf F=I\,d\mathbf l\times\mathbf B$, the force due to the imposed field is radially inward. If $\dot r<0$, the current is anticlockwise, its field points in the $+z$ direction and increases the field inside, while the force is radially outward. In both cases the magnetic force opposes the radial motion, in accordance with [Lenz's law](../../../electromagnetism.md#lenz-s-law).

## 6D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6d/solution">Solution</h3>

↑ **Parent:** [6D](#6d)

On each interval of width $h=1/N$, Taylor expansion about its midpoint shows that the local midpoint-rule error is $O(h^3)$. Summing over $N$ intervals gives the [composite midpoint rule error](../../../numerical-analysis.md#composite-midpoint-rule-error)

$$
\boxed{I(f)-I_N(f)=O(N^{-2})}.
$$

To remove the endpoint singularity, set $x=s^2$. Then

$$
I(f)=\int_0^1 2s f(s^2)\,ds
=\int_0^1 2g(s^2)\,ds,
$$

whose transformed integrand is analytic. Applying the composite midpoint rule in $s$ with $s_n=(n+\tfrac12)/N$ gives

$$
I(f)\approx\frac2N\sum_{n=0}^{N-1}s_nf(s_n^2).
$$

This has the required form when

$$
\boxed{y_n=s_n^2
=\left(\frac{n+\tfrac12}{N}\right)^2}.
$$

The [quadratic substitution for a square-root endpoint singularity](../../../numerical-analysis.md#quadratic-substitution-for-a-square-root-endpoint-singularity) therefore restores second-order convergence.

## 7H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7h/a">a</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/a/solution">Solution</h4>

↑ **Parent:** [A](#7h/a)

With states ordered as $(A,B,C)$ and rows representing the current state, the [Markov chain](../../../markov-process.md#markov-chain) has transition [matrix](../../../vector-space.md#matrix)

$$
\boxed{
P=\begin{pmatrix}
0&1/2&1/2\\
3/4&0&1/4\\
3/4&1/4&0
\end{pmatrix}}.
$$

<h3 id="7h/b">b</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/b/i">i</h4>

↑ **Parent:** [B](#7h/b)

<h5 id="7h/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7h/b/i)

Starting from the airport, after one step the distribution is $(0,1/2,1/2)$. Multiplying once more by $P$ gives

$$
\boxed{\mathbb P(X_2=A)=\frac34,
\qquad
\mathbb P(X_2=B)=\mathbb P(X_2=C)=\frac18}.
$$

<h4 id="7h/b/ii">ii</h4>

↑ **Parent:** [B](#7h/b)

<h5 id="7h/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7h/b/ii)

Let $p_n=\mathbb P(X_n=A)$. Whenever the taxi is away from the airport it returns with probability $3/4$, whereas it must leave whenever it is at the airport. Hence

$$
p_{n+1}=\frac34(1-p_n),
\qquad p_0=1.
$$

Subtracting the fixed point $3/7$ gives

$$
p_{n+1}-\frac37=-\frac34
\left(p_n-\frac37\right).
$$

Therefore

$$
\boxed{
p_n=\frac37+\frac47\left(-\frac34\right)^n
}
$$

for every $n\geq0$, and in particular for the requested $n\geq1$.

## 8G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8g/a">a</h3>

↑ **Parent:** [8G](#8g)

<h4 id="8g/a/solution">Solution</h4>

↑ **Parent:** [A](#8g/a)

Two [matrices](../../../vector-space.md#matrix) are equivalent when $A'=PAQ$ for invertible [matrices](../../../vector-space.md#matrix) $P$ and $Q$ of the appropriate sizes. A change of [basis](../../../vector-space.md#basis) in the codomain multiplies a [matrix](../../../vector-space.md#matrix) on the left, while a change of [basis](../../../vector-space.md#basis) in the domain multiplies it on the right. Hence two [matrices](../../../vector-space.md#matrix) of the same [linear map](../../../vector-space.md#linear-map) in two pairs of [bases](../../../vector-space.md#basis) are equivalent.

Conversely, start with the map $\alpha:F^n\to F^m$ having [matrix](../../../vector-space.md#matrix) $A$ in the standard [bases](../../../vector-space.md#basis). Given $A'=PAQ$, choose domain and codomain [bases](../../../vector-space.md#basis) whose change-of-coordinate [matrices](../../../vector-space.md#matrix) produce $Q$ and $P$; then $A'$ represents the same map in those [bases](../../../vector-space.md#basis). This proves the equivalence.

The column rank of $A$ is the dimension of the span of its columns, and its row rank is the dimension of the span of its rows. If $A$ represents $\alpha:F^n\to F^m$, its column rank is $\operatorname{rank}\alpha$. The transpose represents the dual map

$$
\alpha^*:(F^m)^*\to(F^n)^*,
\qquad \phi\mapsto\phi\circ\alpha,
$$

so the row rank is $\operatorname{rank}\alpha^*$.

If $\operatorname{rank}\alpha=r$, then

$$
\ker\alpha^*=(\operatorname{im}\alpha)^0,
$$

whose dimension is $m-r$: extend a [basis](../../../vector-space.md#basis) of $\operatorname{im}\alpha$ to one of $F^m$ and use the dual [basis](../../../vector-space.md#basis). Rank-nullity now gives $\operatorname{rank}\alpha^*=r$. This proves the [equality of row rank and column rank](../../../linear-algebra.md#equality-of-row-rank-and-column-rank).

<h3 id="8g/b">b</h3>

↑ **Parent:** [8G](#8g)

<h4 id="8g/b/solution">Solution</h4>

↑ **Parent:** [B](#8g/b)

For $I\subseteq[m]$, the independent [vectors](../../../vector-space.md#vector) $\{v_i:i\in I\}$ lie in the coordinate subspace supported on

$$
S_I=\bigcup_{i\in I}\operatorname{supp}(v_i),
$$

which has dimension $|S_I|$. Hence $|I|\leq|S_I|$, and the stated form of [Hall marriage theorem](../../../graph-theory.md#hall-s-marriage-theorem) gives an injection $f$ with $f(i)\in\operatorname{supp}(v_i)$.

Let $V$ be the $n\times m$ [matrix](../../../vector-space.md#matrix) whose $i$th column is $v_i$. Its column rank is $m$. By equality of row and column rank, it has $m$ linearly independent rows. Let $B$ be their indices. The $m\times m$ submatrix $V_B$ is invertible, so its columns are independent. Those columns are exactly the nonzero coordinates of $Bv_1,\ldots,Bv_m$, and therefore these truncated [vectors](../../../vector-space.md#vector) are linearly independent.

Expanding $\det V_B$ gives a permutation $f:[m]\to B$ for which

$$
\prod_{i=1}^m (v_i)_{f(i)}\ne0.
$$

Thus $f(i)\in\operatorname{supp}(v_i)$. Finally, order the coordinates with $B$ first. The [matrix](../../../vector-space.md#matrix) whose columns are the $v_i$ together with the $e_j$ for $j\notin B$ is block triangular, with diagonal blocks $V_B$ and an identity [matrix](../../../vector-space.md#matrix). Its [determinant](../../../linear-algebra.md#determinant) is nonzero. Consequently

$$
\boxed{
\bigl(\{e_j:j\in[n]\}\setminus\{e_{f(i)}:i\in[m]\}\bigr)
\cup\{v_i:i\in[m]\}
}
$$

is a [basis](../../../vector-space.md#basis) of $\mathbb C^n$. This is the [simultaneous basis exchange from a nonzero minor](../../../linear-algebra.md#simultaneous-basis-exchange-from-a-nonzero-minor).

## 9E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9e/a">a</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/a/solution">Solution</h4>

↑ **Parent:** [A](#9e/a)

An $R$-module is free if it has a [basis](../../../vector-space.md#basis): a subset $B$ such that every element has a unique expression as a finite $R$-linear combination of elements of $B$.

Choose a maximal [ideal](../../../commutative-algebra.md#ideal) $\mathfrak m$ of the nonzero [ring](../../../commutative-algebra.md#ring) $R$. If $R^n\cong R^m$, quotienting by $\mathfrak m$ gives

$$
(R/\mathfrak m)^n\cong(R/\mathfrak m)^m.
$$

These are [vector spaces](../../../vector-space.md) over the field $R/\mathfrak m$, so equality of dimension gives $n=m$. This proves [invariant basis number for a commutative ring](../../../module-theory.md#invariant-basis-number-for-a-commutative-ring).

A direct summand of a free module need not be free. Take $R=\mathbb Z/6\mathbb Z$. Its [ideals](../../../commutative-algebra.md#ideal) $P=(2)$ and $Q=(3)$ satisfy

$$
P\cap Q=0,
\qquad P+Q=R,
$$

so $P\oplus Q\cong R$. But $P$ has three elements, whereas a finite-rank free $R$-module has $6^r$ elements; hence $P$ is not free.

<h3 id="9e/b">b</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/b/i">i</h4>

↑ **Parent:** [B](#9e/b)

<h5 id="9e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9e/b/i)

Let $P$ be free with [basis](../../../vector-space.md#basis) $(e_i)_{i\in I}$. Given a surjection $f:M\to N$ and a map $g:P\to N$, choose $m_i\in M$ satisfying $f(m_i)=g(e_i)$. There is a unique [linear map](../../../vector-space.md#linear-map) $h:P\to M$ with $h(e_i)=m_i$, and on every [basis](../../../vector-space.md#basis) [vector](../../../vector-space.md#vector)

$$
(f\circ h)(e_i)=g(e_i).
$$

**Thus $f\circ h=g$, proving that [free modules are projective](../../../module-theory.md#free-modules-are-projective).**

<h4 id="9e/b/ii">ii</h4>

↑ **Parent:** [B](#9e/b)

<h5 id="9e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9e/b/ii)

We prove by induction on $n$ that every submodule $N\subseteq R^n$ is free. The case $n=0$ is immediate. Let $\pi:R^n\to R$ be projection onto the first coordinate. Since $R$ is a principal [ideal](../../../commutative-algebra.md#ideal) domain,

$$
\pi(N)=dR
$$

for some $d$. If $d=0$, then $N\subseteq R^{n-1}$ and induction applies. Otherwise choose $x\in N$ with $\pi(x)=d$. For every $y\in N$, write $\pi(y)=rd$; then $y-rx\in\ker(\pi|_N)$. Also $Rx\cap\ker(\pi|_N)=0$ because $R$ is a domain and $d\ne0$. Therefore

$$
N=Rx\oplus\ker(\pi|_N).
$$

The kernel is a submodule of $R^{n-1}$ and is free by induction, while $Rx\cong R$. Hence $N$ is free. This is the [submodule theorem for free modules over a principal ideal domain](../../../commutative-algebra.md#submodule-theorem-for-free-modules-over-a-principal-ideal-domain).

If $P$ is finitely generated and projective, choose a surjection $f:R^n\to P$. Projectivity supplies $h:P\to R^n$ with $f\circ h=\operatorname{id}_P$, so

$$
R^n=\ker f\oplus h(P).
$$

**Thus $P\cong h(P)$ is a submodule of the finitely generated free module $R^n$, and the result just proved shows that $P$ is free.**

## 10F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10f/solution">Solution</h3>

↑ **Parent:** [10F](#10f)

Differentiability at $x\in\mathbb R^2$ means that there is a [linear map](../../../vector-space.md#linear-map) $Df|_x:\mathbb R^2\to\mathbb R$ such that

$$
f(x+h)=f(x)+Df|_x(h)+o(\|h\|).
$$

The [partial derivatives](../../../calculus.md#partial-derivative) are $D_if(x)=Df|_x(e_i)$ when the [derivative](../../../calculus.md#derivative) exists; independently, they may be defined by the corresponding one-variable difference quotients.

Suppose the [partial derivatives](../../../calculus.md#partial-derivative) exist near $x=(x_1,x_2)$ and are continuous at $x$. Apply the one-dimensional mean value theorem along the two coordinate segments from $x$ to $x+h$. It gives intermediate points $\xi_h,\eta_h\to x$ such that

$$
f(x+h)-f(x)
=D_1f(\xi_h)h_1+D_2f(\eta_h)h_2.
$$

Continuity of the partials makes the remainder after subtracting

$$
D_1f(x)h_1+D_2f(x)h_2
$$

equal to $o(\|h\|)$. Hence $f$ is [differentiable](../../../analysis.md#differentiable-function) and this is its [derivative](../../../calculus.md#derivative).

For the given [function](../../../function.md), writing $r=\sqrt{x^2+y^2}$, at $r>0$ we have

$$
\boxed{
D_1f=2x\sin(1/r)-\frac{x}{r}\cos(1/r),
\qquad
D_2f=2y\sin(1/r)-\frac{y}{r}\cos(1/r)}.
$$

At the origin both [partial derivatives](../../../calculus.md#partial-derivative) are zero, since $f(h,0)/h$ and $f(0,h)/h$ tend to zero. Neither partial is continuous there: along its corresponding coordinate axis the cosine term oscillates without a [limit](../../../calculus.md#limit-of-a-function). Nevertheless

$$
|f(x,y)|\leq r^2=o(r),
$$

so $f$ is [differentiable](../../../analysis.md#differentiable-function) at the origin with [derivative](../../../calculus.md#derivative) zero. This illustrates that [existence of partial derivatives does not imply their continuity](../../../analysis.md#existence-of-partial-derivatives-does-not-imply-their-continuity).

The final assertion is false. Define

$$
g(x,y)=
\begin{cases}
(x^2+y^2)\sin\!\left(\dfrac1{x^2+y^2}\right),&(x,y)\ne(0,0),\\
0,&(x,y)=(0,0).
\end{cases}
$$

Again $|g|\leq r^2$, so $g$ is [differentiable](../../../analysis.md#differentiable-function) at the origin and it is smooth elsewhere. But along the $x$-axis,

$$
D_1g(x,0)=2x\sin(1/x^2)-\frac2x\cos(1/x^2),
$$

is unbounded near zero, and similarly $D_2g(0,y)$ is unbounded. Thus both [partial derivatives](../../../calculus.md#partial-derivative) can be unbounded in every neighbourhood of a point even when the [function](../../../function.md) is [differentiable](../../../analysis.md#differentiable-function) everywhere.

## 11G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11g/a">a</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/a/solution">Solution</h4>

↑ **Parent:** [A](#11g/a)

The surface is obtained by revolving the graph $z=f(x)$ about the $x$-axis. It has a central cylindrical section of radius $b$, two smooth transition collars, and unit spherical caps centred at $(\pm3,0,0)$; its projection onto the $(x,z)$-plane is the region $|z|\leq f(x)$.

For a surface of revolution, the [Gaussian curvature of a surface of revolution](../../../differential-geometry.md#gaussian-curvature-of-a-surface-of-revolution) is

$$
K=-\frac{f''}{f(1+f'^2)^2}.
$$

**Thus the cylindrical region has $K=0$. On each transition collar, $K<0$ where $f''>0$, vanishes at the unique inflection circle, and is positive where $f''<0$. The spherical caps have $K>0$.**

<h3 id="11g/b">b</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/b/solution">Solution</h4>

↑ **Parent:** [B](#11g/b)

The area element is

$$
dA=f\sqrt{1+f'^2}\,dx\,d\theta.
$$

Consequently

$$
K\,dA
=-\frac{f''}{(1+f'^2)^{3/2}}\,dx\,d\theta
=-d\!\left(\frac{f'}{\sqrt{1+f'^2}}\right)d\theta.
$$

At $x=2-a$, smooth matching to the cylinder gives $f'=0$. At $x=2+a$, the spherical formula gives

$$
f'=\frac{1-a}{\sqrt{2a-a^2}},
\qquad
\frac{f'}{\sqrt{1+f'^2}}=1-a.
$$

The [total Gaussian curvature of a surface-of-revolution strip](../../../differential-geometry.md#total-gaussian-curvature-of-a-surface-of-revolution-strip) is therefore

$$
\boxed{\int_RK\,dA=-2\pi(1-a)}.
$$

<h3 id="11g/c">c</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/c/solution">Solution</h4>

↑ **Parent:** [C](#11g/c)

The two curves produced by $y=0$ are meridians, and meridians of a surface of revolution are geodesics. A boundary circle $x=x_0$ is a geodesic precisely when $f'(x_0)=0$, as follows either from the geodesic equations or from its geodesic curvature

$$
k_g=\frac{|f'(x_0)|}{f(x_0)\sqrt{1+f'(x_0)^2}}.
$$

The circle at $x=2-a$ is geodesic because it joins the cylinder smoothly. At the other boundary,

$$
f'(2+a)=\frac{1-a}{\sqrt{2a-a^2}},
$$

which vanishes exactly when $a=1$. Hence the cut pieces are geodesic polygons only for

$$
\boxed{a=1}.
$$

## 12B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12b/i">i</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/i/solution">Solution</h4>

↑ **Parent:** [I](#12b/i)

For $\operatorname{Re}s>0$,

$$
\boxed{
\mathcal L\{H(t-t_0)\}(s)
=\int_{t_0}^{\infty}e^{-st}\,dt
=\frac{e^{-st_0}}s}.
$$

This is the [Laplace transform time-shift rule](../../../analysis.md#laplace-transform-time-shift-rule) in its simplest form.

<h3 id="12b/ii">ii</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12b/ii)

Fourier transformation gives

$$
(k^2+m^2)\widehat G(k)=1,
\qquad
\widehat G(k)=\frac1{k^2+m^2}.
$$

For $x>0$, close the inverse-transform contour in the upper half-plane and take the residue at $k=im$; for $x<0$, close it in the lower half-plane. This gives the [one-dimensional modified Helmholtz Green function](../../../analysis.md#one-dimensional-modified-helmholtz-green-function)

$$
\boxed{G(x)=\frac{e^{-m|x|}}{2m}}.
$$

The same formula works for complex $m$ with $\operatorname{Re}m>0$: it decays at both ends, is continuous at zero, and its [derivative](../../../calculus.md#derivative) has the jump $G'(0+)-G'(0-)=-1$ required by the delta source.

Convolution therefore yields

$$
\boxed{
u(x)=\frac1{2m}\int_{-\infty}^{\infty}
 e^{-m|x-y|}f(y)\,dy}.
$$

<h3 id="12b/iii">iii</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#12b/iii)

Let $U(s,x)=\mathcal L_t\{u(t,x)\}$. The initial data turn the wave equation into

$$
-\frac{\partial^2U}{\partial x^2}+s^2U=f(x).
$$

Using the Green [function](../../../function.md) from part (ii) with $m=s$ gives

$$
U(s,x)=\frac1{2s}\int_{-\infty}^{\infty}
 e^{-s|x-y|}f(y)\,dy.
$$

Since

$$
\mathcal L^{-1}\!\left\{\frac{e^{-as}}s\right\}=H(t-a),
$$

we obtain the [D'Alembert formula with initial velocity](../../../wave-equation.md#d-alembert-formula-with-initial-velocity)

$$
\boxed{
u(t,x)=\frac12\int_{-\infty}^{\infty}
 H(t-|x-y|)f(y)\,dy
=\frac12\int_{x-t}^{x+t}f(y)\,dy}.
$$

## 13C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="13c/solution">Solution</h3>

↑ **Parent:** [13C](#13c)

Write

$$
\mathbf u=\nabla\phi+\beta\nabla\alpha,
\qquad
\mathcal L=-\beta\alpha_t-\frac12\mathbf u\cdot\mathbf u.
$$

Variation of $\phi$ gives $\nabla\cdot\mathbf u=0$. Variation of $\alpha$ gives

$$
\beta_t+\nabla\cdot(\beta\mathbf u)=0,
$$

and variation of $\beta$ gives

$$
\alpha_t+\mathbf u\cdot\nabla\alpha=0.
$$

Using incompressibility, the middle equation becomes

$$
\beta_t+\mathbf u\cdot\nabla\beta=0.
$$

These are the three required Euler-Lagrange equations.

Let $D_t=\partial_t+\mathbf u\cdot\nabla$. Since $D_t\alpha=D_t\beta=0$, differentiating $u_i=\partial_i\phi+\beta\partial_i\alpha$ gives

$$
D_tu_i
=\partial_i(D_t\phi)-u_j\partial_i u_j
=\partial_i\left(D_t\phi-\frac12\mathbf u^2\right).
$$

Now

$$
D_t\phi
=\phi_t+\mathbf u\cdot\nabla\phi
=\phi_t+\mathbf u^2+\beta\alpha_t,
$$

because $\mathbf u\cdot\nabla\alpha=-\alpha_t$. Hence

$$
D_tu_i
=\partial_i\left(\phi_t+\beta\alpha_t+\frac12\mathbf u^2\right)
=-\partial_i p,
$$

where

$$
\boxed{p=-\frac12\mathbf u^2-\phi_t-\beta\alpha_t},
\qquad
\boxed{f(\phi_t,\alpha_t,\beta)=-\phi_t-\beta\alpha_t}.
$$

This is the [Clebsch-potential variational derivation of incompressible Euler flow](../../../fluid-mechanics.md#clebsch-potential-variational-derivation-of-incompressible-euler-flow).

## 14B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="14b/i">i</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/i/solution">Solution</h4>

↑ **Parent:** [I](#14b/i)

For $a=0$ and $\kappa>0$, the [heat kernel](../../../diffusion-equation.md#heat-kernel) gives

$$
\boxed{u(t,x)=\int_{-\infty}^{\infty}K_t(x-y)u_0(y)\,dy}.
$$

As $t\downarrow0$, $K_t$ is a Gaussian of total mass one whose width is of order $\sqrt{\kappa t}$; it becomes a narrow spike at zero and converges to the delta distribution. Thus the convolution tends to $u_0(x)$.

<h3 id="14b/ii">ii</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#14b/ii)

When $\kappa=0$, the characteristics satisfy $x-at=\text{constant}$ and $u$ is constant along them. Therefore

$$
\boxed{u(t,x)=u_0(x-at)}.
$$

<h3 id="14b/iii">iii</h3>

↑ **Parent:** [14B](#14b)

<h4 id="14b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#14b/iii)

Set $v(t,z)=u(t,z+at)$. Then $v_t=\kappa v_{zz}$ and $v(0,z)=u_0(z)$. Applying the heat kernel and returning to $x$ gives the [advection-diffusion heat-kernel solution](../../../diffusion-equation.md#advection-diffusion-heat-kernel-solution)

$$
\boxed{
u(t,x)=\int_{-\infty}^{\infty}
K_t(x-at-y)u_0(y)\,dy}.
$$

## 15A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="15a/i">i</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/i/solution">Solution</h4>

↑ **Parent:** [I](#15a/i)

For $\psi=Ae^{-Bx^2}$,

$$
\psi_t=\left(\frac{A'}A-B'x^2\right)\psi,
\qquad
\psi_{xx}=(-2B+4B^2x^2)\psi.
$$

Substitution into the [Schrödinger equation](../../../physics.md#schrodinger-equation) and comparison of the constant and $x^2$ coefficients gives

$$
\boxed{A'=-i\hbar AB,
\qquad
B'=-\frac{i}{2\hbar}-2i\hbar B^2}.
$$

<h3 id="15a/ii">ii</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#15a/ii)

Put $B=\xi\tan(\phi+\alpha t)$. Matching the constant and $\tan^2$ coefficients in the [Riccati equation](../../../analysis.md#riccati-equation) requires

$$
\xi\alpha=-\frac{i}{2\hbar},
\qquad
\xi\alpha=-2i\hbar\xi^2.
$$

One convenient choice is therefore

$$
\boxed{\xi=\frac1{2\hbar},
\qquad \alpha=-i},
$$

so

$$
\boxed{B(t)=\frac1{2\hbar}\tan(\phi-it)}.
$$

<h3 id="15a/iii">iii</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#15a/iii)

Since $A'/A=-i\hbar B=-\tfrac i2\tan(\phi-it)$ and

$$
\frac d{dt}\log\cos(\phi-it)=i\tan(\phi-it),
$$

integration gives

$$
\boxed{A(t)=A_0[\cos(\phi-it)]^{-1/2}},
$$

with the branch chosen continuously from the initial value. The constant $A_0$ fixes normalization.

<h3 id="15a/iv">iv</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#15a/iv)

Normalizability requires $\operatorname{Re}B>0$. Since

$$
|\psi|^2=|A|^2e^{-(B+B^*)x^2},
$$

the given Gaussian [integral](../../../calculus.md#integral) gives

$$
\boxed{\langle \hat x^2\rangle
=\frac1{2(B+B^*)}
=\frac1{4\operatorname{Re}B}}.
$$

Also $\psi_x=-2Bx\psi$, so integration by parts yields

$$
\langle\hat p^2\rangle
=\hbar^2\int|\psi_x|^2dx
=4\hbar^2|B|^2\langle x^2\rangle.
$$

Therefore

$$
\boxed{\langle\hat p^2\rangle
=\frac{\hbar^2|B|^2}{\operatorname{Re}B}}.
$$

These are the [second moments of a complex Gaussian wave packet](../../../quantum-mechanics.md#second-moments-of-a-complex-gaussian-wave-packet).

## 16D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="16d/solution">Solution</h3>

↑ **Parent:** [16D](#16d)

Taking the vertical component of the curl of the [momentum](../../../classical-mechanics.md#momentum) equation gives

$$
\omega_t+f\nabla\cdot\mathbf u=0.
$$

The continuity equation gives $\eta_t+h_0\nabla\cdot\mathbf u=0$, and hence

$$
\boxed{\frac\partial{\partial t}
\left(\omega-\frac f{h_0}\eta\right)=0}.
$$

Since initially $\mathbf u=0$ and $\eta=\eta_0$,

$$
\omega=\frac f{h_0}(\eta-\eta_0).
$$

Taking the divergence of the [momentum](../../../classical-mechanics.md#momentum) equation and using

$$
\nabla\cdot(\mathbf f\times\mathbf u)=-f\omega
$$

gives

$$
(\nabla\cdot\mathbf u)_t-f\omega=-g\nabla^2\eta.
$$

Differentiate continuity in time and substitute the last two identities to obtain

$$
\boxed{\eta_{tt}-gh_0\nabla^2\eta+f^2\eta=f^2\eta_0}.
$$

Let the [Rossby deformation radius](../../../physics.md#rossby-deformation-radius) be

$$
L_R=\frac{\sqrt{gh_0}}{|f|}.
$$

The even, decaying steady solution of

$$
-L_R^2\eta_\infty''+\eta_\infty=\eta_0
$$

with continuous value and [derivative](../../../calculus.md#derivative) at $x=\pm a$ is

$$
\boxed{
\eta_\infty(x)=
\begin{cases}
\epsilon\left[1-e^{-a/L_R}\cosh(x/L_R)\right],&|x|<a,\\
\epsilon\sinh(a/L_R)e^{-|x|/L_R},&|x|>a.
\end{cases}}
$$

The steady [momentum](../../../classical-mechanics.md#momentum) balance is a [geostrophic balance](../../../physics.md#geostrophic-balance):

$$
\boxed{u=0,
\qquad v=\frac g f\frac{d\eta_\infty}{dx}}.
$$

Thus the flow is parallel to the two edges of the raised strip, in opposite $y$-directions on the two sides; for $f>0$, it points toward $+y$ on the left and $-y$ on the right. Its magnitude is concentrated within a few deformation radii of the edges.

## 17H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="17h/a">a</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/a/solution">Solution</h4>

↑ **Parent:** [A](#17h/a)

Let

$$
S_{xx}=\sum_{i=1}^n(x_i-\bar x)^2,
\qquad
S_{xy}=\sum_{i=1}^n(x_i-\bar x)(Y_i-\bar Y).
$$

Differentiating the Gaussian log-likelihood, equivalently minimizing the residual sum of squares, gives the [ordinary least squares estimators](../../../statistical-modelling.md#ordinary-least-squares-estimators)

$$
\boxed{\hat\beta=\frac{S_{xy}}{S_{xx}},
\qquad
\hat\alpha=\bar Y-\hat\beta\bar x},
$$

assuming $S_{xx}>0$.

<h3 id="17h/b">b</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/b/solution">Solution</h4>

↑ **Parent:** [B](#17h/b)

The centered model has residual sum of squares

$$
\sum_i\{Y_i-\alpha'-\beta'(x_i-\bar x)\}^2.
$$

Its slope normal equation gives

$$
\hat\beta'
=\frac{\sum_i(x_i-\bar x)(Y_i-\bar Y)}
{\sum_i(x_i-\bar x)^2}
=\boxed{\hat\beta}.
$$

<h3 id="17h/c">c</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/c/solution">Solution</h4>

↑ **Parent:** [C](#17h/c)

The intercept normal equation is

$$
\sum_i\{Y_i-\hat\alpha'-\hat\beta'(x_i-\bar x)\}=0.
$$

Because the centered predictors sum to zero,

$$
\boxed{\hat\alpha'=\bar Y}.
$$

Meanwhile $\hat\alpha=\bar Y-\hat\beta\bar x$, so the two intercept estimates are unequal in general. The parameters themselves satisfy $\alpha'=\alpha+\beta\bar x$.

<h3 id="17h/d">d</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/d/solution">Solution</h4>

↑ **Parent:** [D](#17h/d)

Averaging the centered model gives

$$
\hat\alpha'=\bar Y
=\alpha'+\bar\epsilon.
$$

Therefore

$$
\boxed{\hat\alpha'\sim N\left(\alpha',\frac{\sigma^2}{n}\right)}.
$$

Writing $z_{0.975}=\Phi^{-1}(0.975)$, an exact 95% confidence interval is

$$
\boxed{\bar Y\pm z_{0.975}\frac\sigma{\sqrt n}}.
$$

<h3 id="17h/e">e</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/e/solution">Solution</h4>

↑ **Parent:** [E](#17h/e)

Use the residual variance estimator

$$
s^2=\frac1{n-2}\sum_{i=1}^n
\{Y_i-\hat\alpha'-\hat\beta'(x_i-\bar x)\}^2.
$$

Under the Gaussian linear model, $\bar Y$ is independent of $s^2$ and

$$
\frac{(n-2)s^2}{\sigma^2}\sim\chi^2_{n-2}.
$$

Consequently the [Student t confidence interval for a centered regression intercept](../../../statistical-inference.md#student-t-confidence-interval-for-a-centered-regression-intercept) follows from

$$
\frac{\bar Y-\alpha'}{s/\sqrt n}\sim t_{n-2}.
$$

It is

$$
\boxed{\bar Y\pm t_{n-2,0.975}\frac{s}{\sqrt n}}.
$$

The displayed pivotal quantity lies between its 2.5% and 97.5% quantiles with probability $0.95$, which proves the stated coverage.

## 18H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

Newton's method for minimization uses

$$
\boxed{x_{k+1}=x_k-[\nabla^2f(x_k)]^{-1}\nabla f(x_k)}.
$$

For a quantitative local bound, suppose on a convex neighbourhood containing the iterates that

$$
mI\preceq\nabla^2f(x)\preceq LI,
\qquad
\|\nabla^2f(x)-\nabla^2f(y)\|\leq M\|x-y\|,
$$

with $m>0$, and let $x^*$ be the minimizer. The [integral](../../../calculus.md#integral) form of the [gradient](../../../calculus.md#gradient) and the Hessian Lipschitz bound give the [quadratic convergence bound for Newton's method](../../../mathematical-optimization.md#quadratic-convergence-bound-for-newton-s-method)

$$
\|x_{k+1}-x^*\|
\leq\frac M{2m}\|x_k-x^*\|^2.
$$

If $q=M\|x_0-x^*\|/(2m)<1$, induction yields

$$
\|x_k-x^*\|\leq\frac{2m}{M}q^{2^k}.
$$

Since $f(x)-f(x^*)\leq L\|x-x^*\|^2/2$,

$$
\boxed{f(x_k)-f(x^*)
\leq\frac{2Lm^2}{M^2}q^{2^{k+1}}}.
$$

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

If $x_k\geq1$, then positivity and the [arithmetic-geometric mean inequality](../../../mathematical-optimization.md#arithmetic-geometric-mean-inequality) give

$$
x_{k+1}=\frac12\left(x_k+\frac a{x_k}\right)
\geq\sqrt a\geq1.
$$

Thus all iterates remain in $[1,\infty)$.

Consider the strictly convex [function](../../../function.md)

$$
f(x)=\frac{x^3}{3}-ax
$$

on $[1,\infty)$. Since $f'(x)=x^2-a$ and $f''(x)=2x$, its Newton minimization step is

$$
x-\frac{f'(x)}{f''(x)}
=\frac12\left(x+\frac ax\right).
$$

Its unique minimizer is $x^*=\sqrt a$.

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

Every $x_0\in[1,\infty)$ works. Indeed, $x_1\geq\sqrt a$, and whenever $x_k\geq\sqrt a$,

$$
0\leq x_{k+1}-\sqrt a
=\frac{(x_k-\sqrt a)^2}{2x_k}
\leq x_k-\sqrt a.
$$

The iterates from $k=1$ onward therefore decrease to a [limit](../../../calculus.md#limit-of-a-function), and the recurrence forces that [limit](../../../calculus.md#limit-of-a-function) to be $\sqrt a$.

There is also an explicit error bound. Put

$$
q=\left|\frac{x_0-\sqrt a}{x_0+\sqrt a}\right|<1.
$$

A direct calculation gives

$$
\frac{x_{k+1}-\sqrt a}{x_{k+1}+\sqrt a}
=\left(\frac{x_k-\sqrt a}{x_k+\sqrt a}\right)^2.
$$

Hence, for $k\geq1$,

$$
\boxed{
|x_k-\sqrt a|
=\frac{2\sqrt a\,q^{2^k}}{1-q^{2^k}}
\leq\frac{2\sqrt a}{1-q}q^{2^k}}.
$$

This double-exponential decay is consistent with the Newton bound in part (a). For the chosen objective, the supplied factorization also gives

$$
f(x)-f(\sqrt a)
=\frac13(x-\sqrt a)^2(x+2\sqrt a),
$$

so convergence of the objective and convergence of the iterates are equivalent on $[1,\infty)$.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
