# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperib_2_2018.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperib_2_2018.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2G](#2g)
  - [a](#2g/a)
    - [Solution](#2g/a/solution)
  - [b](#2g/b)
    - [Solution](#2g/b/solution)
- [3F](#3f)
  - [Solution](#3f/solution)
- [4E](#4e)
  - [Solution](#4e/solution)
- [5C](#5c)
  - [Solution](#5c/solution)
- [6C](#6c)
  - [Solution](#6c/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
- [8H](#8h)
  - [Solution](#8h/solution)
- [9H](#9h)
  - [Solution](#9h/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
- [11G](#11g)
  - [a](#11g/a)
    - [Solution](#11g/a/solution)
  - [b](#11g/b)
    - [i](#11g/b/i)
      - [Solution](#11g/b/i/solution)
    - [ii](#11g/b/ii)
      - [Solution](#11g/b/ii/solution)
    - [iii](#11g/b/iii)
      - [Solution](#11g/b/iii/solution)
- [12F](#12f)
  - [a](#12f/a)
    - [Solution](#12f/a/solution)
  - [b](#12f/b)
    - [Solution](#12f/b/solution)
  - [c](#12f/c)
    - [Solution](#12f/c/solution)
- [13A](#13a)
  - [a](#13a/a)
    - [Solution](#13a/a/solution)
  - [b](#13a/b)
    - [Solution](#13a/b/solution)
  - [c](#13a/c)
    - [Solution](#13a/c/solution)
  - [d](#13a/d)
    - [Solution](#13a/d/solution)
- [14G](#14g)
  - [a](#14g/a)
    - [Solution](#14g/a/solution)
  - [b](#14g/b)
    - [Solution](#14g/b/solution)
  - [c](#14g/c)
    - [Solution](#14g/c/solution)
  - [d](#14g/d)
    - [Solution](#14g/d/solution)
- [15B](#15b)
  - [Solution](#15b/solution)
- [16A](#16a)
  - [a](#16a/a)
    - [Solution](#16a/a/solution)
  - [b](#16a/b)
    - [Solution](#16a/b/solution)
- [17B](#17b)
  - [Solution](#17b/solution)
- [18C](#18c)
  - [Solution](#18c/solution)
- [19D](#19d)
  - [Solution](#19d/solution)
- [20H](#20h)
  - [i](#20h/i)
    - [Solution](#20h/i/solution)
  - [ii](#20h/ii)
    - [Solution](#20h/ii/solution)
  - [iii](#20h/iii)
    - [Solution](#20h/iii/solution)

## 1E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

The [dual vector space](../../../linear-algebra.md#linear-functional) is $V^*=\operatorname{Hom}_{\mathbb R}(V,\mathbb R)$, the [vector space](../../../vector-space.md) of all [linear functionals](../../../linear-algebra.md#linear-functional) on $V$. For a [vector subspace](../../../vector-space.md#vector-subspace) $U\leq V$, its [annihilator of a vector subspace](../../../linear-algebra.md#annihilator-of-a-vector-subspace) is

$$
U^0=\{\phi\in V^*: \phi(u)=0\text{ for every }u\in U\}.
$$

Given a [basis](../../../vector-space.md#basis) $x_1,\ldots,x_n$, define $x_i^*$ by $x_i^*(x_j)=\delta_{ij}$ and extend linearly. If $\sum_i a_i x_i^*=0$, evaluation at $x_j$ gives $a_j=0$, so the $x_i^*$ are [linearly independent](../../../vector-space.md#linear-independence). Every $\phi\in V^*$ satisfies

$$
\phi=\sum_{i=1}^n\phi(x_i)x_i^*,
$$

so they also [span](../../../vector-space.md#linear-span) $V^*$ and therefore form its [dual basis](../../../linear-algebra.md#dual-basis).

Write $\phi=a x_1^*+b x_2^*+c x_3^*+d x_4^*$. The condition $\phi\in U^0$ is

$$
a+2b+3c+4d=0,\qquad 5a+6b+7c+8d=0.
$$

[Gaussian elimination](../../../numerical-analysis.md#gaussian-elimination) gives $b=-2c-3d$ and $a=c+2d$. Hence

$$
\boxed{U^0=\operatorname{span}\{x_1^*-2x_2^*+x_3^*,\;2x_1^*-3x_2^*+x_4^*\}.}
$$

## 2G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2g/a">a</h3>

↑ **Parent:** [2G](#2g)

<h4 id="2g/a/solution">Solution</h4>

↑ **Parent:** [A](#2g/a)

Let $S=\{1,x,x^2,\ldots\}$. Since a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain) is an [integral domain](../../../commutative-algebra.md#integral-domain) and $x\ne0$, $S$ is a [multiplicative subset](../../../commutative-algebra.md#multiplicatively-closed-set) avoiding zero. The stated [equivalence relation](../../../set-theory.md#equivalence-relation) and operations are precisely those of the [localization of a ring](../../../commutative-algebra.md#localization-of-a-ring) $S^{-1}R$.

For completeness, reflexivity and symmetry are immediate, while transitivity follows by multiplying the two cross-multiplication identities and cancelling a nonzero power of $x$. If $(r,x^n)\sim(s,x^m)$ and $(r',x^{n'})\sim(s',x^{m'})$, cross multiplication shows that the proposed sums and products are equivalent. Thus the operations do not depend on representatives. The usual fraction calculations then prove associativity, commutativity and distributivity, with identities $[(0,1)]$ and $[(1,1)]$. **Therefore $R'$ is a well-defined commutative ring.**

<h3 id="2g/b">b</h3>

↑ **Parent:** [2G](#2g)

<h4 id="2g/b/solution">Solution</h4>

↑ **Parent:** [B](#2g/b)

Let $J$ be an [ideal](../../../commutative-algebra.md#ideal) of $R'=S^{-1}R$ and contract it to

$$
I=\{r\in R:r/1\in J\}.
$$

This is an ideal of $R$, so $I=(d)$ because $R$ is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain). Every $x^n/1$ is a [unit in a ring](../../../algebra.md#unit-in-a-ring) $R'$. Consequently, if $r/x^n\in J$, then $r/1=(x^n/1)(r/x^n)\in J$, so $r\in(d)$ and $r/x^n\in(d/1)$. Conversely $d/1\in J$, hence every multiple of it belongs to $J$. Thus

$$
\boxed{J=(d/1),}
$$

so every ideal of $R'$ is principal. The localization remains an [integral domain](../../../commutative-algebra.md#integral-domain); hence **$R'$ is a principal ideal domain.**

## 3F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3f/solution">Solution</h3>

↑ **Parent:** [3F](#3f)

The [L1 norm](../../../functional-analysis.md#l1-norm) properties of absolute homogeneity and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) follow from the corresponding properties of the absolute value and the [integral](../../../calculus.md#integral). If $\|f\|_1=0$, the nonnegative [continuous function](../../../calculus.md#continuous-function) $|f|$ has zero integral. Were $|f(x_0)|>0$, continuity would make it bounded below by a positive number on a nontrivial interval, contradicting the zero integral. Thus $f=0$, proving positive definiteness.

Put $M=\|f\|_\infty$ and choose the continuous [cutoff function](../../../distribution-theory.md#cutoff-function)

$$
\eta_n(x)=\min\{1,nx,n(1-x)\},\qquad g_n=\eta_n f.
$$

Then $g_n(0)=g_n(1)=0$, $\|g_n\|_\infty\leq M$, and $f-g_n$ is supported in the two endpoint intervals of total length $2/n$. Therefore

$$
\|f-g_n\|_1\leq\frac{2M}{n}\longrightarrow0.
$$

Now suppose $\int_0^1fg=0$ for every $g\in\mathcal S$. Apply this to the above $g_n$. By the [uniform norm](../../../functional-analysis.md#supremum-norm) bound,

$$
0\leq\int_0^1f^2
=\int_0^1f(f-g_n)
\leq\|f\|_\infty\|f-g_n\|_1\longrightarrow0.
$$

Hence $\int_0^1f^2=0$, and continuity again gives **$f=0$.**

## 4E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4e/solution">Solution</h3>

↑ **Parent:** [4E](#4e)

A [metric space](../../../topological-analysis.md#metric-space) metric $d:X\times X\to[0,\infty)$ satisfies positivity, $d(x,y)=0$ exactly when $x=y$, symmetry, and the [triangle inequality](../../../topological-analysis.md#triangle-inequality). A subset $U\subseteq X$ is an [open set](../../../topology.md#open-set) when every $x\in U$ has some $\varepsilon>0$ with the open ball $B_d(x,\varepsilon)\subseteq U$.

Both $\varnothing$ and $X$ are open. An arbitrary union of open sets is open because a point lies in one member supplying a ball. A finite intersection is open because the minimum of the finitely many available radii supplies a ball. Thus the metric-open sets satisfy the [topology axioms](../../../topology.md#topology-axiom).

For $C[0,1]$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $d_1(f,g)\leq d_2(f,g)$, so the $d_2$ topology is at least as fine as the $d_1$ topology. To see strictness, define the continuous triangular spikes

$$
f_n(x)=\sqrt n\max\{1-nx,0\}.
$$

Then

$$
d_1(f_n,0)=\frac1{2\sqrt n}\longrightarrow0,
\qquad
d_2(f_n,0)^2=\int_0^{1/n}n(1-nx)^2\,dx=\frac13.
$$

Thus $f_n$ converges to zero in the [L1 norm](../../../functional-analysis.md#l1-norm) but not in the [L2 norm](../../../real-analysis.md#l2-norm). **The two metrics induce different topologies.**

## 5C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5c/solution">Solution</h3>

↑ **Parent:** [5C](#5c)

Along a curve $s\mapsto(x(s),y(s))$, the [chain rule](../../../calculus.md#chain-rule) gives

$$
\frac d{ds}u_x=u_{xx}\dot x+u_{xy}\dot y,
\qquad
\frac d{ds}u_y=u_{xy}\dot x+u_{yy}\dot y.
$$

Together with the [second-order partial differential equation](../../../partial-differential-equation.md#second-order-partial-differential-equation), these form a [linear system](../../../linear-algebra.md#system-of-linear-equations) for $(u_{xx},u_{xy},u_{yy})$ whose coefficient matrix is

$$
\begin{pmatrix}
\dot x&\dot y&0\\
0&\dot x&\dot y\\
a&2b&c
\end{pmatrix}.
$$

A [characteristic curve](../../../partial-differential-equation.md#characteristic-curve) is precisely one along which this system is singular, equivalently where the [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) vanishes on a normal covector. Taking the [determinant](../../../linear-algebra.md#determinant) yields

$$
\boxed{a\dot y^2-2b\dot x\dot y+c\dot x^2=0.}
$$

## 6C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6c/solution">Solution</h3>

↑ **Parent:** [6C](#6c)

For a time-independent current, the [Maxwell equations](../../../electromagnetism.md#maxwell-equations) reduce to [magnetostatics](../../../electromagnetism.md#magnetostatics):

$$
\nabla\mathbin\cdot\mathbf B=0,
\qquad
\nabla\mathbin\times\mathbf B=\mu_0\mathbf j.
$$

Write $\mathbf B=\nabla\mathbin\times\mathbf A$ using a [vector potential](../../../calculus.md#vector-potential) and choose the [Coulomb gauge](../../../electromagnetism.md#coulomb-gauge) $\nabla\mathbin\cdot\mathbf A=0$. The vector identity for the curl of a curl gives the [Poisson equation](../../../partial-differential-equation.md#poisson-equation)

$$
-\nabla^2\mathbf A=\mu_0\mathbf j.
$$

The free-space [Green function](../../../analysis.md#green-s-function) therefore gives

$$
\mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\int_V
\frac{\mathbf j(\mathbf r')}{|\mathbf r-\mathbf r'|}\,dV'.
$$

Taking the [curl](../../../calculus.md#curl) with respect to $\mathbf r$, moving it under the integral, and using $\nabla(1/|\mathbf r-\mathbf r'|)=-(\mathbf r-\mathbf r')/|\mathbf r-\mathbf r'|^3$ gives the [Biot-Savart law](../../../electromagnetism.md#biot-savart-law)

$$
\boxed{\mathbf B(\mathbf r)=\frac{\mu_0}{4\pi}\int_V
\frac{\mathbf j(\mathbf r')\mathbin\times(\mathbf r-\mathbf r')}{|\mathbf r-\mathbf r'|^3}\,dV'.}
$$

## 7D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

Write $\mathbf g=-g\mathbf e_z$. The vertical component of the balance gives [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure),

$$
p(x,y,z)=p_0+\rho g[h(x,y)-z].
$$

Its horizontal [gradient](../../../calculus.md#gradient) is $\nabla_h p=\rho g\nabla_hh$. The horizontal balance is consequently

$$
f\mathbf e_z\mathbin\times\mathbf u=-g\nabla_hh,
\qquad
\mathbf u=\frac gf\mathbf e_z\mathbin\times\nabla_hh.
$$

Thus $\mathbf u\mathbin\cdot\nabla_hh=0$: the velocity is tangent to every [level set](../../../topology.md#level-set) of $h$, so those contours are [streamlines](../../../fluid-mechanics.md#streamline) of the [geostrophic flow](../../../geophysical-fluid-dynamics.md#geostrophic-flow).

Across a vertical section joining the contours $h_0$ and $h_0+\Delta h$, an element of horizontal distance normal to the contours is $dn=dh/|\nabla_hh|$, while $|\mathbf u|=(g/f)|\nabla_hh|$. The [volumetric flow rate](../../../fluid-mechanics.md#volumetric-flow-rate) is therefore

$$
Q=\int_{h_0}^{h_0+\Delta h}h\frac gf|\nabla_hh|\frac{dh}{|\nabla_hh|}
=\frac g{2f}[(h_0+\Delta h)^2-h_0^2]
\sim\boxed{\frac{gh_0\Delta h}{f}}.
$$

For [dimensional analysis](../../../physics.md#dimensional-analysis), $[g]=LT^{-2}$, $[f]=T^{-1}$ and $[h_0]=[\Delta h]=L$, so the result has dimension $L^3T^{-1}$, exactly that of a volume flux.

## 8H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8h/solution">Solution</h3>

↑ **Parent:** [8H](#8h)

A [simple hypothesis](../../../statistical-modelling.md#simple-hypothesis) specifies a single probability distribution. For a test with rejection region $R$, its [size of a statistical test](../../../statistical-modelling.md#size-of-a-statistical-test) is the rejection probability under the simple [null hypothesis](../../../statistical-modelling.md#null-hypothesis), while its [statistical power](../../../probability-and-statistics.md#statistical-power) against the simple alternative is the rejection probability under that alternative. The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) states that among tests of size at most $\alpha$, a test rejecting for the largest values of the [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) $f_1/f_0$ has greatest power, with boundary randomization if needed.

Here

$$
\frac{f_1(x)}{f_0(x)}=\frac32(1-x^2),
$$

which decreases with $|x|$. The best test therefore rejects for $|X|\leq c$. Under $H_0$, $\mathbb P_0(|X|\leq c)=c$, so size $0.05$ requires $c=0.05=1/20$. Its power is

$$
\boxed{\mathbb P_1(|X|\leq1/20)
=\int_{-1/20}^{1/20}\frac34(1-x^2)\,dx
=\frac{1199}{16000}=0.0749375.}
$$

**Thus reject $H_0$ exactly when $|X|\leq0.05$.**

## 9H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9h/solution">Solution</h3>

↑ **Parent:** [9H](#9h)

A function $f:\mathbb R^n\to\mathbb R$ is a [convex function](../../../real-analysis.md#convex-function) when

$$
f((1-t)x_0+tx_1)\leq(1-t)f(x_0)+tf(x_1)
$$

for every $x_0,x_1$ and $t\in[0,1]$.

Fix $b_0,b_1\in\mathbb R$, $t\in[0,1]$, and $\varepsilon>0$. Since the [value function](../../../mathematical-optimization.md#value-function) is finite, choose $x_i$ with

$$
g(x_i)\leq b_i,
\qquad
f(x_i)\leq\phi(b_i)+\varepsilon.
$$

For the [convex combination](../../../mathematical-optimization.md#convex-combination) $x_t=(1-t)x_0+tx_1$, convexity of $g$ gives

$$
g(x_t)\leq(1-t)b_0+tb_1,
$$

so $x_t$ is feasible for the intermediate right-hand side. Convexity of $f$ then gives

$$
\phi((1-t)b_0+tb_1)
\leq f(x_t)
\leq(1-t)\phi(b_0)+t\phi(b_1)+\varepsilon.
$$

Letting $\varepsilon\downarrow0$ proves

$$
\boxed{\phi((1-t)b_0+tb_1)\leq(1-t)\phi(b_0)+t\phi(b_1),}
$$

so **$\phi$ is convex.**

## 10E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

View $X$ as the matrix of a [linear map](../../../vector-space.md#linear-map) $T:F^m\to F^n$ of [matrix rank](../../../vector-space.md#matrix-rank) $r$. Choose vectors $u_1,\ldots,u_r$ whose images form a [basis](../../../vector-space.md#basis) of $\operatorname{im}T$, extend them by a basis of $\ker T$ to a basis of $F^m$, and extend $Tu_1,\ldots,Tu_r$ to a basis of $F^n$. In these two bases the matrix of $T$ is the [rank normal form](../../../linear-algebra.md#rank-normal-form)

$$
\begin{pmatrix}I_r&0\\0&0\end{pmatrix}.
$$

The two changes of basis give invertible $P,Q$ with the displayed matrix equal to $Q^{-1}XP$.

For the [block upper triangular matrix](../../../linear-algebra.md#block-upper-triangular-matrix) $A=\begin{pmatrix}B&D\\0&C\end{pmatrix}$, every nonzero term in the [Leibniz formula for determinants](../../../linear-algebra.md#leibniz-formula-for-determinants) sends the rows belonging to $C$ into the columns belonging to $C$; bijectivity then sends the remaining rows into the $B$ columns. The permutation sum consequently factors into the determinant sums for $B$ and $C$, proving

$$
\boxed{\det A=\det B\det C.}
$$

Finally suppose $L(X)=0$, so $AX=XB$: the map $X:\mathbb C^m\to\mathbb C^n$ is an [intertwining operator](../../../representation-theory.md#intertwining-operator). If $v$ lies in the [generalized eigenspace](../../../linear-operator-theory.md#generalized-eigenspace) of $B$ for $\lambda$, then for some $k$,

$$
(A-\lambda I)^kXv=X(B-\lambda I)^kv=0.
$$

Because $A$ and $B$ have no common [eigenvalue](../../../linear-operator-theory.md#eigenvalue), $A-\lambda I$ is invertible, hence $Xv=0$. The generalized eigenspaces of $B$ span $\mathbb C^m$, so $X=0$. Thus **the [Sylvester equation](../../../linear-algebra.md#sylvester-equation) operator $L$ is injective.**

## 11G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11g/a">a</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/a/solution">Solution</h4>

↑ **Parent:** [A](#11g/a)

First, every nonzero nonunit in a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain) factors into [irreducible elements](../../../commutative-algebra.md#irreducible-element). Otherwise repeatedly choose a proper nonunit factor $a_{j+1}$ of $a_j$; then the principal ideals

$$
(a_1)\subsetneq(a_2)\subsetneq\cdots
$$

form a strictly increasing chain, contradicting the [ascending chain condition](../../../algebra.md#ascending-chain-condition), since every principal ideal domain is a [Noetherian ring](../../../algebra.md#noetherian-ring).

Next every irreducible $p$ is a [prime element](../../../commutative-algebra.md#prime-element). If $p\mid ab$ but $p\nmid a$, then $\gcd(p,a)=1$. The [Bezout identity](../../../algebra.md#bezout-identity) gives $up+va=1$, so multiplying by $b$ shows $p\mid b$. Thus irreducibles are prime.

Existence of an irreducible factorization and primality give uniqueness: an irreducible on one side divides the product on the other, hence is associate to one factor; cancel and continue. **Therefore every principal ideal domain is a [unique factorization domain](../../../algebra.md#unique-factorization-domain).**

<h3 id="11g/b">b</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/b/i">i</h4>

↑ **Parent:** [B](#11g/b)

<h5 id="11g/b/i/solution">Solution</h5>

↑ **Parent:** [I](#11g/b/i)

Any [unit in a ring](../../../algebra.md#unit-in-a-ring) of $R$ must also be a unit of $\mathbb Q[X]$, hence a nonzero constant $q\in\mathbb Q$. Membership of both $q$ and $q^{-1}$ in $R$ requires $q,q^{-1}\in\mathbb Z$, so

$$
\boxed{R^\times=\{1,-1\}.}
$$

<h4 id="11g/b/ii">ii</h4>

↑ **Parent:** [B](#11g/b)

<h5 id="11g/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11g/b/ii)

Let $f\in R$ be irreducible. If $\deg f=0$, then $f\in\mathbb Z$. A nonzero integer that is neither a unit nor, up to sign, a [prime number](../../../number-theory.md#prime-number) factors nontrivially in $R$, so necessarily $f=\pm p$ for a prime $p$.

Now suppose $\deg f\geq1$ and write $m=f(0)\in\mathbb Z$. If $m=0$, then

$$
f=2(f/2),
$$

and both factors lie in $R$ and are nonunits. If $|m|>1$, choose a prime $p\mid m$; then $f=p(f/p)$ is again a factorization into two nonunits of $R$, since $(f/p)(0)=m/p\in\mathbb Z$. Both cases contradict irreducibility. Hence

$$
\boxed{\deg f\geq1\quad\Longrightarrow\quad f(0)=\pm1.}
$$

<h4 id="11g/b/iii">iii</h4>

↑ **Parent:** [B](#11g/b)

<h5 id="11g/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#11g/b/iii)

Suppose $X=f_1\cdots f_s$ were a product of [irreducible elements](../../../commutative-algebra.md#irreducible-element) of $R$. Since [degree of a polynomial](../../../polynomial.md#degree-of-a-polynomial) is additive under products, exactly one factor has positive degree and all the others are constant. By the preceding classification, the positive-degree factor has constant term $\pm1$, while every constant irreducible is $\pm p$ for a prime $p$. Their product therefore has a nonzero constant term, contradicting $X(0)=0$.

Thus **$X$ is not a product of irreducibles**, so this [integral domain](../../../commutative-algebra.md#integral-domain) is not an [atomic domain](../../../commutative-algebra.md#atomic-domain) and in particular is not a [unique factorization domain](../../../algebra.md#unique-factorization-domain).

## 12F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12f/a">a</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/a/solution">Solution</h4>

↑ **Parent:** [A](#12f/a)

A map $f:A\to\mathbb R$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) with [Lipschitz constant](../../../real-analysis.md#lipschitz-constant) $L$ when

$$
|f(y)-f(z)|\leq Ld(y,z)
$$

for all $y,z\in A$.

Fix $y_0\in A$. The Lipschitz inequality and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) imply

$$
f(y)+Ld(x,y)\geq f(y_0)-Ld(y,y_0)+Ld(x,y)
\geq f(y_0)-Ld(x,y_0),
$$

while choosing $y=y_0$ gives a finite upper bound. Hence the [infimum](../../../real-analysis.md#infimum) defining $F(x)$ is a real number.

If $x\in A$, then $f(x)\leq f(y)+Ld(x,y)$ for every $y\in A$, while $y=x$ gives the reverse inequality after taking the infimum. Thus $F(x)=f(x)$. For arbitrary $x,z\in X$,

$$
f(y)+Ld(x,y)\leq f(y)+Ld(z,y)+Ld(x,z).
$$

Taking infima gives $F(x)\leq F(z)+Ld(x,z)$; interchanging $x,z$ gives

$$
\boxed{|F(x)-F(z)|\leq Ld(x,z).}
$$

This is the [McShane extension theorem](../../../real-analysis.md#mcshane-extension-theorem): **$F$ extends $f$ without increasing its Lipschitz constant.**

<h3 id="12f/b">b</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/b/solution">Solution</h4>

↑ **Parent:** [B](#12f/b)

Two norms $N_1,N_2$ are [equivalent norms](../../../functional-analysis.md#equivalent-norms) when constants $c,C>0$ satisfy

$$
cN_1(v)\leq N_2(v)\leq CN_1(v)
$$

for every $v$.

For $x,y\in\mathbb R^n$, the reverse [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
|g(x)-g(y)|
\leq\left\|\sum_{i=1}^n(x_i-y_i)e_i\right\|
\leq\sum_{i=1}^n|x_i-y_i|\,\|e_i\|
\leq C_0\|x-y\|_2
$$

by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Hence $g$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity), and therefore continuous.

On the compact Euclidean [unit sphere](../../../topology.md#unit-sphere), $g$ is positive and continuous, so the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) gives $0<m\leq g\leq M<\infty$. Homogeneity then yields

$$
m\|x\|_2\leq g(x)\leq M\|x\|_2.
$$

Thus every norm on a [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space) is equivalent to the [Euclidean norm](../../../functional-analysis.md#euclidean-norm); comparing two such bounds proves **any two norms on $V$ are Lipschitz equivalent.**

<h3 id="12f/c">c</h3>

↑ **Parent:** [12F](#12f)

<h4 id="12f/c/solution">Solution</h4>

↑ **Parent:** [C](#12f/c)

Let $P_n$ be the [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space) of real polynomials of degree at most $n$. For fixed $a>0$,

$$
N(p)=\sup_{x\in[0,a]}|p(x)|
$$

is a [norm](../../../functional-analysis.md#norm): if it vanishes, the polynomial vanishes on an interval and hence is the zero polynomial. Also

$$
M(p)=N(p)+\sup_{x\in[0,1]}|p'(x)|
$$

is a norm on $P_n$. By [finite-dimensional equivalence of norms](../../../functional-analysis.md#finite-dimensional-equivalence-of-norms), there is $C>0$, depending only on $n$ and $a$, such that $M(p)\leq C N(p)$. Therefore

$$
\sup_{x\in[0,1]}|p'(x)|\leq C\sup_{x\in[0,a]}|p(x)|.
$$

The [extreme value theorem](../../../real-analysis.md#extreme-value-theorem) supplies $y\in[0,a]$ at which the last supremum is attained, and hence

$$
\boxed{\sup_{x\in[0,1]}|p'(x)|\leq C|p(y)|.}
$$

## 13A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13a/a">a</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/a/solution">Solution</h4>

↑ **Parent:** [A](#13a/a)

On an annulus $r<|z-z_0|<R$, the [Laurent theorem](../../../analysis.md#laurent-theorem) represents an analytic function uniquely as

$$
f(z)=\sum_{n=-\infty}^{\infty}a_n(z-z_0)^n.
$$

For any positively oriented simple closed contour $C$ in the annulus winding once around $z_0$, the coefficients in the [Laurent series](../../../analysis.md#laurent-series) are

$$
\boxed{a_n=\frac1{2\pi i}\oint_C
\frac{f(\zeta)}{(\zeta-z_0)^{n+1}}\,d\zeta.}
$$

The formula follows from the [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) applied term by term, and it is independent of the chosen contour by the [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem).

<h3 id="13a/b">b</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/b/solution">Solution</h4>

↑ **Parent:** [B](#13a/b)

Using the Taylor series of the exponential and series division,

$$
\frac1{e^{2z}-1}
=\frac1{2z}-\frac12+\frac z6-\frac{z^3}{90}+O(z^5).
$$

Thus the first three nonzero Laurent terms are

$$
\boxed{\frac1{2z}-\frac12+\frac z6.}
$$

The singularities occur at $z=k\pi i$. The nearest nonzero ones are $\pm\pi i$, so this [Laurent series](../../../analysis.md#laurent-series) is valid on **$0<|z|<\pi$**.

<h3 id="13a/c">c</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/c/solution">Solution</h4>

↑ **Parent:** [C](#13a/c)

The function $f$ has a [simple pole](../../../isolated-singularity.md#simple-pole) of residue $1/2$ at every $z=k\pi i$, because $(e^{2z}-1)'=2$ there. At $z=0$, the term $1/(2z)$ in $g$ cancels the principal part of $f$. For $1\leq k\leq m$, the summand

$$
\frac z{z^2+\pi^2k^2}
$$

has residue $1/2$ at each of $z=\pm k\pi i$, so it cancels the corresponding pole of $f$. Therefore all possible singularities of $F$ in $|z|<(m+1)\pi$ are [removable singularities](../../../isolated-singularity.md#removable-singularity): they are $0$ and $\pm k\pi i$ for $1\leq k\leq m$. **After filling them in, $F$ is analytic throughout that disc.**

<h3 id="13a/d">d</h3>

↑ **Parent:** [13A](#13a)

<h4 id="13a/d/solution">Solution</h4>

↑ **Parent:** [D](#13a/d)

Write the function from the preceding part as $F_m$. Its expansion at zero is

$$
F_m(z)=-\frac12+z\left(\frac16-
\frac1{\pi^2}\sum_{k=1}^m\frac1{k^2}\right)+O(z^3).
$$

Hence the [residue theorem](../../../analysis.md#residue-theorem) gives

$$
\frac1{2\pi i}\oint_{C_R}\frac{F_m(z)}{z^2}\,dz
=F_m'(0)=\frac16-\frac1{\pi^2}\sum_{k=1}^m\frac1{k^2}.
$$

Choose $R=R_m=(m+\tfrac12)\pi$. This circle stays a distance at least $\pi/2$ from every pole of $f$, so $f$ is bounded uniformly on it. Moreover

$$
\sum_{k=1}^m\left|\frac z{z^2+\pi^2k^2}\right|
\leq\sum_{k=1}^m\frac{R_m}{R_m^2-\pi^2k^2}
=O(\log m).
$$

Thus $\max_{C_{R_m}}|F_m|=O(\log m)$, and the [ML inequality](../../../complex-analysis.md#estimation-lemma) yields

$$
\left|\oint_{C_{R_m}}\frac{F_m(z)}{z^2}\,dz\right|
=O\left(\frac{\log m}{m}\right)\longrightarrow0.
$$

Letting $m\to\infty$ solves the [Basel problem](../../../analytic-number-theory.md#basel-problem):

$$
\boxed{\sum_{k=1}^{\infty}\frac1{k^2}=\frac{\pi^2}{6}.}
$$

## 14G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14g/a">a</h3>

↑ **Parent:** [14G](#14g)

<h4 id="14g/a/solution">Solution</h4>

↑ **Parent:** [A](#14g/a)

The characteristic polynomial of $A$ is

$$
t^2-(\operatorname{tr}A)t+1.
$$

When $|\operatorname{tr}A|>2$, its discriminant is positive, so $A$ has two distinct real [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda,\lambda^{-1}$ and two independent real [eigenvectors](../../../linear-operator-theory.md#eigenvector). Let $P$ have those eigenvectors as columns. Rescaling one column makes $\det P=1$ without changing the diagonalization. Hence $P\in SL_2(\mathbb R)$ and

$$
\boxed{P^{-1}AP=\begin{pmatrix}\lambda&0\\0&\lambda^{-1}\end{pmatrix}.}
$$

This is the normal form of a [hyperbolic element of PSL2(R)](../../../geometry-and-topology.md#hyperbolic-element-of-psl2-r).

<h3 id="14g/b">b</h3>

↑ **Parent:** [14G](#14g)

<h4 id="14g/b/solution">Solution</h4>

↑ **Parent:** [B](#14g/b)

Write $B=\operatorname{diag}(\lambda,\lambda^{-1})$ and $q=\lambda^2>0$, so its [Möbius transformation](../../../group-theory.md#mobius-transformation) is $z\mapsto qz$, with $q\ne1$. For $z=u+iv$, the [Hyperbolic distance in the Poincare half-plane](../../../geometry-and-topology.md#hyperbolic-distance-in-the-poincare-half-plane) satisfies

$$
\cosh\rho(z,qz)
=1+\frac{|z-qz|^2}{2\operatorname{Im}z\operatorname{Im}(qz)}
=1+\frac{(q-1)^2}{2q}
\left(1+\frac{u^2}{v^2}\right).
$$

At $z=i$, the final parenthesis is $1$. Since $\cosh$ is strictly increasing on nonnegative arguments, every $z$ off the imaginary axis has

$$
\boxed{\rho(z,Bz)>\rho(i,Bi).}
$$

<h3 id="14g/c">c</h3>

↑ **Parent:** [14G](#14g)

<h4 id="14g/c/solution">Solution</h4>

↑ **Parent:** [C](#14g/c)

A fixed point of $A$ satisfies

$$
cz^2+(d-a)z-b=0.
$$

Its discriminant is

$$
(d-a)^2+4bc=(a+d)^2-4=(\operatorname{tr}A)^2-4<0,
$$

where $ad-bc=1$ was used. Thus the two roots are nonreal complex conjugates, and exactly one lies in the upper half-plane. Consequently **every [elliptic element of PSL2(R)](../../../geometry-and-topology.md#elliptic-element-of-psl2-r) fixes a point of $\mathbb H$.**

<h3 id="14g/d">d</h3>

↑ **Parent:** [14G](#14g)

<h4 id="14g/d/solution">Solution</h4>

↑ **Parent:** [D](#14g/d)

Take the [parabolic element of PSL2(R)](../../../geometry-and-topology.md#parabolic-element-of-psl2-r)

$$
A=\begin{pmatrix}1&1\\0&1\end{pmatrix},
\qquad z\longmapsto z+1.
$$

It fixes no point in $\mathbb H$. A [Geodesic in the Poincare half-plane model](../../../geometry-and-topology.md#geodesic-in-the-poincare-half-plane-model) is determined by its unordered pair of ideal endpoints: either two real numbers or one real number together with $\infty$. Translation adds one to every finite endpoint, so no such pair is invariant. Therefore **this $A$ preserves neither a point nor a hyperbolic line in $\mathbb H$.**

## 15B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15b/solution">Solution</h3>

↑ **Parent:** [15B](#15b)

For a variation $y+\varepsilon\eta$ with $\eta=\eta'=0$ at both endpoints, the [first variation](../../../calculus-of-variations.md#first-variation) is

$$
\delta I=\int_{x_0}^{x_1}
(f_y\eta+f_{y'}\eta'+f_{y''}\eta'')\,dx.
$$

Two applications of [integration by parts](../../../calculus.md#integration-by-parts) remove derivatives from $\eta$. The boundary terms vanish, and the [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) gives the [higher-order Euler-Lagrange equation](../../../analysis.md#higher-order-euler-lagrange-equation)

$$
\boxed{f_y-\frac d{dx}f_{y'}+\frac{d^2}{dx^2}f_{y''}=0.}
$$

For the stated integrand,

$$
f_y=2y,\qquad f_{y'}=4y'+2y'',\qquad f_{y''}=2(y'+y''),
$$

so the equation reduces to

$$
y^{(4)}-2y''+y=0,
\qquad (D^2-1)^2y=0.
$$

The general solution of this [linear ordinary differential equation](../../../differential-equation.md#linear-ordinary-differential-equation) is

$$
y=(A+Bx)e^x+(C+Dx)e^{-x}.
$$

Decay and finiteness of the integral force $A=B=0$; $y(0)=1$ gives $C=1$, and $y'(0)=2$ gives $D=3$. Hence the unique stationary function is

$$
\boxed{y(x)=(3x+1)e^{-x}.}
$$

## 16A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16a/a">a</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/a/solution">Solution</h4>

↑ **Parent:** [A](#16a/a)

The function is an [even function](../../../calculus.md#even-function), so every sine [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) vanishes. Direct integration gives

$$
a_0=\frac2\pi\int_0^\pi x\,dx=\pi,
\qquad
a_n=\frac2\pi\int_0^\pi x\cos(nx)\,dx
=\frac{2}{\pi n^2}((-1)^n-1).
$$

Thus

$$
\boxed{|x|=\frac\pi2-\frac4\pi
\sum_{k=0}^{\infty}
\frac{\cos((2k+1)x)}{(2k+1)^2}}
$$

for the $2\pi$-periodic extension.

<h3 id="16a/b">b</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/b/solution">Solution</h4>

↑ **Parent:** [B](#16a/b)

The homogeneous solutions $(C_1+C_2x)e^{-x}$ are not $2\pi$-periodic unless $C_1=C_2=0$, so there is a unique periodic solution. For a forcing term $a_n\cos(nx)$, a trial solution $A_n\cos(nx)+B_n\sin(nx)$ gives

$$
A_n=\frac{a_n(1-n^2)}{(1+n^2)^2},
\qquad
B_n=\frac{2na_n}{(1+n^2)^2}.
$$

Using the [Fourier series](../../../fourier-series.md) from part (a), for which only odd $n$ occur and $a_n=-4/(\pi n^2)$, yields

$$
\boxed{
y(x)=\frac\pi2-\frac4\pi
\sum_{\substack{n\geq1\\n\text{ odd}}}
\frac{(1-n^2)\cos(nx)+2n\sin(nx)}{n^2(1+n^2)^2}.}
$$

The coefficients decay fast enough to differentiate the series twice term by term, verifying the equation and periodicity.

## 17B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17b/solution">Solution</h3>

↑ **Parent:** [17B](#17b)

In atomic units the [Time-independent Schrödinger equation](../../../physics.md#time-independent-schrodinger-equation) is

$$
\left(-\frac12\nabla^2-\frac1r\right)\psi=E\psi.
$$

The displayed equation is the [Radial Schrodinger equation for the hydrogen atom](../../../physics.md#radial-schrodinger-equation-for-the-hydrogen-atom). Its radial derivative terms come from the [Laplacian in spherical coordinates](../../../partial-differential-equation.md#laplacian-in-spherical-coordinates), the Coulomb term is the potential $-1/r$, and separation into [spherical harmonics](../../../analysis.md#spherical-harmonic) uses the [orbital angular momentum](../../../quantum-mechanics.md#orbital-angular-momentum) eigenvalue $l(l+1)$, producing the centrifugal term $-l(l+1)R/r^2$.

For $E=-1/(2n^2)$, substitute $R=r^\alpha e^{-r/n}$. Dividing the equation by $R$ and comparing powers of $r$ gives

$$
\alpha(\alpha+1)=l(l+1),
\qquad
\frac{\alpha+1}{n}=1.
$$

The solution regular at the origin has $\alpha=l$, and when $l=n-1$ both equations agree. This is the [circular Coulomb bound state](../../../physics.md#circular-coulomb-bound-state). Thus

$$
\boxed{\alpha=n-1.}
$$

The radial probability measure is $|R(r)|^2r^2\,dr$. With $a=2/n$ and the [Gamma integral](../../../complex-analysis.md#gamma-integral), the [mean radius of a circular Coulomb bound state](../../../physics.md#mean-radius-of-a-circular-coulomb-bound-state) is

$$
\langle r\rangle
=\frac{\int_0^\infty r^{2n+1}e^{-ar}\,dr}
{\int_0^\infty r^{2n}e^{-ar}\,dr}
=\frac{2n+1}{a}
=\boxed{\frac{n(2n+1)}2}.
$$

At fixed [principal quantum number](../../../physics.md#principal-quantum-number) $n$, the allowed [orbital angular momentum](../../../quantum-mechanics.md#orbital-angular-momentum) quantum numbers are $l=0,\ldots,n-1$, and each has [magnetic quantum number](../../../quantum-mechanics.md#magnetic-quantum-number) $m=-l,\ldots,l$. Hence the orbital [quantum degeneracy](../../../quantum-mechanics.md#degenerate-energy-levels) is

$$
\boxed{\sum_{l=0}^{n-1}(2l+1)=n^2.}
$$

Including electron spin would double this to $2n^2$, but spin is absent from the stated wavefunctions.

## 18C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18c/solution">Solution</h3>

↑ **Parent:** [18C](#18c)

Write the jump from side $-$ to side $+$ as $[\mathbf F]=\mathbf F_+-\mathbf F_-$. A thin rectangular loop in the static [Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) and a thin pillbox in [Gauss's law for magnetism](../../../electromagnetism.md#gauss-s-law-for-magnetism) give

$$
\boxed{\mathbf n\mathbin\times[\mathbf E]=0,
\qquad
\mathbf n\mathbin\cdot[\mathbf B]=0.}
$$

Thus the tangential electric field and normal magnetic field are continuous in the plane's rest frame.

For the boost $\mathbf v=v\mathbf n$, the [Lorentz transformation of electromagnetic fields](../../../electromagnetism.md#lorentz-transformation-of-electromagnetic-fields) gives

$$
\mathbf E'_t=\gamma(\mathbf E_t+\mathbf v\mathbin\times\mathbf B),
\qquad
B'_n=B_n.
$$

Therefore

$$
\boxed{[B'_n]=0.}
$$

Moreover $[\mathbf E]$ is purely normal, so $[\mathbf B'_t]=\gamma[\mathbf B_t]$. Consequently the transformed tangential boundary condition is

$$
\boxed{[\mathbf E'_t]=\mathbf v\mathbin\times[\mathbf B'_t].}
$$

Using the [magnetic-field jump across a surface current](../../../electromagnetism.md#magnetic-field-jump-across-a-surface-current), $\mathbf n\times[\mathbf B]=\mu_0\mathbf K$, this can equivalently be written

$$
\boxed{[\mathbf E'_t]=\mu_0\gamma v\mathbf K.}
$$

The nonzero jump is consistent with Faraday's law because the magnetic-field discontinuity itself moves through Albert's frame.

## 19D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="19d/solution">Solution</h3>

↑ **Parent:** [19D](#19d)

This is the [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process) applied degree by degree. Inductively, subtracting projections onto $p_0,\ldots,p_n$ makes $p_{n+1}$ orthogonal to every earlier polynomial. Since every subtracted polynomial has degree at most $n$, the leading coefficient of the monic $q_{n+1}$ remains one, so $p_{n+1}$ is a real [monic orthogonal polynomial](../../../numerical-analysis.md#monic-orthogonal-polynomial) of degree exactly $n+1$.

Now take $q_{n+1}=xp_n$. For $k\leq n-2$, symmetry of the [inner product](../../../linear-algebra.md#inner-product) gives

$$
\langle xp_n,p_k\rangle=\langle p_n,xp_k\rangle=0,
$$

because $xp_k$ has degree at most $n-1$. Only the $p_n$ and $p_{n-1}$ projections remain, yielding the [three-term recurrence for monic orthogonal polynomials](../../../numerical-analysis.md#three-term-recurrence-for-monic-orthogonal-polynomials)

$$
p_{n+1}=(x-\alpha_n)p_n-\beta_np_{n-1},
$$

where

$$
\boxed{\alpha_n=\frac{\langle xp_n,p_n\rangle}{\langle p_n,p_n\rangle},
\qquad
\beta_n=\frac{\langle p_n,p_n\rangle}{\langle p_{n-1},p_{n-1}\rangle}.}
$$

The second identity uses $xp_{n-1}=p_n$ plus lower-degree terms.

For the symmetric Legendre inner product, parity gives $\alpha_n=0$. Starting with $p_0=1$, one obtains $p_1=x$, then

$$
\beta_1=\frac{\int_{-1}^1x^2\,dx}{\int_{-1}^1 1\,dx}=\frac13,
\qquad
\beta_2=\frac{\int_{-1}^1(x^2-1/3)^2\,dx}{\int_{-1}^1x^2\,dx}=\frac4{15}.
$$

Thus the first four monic [Legendre polynomials](../../../differential-equation.md#legendre-polynomial) are

$$
\boxed{p_0=1,\qquad p_1=x,\qquad
p_2=x^2-\frac13,\qquad
p_3=x^3-\frac35x.}
$$

## 20H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="20h/i">i</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/i/solution">Solution</h4>

↑ **Parent:** [I](#20h/i)

For a finite irreducible [Markov chain](../../../markov-process.md#markov-chain) with [invariant distribution](../../../markov-process.md#stationary-distribution) $\pi$, the [mean recurrence time](../../../markov-process.md#mean-recurrence-time) of state $i$ is

$$
\mathbb E_iT_i^+=\frac1{\pi_i}.
$$

The [simple random walk on the hypercube](../../../markov-process.md#simple-random-walk-on-the-hypercube) has the uniform invariant distribution because the [hypercube graph](../../../graph.md#hypercube-graph) is regular, so every vertex has mass $2^{-n}$. Therefore the expected first positive return time to the initial vertex is

$$
\boxed{2^n.}
$$

<h3 id="20h/ii">ii</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#20h/ii)

Let $h$ be the expected [hitting time](../../../markov-process.md#first-passage-time) from any neighbour of the origin back to the origin. After the first step, the return-time calculation from part (i) gives

$$
2^n=1+h,
$$

so $h=2^n-1$. Translation by the target vertex is a [graph automorphism](../../../graph.md#graph-automorphism) of the hypercube that exchanges the origin and that adjacent vertex, so the reverse expected hitting time is the same. Hence

$$
\boxed{\mathbb E_0T_{(0,\ldots,0,1)}=2^n-1.}
$$

<h3 id="20h/iii">iii</h3>

↑ **Parent:** [20H](#20h)

<h4 id="20h/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#20h/iii)

Measure vertices by their [Hamming distance](../../../coding-theory.md#hamming-distance) from the target and let $h_k$ be the expected hitting time when that distance is $k$. We already know $h_1=2^n-1$. From distance one, one of the $n$ coordinate flips reaches the target and the other $n-1$ flips move to distance two. [First-step analysis](../../../analysis.md#first-step-analysis) therefore gives

$$
h_1=1+\frac1n h_0+\frac{n-1}{n}h_2,
\qquad h_0=0.
$$

For $n\geq2$,

$$
\boxed{h_2=\frac{n}{n-1}(h_1-1)
=\frac{n(2^n-2)}{n-1}.}
$$

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
