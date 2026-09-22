# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2005/PaperIB_2.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2005/PaperIB_2.pdf)

**Table of contents**

- [1C](#1c)
  - [Solution](#1c/solution)
- [2C](#2c)
  - [Solution](#2c/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
- [6H](#6h)
  - [Solution](#6h/solution)
- [7G](#7g)
  - [Solution](#7g/solution)
- [8E](#8e)
  - [Solution](#8e/solution)
- [9D](#9d)
  - [Solution](#9d/solution)
- [10C](#10c)
  - [i](#10c/i)
    - [Solution](#10c/i/solution)
  - [ii](#10c/ii)
    - [Solution](#10c/ii/solution)
- [11C](#11c)
  - [Solution](#11c/solution)
- [12A](#12a)
  - [Solution](#12a/solution)
- [13B](#13b)
  - [i](#13b/i)
    - [Solution](#13b/i/solution)
  - [ii](#13b/ii)
    - [Solution](#13b/ii/solution)
- [14F](#14f)
  - [Solution](#14f/solution)
- [15E](#15e)
  - [Solution](#15e/solution)
- [16G](#16g)
  - [Solution](#16g/solution)
- [17H](#17h)
  - [Solution](#17h/solution)
- [18F](#18f)
  - [a](#18f/a)
    - [Solution](#18f/a/solution)
  - [b](#18f/b)
    - [Solution](#18f/b/solution)
- [19D](#19d)
  - [Solution](#19d/solution)
- [20D](#20d)
  - [Solution](#20d/solution)

## 1C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1c/solution">Solution</h3>

↑ **Parent:** [1C](#1c)

Direct [matrix](../../../vector-space.md#matrix) multiplication gives the multiplication table

$$
J^2=K^2=L^2=-I,\qquad JK=L,\quad KL=J,\quad LJ=K,\qquad KJ=-L,\quad LK=-J,\quad JL=-K.
$$

Together with $I$ acting as the identity, this shows that the product of any two real [linear combinations](../../../vector-space.md#linear-combination) is again a real [linear combination](../../../vector-space.md#linear-combination). Thus $\Omega$ is closed under multiplication. It is the [complex matrix representation of quaternions](../../../algebra.md#complex-matrix-representation-of-quaternions).

Its general element has the form

$$
\alpha=\begin{pmatrix}a+ib&c+id\\-c+id&a-ib\end{pmatrix}.
$$

If this [matrix](../../../vector-space.md#matrix) is zero, real and imaginary parts of its first row give $a=b=c=d=0$. Hence $I,J,K,L$ are linearly independent over $\mathbb R$ and form a [basis](../../../vector-space.md#basis):

$$
\boxed{\dim_{\mathbb R}\Omega=4.}
$$

Put $v=bJ+cK+dL$. Since distinct [imaginary units](../../../complex-analysis.md#imaginary-unit) anticommute, the mixed terms in $v^2$ cancel, leaving $v^2=-(b^2+c^2+d^2)I$. Scalars commute with $v$, so

$$
(aI+v)(aI-v)=a^2I-v^2=(a^2+b^2+c^2+d^2)I.
$$

The reversed product is the same. The coefficient is strictly positive for every nonzero element. Consequently

$$
\boxed{\alpha^{-1}=\frac{aI-bJ-cK-dL}{a^2+b^2+c^2+d^2}\in\Omega\qquad(\alpha\ne0).}
$$

This also identifies $\Omega$ as a real noncommutative [division algebra](../../../algebra.md#division-algebra), not as the full algebra of complex two-by-two [matrices](../../../vector-space.md#matrix).

## 2C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2c/solution">Solution</h3>

↑ **Parent:** [2C](#2c)

A [group automorphism](../../../algebra.md#group-automorphism) is a bijective [group homomorphism](../../../group-theory.md#group-homomorphism) from $G$ to itself. The multiplication in $\operatorname{Aut}(G)$ is composition: $(\alpha\beta)(g)=\alpha(\beta(g))$. Composition is associative, the identity map is the identity element, and each inverse [bijection](../../../function.md#bijection) is again a [homomorphism](../../../algebra.md#homomorphism), so these maps form the [automorphism group](../../../group-theory.md#automorphism-group).

For conjugation by $h$, multiplication is preserved because

$$
h(g_1g_2)h^{-1}=(hg_1h^{-1})(hg_2h^{-1}).
$$

Conjugation by $h^{-1}$ is its inverse, so $\psi(h)$ is an [group automorphism](../../../algebra.md#group-automorphism). Moreover

$$
\psi(h_1h_2)(g)=h_1h_2g h_2^{-1}h_1^{-1}
=\psi(h_1)(\psi(h_2)(g)).
$$

Hence **$\psi:G\to\operatorname{Aut}(G)$ is a [homomorphism](../../../algebra.md#homomorphism)**, with image the [inner automorphisms](../../../group-theory.md#inner-automorphism). Its [group homomorphism kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) is the [group center](../../../group-theory.md#center-of-a-group) of $G$, since $\psi(h)$ is the identity precisely when $hg=gh$ for every $g$.

## 3B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

A [function](../../../function.md) $f:I\to\mathbb R$ is [uniformly continuous](../../../topological-analysis.md#uniform-continuity) if

$$
\forall\varepsilon>0\ \exists\delta>0\ \forall x,y\in I:
\quad |x-y|<\delta\Longrightarrow |f(x)-f(y)|<\varepsilon.
$$

The same $\delta$ must work at every point of $I$.

**Every [uniformly continuous](../../../topological-analysis.md#uniform-continuity) [function](../../../function.md) on $(0,1)$ is bounded.** Choose the tolerance $\delta$ for $\varepsilon=1$ and an integer $N$ with $1/N<\delta$. The finitely many centers $c_j=(j+1/2)/N$, $0\leq j<N$, cover the interval by cells of radius $1/(2N)$. For each $x$, one center satisfies $|f(x)-f(c_j)|<1$. Thus $|f(x)|\leq1+\max_j|f(c_j)|$. This is the [uniformly continuous function on a totally bounded set is bounded](../../../topological-analysis.md#uniformly-continuous-function-on-a-totally-bounded-set-is-bounded) argument; closedness of the interval is unnecessary.

**The reciprocal [function](../../../function.md) is not [uniformly continuous](../../../topological-analysis.md#uniform-continuity) on $(0,1)$.** It is unbounded, already contradicting the preceding result. Directly, $x_n=1/(n+1)$ and $y_n=1/(n+2)$ have distance tending to zero while $|1/x_n-1/y_n|=1$.

**The oscillating [function](../../../function.md) $\sin(1/x)$ is not [uniformly continuous](../../../topological-analysis.md#uniform-continuity) either**, despite being bounded. Take

$$
x_n=\frac1{2\pi n+\pi/2},\qquad y_n=\frac1{2\pi n+3\pi/2}.
$$

Their distance tends to zero, but their [function](../../../function.md) values are $1$ and $-1$. The fixed output gap of two contradicts the uniform-continuity condition, for example with $\varepsilon=1$.

## 4A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

Suppose the union $W$ has a separation $W=A\cup B$ into disjoint, nonempty, relatively open subsets. Each [connected](../../../geometry-and-topology.md#connected-space) $U_j$ must lie entirely in one of them: otherwise its intersections with $A$ and $B$ would separate $U_j$ in its [subspace topology](../../../topology.md#subspace-topology). In particular $U_1$ lies on one side, say $A$. Every other $U_j$ intersects $U_1$, so it cannot lie in $B$ and must also lie in $A$. Then $W\subseteq A$, contradicting $B\ne\varnothing$. **The union is [connected](../../../geometry-and-topology.md#connected-space).** This is the [connected union with a connected hub](../../../geometry-and-topology.md#connected-union-with-a-connected-hub) argument.

For path-connectedness, take any $x\in U_i$ and $y\in U_j$. Choose $a\in U_i\cap U_1$ and $b\in U_j\cap U_1$. There is a [path](../../../geometry-and-topology.md#continuous-path) from $x$ to $a$ inside $U_i$, a [path](../../../geometry-and-topology.md#continuous-path) from $a$ to $b$ inside $U_1$, and a [path](../../../geometry-and-topology.md#continuous-path) from $b$ to $y$ inside $U_j$. Concatenate the three [paths](../../../geometry-and-topology.md#continuous-path) on successive thirds of $[0,1]$. They agree at the joining points, so the resulting map is [continuous](../../../calculus.md#continuous-function) and remains in $W$. **The union is [path-connected](../../../geometry-and-topology.md#path-connected-space).** There need not be a single point common to all the subsets.

## 5E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

Use the causal [Green function](../../../analysis.md#green-s-function): it vanishes before the forcing time $t'$. For $t>t'$ it solves the homogeneous equation, is [continuous](../../../calculus.md#continuous-function) at $t=t'$ with value zero, and has first-derivative jump one. These conditions give

$$
\boxed{G(t,t')=\begin{cases}\sinh(k(t-t'))/k,&t\geq t',\\0,&t<t'.\end{cases}}
$$

Indeed the right [derivative](../../../calculus.md#derivative) at the forcing time is one and the left [derivative](../../../calculus.md#derivative) is zero, so $(\partial_t^2-k^2)G=\delta(t-t')$ distributionally. If $k=0$, use the [continuous](../../../calculus.md#continuous-function) limit $G(t,t')=(t-t')$ on its causal support.

For $k\ne0$, differentiating the [integral](../../../calculus.md#integral) solution gives

$$
\dot x(t)=\int_0^t\cosh(k(t-t'))f(t')\,dt',\qquad
\ddot x(t)=f(t)+k^2\int_0^t\frac{\sinh(k(t-t'))}{k}f(t')\,dt'.
$$

Both initial values vanish and $\ddot x-k^2x=f$. This verifies the requested representation and its sign. The $k=0$ formula similarly gives $\ddot x=f$.

## 6H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6h/solution">Solution</h3>

↑ **Parent:** [6H](#6h)

In SI units, the sourced [Maxwell equations](../../../electromagnetism.md#maxwell-equations) are

$$
\nabla\cdot\mathbf E=\rho/\epsilon_0,\qquad\nabla\cdot\mathbf B=0,
\qquad\nabla\times\mathbf E=-\partial_t\mathbf B,
\qquad\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E.
$$

Take the [divergence](../../../calculus.md#divergence) of the last equation. The [divergence](../../../calculus.md#divergence) of a [curl](../../../calculus.md#curl) vanishes; using the first equation gives the necessary local conservation law

$$
\boxed{\partial_t\rho+\nabla\cdot\mathbf J=0.}
$$

For sources supported in a fixed region, integrate over a containing surface where the current vanishes. The [divergence](../../../calculus.md#divergence) theorem gives

$$
\frac{d}{dt}\int_V\rho\,d^3x=-\int_{\partial V}\mathbf J\cdot\mathbf n\,dS=0.
$$

Thus the total charge is constant. For each component of the [electric dipole moment](../../../electromagnetism.md#electric-dipole-moment), integration by parts gives

$$
\frac{d}{dt}\int_Vx_i\rho\,d^3x
=-\int_Vx_i\partial_jJ_j\,d^3x
=-\int_{\partial V}x_i\mathbf J\cdot\mathbf n\,dS+\int_VJ_i\,d^3x.
$$

The surface term again vanishes, so

$$
\boxed{\frac{d}{dt}\int_V\mathbf x\rho\,d^3x=\int_V\mathbf J\,d^3x.}
$$

Smooth [compact](../../../topology.md#compact-space) support suffices for these manipulations; equivalently one may integrate the [charge continuity equation](../../../electromagnetism.md#charge-continuity-equation) over all space and use the fixed support to identify the [integrals](../../../calculus.md#integral) with those over $V$.

## 7G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7g/solution">Solution</h3>

↑ **Parent:** [7G](#7g)

Set $T=\Delta t_A$, $\beta=v/c$ and $\gamma=(1-\beta^2)^{-1/2}$. In Alice's inertial coordinates the departure, turn and return events are $(t,x)=(0,0)$, $(T/2,vT/2)$ and $(T,0)$. Alice's [worldline](../../../special-relativity.md#world-line) is vertical; Bob's consists of two straight timelike segments of slopes $dx/dt=\pm v$, joined by the short turnaround. Equal speeds and the same endpoints give equal coordinate durations on the two legs.

The Minkowski proper-time element for Bob is $d\tau=\sqrt{1-v^2/c^2}\,dt$, while Alice at rest has $d\tau=dt$. Integrating on both legs gives

$$
\boxed{\Delta t_B=\frac T\gamma=\sqrt{1-v^2/c^2}\,\Delta t_A.}
$$

Acceleration itself need not cause a large direct change in the clock rate. Its role is to make Bob change inertial frames and reunite with Alice, so the two worldlines have different proper lengths between the same events.

To describe Bob's assignment of Alice's age, apply [relativity of simultaneity](../../../special-relativity.md#relativity-of-simultaneity) to lines of equal coordinate time in his instantaneous inertial frames. At the turn the outbound line is $t-vx/c^2=T(1-\beta^2)/2$; it intersects Alice at $t_-=T(1-\beta^2)/2$. The inbound line is $t+vx/c^2=T(1+\beta^2)/2$ and intersects her at $t_+=T(1+\beta^2)/2$. Thus the negligibly short change of rest frame advances Bob's assigned Alice age by $t_+-t_-=\beta^2T$. On each inertial leg he assigns Alice an aging rate $1/\gamma$ per unit of his own [proper time](../../../special-relativity.md#proper-time), but the frame dependence expressed by [relativity of simultaneity](../../../special-relativity.md#relativity-of-simultaneity) removes the apparent symmetric-time-dilation paradox.

If “sees” means clocks read from received light, there is no instantaneous jump in Alice's displayed age. A light signal received at Bob's event was emitted from Alice at $t_e=t-|x|/c$. On the outbound leg $t_e=(1-\beta)t$; on the inbound leg $t_e=(1+\beta)t-\beta T$. Consequently the observed aging rates per Bob [proper time](../../../special-relativity.md#proper-time) are

$$
\frac{dt_e}{d\tau}=\gamma(1-\beta)=\sqrt{\frac{1-\beta}{1+\beta}}\quad\text{outbound},\qquad
\frac{dt_e}{d\tau}=\gamma(1+\beta)=\sqrt{\frac{1+\beta}{1-\beta}}\quad\text{inbound}.
$$

He receives slowly running, redshifted clock signals on the outward leg and rapidly running, blueshifted signals on the return. Integrating both rates over the equal proper durations $T/(2\gamma)$ gives total received Alice aging $T$, with the two expressions [continuous](../../../calculus.md#continuous-function) at the turn.

<a id="7g/image-twin-voyage-inertial-worldlines-turnaround-simultaneity-lines-and-alice-ages-assigned-or-optically-received-by-bob"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2-twin-clocks.png)

**[Figure 1](#7g/image-twin-voyage-inertial-worldlines-turnaround-simultaneity-lines-and-alice-ages-assigned-or-optically-received-by-bob). Twin voyage: inertial worldlines, turnaround simultaneity lines, and Alice ages assigned or optically received by Bob**.

The diagram distinguishes the reassignment due to [relativity of simultaneity](../../../special-relativity.md#relativity-of-simultaneity) from the [continuous](../../../calculus.md#continuous-function) optical observation; both descriptions give the same ages when the twins meet again.

## 8E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8e/solution">Solution</h3>

↑ **Parent:** [8E](#8e)

The intended dynamical assumption is steady inviscid Euler flow of constant density, with conservative body-force potential $\Phi$. Its equation is $(\mathbf u\cdot\nabla)\mathbf u=-\nabla(p/\rho+\Phi)$. The [vector](../../../vector-space.md#vector) identity

$$
(\mathbf u\cdot\nabla)\mathbf u=\nabla(\tfrac12|\mathbf u|^2)-\mathbf u\times(\nabla\times\mathbf u)
$$

then gives

$$
\boxed{\mathbf u\times\boldsymbol\omega=\nabla H,\qquad
H=\frac p\rho+\Phi+\frac12|\mathbf u|^2.}
$$

With no body force take $\Phi=0$. Taking the [scalar product](../../../linear-algebra.md#dot-product) with $\mathbf u$ yields $\mathbf u\cdot\nabla H=0$, so the [Bernoulli function](../../../fluid-mechanics.md#bernoulli-function) is constant along streamlines, though not necessarily the same constant on different streamlines.

Choose the planar [streamfunction](../../../fluid-mechanics.md#stream-function) convention $\mathbf u=(\psi_y,-\psi_x,0)$. Then $\boldsymbol\omega=(0,0,\omega)$ with $\omega=-\nabla^2\psi$, and

$$
\mathbf u\times\boldsymbol\omega=(-\omega\psi_x,-\omega\psi_y,0)=-\omega\nabla\psi.
$$

If locally $H=H(\psi)$, comparison with $\nabla H=H'(\psi)\nabla\psi$ gives

$$
\boxed{\frac{dH}{d\psi}+\omega=0}
$$

on the nonstagnant part of that flow. It extends to isolated stagnation points by continuity. Where the [streamfunction](../../../fluid-mechanics.md#stream-function) is constant on an entire open region, cancellation of its zero [gradient](../../../calculus.md#gradient) alone imposes no [derivative](../../../calculus.md#derivative) condition on an arbitrarily extended $H(\psi)$.

Steadiness and incompressibility alone, without the inviscid dynamical assumption, do not imply the stated identity. In a steady Newtonian viscous flow the correct form has $\mathbf u\times\boldsymbol\omega=\nabla H-\nu\nabla^2\mathbf u$. For example, a pressure-driven planar [Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation) has a nonzero streamwise pressure [gradient](../../../calculus.md#gradient) balanced by viscosity, while $\mathbf u\times\boldsymbol\omega$ has no streamwise component. This identifies the required qualification of the printed premise.

## 9D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9d/solution">Solution</h3>

↑ **Parent:** [9D](#9d)

In a finite two-person [zero-sum game](../../../game-theory.md#zero-sum-game) the row player chooses $i$, the column player chooses $j$, and the row player receives $a_{ij}$ while the column player receives $-a_{ij}$. The row player maximizes that payoff and the column player minimizes it. Mixed strategies are [probability](../../../probability-theory.md#probability) [vectors](../../../vector-space.md#vector) $x\in\mathbb R^m$ and $y\in\mathbb R^n$, giving expected row payoff $x^TAy$.

Against a fixed row mixture, the worst column is a pure column, so the row problem introduces its guaranteed payoff $v$:

$$
\boxed{\max_{x,v}v:\quad x\geq0,\quad\mathbf1^Tx=1,\quad A^Tx\geq v\mathbf1.}
$$

Similarly the column player minimizes an upper guarantee $w$:

$$
\boxed{\min_{y,w}w:\quad y\geq0,\quad\mathbf1^Ty=1,\quad Ay\leq w\mathbf1.}
$$

The values $v,w$ are unrestricted real variables; no positivity shift of the [matrix](../../../vector-space.md#matrix) is required.

To see the [linear programming duality](../../../mathematical-optimization.md#linear-programming-duality) explicitly, introduce nonnegative multipliers $y$ for the first problem's payoff inequalities and multiplier $w$ for its normalization. Its upper-bound Lagrangian is

$$
\mathcal L=v+y^T(A^Tx-v\mathbf1)+w(1-\mathbf1^Tx)
=w+v(1-\mathbf1^Ty)+x^T(Ay-w\mathbf1).
$$

The supremum over free $v$ and nonnegative $x$ is finite precisely when $\mathbf1^Ty=1$ and $Ay\leq w\mathbf1$, and is then $w$. Minimizing it gives the displayed column problem, proving that the programs are a dual pair.

A sufficient optimality certificate is a pair of [probability](../../../probability-theory.md#probability) [vectors](../../../vector-space.md#vector) and a common value $v_*$ satisfying

$$
\boxed{Ay\leq v_*\mathbf1,\qquad A^Tx\geq v_*\mathbf1.}
$$

Equivalently, both programs are feasible with equal values. Positive-probability rows then have $(Ay)_i=v_*$ and positive-probability columns have $(A^Tx)_j=v_*$, the [complementary slackness](../../../mathematical-optimization.md#complementary-slackness) conditions. These conditions certify a [saddle point](../../../analysis.md#saddle-point) and hence optimal mixed strategies for both players.

## 10C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10c/i">i</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/i/solution">Solution</h4>

↑ **Parent:** [I](#10c/i)

For a complex square [matrix](../../../vector-space.md#matrix), define its [determinant](../../../linear-algebra.md#determinant) by

$$
\det A=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)\prod_{i=1}^na_{i,\sigma(i)}.
$$

The [cofactor](../../../linear-algebra.md#cofactor) is $C_{ij}=(-1)^{i+j}\det A^{(ij)}$, where $A^{(ij)}$ deletes row $i$ and column $j$. The adjugate is the transposed [cofactor matrix](../../../linear-algebra.md#cofactor-matrix), $\operatorname{adj}(A)_{ij}=C_{ji}$.

The $(i,j)$ entry of $\operatorname{adj}(A)A$ is $\sum_kC_{ki}a_{kj}$. For $j=i$, expansion along column $i$ gives $\det A$. For $j\ne i$, this same sum is the [determinant](../../../linear-algebra.md#determinant) of the [matrix](../../../vector-space.md#matrix) obtained by replacing column $i$ by column $j$: deleting the replaced column leaves all its [cofactors](../../../linear-algebra.md#cofactor) unchanged. The new [matrix](../../../vector-space.md#matrix) has two equal columns, so its [determinant](../../../linear-algebra.md#determinant) is zero. Thus

$$
\boxed{\operatorname{adj}(A)A=(\det A)I_n.}
$$

This proof does not assume invertibility and therefore also covers singular [matrices](../../../vector-space.md#matrix).

<h3 id="10c/ii">ii</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10c/ii)

The cyclic [matrix](../../../vector-space.md#matrix) acts by $(v_1,v_2,v_3,v_4)\mapsto(v_2,v_3,v_4,v_1)$. For each fourth root of unity $\lambda$, the [vector](../../../vector-space.md#vector) $v_\lambda=(1,\lambda,\lambda^2,\lambda^3)^T$ satisfies $Av_\lambda=\lambda v_\lambda$, because $\lambda^4=1$. This supplies the four distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) and nonzero [eigenvectors](../../../linear-operator-theory.md#eigenvector):

$$
\begin{array}{c|c}
\lambda&v_\lambda^T\\\hline
1&(1,1,1,1)\\
-1&(1,-1,1,-1)\\
i&(1,i,-1,-i)\\
-i&(1,-i,-1,i)
\end{array}
$$

[Eigenvectors](../../../linear-operator-theory.md#eigenvector) for distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are linearly independent. Thus, with these columns in the indicated order,

$$
P=\begin{pmatrix}1&1&1&1\\1&-1&i&-i\\1&1&-1&-1\\1&-1&-i&i\end{pmatrix},\qquad
\boxed{P^{-1}AP=\operatorname{diag}(1,-1,i,-i).}
$$

They form a [basis](../../../vector-space.md#basis) over $\mathbb C$, so there are no other [eigenvalues](../../../linear-operator-theory.md#eigenvalue). Equivalently the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is $\lambda^4-1$.

## 11C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11c/solution">Solution</h3>

↑ **Parent:** [11C](#11c)

Let $F=\mathbb Ze_1\oplus\mathbb Ze_2$ and $N=\mathbb Z(6e_1+9e_2)$. The precise presented [group](../../../group.md) is $A=F/N$, with $x=e_1+N$ and $y=e_2+N$. It is abelian and has exactly the imposed additive relation and its integer multiples.

Change the [integral](../../../calculus.md#integral) [basis](../../../vector-space.md#basis) to $u=2e_1+3e_2$, $v=e_1+2e_2$. The change-of-basis [determinant](../../../linear-algebra.md#determinant) is $2\cdot2-3\cdot1=1$, so these are a [basis](../../../vector-space.md#basis) of the [free abelian group](../../../group-theory.md#free-abelian-group). Explicitly, $e_1=2u-3v$ and $e_2=-u+2v$. The relation generator becomes $6e_1+9e_2=3u$. Therefore

$$
\boxed{A\cong(\mathbb Zu/3\mathbb Zu)\oplus\mathbb Zv\cong\mathbb Z/3\mathbb Z\oplus\mathbb Z.}
$$

The image of $u$ is nonzero, since $(2,3)$ is not an integer multiple of $(6,9)$, but three times it vanishes. Thus $A$ has an element of exact order three. A [free abelian group](../../../group-theory.md#free-abelian-group) has no nonzero finite-order element, so **$A$ is not free abelian**.

## 12A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12a/solution">Solution</h3>

↑ **Parent:** [12A](#12a)

For a [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $g$, write $s(t)=\sqrt{g_{\gamma(t)}(\dot\gamma(t),\dot\gamma(t))}$. Use the [energy of a curve](../../../riemannian-geometry.md#energy-of-a-curve) normalization compatible with the requested inequality:

$$
L(\gamma)=\int_0^1s(t)\,dt,\qquad E(\gamma)=\int_0^1s(t)^2\,dt.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) here has the direct variance form

$$
E-L^2=\int_0^1(s(t)-L)^2\,dt\geq0.
$$

Equality holds exactly when $s$ is constant almost everywhere, hence everywhere for a smooth [curve](../../../topology.md#curve). With the alternative [energy of a curve](../../../riemannian-geometry.md#energy-of-a-curve) convention containing a factor $1/2$, the same assertion reads $L^2\leq2E$.

In the upper half-plane write $\gamma=u+iv$, $v>0$, and use $ds^2=(du^2+dv^2)/v^2$. Let the endpoints be $P=ip$, $Q=iq$, $p,q>0$. Then

$$
L=\int_0^1\frac{\sqrt{\dot u^2+\dot v^2}}v\,dt
\geq\int_0^1\frac{|\dot v|}v\,dt
\geq\left|\log\frac qp\right|.
$$

The first equality requires $\dot u=0$ throughout. Endpoint values force $u=0$. The second equality requires the [derivative](../../../calculus.md#derivative) of $\log v$ to have one sign, so $v$ is [monotone](../../../calculus.md#monotonic-function). Conversely every smooth [monotone](../../../calculus.md#monotonic-function) positive $v$ with these endpoints attains this bound. Consequently **the absolute length minimizers are precisely the vertical [curves](../../../topology.md#curve) with [monotone](../../../calculus.md#monotonic-function) height**, including a constant [curve](../../../topology.md#curve) when $P=Q$, and the distance is $|\log(q/p)|$.

For [curves](../../../topology.md#curve) stationary for the [energy of a curve](../../../riemannian-geometry.md#energy-of-a-curve), fixed-endpoint variations give the Euler–Lagrange equations for $F=(\dot u^2+\dot v^2)/v^2$:

$$
\frac d{dt}\left(\frac{\dot u}{v^2}\right)=0,\qquad v\ddot v-\dot v^2+\dot u^2=0.
$$

Thus $\dot u=cv^2$ for a constant $c$. Since $u(1)-u(0)=0$, integration gives $c\int_0^1v^2dt=0$, hence $c=0$. The second equation then becomes $(\dot v/v)'=0$. Therefore

$$
\boxed{\gamma(t)=ip\exp\left[t\log(q/p)\right],\qquad \dot v/v=\log(q/p).}
$$

It has constant hyperbolic speed, is one of the absolute length minimizers, and also has minimum [energy of a curve](../../../riemannian-geometry.md#energy-of-a-curve) $E=[\log(q/p)]^2$.

## 13B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13b/i">i</h3>

↑ **Parent:** [13B](#13b)

<h4 id="13b/i/solution">Solution</h4>

↑ **Parent:** [I](#13b/i)

Choose $a_0\in A$ and put $R=\|a_0-y\|$. The intersection $K=A\cap\overline B(y,R)$ is nonempty, closed and bounded in $\mathbb R^n$, hence [compact](../../../topology.md#compact-space). The [continuous](../../../calculus.md#continuous-function) distance [function](../../../function.md) $a\mapsto\|a-y\|$ attains a minimum at some $x\in K$. For $a\in A\setminus K$ its value is strictly greater than $R$, while the value at $x$ is at most that at $a_0$, namely $R$. Thus this minimum on $K$ is a minimum on all of $A$:

$$
\boxed{x\in A,\qquad\|x-y\|\leq\|a-y\|\quad\text{for every }a\in A.}
$$

The set $A$ itself need not be bounded; only the [compact](../../../topology.md#compact-space) portion needed to find the nearest point is bounded.

<h3 id="13b/ii">ii</h3>

↑ **Parent:** [13B](#13b)

<h4 id="13b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#13b/ii)

Suppose two distinct minimizers $x_1,x_2$ have the same minimum distance $d$ from $y$. [Convexity](../../../real-analysis.md#convex-function) puts their midpoint $z=(x_1+x_2)/2$ in $A$. Expanding the [Euclidean norm](../../../functional-analysis.md#euclidean-norm) gives

$$
\|z-y\|^2=\frac12\|x_1-y\|^2+\frac12\|x_2-y\|^2-\frac14\|x_1-x_2\|^2
=d^2-\frac14\|x_1-x_2\|^2<d^2,
$$

contradicting minimality. Therefore **the nearest point is unique**. Together with the preceding existence proof, this defines the metric projection onto a nonempty closed [convex set](../../../mathematical-optimization.md#convex-set).

## 14F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14f/solution">Solution</h3>

↑ **Parent:** [14F](#14f)

Close the real-line contour by a positively oriented upper semicircle of radius $R$, beyond every pole. The rational [function](../../../function.md) is $O(R^{-2})$ uniformly on that arc, and $|e^{iz}|=e^{-\Im z}\leq1$. Its arc [integral](../../../calculus.md#integral) is therefore $O(R^{-1})$ and vanishes. The real [integral](../../../calculus.md#integral) is absolutely convergent, while no pole lies on it. The residue theorem gives

$$
\boxed{\int_{-\infty}^{\infty}F(x)e^{ix}\,dx
=2\pi i\sum_{\Im z_j>0}\operatorname{Res}_{z=z_j}\bigl(F(z)e^{iz}\bigr).}
$$

Only actual poles contribute; any removable zero of the denominator has zero residue. The same contour proof covers poles of any order.

For the particular denominator, the upper poles are $a=1+i$ and $b=-1+i$. They are simple, with residues $e^{ia}/(4a^3)$ and $e^{ib}/(4b^3)$. Since

$$
\frac1{4a^3}=\frac{-1-i}{16},\qquad
\frac1{4b^3}=\frac{1-i}{16},
$$

their sum is

$$
\frac{e^{-1}}{16}\bigl[(-1-i)e^{i}+(1-i)e^{-i}\bigr]
=-\frac{i e^{-1}}8(\cos1+\sin1).
$$

Multiplication by $2\pi i$ gives the real answer. The sine part of the real-line [integral](../../../calculus.md#integral) is zero by oddness, so

$$
\boxed{\int_{-\infty}^{\infty}\frac{\cos x}{4+x^4}\,dx
=\frac{\pi}{4e}(\cos1+\sin1).}
$$

## 15E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15e/solution">Solution</h3>

↑ **Parent:** [15E](#15e)

Fixed endpoint variations yield the Euler–Lagrange equation

$$
F_r-\frac d{dz}F_{r'}=0.
$$

When $F$ is independent of $z$, differentiation gives

$$
\frac d{dz}(F-r'F_{r'})=r'\left(F_r-\frac d{dz}F_{r'}\right)=0.
$$

This is the [Beltrami identity](../../../analysis.md#beltrami-identity). Denote the constant by $1/k$ when nonzero; for a general Lagrangian a zero constant is also possible.

The film area is $S=2\pi\int_{-H}^Hr\sqrt{1+r'^2}\,dz$. Suppressing its harmless positive factor $2\pi$, take $F=r\sqrt{1+r'^2}$. The Euler–Lagrange equation reduces to

$$
\boxed{rr''=1+r'^2,\qquad r(-H)=r(H)=R.}
$$

The [first integral](../../../differential-equation.md#first-integral) is $r/\sqrt{1+r'^2}=1/k$ with $k>0$. Hence $1+r'^2=k^2r^2$ and, using the [differential equation](../../../differential-equation.md) without dividing by $r'$, $r''=k^2r$. The positive solution obeying that [first integral](../../../differential-equation.md#first-integral) is $r=k^{-1}\cosh(k(z-z_0))$. Equal endpoint radii force $z_0=0$, giving

$$
\boxed{r(z)=k^{-1}\cosh(kz),\qquad R=k^{-1}\cosh(kH).}
$$

Thus every smooth positive stationary film in this axisymmetric class is a [catenoid](../../../differential-geometry.md#catenoid).

Put $u=kH>0$. The boundary equation is $R/H=f(u)=\cosh u/u$. The [function](../../../function.md) tends to infinity at both endpoints of $(0,\infty)$, and

$$
f'(u)=\frac{u\sinh u-\cosh u}{u^2}.
$$

Its minimum occurs when $u=\coth u$. The [function](../../../function.md) $u-\coth u$ is strictly increasing, with [derivative](../../../calculus.md#derivative) $1+\operatorname{csch}^2u>0$, and has limits $-\infty$ and $+\infty$. It therefore has exactly one positive zero $A$. At this point $1/A=\tanh A$, so $f(A)=\sinh A$. This proves the [catenoid existence threshold for equal rings](../../../differential-geometry.md#catenoid-existence-threshold-for-equal-rings):

$$
\boxed{R/H<\sinh A\Longrightarrow\text{no smooth connected catenoid solution}.}
$$

At equality there is one stationary solution and above it two. The equation describes candidates for an area minimum, not a guarantee that both branches minimize. The thinner-neck branch is unstable to suitable axisymmetric variations; topology-changing collapse can also compete with [connected](../../../geometry-and-topology.md#connected-space) films. In particular two separate planar disks have area $2\pi R^2$. The derived threshold concerns existence of the smooth annular stationary film; it does not exclude such disconnected competitors.

## 16G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16g/solution">Solution</h3>

↑ **Parent:** [16G](#16g)

On a suitable dense domain of smooth rapidly decreasing [wave functions](../../../quantum-mechanics.md#wave-function), the canonical [commutator](../../../lie-algebra.md#commutator) is $[x,p]=i\hbar$. Expanding the two [ladder operators](../../../semisimple-lie-algebra.md#ladder-operator) gives

$$
[a,a^\dagger]=\frac12\left[\beta x+\frac{ip}{\beta\hbar},\beta x-\frac{ip}{\beta\hbar}\right]
=\frac12(1+1)=1.
$$

Their sum and difference give

$$
\boxed{x=\frac{a+a^\dagger}{\sqrt2\beta},\qquad
p=\frac{\beta\hbar}{i\sqrt2}(a-a^\dagger).}
$$

Direct multiplication, retaining the operator order, gives

$$
a^\dagger a=\frac12\left[\beta^2x^2+\frac{p^2}{\beta^2\hbar^2}+\frac{i[x,p]}\hbar\right]
=\frac12\left[\beta^2x^2+\frac{p^2}{\beta^2\hbar^2}-1\right].
$$

Using $\beta^2=m\omega/\hbar$ identifies the [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics):

$$
\boxed{H=\hbar\omega(a^\dagger a+\tfrac12).}
$$

For any admissible [wave function](../../../quantum-mechanics.md#wave-function), adjointness gives

$$
\langle\Psi,H\Psi\rangle=\hbar\omega\left(\|a\Psi\|^2+\tfrac12\|\Psi\|^2\right)
\geq\tfrac12\hbar\omega\|\Psi\|^2.
$$

For the conventional normalized state $\|\Psi\|=1$, this is the stated lower bound $E\geq\hbar\omega/2$. For an unnormalized [function](../../../function.md) the [norm](../../../functional-analysis.md#norm) factor must be retained; rescaling a [wave function](../../../quantum-mechanics.md#wave-function) cannot leave its unnormalized [energy](../../../classical-mechanics.md#energy) [integral](../../../calculus.md#integral) bounded below by a fixed positive number.

Equality holds exactly when $a\Psi_0=0$. In position representation this equation is $(\beta x+\beta^{-1}\partial_x)\Psi_0=0$, whose normalized square-integrable solution is

$$
\boxed{\Psi_0(x)=\left(\frac{\beta^2}{\pi}\right)^{1/4}e^{-\beta^2x^2/2},\qquad E_0=\tfrac12\hbar\omega.}
$$

This construction establishes existence of a state attaining the bound, and hence proves that it is the [ground state](../../../quantum-mechanics.md#ground-state).

The [commutator](../../../lie-algebra.md#commutator) $[a,a^\dagger]=1$ implies $[H,a^\dagger]=\hbar\omega a^\dagger$. Repeatedly commuting through the product gives

$$
H(a^\dagger)^n\Psi_0=(a^\dagger)^nH\Psi_0+n\hbar\omega(a^\dagger)^n\Psi_0
=\hbar\omega(n+\tfrac12)(a^\dagger)^n\Psi_0.
$$

These [vectors](../../../vector-space.md#vector) are nonzero: the identity $a(a^\dagger)^n\Psi_0=n(a^\dagger)^{n-1}\Psi_0$ gives their [norm](../../../functional-analysis.md#norm) squared $n!$ by induction. Therefore

$$
\boxed{\Psi_n=\frac{(a^\dagger)^n}{\sqrt{n!}}\Psi_0,\qquad E_n=(n+\tfrac12)\hbar\omega.}
$$

For time-dependent stationary states multiply each spatial eigenfunction by $e^{-iE_nt/\hbar}$.

## 17H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17h/solution">Solution</h3>

↑ **Parent:** [17H](#17h)

In Cartesian coordinates the [magnetic field](../../../electromagnetism.md#magnetic-field) is $(bx,by,-2bz)$. Its [divergence](../../../calculus.md#divergence) is $b+b-2b=0$, and all components of its [curl](../../../calculus.md#curl) vanish. Thus it satisfies the static vacuum magnetic equations $\nabla\cdot\mathbf B=0$ and $\nabla\times\mathbf B=0$, with no [electric current](../../../electromagnetism.md#electric-current) in the region.

Fix clockwise orientation as viewed from above, looking down the positive $z$-axis. Its positive area normal is $-\mathbf e_z$. The loop's external [magnetic flux](../../../electromagnetism.md#magnetic-flux) is therefore

$$
\boxed{\Phi_B=2\pi ba^2z=Kz,\qquad K=2\pi ba^2.}
$$

With the opposite normal its flux has the opposite sign. On the circle $\mathbf B=ba\mathbf e_r-2bz\mathbf e_z$ and clockwise line element is $d\boldsymbol\ell=-a\mathbf e_\varphi d\varphi$. The [Lorentz force](../../../electromagnetism.md#lorentz-force) element is

$$
I\,d\boldsymbol\ell\times\mathbf B=Iba^2\mathbf e_z\,d\varphi+2Ibaz\mathbf e_r\,d\varphi.
$$

The radial terms cancel around the circle, so

$$
\boxed{\mathbf F_B=KI\mathbf e_z.}
$$

This fixes the current/flux/force signs together.

Neglect [self-inductance](../../../electromagnetism.md#self-inductance) initially, so [Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) and [Ohm's law](../../../electromagnetism.md#ohm-s-law) give $RI=-K\dot z$. Including gravity then gives

$$
\boxed{m\ddot z=-mg-\frac{K^2}{R}\dot z.}
$$

For $R>0$ and $K\ne0$, the terminal solution is $z=z_0-vt$ with

$$
\boxed{v=\frac{mgR}{K^2}=\frac{mgR}{4\pi^2b^2a^4}.}
$$

The general [velocity](../../../classical-mechanics.md#velocity) relaxes exponentially to $-v$ on time scale $mR/K^2$. In the terminal state $I=Kv/R$, and the Joule-heating rate is

$$
I^2R=\frac{K^2v^2}{R}=mgv=-\frac{d}{dt}(mgz).
$$

Thus all the lost [gravitational potential energy](../../../classical-mechanics.md#gravitational-energy) becomes resistive heat when kinetic [energy](../../../classical-mechanics.md#energy) is constant.

Within the zero-inductance approximation $v\to0$ as $R\to0$; finite-speed motion would require an unbounded current. This limit is singular, so it is important to describe the physical ideal-conductor limit separately. With finite [self-inductance](../../../electromagnetism.md#self-inductance) $\mathcal L$, the circuit equation is $\mathcal L\dot I+RI=-K\dot z$. At $R=0$, total linked flux $\mathcal LI+Kz$ is conserved and there is no [Joule heating](../../../electromagnetism.md#joule-heating). If $I=0$ initially at $z_0$, then

$$
I=-\frac K{\mathcal L}(z-z_0),\qquad
m\ddot z=-mg-\frac{K^2}{\mathcal L}(z-z_0).
$$

This [lossless limit of magnetic loop braking](../../../electromagnetism.md#lossless-limit-of-magnetic-loop-braking) has undamped oscillations about $z_0-mg\mathcal L/K^2$, with magnetic [energy](../../../classical-mechanics.md#energy) storing and returning mechanical [energy](../../../classical-mechanics.md#energy). It has no generic dissipative terminal descent. Thus the vanishing terminal speed is the formal resistive-model limit, not a justification for dropping inductance in a perfectly conducting moving loop.

## 18F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18f/a">a</h3>

↑ **Parent:** [18F](#18f)

<h4 id="18f/a/solution">Solution</h4>

↑ **Parent:** [A](#18f/a)

Take $Q_j$ nonzero of exact degree $j$, so $Q_0,\ldots,Q_n$ are an [orthogonal](../../../linear-algebra.md#orthogonal-vectors) [basis](../../../vector-space.md#basis) of the [polynomials](../../../polynomial.md) of degree at most $n$. Their [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) is

$$
\boxed{p_n=\sum_{j=0}^n\frac{(f,Q_j)}{(Q_j,Q_j)}Q_j.}
$$

Indeed its residual is [orthogonal](../../../linear-algebra.md#orthogonal-vectors) to every such [polynomial](../../../polynomial.md). For another [polynomial](../../../polynomial.md) $q=p_n+r$ of degree at most $n$, the squared error is

$$
\|f-q\|^2=\|f-p_n\|^2+\|r\|^2,
$$

since the cross term vanishes. It is uniquely minimized at $r=0$. The approximation need not have exact degree $n$ when the highest coefficient happens to vanish.

<h3 id="18f/b">b</h3>

↑ **Parent:** [18F](#18f)

<h4 id="18f/b/solution">Solution</h4>

↑ **Parent:** [B](#18f/b)

Use first-kind [Chebyshev polynomials](../../../numerical-analysis.md#chebyshev-polynomial) $T_j$, characterized by $T_j(\cos\theta)=\cos(j\theta)$. Substituting $x=\cos\theta$ converts the weighted [inner product](../../../linear-algebra.md#inner-product) into $\int_0^\pi g(\cos\theta)h(\cos\theta)d\theta$. Hence these [polynomials](../../../polynomial.md) are [orthogonal](../../../linear-algebra.md#orthogonal-vectors), with squared [norms](../../../functional-analysis.md#norm) $\pi$ for $j=0$ and $\pi/2$ for $j\geq1$.

For the specified [function](../../../function.md), $f(\cos\theta)=\sin\theta$. Its constant projection coefficient is $\pi^{-1}\int_0^\pi\sin\theta\,d\theta=2/\pi$. For $j\geq1$ the coefficient is $(2/\pi)\int_0^\pi\sin\theta\cos(j\theta)d\theta$. Symmetry about $\pi/2$ makes it zero for odd $j$. For $j=2m$, the product-to-sum identity gives

$$
\int_0^\pi\sin\theta\cos(2m\theta)d\theta
=\frac1{1+2m}+\frac1{1-2m}=\frac2{1-4m^2}.
$$

Therefore the [Chebyshev projection of a semicircle](../../../numerical-analysis.md#chebyshev-projection-of-a-semicircle) is

$$
\boxed{p_n(x)=\frac2\pi-\frac4\pi\sum_{m=1}^{\lfloor n/2\rfloor}\frac{T_{2m}(x)}{4m^2-1}.}
$$

In particular the best degree-at-most-$n$ [polynomial](../../../polynomial.md) is even, so for odd $n$ its actual degree is at most $n-1$.

## 19D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="19d/solution">Solution</h3>

↑ **Parent:** [19D](#19d)

For observed data $x$, let $F_x$ be the [posterior](../../../statistical-inference.md#bayesian-posterior) [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function). Assuming finite [posterior](../../../statistical-inference.md#bayesian-posterior) first moment, the [posterior](../../../statistical-inference.md#bayesian-posterior) risk under [asymmetric absolute-error loss](../../../statistical-inference.md#asymmetric-absolute-error-loss) is

$$
R_x(a)=\gamma\int_a^\infty(\theta-a)\pi(\theta\mid x)d\theta
+\delta\int_{-\infty}^a(a-\theta)\pi(\theta\mid x)d\theta.
$$

At points where the [posterior](../../../statistical-inference.md#bayesian-posterior) has a density, differentiation gives $R_x'(a)=(\gamma+\delta)F_x(a)-\gamma$. Risk is convex, so a global minimum is a [posterior](../../../statistical-inference.md#bayesian-posterior) [quantile](../../../probability-theory.md#quantile-function):

$$
\boxed{a(x)=F_x^{-1}\left(\frac\gamma{\gamma+\delta}\right).}
$$

More generally any $a$ with $F_x(a^-)\leq\gamma/(\gamma+\delta)\leq F_x(a)$ minimizes risk. This is the [Bayes quantile under asymmetric absolute-error loss](../../../statistical-inference.md#bayes-quantile-under-asymmetric-absolute-error-loss); a larger cost for underestimation moves the chosen [quantile](../../../probability-theory.md#quantile-function) upward.

For the uniform sampling model set $M=\max_iX_i$. For a valid positive sample the [likelihood](../../../statistical-modelling.md#likelihood-function) is $\theta^{-n}\mathbf1_{\{\theta>M\}}$. Multiplying by the [prior](../../../statistical-inference.md#prior-probability) cancels its power of $\theta$ and gives [posterior](../../../statistical-inference.md#bayesian-posterior) density proportional to $e^{-\theta}\mathbf1_{\{\theta>M\}}$. Normalization yields

$$
\pi(\theta\mid x)=e^{-(\theta-M)}\mathbf1_{\{\theta>M\}},\qquad
F_x(a)=1-e^{-(a-M)}\quad(a\geq M).
$$

Solving the [quantile](../../../probability-theory.md#quantile-function) equation gives the explicit Bayes estimate

$$
\boxed{a(X_1,\ldots,X_n)=M+\log\left(\frac{\gamma+\delta}{\delta}\right).}
$$

The [posterior](../../../statistical-inference.md#bayesian-posterior) is the sample maximum plus a unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) displacement; it has finite first moment, so the preceding risk minimization is justified here.

## 20D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="20d/solution">Solution</h3>

↑ **Parent:** [20D](#20d)

The transition row sums to one, since $p\sum_{k=0}^iq^k+q^{i+1}=1$. From any state the [Markov chain](../../../markov-process.md#markov-chain) can reach zero, and from zero consecutive upward moves reach every state; hence it is irreducible. Its self-transition at zero has [probability](../../../probability-theory.md#probability) $q>0$, so it is [aperiodic](../../../markov-process.md#aperiodic-markov-chain). It is the [reflected chain with geometric downward jumps](../../../markov-process.md#reflected-chain-with-geometric-downward-jumps).

Put $h_0=1$ for the hitting problem. The first-step equations for $i\geq1$ are

$$
\boxed{h_i=q^{i+1}+p\sum_{j=1}^{i+1}q^{i-j+1}h_j.}
$$

Subtracting $q$ times the equation at $i-1$ gives the [linear recurrence relation](../../../algebra.md#linear-recurrence-relation), valid for $i\geq2$,

$$
\boxed{ph_{i+1}-h_i+qh_{i-1}=0.}
$$

The separate boundary equation at $i=1$ is $h_1=q^2+pqh_1+ph_2$. It must not be replaced by the [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) with $h_0=1$: the absorbing hitting convention at zero is different from applying a first-step return equation there.

For $p\ne q$, the [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) has roots $1$ and $r=q/p$, so $h_i=A+Br^i$ for $i\geq1$. The boundary equation gives $B=r(1-A)$. If $p<1/2$, then $r>1$ and boundedness of probabilities forces $B=0$, hence $A=1$. If $p=1/2$, the repeated-root solution is $A+Bi$; boundedness again gives $B=0$ and the boundary equation gives $A=1$.

For $p>1/2$, $r<1$ and the nonnegative harmonic candidate $\widetilde h_i=r^{i+1}$, together with $\widetilde h_0=1$, satisfies every first-step equation. Hitting-by-time-$n$ probabilities start from zero off the target and iterate those equations, so by induction they are bounded above by this candidate. Taking their increasing limit gives $h_i\leq r^{i+1}$. But the general bounded solution has limit $A\geq0$ as $i\to\infty$, forcing $A=0$ under that bound. Thus

$$
\boxed{h_i=\begin{cases}1,&p\leq1/2,\\(q/p)^{i+1},&p>1/2,\end{cases}\qquad i\geq1.}
$$

In particular the transient exponent is $i+1$, fixed by the original boundary equation.

The [probability](../../../probability-theory.md#probability) of a subsequent return to zero when starting there is $f_{00}=q+ph_1$. It is one for $p\leq1/2$, so the [Markov chain](../../../markov-process.md#markov-chain) is recurrent there. For $p>1/2$ it equals $q+p(q/p)^2=q/p<1$, so the [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) is transient.

For a stationary [probability](../../../probability-theory.md#probability) [vector](../../../vector-space.md#vector) $\pi$, balance at zero and one gives $\pi_1=(p/q)\pi_0$. Subtracting adjacent balance equations gives

$$
q\pi_{j+1}-\pi_j+p\pi_{j-1}=0\qquad(j\geq1),
$$

so this initial ratio propagates and $\pi_j=\pi_0(p/q)^j$. It can be normalized only when $p<q$. In that case

$$
\boxed{\pi_j=\left(1-\frac pq\right)\left(\frac pq\right)^j,\qquad j=0,1,2,\ldots.}
$$

Direct substitution verifies all balance equations, including $\pi_0=q\sum_i\pi_iq^i$. An [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) admitting this stationary [probability](../../../probability-theory.md#probability) law is [positive recurrent](../../../markov-process.md#positive-recurrent-markov-chain), with mean return time $1/\pi_0=q/(q-p)$. At $p=q$ the [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) and boundary relation force every $\pi_j$ equal; no such nonzero sequence is summable. The recurrent chain is therefore [null recurrent](../../../markov-process.md#null-recurrent-state). In summary,

$$
\boxed{p<1/2:\ \text{positive recurrent};\qquad p=1/2:\ \text{null recurrent};\qquad p>1/2:\ \text{transient}.}
$$

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
