# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperib_2_2023.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperib_2_2023.pdf)

**Table of contents**

- [1E](#1e)
  - [i](#1e/i)
    - [Solution](#1e/i/solution)
  - [ii](#1e/ii)
    - [Solution](#1e/ii/solution)
  - [Solution](#1e/solution)
- [2G](#2g)
  - [Solution](#2g/solution)
- [3A](#3a)
  - [Solution](#3a/solution)
- [4D](#4d)
  - [Solution](#4d/solution)
- [5C](#5c)
  - [a](#5c/a)
    - [i](#5c/a/i)
      - [Solution](#5c/a/i/solution)
    - [ii](#5c/a/ii)
      - [Solution](#5c/a/ii/solution)
  - [b](#5c/b)
    - [Solution](#5c/b/solution)
- [6H](#6h)
  - [a](#6h/a)
    - [Solution](#6h/a/solution)
  - [b](#6h/b)
    - [Solution](#6h/b/solution)
  - [c](#6h/c)
    - [Solution](#6h/c/solution)
  - [d](#6h/d)
    - [Solution](#6h/d/solution)
- [7H](#7h)
  - [Solution](#7h/solution)
- [8F](#8f)
  - [Solution](#8f/solution)
- [9E](#9e)
  - [a](#9e/a)
    - [Solution](#9e/a/solution)
  - [b](#9e/b)
    - [i](#9e/b/i)
      - [Solution](#9e/b/i/solution)
    - [ii](#9e/b/ii)
      - [Solution](#9e/b/ii/solution)
    - [Solution](#9e/b/solution)
- [10G](#10g)
  - [Solution](#10g/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12B](#12b)
  - [a](#12b/a)
    - [Solution](#12b/a/solution)
  - [b](#12b/b)
    - [i](#12b/b/i)
      - [Solution](#12b/b/i/solution)
    - [ii](#12b/b/ii)
      - [Solution](#12b/b/ii/solution)
    - [iii](#12b/b/iii)
      - [Solution](#12b/b/iii/solution)
- [13C](#13c)
  - [a](#13c/a)
    - [Solution](#13c/a/solution)
  - [b](#13c/b)
    - [i](#13c/b/i)
      - [Solution](#13c/b/i/solution)
    - [ii](#13c/b/ii)
      - [Solution](#13c/b/ii/solution)
    - [iii](#13c/b/iii)
      - [Solution](#13c/b/iii/solution)
    - [iv](#13c/b/iv)
      - [Solution](#13c/b/iv/solution)
    - [v](#13c/b/v)
      - [Solution](#13c/b/v/solution)
- [14A](#14a)
  - [a](#14a/a)
    - [Solution](#14a/a/solution)
    - [i](#14a/a/i)
      - [Solution](#14a/a/i/solution)
    - [ii](#14a/a/ii)
      - [Solution](#14a/a/ii/solution)
    - [iii](#14a/a/iii)
      - [Solution](#14a/a/iii/solution)
  - [b](#14a/b)
    - [i](#14a/b/i)
      - [Solution](#14a/b/i/solution)
    - [ii](#14a/b/ii)
      - [Solution](#14a/b/ii/solution)
- [15D](#15d)
  - [a](#15d/a)
    - [Solution](#15d/a/solution)
  - [b](#15d/b)
    - [i](#15d/b/i)
      - [Solution](#15d/b/i/solution)
    - [ii](#15d/b/ii)
      - [Solution](#15d/b/ii/solution)
- [16D](#16d)
  - [a](#16d/a)
    - [Solution](#16d/a/solution)
  - [b](#16d/b)
    - [Solution](#16d/b/solution)
  - [c](#16d/c)
    - [Solution](#16d/c/solution)
  - [d](#16d/d)
    - [Solution](#16d/d/solution)
  - [e](#16d/e)
    - [Solution](#16d/e/solution)
- [17B](#17b)
  - [a](#17b/a)
    - [Solution](#17b/a/solution)
  - [b](#17b/b)
    - [Solution](#17b/b/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [Solution](#18h/c/solution)
  - [d](#18h/d)
    - [Solution](#18h/d/solution)

## 1E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1e/i">i</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/i/solution">Solution</h4>

↑ **Parent:** [I](#1e/i)

Let $e^2=e$ with $e\ne0,1$. Then $e(1-e)=0$, and the [ideals](../../../commutative-algebra.md#ideal) $eR$ and $(1-e)R$ are nonzero [rings](../../../commutative-algebra.md#ring) with identities $e$ and $1-e$. Define

$$
\Phi:R\longrightarrow eR\times(1-e)R,
\qquad
\Phi(r)=(er,(1-e)r).
$$

This is a [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism). Its inverse is $(x,y)\mapsto x+y$, because $ex=x$, $(1-e)y=y$, and the cross terms vanish. Hence $R\cong eR\times(1-e)R$, proving (ii).

<h3 id="1e/ii">ii</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1e/ii)

Conversely, if $R\cong R_1\times R_2$ with both factors nontrivial, the inverse image of $(1_{R_1},0)$ is an [idempotent](../../../commutative-algebra.md#idempotent). It is neither zero nor one, so (i) holds. This completes the [ring product decomposition by an idempotent](../../../commutative-algebra.md#ring-product-decomposition-by-an-idempotent) equivalence.

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

For

$$
R=\{(a,b)\in\mathbb Z^2:a\equiv b\pmod2\},
$$

the parity condition is preserved by componentwise addition, negation, and multiplication, and $(1,1)$ is the identity. Thus $R$ is a [ring](../../../commutative-algebra.md#ring).

It is not an [integral](../../../calculus.md#integral) domain, since $(2,0)$ and $(0,2)$ are nonzero elements of $R$ whose product is zero. It is also not a product of two nontrivial [rings](../../../commutative-algebra.md#ring). Indeed, an [idempotent](../../../commutative-algebra.md#idempotent) in $\mathbb Z^2$ has each coordinate in $\{0,1\}$, and the parity condition leaves only $(0,0)$ and $(1,1)$. The proved equivalence then excludes a nontrivial product decomposition.

## 2G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2g/solution">Solution</h3>

↑ **Parent:** [2G](#2g)

Suppose first that $X$ is connected and $f:X\to\mathbb Z$ is continuous. Its image is connected by the [continuous image of a connected space](../../../geometry-and-topology.md#continuous-image-of-a-connected-space), but $\mathbb Z$ is discrete, so its only connected nonempty subsets are singletons. Hence $f$ is constant.

Conversely, if $X=U\cup V$ is a disconnection into nonempty disjoint [open sets](../../../topology.md#open-set), the [function](../../../function.md) equal to zero on $U$ and one on $V$ is continuous and nonconstant. This proves the [integer-valued function criterion for connectedness](../../../geometry-and-topology.md#integer-valued-function-criterion-for-connectedness).

Now let $f:X\to\mathbb Z$ be continuous under the hypotheses on the family $\mathcal A$. Each restriction $f|_A$ is constant because $A$ is connected. If $A,B\in\mathcal A$, a point of $A\cap B$ shows that their two constants agree. Since the sets cover $X$, $f$ is constant on $X$, and the criterion proves that $X$ is connected. This is the [pairwise-intersecting connected cover](../../../geometry-and-topology.md#pairwise-intersecting-connected-cover) argument.

Finally, fix $y_0\in Y$. For each $x\in X$, the set

$$
A_x=(X\times\{y_0\})\cup(\{x\}\times Y)
$$

is connected: its two connected pieces meet at $(x,y_0)$. The sets $A_x$ cover $X\times Y$ and any two share $X\times\{y_0\}$. The preceding result proves that $X\times Y$ is connected, giving the [product of connected spaces](../../../geometry-and-topology.md#product-of-connected-spaces) result.

## 3A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3a/solution">Solution</h3>

↑ **Parent:** [3A](#3a)

The [function](../../../function.md) is odd, so only sine coefficients occur. For $n\geq1$,

$$
b_n=\frac2\pi\int_0^\pi(x^3-\pi^2x)\sin(nx)\,dx.
$$

Integration by parts gives

$$
\int_0^\pi x\sin(nx)\,dx=-\frac{\pi(-1)^n}{n},
$$

and

$$
\int_0^\pi x^3\sin(nx)\,dx
=-\frac{\pi^3(-1)^n}{n}+\frac{6\pi(-1)^n}{n^3}.
$$

The terms of order $1/n$ cancel, leaving

$$
b_n=\frac{12(-1)^n}{n^3}.
$$

Thus

$$
x^3-\pi^2x
=12\sum_{n=1}^{\infty}\frac{(-1)^n}{n^3}\sin(nx),
\qquad -\pi<x<\pi.
$$

The [Parseval identity](../../../fourier-analysis.md#parseval-identity) gives

$$
\frac1\pi\int_{-\pi}^{\pi}(x^3-\pi^2x)^2\,dx
=144\sum_{n=1}^{\infty}\frac1{n^6}.
$$

Direct integration yields

$$
\frac1\pi\int_{-\pi}^{\pi}
(x^6-2\pi^2x^4+\pi^4x^2)\,dx
=\frac{16\pi^6}{105}.
$$

Therefore

$$
\boxed{\sum_{n=1}^{\infty}\frac1{n^6}=\frac{\pi^6}{945}},
$$

as recorded in the [Fourier series of x cubed minus pi squared x](../../../fourier-series.md#fourier-series-of-x-cubed-minus-pi-squared-x).

## 4D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4d/solution">Solution</h3>

↑ **Parent:** [4D](#4d)

A capacitor consists of two conductors carrying equal and opposite charges. Its [capacitance](../../../electromagnetism.md#capacitance) is

$$
C=\frac QV,
$$

where $Q$ is the magnitude of the charge on either conductor and $V$ is their potential difference.

For $a<r<b$, a coaxial Gaussian cylinder of length $\ell$ encloses charge $\lambda\ell$. [Gauss's law](../../../electromagnetism.md#gauss-s-law) gives

$$
E(r)=\frac{\lambda}{2\pi\epsilon_0r}\,e_r.
$$

Taking $V$ to mean the inner potential minus the outer potential,

$$
V=\int_a^bE(r)\,dr
=\frac{\lambda}{2\pi\epsilon_0}\log\frac ba.
$$

Since $Q=\lambda L$,

$$
\boxed{C=\frac{2\pi\epsilon_0L}{\log(b/a)}}.
$$

The field energy is

$$
\begin{aligned}
U
&=\frac{\epsilon_0}{2}
\int_a^bE(r)^2(2\pi rL)\,dr\\
&=\frac{\lambda^2L}{4\pi\epsilon_0}\log\frac ba
=\frac12(\lambda L)
\left(\frac{\lambda}{2\pi\epsilon_0}\log\frac ba\right)
=\frac12QV.
\end{aligned}
$$

These are the standard [coaxial cylindrical capacitor](../../../electromagnetism.md#coaxial-cylindrical-capacitor) formulas.

## 5C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5c/a">a</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/a/i">i</h4>

↑ **Parent:** [A](#5c/a)

<h5 id="5c/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5c/a/i)

The divergence is the trace of the velocity-gradient tensor:

$$
\nabla\cdot u=A+E+I.
$$

Thus the flow is incompressible exactly when

$$
\boxed{A+E+I=0}.
$$

The constant [vector](../../../vector-space.md#vector) $U_0$ is unrestricted.

<h4 id="5c/a/ii">ii</h4>

↑ **Parent:** [A](#5c/a)

<h5 id="5c/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5c/a/ii)

The [vorticity](../../../fluid-mechanics.md#vorticity) is

$$
\nabla\times u=(H-F,\ C-G,\ D-B).
$$

Hence the flow is irrotational exactly when

$$
\boxed{H=F,\qquad C=G,\qquad D=B},
$$

equivalently when $\Gamma$ is symmetric. Again, $U_0$ is unrestricted.

<h3 id="5c/b">b</h3>

↑ **Parent:** [5C](#5c)

<h4 id="5c/b/solution">Solution</h4>

↑ **Parent:** [B](#5c/b)

A [streamline](../../../fluid-mechanics.md#streamline) $x(s)=(x(s),y(s),z(s))$ satisfies

$$
\dot x=\alpha y,
\qquad
\dot y=-\alpha x,
\qquad
\dot z=\beta,
$$

with $(x(0),y(0),z(0))=(1,0,0)$. Therefore

$$
\boxed{x(s)=\cos(\alpha s),\qquad
y(s)=-\sin(\alpha s),\qquad
z(s)=\beta s}.
$$

For $\beta\ne0$ this is a helix, with $x=\cos(\alpha z/\beta)$ and $y=-\sin(\alpha z/\beta)$; for $\beta=0$ it is the unit circle in the plane $z=0$.

## 6H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6h/a">a</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/a/solution">Solution</h4>

↑ **Parent:** [A](#6h/a)

Apart from constants, the log-likelihood is

$$
\ell(\theta)=-\frac1{2\sigma^2}\sum_{i=1}^n(X_i-\theta)^2.
$$

Differentiating gives $\ell'(\theta)=n(\overline X-\theta)/\sigma^2$, so

$$
\boxed{\widehat\theta_{\mathrm{MLE}}=\overline X}.
$$

<h3 id="6h/b">b</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/b/solution">Solution</h4>

↑ **Parent:** [B](#6h/b)

Since

$$
\overline X\sim N\left(\theta,\frac{\sigma^2}{n}\right),
$$

an exact 95 percent confidence interval is

$$
\boxed{
\overline X\mathbin{\pm}z_{0.975}\frac{\sigma}{\sqrt n}
},
\qquad z_{0.975}\simeq1.96.
$$

<h3 id="6h/c">c</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/c/solution">Solution</h4>

↑ **Parent:** [C](#6h/c)

Write the posterior mean and variance as

$$
m_n=\frac{n\overline X/\sigma^2+\mu/\nu^2}
{n/\sigma^2+1/\nu^2},
\qquad
v_n=\left(\frac n{\sigma^2}+\frac1{\nu^2}\right)^{-1}.
$$

The central 95 percent posterior credible interval is

$$
\boxed{m_n\mathbin{\pm}z_{0.975}\sqrt{v_n}}.
$$

<h3 id="6h/d">d</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/d/solution">Solution</h4>

↑ **Parent:** [D](#6h/d)

As $n\to\infty$,

$$
m_n-\overline X
=\frac{\sigma^2(\mu-\overline X)}{n\nu^2+\sigma^2}
=O_p(n^{-1}),
$$

while

$$
\sqrt{v_n}
=\frac{\sigma}{\sqrt n}
\left(1+\frac{\sigma^2}{n\nu^2}\right)^{-1/2}
\sim\frac{\sigma}{\sqrt n}.
$$

Thus the credible interval and confidence interval have asymptotically equal centres and half-widths, and both contract around the true parameter. Their interpretations remain different: the confidence statement concerns repeated samples, whereas the credible statement concerns posterior probability. This is [normal-normal conjugacy with known observation variance](../../../probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance).

## 7H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7h/solution">Solution</h3>

↑ **Parent:** [7H](#7h)

Use

$$
L(x,y,z,\lambda)
=x^2+y^4+z^6-\lambda(x+2y+3z-6).
$$

Stationarity gives

$$
2x=\lambda,
\qquad
4y^3=2\lambda,
\qquad
6z^5=3\lambda.
$$

Putting $t=\lambda/2$, this becomes

$$
x=t,\qquad y=t^{1/3},\qquad z=t^{1/5},
$$

and the constraint requires

$$
t+2t^{1/3}+3t^{1/5}=6.
$$

The left side is strictly increasing, and $t=1$ solves the equation. Hence

$$
\boxed{(x,y,z)=(1,1,1)},
\qquad
\boxed{f_{\min}=3},
\qquad
\lambda=2.
$$

The objective is convex and the constraint is affine. Its tangent-plane inequality at $(1,1,1)$ gives, for every feasible $(x,y,z)$,

$$
f(x,y,z)\geq3+(2,4,6)\cdot(x-1,y-1,z-1)=3,
$$

so the Lagrange point is globally optimal. Moreover, at the dual value $\lambda=2$, the infimum of the [Lagrangian function in constrained optimization](../../../calculus-of-variations.md#lagrangian-function-in-constrained-optimization) is attained at the same point and equals three. The primal and dual values coincide, so strong duality holds.

For the value [function](../../../function.md), the multiplier convention above gives the [derivative of a constrained value function](../../../mathematical-optimization.md#derivative-of-a-constrained-value-function)

$$
\phi'(b)=\lambda(b).
$$

At $b=6$, therefore,

$$
\boxed{\phi'(6)=2}.
$$

## 8F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8f/solution">Solution</h3>

↑ **Parent:** [8F](#8f)

For an $n\times n$ [matrix](../../../vector-space.md#matrix) $A$, the characteristic [polynomial](../../../polynomial.md) is

$$
\chi_A(t)=\det(tI-A).
$$

The [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) states that $\chi_A(A)=0$.

Over $\mathbb C$, choose a [basis](../../../vector-space.md#basis) in which $A$ is upper triangular, with diagonal entries $\lambda_1,\ldots,\lambda_n$. For the standard invariant flag $V_j=\langle e_1,\ldots,e_j\rangle$,

$$
(A-\lambda_jI)V_j\subseteq V_{j-1}.
$$

The factors $A-\lambda_jI$ commute, so applying their product in descending order sends $V_n$ successively into $V_{n-1},\ldots,V_0=0$. Hence

$$
0=\prod_{j=1}^n(A-\lambda_jI)=\chi_A(A),
$$

which proves the theorem.

Direct expansion gives the commutator product rule:

$$
\begin{aligned}
[X,YZ]
&=XYZ-YZX\\
&=(XY-YX)Z+Y(XZ-ZX)\\
&=[X,Y]Z+Y[X,Z].
\end{aligned}
$$

Put $C=[B,A]$. Since $C$ commutes with $A$, repeated use of the product rule gives

$$
[B,A^r]=\sum_{j=0}^{r-1}A^jCA^{r-1-j}=rA^{r-1}C.
$$

By [linearity](../../../vector-space.md#linearity), for every [polynomial](../../../polynomial.md) $\varphi$,

$$
[B,\varphi(A)]=\varphi'(A)C.
$$

Let $D(X)=[B,X]$ and suppose $f(A)=0$. For $k=1$,

$$
f'(A)C=D(f(A))=0.
$$

Assume inductively that

$$
uC^m=0,
\qquad
u=f^{(k)}(A),\quad m=2^k-1.
$$

Both $u$ and $C$ are [polynomials](../../../polynomial.md) in, or commute with, $A$, so $uC^m=C^mu=0$. Apply the derivation $D$ to $uC^m=0$ and multiply on the left by $C^m$:

$$
0=C^mD(u)C^m+C^muD(C^m)=C^mD(u)C^m.
$$

Since $D(u)=f^{(k+1)}(A)C$, this says

$$
f^{(k+1)}(A)C^{2m+1}
=f^{(k+1)}(A)C^{2^{k+1}-1}=0.
$$

The induction is complete. Taking $f=\chi_A$ and $k=n$ gives

$$
n!\,C^{2^n-1}=0.
$$

**Thus $[B,A]$ is nilpotent, which is the [Jacobson lemma for a commuting commutator](../../../linear-operator-theory.md#jacobson-lemma-for-a-commuting-commutator).**

## 9E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9e/a">a</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/a/solution">Solution</h4>

↑ **Parent:** [A](#9e/a)

Let $Q$ act by left multiplication on the set $G/P$ of left cosets. Every orbit has size a power of $p$, while

$$
|G/P|
$$

is not divisible by $p$. Therefore at least one orbit has size one. If $gP$ is fixed, then $qgP=gP$ for every $q\in Q$, so $g^{-1}Qg\leq P$, equivalently

$$
Q\leq gPg^{-1}.
$$

This is [Sylow containment from a coset fixed point](../../../finite-group-theory.md#sylow-containment-from-a-coset-fixed-point).

The remaining [Sylow theorems](../../../finite-group-theory.md#sylow-theorems) state that Sylow $p$-subgroups exist, that any two are conjugate, and that their number $n_p$ satisfies

$$
\boxed{n_p\equiv1\pmod p,
\qquad
n_p\mid |G|/|P|.}
$$

<h3 id="9e/b">b</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/b/i">i</h4>

↑ **Parent:** [B](#9e/b)

<h5 id="9e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#9e/b/i)

By transitivity and the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem),

$$
|G|=7|G_x|=7\cdot24=168=2^3\cdot3\cdot7.
$$

Inside $G_x\cong S_4$, there are three Sylow $2$-subgroups, each of order eight, and four Sylow $3$-subgroups, each of order three. These are also Sylow [subgroups](../../../group.md#subgroup) of $G$.

<h4 id="9e/b/ii">ii</h4>

↑ **Parent:** [B](#9e/b)

<h5 id="9e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9e/b/ii)

Count pairs $(x,P)$ where $P$ is a Sylow $2$-subgroup fixing $x$. Each of the seven point stabilizers contains three such [subgroups](../../../group.md#subgroup), giving 21 pairs. Conversely, a $2$-group acting on seven points has a fixed point, and a Sylow $2$-subgroup cannot fix two points because a two-point stabilizer has order four. Hence every Sylow $2$-subgroup occurs in exactly one pair, so

$$
n_2=21.
$$

Similarly, each point stabilizer contains four Sylow $3$-subgroups, giving 28 pairs. A [group](../../../group.md) of order three acting on seven points has a fixed point, and it cannot fix two because a two-point stabilizer is a $2$-group. Thus

$$
n_3=28.
$$

The Sylow congruence and divisibility conditions give $n_7\in\{1,8\}$. Regard the faithful action as an embedding $G\leq S_7$. If $n_7=1$, its Sylow $7$-subgroup $P$ is normal, so $G\leq N_{S_7}(P)$. The stated fact gives $|N_{S_7}(P)|=7\cdot6=42$, impossible for a [subgroup](../../../group.md#subgroup) $G$ of order 168. Hence

$$
n_7=8.
$$

These are the [Sylow counts in a faithful degree-seven action with S4 point stabilizers](../../../finite-group-theory.md#sylow-counts-in-a-faithful-degree-seven-action-with-s4-point-stabilizers).

<h4 id="9e/b/solution">Solution</h4>

↑ **Parent:** [B](#9e/b)

Let $N\mathrel{\trianglelefteq}G$ be proper. If $7$ divides $|N|$, then $N$ contains a Sylow $7$-subgroup of $G$, and normality makes it contain all eight of them. Thus $n_7(N)=8$, so the Sylow divisibility theorem gives

$$
56=7\cdot8\mid |N|.
$$

Since $|N|$ divides 168 and $N$ is proper, this forces $|N|=56$.

Every nontrivial normal [subgroup](../../../group.md#subgroup) is transitive by [normal subgroup orbits in a faithful prime-degree action](../../../group-theory.md#normal-subgroup-orbits-in-a-faithful-prime-degree-action). Hence

$$
|N\cap G_x|=|N_x|=56/7=8.
$$

But $N\cap G_x$ is normal in $G_x\cong S_4$, whereas $S_4$ has three, rather than one, Sylow $2$-subgroups. This contradiction proves that no proper normal [subgroup](../../../group.md#subgroup) has order divisible by seven.

If instead $3$ divides $|N|$, normality makes $N$ contain all 28 Sylow $3$-subgroups of $G$. Hence $n_3(N)=28$, so $28$ divides $|N|/3$ and therefore $84$ divides $|N|$. A proper such [subgroup](../../../group.md#subgroup) would have order 84, which is divisible by seven and has just been ruled out.

Finally, if $N$ is any nontrivial normal [subgroup](../../../group.md#subgroup), the prime-degree orbit argument makes $N$ transitive, so seven divides $|N|$. This is impossible for a proper normal [subgroup](../../../group.md#subgroup). Therefore $G$ is simple.

## 10G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10g/solution">Solution</h3>

↑ **Parent:** [10G](#10g)

A [sequence](../../../real-analysis.md#sequence) $f_n:S\to\mathbb R$ converges uniformly to $f$ if, for every $\varepsilon>0$, there is $N$ such that

$$
|f_n(x)-f(x)|<\varepsilon
$$

for every $x\in S$ and every $n\geq N$. A map $h:M\to N$ is uniformly continuous if, for every $\varepsilon>0$, there is $\delta>0$ such that

$$
d_M(x,y)<\delta\quad\Longrightarrow\quad d_N(h(x),h(y))<\varepsilon
$$

for all $x,y\in M$.

If $f\in C_0(\mathbb R^d)$, choose a ball outside which $|f|<1$. On the closed ball, continuity gives boundedness, so $f$ is bounded everywhere.

Now let $(f_n)$ be Cauchy in the uniform metric. For each $x$, $(f_n(x))$ is Cauchy in $\mathbb R$; let its [limit](../../../calculus.md#limit-of-a-function) be $f(x)$. Passing to the pointwise [limit](../../../calculus.md#limit-of-a-function) in the uniform Cauchy estimate shows that $f_n\to f$ uniformly. Hence $f$ is continuous. Given $\varepsilon>0$, choose $n$ with $\|f-f_n\|_\infty<\varepsilon/2$, and then choose $K$ so that $|f_n(x)|<\varepsilon/2$ for $\|x\|>K$. It follows that $f$ also vanishes at infinity. Thus $C_0(\mathbb R^d)$ is complete, as in [completeness of continuous functions vanishing at infinity](../../../functional-analysis.md#completeness-of-continuous-functions-vanishing-at-infinity).

Every $f\in C_0(\mathbb R^d)$ is uniformly continuous. Given $\varepsilon>0$, choose $R$ so that $|f(x)|<\varepsilon/2$ outside the ball of radius $R$. On the compact ball of radius $R+1$, $f$ is uniformly continuous; choose the corresponding $\delta\leq1$. If two points at distance below $\delta$ are not both in that ball, then both lie outside the ball of radius $R$, and their [function](../../../function.md) values differ by less than $\varepsilon$.

For the final [sequence](../../../real-analysis.md#sequence), continuity of $\varepsilon$ at zero gives, for each fixed $x$,

$$
f_n(x)=\sqrt{x^2+\varepsilon(x/n)}\longrightarrow|x|.
$$

Thus [pointwise convergence](../../../real-analysis.md#pointwise-convergence) is compulsory. [Uniform convergence](../../../real-analysis.md#uniform-convergence) need not hold: with $\varepsilon(t)=t^2$,

$$
f_n(x)-|x|
=|x|\left(\sqrt{1+n^{-2}}-1\right),
$$

which is unbounded as a [function](../../../function.md) of $x$ for every fixed $n$.

Under the additional bound $\varepsilon(t)\leq M|t|$, however,

$$
0\leq f_n(x)-|x|
=\frac{\varepsilon(x/n)}{\sqrt{x^2+\varepsilon(x/n)}+|x|}
\leq\frac Mn
$$

for $x\ne0$, and the difference is zero at $x=0$. Hence convergence is uniform, by the [uniform square-root perturbation under linear growth](../../../functional-analysis.md#uniform-square-root-perturbation-under-linear-growth) estimate. The pointwise answer remains yes.

## 11F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

The [tangent vectors](../../../differential-geometry.md#tangent-vector) of

$$
\sigma(u,v)=(u,v,f(u,v))
$$

are

$$
\sigma_u=(1,0,f_u),
\qquad
\sigma_v=(0,1,f_v).
$$

Hence the [first fundamental form](../../../differential-geometry.md#first-fundamental-form) has coefficients

$$
E=1+f_u^2,
\qquad
F=f_uf_v,
\qquad
G=1+f_v^2.
$$

Put

$$
W=\sqrt{1+f_u^2+f_v^2}.
$$

The upward [unit normal](../../../differential-geometry.md#unit-normal) is $N=(-f_u,-f_v,1)/W$, so the [second fundamental form](../../../second-fundamental-form.md) has coefficients

$$
e=\frac{f_{uu}}W,
\qquad
f_{II}=\frac{f_{uv}}W,
\qquad
g=\frac{f_{vv}}W.
$$

Thus the two forms are

$$
I=E\,du^2+2F\,du\,dv+G\,dv^2,
\qquad
II=e\,du^2+2f_{II}\,du\,dv+g\,dv^2.
$$

The [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) is

$$
K=\frac{eg-f_{II}^2}{EG-F^2}.
$$

Since $EG-F^2=W^2$, the graph formula is

$$
\boxed{
K=\frac{f_{uu}f_{vv}-f_{uv}^2}
{(1+f_u^2+f_v^2)^2}
},
$$

as in [Gaussian curvature of a graph surface](../../../second-fundamental-form.md#gaussian-curvature-of-a-graph-surface).

For the final claim, fix a point of $\gamma$ and make a [rigid motion](../../../geometry-and-topology.md#rigid-transformation) taking $P$ to the plane $z=0$. The common tangent plane is horizontal, so locally $\Sigma$ is the graph $z=f(u,v)$. Along the projected curve $c(s)$ of tangency,

$$
f(c(s))=0,
\qquad
\nabla f(c(s))=0.
$$

Differentiating the second identity gives

$$
\operatorname{Hess}f(c(s))\,c'(s)=0.
$$

Because $c$ is a [smooth curve](../../../differential-geometry.md#smooth-curve), $c'(s)\ne0$, so the Hessian is singular. Its [determinant](../../../linear-algebra.md#determinant) is zero, and the graph formula gives $K=0$ at every point of $\gamma$. This is [tangency to a plane along a curve forces zero Gaussian curvature](../../../second-fundamental-form.md#tangency-to-a-plane-along-a-curve-forces-zero-gaussian-curvature).

## 12B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12b/a">a</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/a/solution">Solution</h4>

↑ **Parent:** [A](#12b/a)

Let $|f(z)|\leq K$ on $\operatorname{Re}z>0$. If $\operatorname{Re}z>c$, the circle $|w-z|=c$ lies in that half-plane. The [Cauchy derivative formula](../../../complex-analysis.md#cauchy-derivative-formula) gives

$$
|f'(z)|\leq\frac Kc.
$$

The [line segment](../../../mathematical-optimization.md#line-segment) joining $z_1$ to $z_2$ remains in $\operatorname{Re}z>c$, so

$$
|f(z_1)-f(z_2)|
\leq\frac Kc|z_1-z_2|.
$$

**Thus one may take $M=K/c$, as in the [lipschitz bound inside a bounded analytic half-plane](../../../complex-analysis.md#lipschitz-bound-inside-a-bounded-analytic-half-plane).**

<h3 id="12b/b">b</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/b/i">i</h4>

↑ **Parent:** [B](#12b/b)

<h5 id="12b/b/i/solution">Solution</h5>

↑ **Parent:** [I](#12b/b/i)

The [Liouville theorem](../../../complex-analysis.md#liouville-theorem) states that every bounded [entire function](../../../complex-analysis.md#entire-function) is constant.

<h4 id="12b/b/ii">ii</h4>

↑ **Parent:** [B](#12b/b)

<h5 id="12b/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12b/b/ii)

Suppose $g(\mathbb C)$ is not dense. Then some [open disc](../../../topology.md#open-disc) $D(w,r)$ is disjoint from the image, so

$$
F(z)=\frac1{g(z)-w}
$$

is entire and satisfies $|F(z)|\leq1/r$. Liouville's theorem makes $F$, and hence $g$, constant, a contradiction. Therefore every nonconstant entire $g$ has dense image, as asserted by [dense image of a nonconstant entire function](../../../complex-analysis.md#dense-image-of-a-nonconstant-entire-function).

<h4 id="12b/b/iii">iii</h4>

↑ **Parent:** [B](#12b/b)

<h5 id="12b/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#12b/b/iii)

Write $h(z)=\sum_{n=0}^{\infty}a_nz^n$. Cauchy's coefficient formula on $|z|=R$ gives

$$
a_n=\frac1{2\pi R^n}
\int_0^{2\pi}h(Re^{i\theta})e^{-in\theta}\,d\theta.
$$

Except at the two measure-zero points where $\cos\theta=0$, the hypothesis gives

$$
|h(Re^{i\theta})|
\leq R^{-1/2}|\cos\theta|^{-1/2}.
$$

Since $|\cos\theta|^{-1/2}$ is integrable,

$$
|a_n|
\leq C R^{-n-1/2}
$$

for a constant $C$ independent of $R$. Letting $R\to\infty$ shows that every $a_n=0$. Hence $h\equiv0$, in particular $h$ is constant. This proves the [entire function under a horizontal inverse-square-root bound](../../../complex-analysis.md#entire-function-under-a-horizontal-inverse-square-root-bound) result.

## 13C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13c/a">a</h3>

↑ **Parent:** [13C](#13c)

<h4 id="13c/a/solution">Solution</h4>

↑ **Parent:** [A](#13c/a)

Take a [variation](../../../calculus-of-variations.md#variation) $y+\varepsilon\eta$, where the [differentiable function](../../../analysis.md#differentiable-function) $\eta$ obeys

$$
\eta(a)=\eta(b)=\eta'(a)=\eta'(b)=0
$$

because both $y$ and its first [derivative](../../../calculus.md#derivative) have fixed endpoint values. The [first variation](../../../calculus-of-variations.md#first-variation) of the [functional](../../../calculus-of-variations.md#functional) is

$$
\delta L
=\int_a^b
\left(F_y\eta+F_{y'}\eta'+F_{y''}\eta''\right)\,dx.
$$

Applying [integration by parts](../../../calculus.md#integration-by-parts) once to the second term and twice to the third gives

$$
\begin{aligned}
\delta L
={}&\int_a^b
\left[
F_y-\frac d{dx}F_{y'}
+\frac{d^2}{dx^2}F_{y''}
\right]\eta\,dx\\
&+\left[
F_{y'}\eta+F_{y''}\eta'
-\frac d{dx}(F_{y''})\eta
\right]_a^b.
\end{aligned}
$$

The endpoint conditions on $\eta$ and $\eta'$ make every boundary term zero. Since the remaining [integral](../../../calculus.md#integral) vanishes for every admissible variation, the [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) yields the [higher-order Euler-Lagrange equation](../../../analysis.md#higher-order-euler-lagrange-equation)

$$
\boxed{
F_y-\frac d{dx}F_{y'}
+\frac{d^2}{dx^2}F_{y''}=0
}.
$$

<h3 id="13c/b">b</h3>

↑ **Parent:** [13C](#13c)

<h4 id="13c/b/i">i</h4>

↑ **Parent:** [B](#13c/b)

<h5 id="13c/b/i/solution">Solution</h5>

↑ **Parent:** [I](#13c/b/i)

Here

$$
F(x,y,y',y'')=\frac A2(y'')^2+\rho gy.
$$

Substitution into the [higher-order Euler-Lagrange equation](../../../analysis.md#higher-order-euler-lagrange-equation) gives the fourth-order [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation)

$$
\boxed{Ay''''+\rho g=0}.
$$

<h4 id="13c/b/ii">ii</h4>

↑ **Parent:** [B](#13c/b)

<h5 id="13c/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#13c/b/ii)

Integrating the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) four times gives a quartic [polynomial](../../../polynomial.md). It is useful to use the [linearity](../../../vector-space.md#linearity) of the equation and split the solution into a gravity part and a force part:

$$
y=y_0+y_F,
$$

where

$$
y_0(x)
=-\frac{\rho g}{24A}x^2(6L^2-4Lx+x^2)
$$

satisfies the clamped and torque-free [boundary conditions](../../../differential-equation.md#boundary-condition) with $F=0$, while

$$
y_F(x)=\frac{F}{6A}x^2(3L-x)
$$

satisfies the homogeneous equation and contributes the endpoint [force](../../../classical-mechanics.md#force). Direct [differentiation](../../../calculus.md#differentiation) verifies

$$
y(0)=y'(0)=0,\qquad y''(L)=0,\qquad -Ay'''(L)=F.
$$

Thus

$$
\boxed{
y(x)=-\frac{\rho g}{24A}x^2(6L^2-4Lx+x^2)
+\frac{F}{6A}x^2(3L-x)
},
$$

the [clamped-free beam under uniform load and endpoint force](../../../analysis.md#clamped-free-beam-under-uniform-load-and-endpoint-force).

<h4 id="13c/b/iii">iii</h4>

↑ **Parent:** [B](#13c/b)

<h5 id="13c/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#13c/b/iii)

Evaluating the [function](../../../function.md) at the endpoint gives the [displacement](../../../classical-mechanics.md#displacement)

$$
\Delta=y(L)
=-\frac{\rho gL^4}{8A}+\frac{FL^3}{3A}.
$$

Therefore

$$
\boxed{h_0=-\frac{\rho gL^4}{8A}},
\qquad
\boxed{h=\frac{FL^3}{3A}},
\qquad
\boxed{\Delta=h_0+h}.
$$

The force-induced displacement $h$ is a [linear map](../../../vector-space.md#linear-map) of $F$.

<h4 id="13c/b/iv">iv</h4>

↑ **Parent:** [B](#13c/b)

<h5 id="13c/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#13c/b/iv)

Substitute $y=y_0+y_F$ into the energy [functional](../../../calculus-of-variations.md#functional) and integrate the resulting [polynomial](../../../polynomial.md):

$$
\begin{aligned}
E
&=\int_0^L
\left[\frac A2(y'')^2+\rho gy\right]\,dx\\
&=-\frac{\rho^2g^2L^5}{40A}
+\frac{F^2L^3}{6A}.
\end{aligned}
$$

The term linear in $F$ cancels. Hence

$$
\boxed{E_0=-\frac{\rho^2g^2L^5}{40A}},
\qquad
\boxed{\mathcal E=\frac{F^2L^3}{6A}},
\qquad
\boxed{E=E_0+\mathcal E}.
$$

As required, $E_0$ is independent of the [force](../../../classical-mechanics.md#force) and $\mathcal E$ is a [quadratic function](../../../polynomial.md#quadratic-function) of it.

<h4 id="13c/b/v">v</h4>

↑ **Parent:** [B](#13c/b)

<h5 id="13c/b/v/solution">Solution</h5>

↑ **Parent:** [V](#13c/b/v)

Taking the [derivative](../../../calculus.md#derivative) of the force-dependent energy gives

$$
\boxed{
\frac{d\mathcal E}{dF}
=\frac{FL^3}{3A}
=h
}.
$$

**Thus the [derivative](../../../calculus.md#derivative) of the additional minimized internal energy with respect to the applied [force](../../../classical-mechanics.md#force) equals the resulting endpoint [displacement](../../../classical-mechanics.md#displacement). This is the [endpoint force derivative of clamped-free beam energy](../../../analysis.md#endpoint-force-derivative-of-clamped-free-beam-energy).**

## 14A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14a/a">a</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/a/solution">Solution</h4>

↑ **Parent:** [A](#14a/a)

Apply [separation of variables](../../../partial-differential-equation.md#separation-of-variables) to the [Laplace equation in polar coordinates](../../../partial-differential-equation.md#laplace-equation-in-polar-coordinates) by writing $\phi(r,\theta)=R(r)\Theta(\theta)$. Division by $R\Theta$ gives

$$
\frac{r(rR')'}R=-\frac{\Theta''}{\Theta}=n^2.
$$

The requirement that $\Theta$ be a real $2\pi$-[periodic function](../../../function.md#periodic-function) restricts the separation constants to $n^2$, with angular factors $\cos(n\theta)$ and $\sin(n\theta)$. For $n\geq1$, the radial [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) is an Euler equation with solutions $r^n$ and $r^{-n}$. For the zero mode, $\Theta$ is constant and

$$
(rR')'=0,
$$

so $R=a_0+c_0\log r$. By [linearity](../../../vector-space.md#linearity), superposition gives

$$
\boxed{
\begin{aligned}
\phi(r,\theta)
={}&a_0+c_0\log r\\
&+\sum_{n=1}^{\infty}(a_nr^n+c_nr^{-n})\cos(n\theta)\\
&+\sum_{n=1}^{\infty}(b_nr^n+d_nr^{-n})\sin(n\theta).
\end{aligned}
}
$$

This is the separated expansion of a [harmonic function](../../../partial-differential-equation.md#harmonic-function) in a circular region.

<h4 id="14a/a/i">i</h4>

↑ **Parent:** [A](#14a/a)

<h5 id="14a/a/i/solution">Solution</h5>

↑ **Parent:** [I](#14a/a/i)

Regularity at the origin excludes the [natural logarithm](../../../calculus.md#natural-logarithm) and every negative radial power. Thus

$$
\boxed{c_0=0,\qquad c_n=d_n=0\quad(n\geq1)}.
$$

The coefficients $a_0,a_n,b_n$ remain arbitrary.

<h4 id="14a/a/ii">ii</h4>

↑ **Parent:** [A](#14a/a)

<h5 id="14a/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#14a/a/ii)

Regularity at infinity excludes the [natural logarithm](../../../calculus.md#natural-logarithm) and every positive radial power. Thus

$$
\boxed{c_0=0,\qquad a_n=b_n=0\quad(n\geq1)}.
$$

The constant $a_0$ and the decaying coefficients $c_n,d_n$ remain arbitrary.

<h4 id="14a/a/iii">iii</h4>

↑ **Parent:** [A](#14a/a)

<h5 id="14a/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#14a/a/iii)

An [annulus](../../../topology.md#annulus-mathematics) stays away from both the origin and infinity, so every displayed radial mode is regular there. Therefore none of the coefficients is forced to vanish.

<h3 id="14a/b">b</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/b/i">i</h4>

↑ **Parent:** [B](#14a/b)

<h5 id="14a/b/i/solution">Solution</h5>

↑ **Parent:** [I](#14a/b/i)

Write $s=\log r$, so the two circular boundaries are $s=0$ and $s=2$. The zero angular mode must interpolate between $-1$ and $1$, giving $s-1=\log r-1$.

For the $n$th cosine mode, the radial factor has equal value $A_n$ at both boundaries. The unique [harmonic function](../../../partial-differential-equation.md#harmonic-function) with those data is

$$
A_n\frac{\cosh(n(s-1))}{\cosh n}\cos(n\theta).
$$

Hence the solution of the annular [Dirichlet problem](../../../analysis.md#dirichlet-problem) is

$$
\boxed{
\phi(r,\theta)
=\log r-1
+\sum_{n=1}^{\infty}
A_n\frac{\cosh(n(\log r-1))}{\cosh n}\cos(n\theta)
}.
$$

At $r=1$ and $r=e^2$, the [hyperbolic cosine](../../../calculus.md#hyperbolic-cosine) quotient equals one, so the [boundary conditions](../../../differential-equation.md#boundary-condition) are satisfied term by term.

<h4 id="14a/b/ii">ii</h4>

↑ **Parent:** [B](#14a/b)

<h5 id="14a/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#14a/b/ii)

The mean of $f$ is zero. Its [Fourier cosine series](../../../fourier-series.md#fourier-cosine-series) coefficients are

$$
\begin{aligned}
A_n
&=\frac1\pi\left[
\int_0^\pi\left(\frac\pi2-\theta\right)\cos(n\theta)\,d\theta
+\int_\pi^{2\pi}\left(\theta-\frac{3\pi}2\right)\cos(n\theta)\,d\theta
\right]\\
&=\frac{2(1-(-1)^n)}{\pi n^2}.
\end{aligned}
$$

Thus $A_n=0$ for [even](../../../calculus.md#even-function) $n$ and $A_n=4/(\pi n^2)$ for [odd](../../../calculus.md#odd-function) $n$. Substitution into part (i) yields

$$
\boxed{
\phi(r,\theta)
=\log r-1
+\frac4\pi
\sum_{\substack{n\geq1\\ n\ {\rm odd}}}
\frac{\cosh(n(\log r-1))}{n^2\cosh n}\cos(n\theta)
}.
$$

## 15D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15d/a">a</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/a/solution">Solution</h4>

↑ **Parent:** [A](#15d/a)

The [Schrödinger equation](../../../physics.md#schrodinger-equation) and its complex conjugate are

$$
i\hbar\frac{\partial\psi}{\partial t}
=-\frac{\hbar^2}{2m}\nabla^2\psi+U\psi,
\qquad
-i\hbar\frac{\partial\psi^*}{\partial t}
=-\frac{\hbar^2}{2m}\nabla^2\psi^*+U\psi^*.
$$

Because the potential $U$ is real, its two contributions cancel when differentiating the [probability density](../../../quantum-mechanics.md#probability-density) $\rho=\psi^*\psi$. Therefore

$$
\begin{aligned}
\frac{\partial\rho}{\partial t}
&=\psi^*\frac{\partial\psi}{\partial t}
+\psi\frac{\partial\psi^*}{\partial t}\\
&=\frac{i\hbar}{2m}
\left(\psi^*\nabla^2\psi-\psi\nabla^2\psi^*\right)\\
&=-\nabla\cdot
\left[
-\frac{i\hbar}{2m}
\left(\psi^*\nabla\psi-\psi\nabla\psi^*\right)
\right].
\end{aligned}
$$

The expression in square brackets is the [probability current](../../../quantum-mechanics.md#probability-current) $J$, so

$$
\boxed{\frac{\partial\rho}{\partial t}+\nabla\cdot J=0}.
$$

This [probability continuity equation](../../../quantum-mechanics.md#probability-continuity-equation) says that probability can leave a region only through the current across its boundary.

<h3 id="15d/b">b</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/b/i">i</h4>

↑ **Parent:** [B](#15d/b)

<h5 id="15d/b/i/solution">Solution</h5>

↑ **Parent:** [I](#15d/b/i)

Write the spatial factors of the stationary [wavefunction](../../../quantum-mechanics.md#wave-function) as

$$
\psi(x,t)=e^{-iEt/\hbar}
\begin{cases}
e^{ikx}+R e^{-ikx},&x<-a,\\
C e^{kx}+D e^{-kx},&-a<x<a,\\
T e^{ikx},&x>a,
\end{cases}
$$

where

$$
k=\frac{\sqrt{2mE}}{\hbar}.
$$

Since $U_0-E=E$, the decay constant inside the [potential barrier](../../../quantum-mechanics.md#potential-barrier) is also $k$. Continuity of the [wavefunction](../../../quantum-mechanics.md#wave-function) and its first [derivative](../../../calculus.md#derivative) at $x=-a$ and $x=a$ gives four linear equations. Solving them yields

$$
T=\frac{e^{-2ika}}{\cosh(2ka)}.
$$

Consequently the transmitted wave is

$$
\boxed{
\psi_{\rm tr}(x,t)
=\frac{\exp\!\left(i[k(x-2a)-Et/\hbar]\right)}
{\cosh(2ka)}
},
\qquad x>a,
$$

and its [probability density](../../../quantum-mechanics.md#probability-density) is

$$
\boxed{
\rho_{\rm tr}(x,t)=|\psi_{\rm tr}|^2
=\operatorname{sech}^2(2ka)
}.
$$

This is [finite square barrier transmission at half barrier height](../../../quantum-mechanics.md#finite-square-barrier-transmission-at-half-barrier-height).

<h4 id="15d/b/ii">ii</h4>

↑ **Parent:** [B](#15d/b)

<h5 id="15d/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#15d/b/ii)

For a plane wave $A e^{i(kx-Et/\hbar)}$, the [probability current](../../../quantum-mechanics.md#probability-current) is

$$
J=\frac{\hbar k}{m}|A|^2.
$$

The incident amplitude is one and the transmitted amplitude is $T$, so

$$
\boxed{
\frac{J_{\rm tr}}{J_{\rm in}}
=|T|^2
=\operatorname{sech}^2(2ka)
}.
$$

This is the transmission probability for [quantum tunnelling](../../../quantum-mechanics.md#quantum-tunnelling). In the [stationary state](../../../quantum-mechanics.md#stationary-state), $\partial\rho/\partial t=0$, so the [continuity equation](../../../physics.md#continuity-equation) makes the net current independent of position. The reflected current therefore supplies the remainder:

$$
\boxed{\frac{|J_{\rm refl}|}{J_{\rm in}}
=1-\operatorname{sech}^2(2ka)
=\tanh^2(2ka).}
$$

## 16D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16d/a">a</h3>

↑ **Parent:** [16D](#16d)

<h4 id="16d/a/solution">Solution</h4>

↑ **Parent:** [A](#16d/a)

Let $x^\mu=(ct,\mathbf x)$, let $\tau$ be [proper time](../../../special-relativity.md#proper-time), and define the [four-velocity](../../../special-relativity.md#four-velocity) and [four-momentum](../../../special-relativity.md#four-momentum) by

$$
u^\mu=\frac{dx^\mu}{d\tau}=\gamma(c,\mathbf v),
\qquad
p^\mu=mu^\mu=(\mathcal E/c,\mathbf p).
$$

If $F^{\mu\nu}$ is the [electromagnetic field tensor](../../../electromagnetism.md#electromagnetic-field-tensor), the covariant [Lorentz force](../../../electromagnetism.md#lorentz-force) law is

$$
\boxed{\frac{dp^\mu}{d\tau}=qF^{\mu\nu}u_\nu}.
$$

The temporal component and three spatial components respectively give

$$
\boxed{\frac{d\mathcal E}{dt}=q\mathbf E\cdot\mathbf v},
\qquad
\boxed{\frac{d\mathbf p}{dt}
=q(\mathbf E+\mathbf v\times\mathbf B)}.
$$

Here $\mathcal E=\gamma mc^2$ is the relativistic [energy](../../../classical-mechanics.md#energy) and $\mathbf p=\gamma m\mathbf v$ is the relativistic [momentum](../../../classical-mechanics.md#momentum). In the nonrelativistic [limit](../../../calculus.md#limit-of-a-function), $\gamma\to1$, so the spatial equation becomes

$$
m\frac{d\mathbf v}{dt}
=q(\mathbf E+\mathbf v\times\mathbf B),
$$

the usual Lorentz-force law.

<h3 id="16d/b">b</h3>

↑ **Parent:** [16D](#16d)

<h4 id="16d/b/solution">Solution</h4>

↑ **Parent:** [B](#16d/b)

The temporal component found in part (a) gives directly

$$
\boxed{
\mathcal E(t)-\mathcal E(0)
=q\int_0^t\mathbf E\cdot\mathbf v(s)\,ds
}.
$$

For a constant [electric field](../../../electromagnetism.md#electric-field), this is the work done by the field along the particle trajectory:

$$
\boxed{
\mathcal E(t)=\mathcal E(0)
+q\mathbf E\cdot[\mathbf x(t)-\mathbf x(0)]
}.
$$

<h3 id="16d/c">c</h3>

↑ **Parent:** [16D](#16d)

<h4 id="16d/c/solution">Solution</h4>

↑ **Parent:** [C](#16d/c)

With $\mathbf B=0$ and $\mathbf E=(0,0,E)$, the spatial [Lorentz force](../../../electromagnetism.md#lorentz-force) equation gives

$$
p_x=p_0,\qquad p_y=0,\qquad p_z=qEt.
$$

The [relativistic energy-momentum relation](../../../special-relativity.md#energy-momentum-relation) therefore yields

$$
\boxed{
\mathcal E(t)=
\sqrt{\mathcal E_0^2+c^2q^2E^2t^2}
},
\qquad
\mathcal E_0=\sqrt{m^2c^4+c^2p_0^2}.
$$

Since $\mathbf v=c^2\mathbf p/\mathcal E$,

$$
\dot z=\frac{c^2qEt}{\mathcal E(t)}.
$$

Integration from the initial [position](../../../classical-mechanics.md#position) $z(0)=0$ gives

$$
\boxed{
z(t)=
\frac{\sqrt{\mathcal E_0^2+c^2q^2E^2t^2}-\mathcal E_0}{qE}
}.
$$

<h3 id="16d/d">d</h3>

↑ **Parent:** [16D](#16d)

<h4 id="16d/d/solution">Solution</h4>

↑ **Parent:** [D](#16d/d)

The $x$ component of the [velocity](../../../classical-mechanics.md#velocity) is

$$
\dot x=\frac{c^2p_0}{\mathcal E(t)}.
$$

Thus

$$
x(t)=\frac{cp_0}{qE}
\operatorname{arsinh}\left(\frac{cqEt}{\mathcal E_0}\right).
$$

Solving this equation for $t$ gives

$$
\frac{cqEt}{\mathcal E_0}
=\sinh\left(\frac{qEx}{cp_0}\right).
$$

Substitution into the expression for $z(t)$ and the identity $1+\sinh^2u=\cosh^2u$ produce the trajectory

$$
\boxed{
z(x)=\frac{\mathcal E_0}{qE}
\left[
\cosh\left(\frac{qEx}{cp_0}\right)-1
\right]
}.
$$

This is [relativistic motion in a constant electric field with transverse momentum](../../../special-relativity.md#relativistic-motion-in-a-constant-electric-field-with-transverse-momentum).

<h3 id="16d/e">e</h3>

↑ **Parent:** [16D](#16d)

<h4 id="16d/e/solution">Solution</h4>

↑ **Parent:** [E](#16d/e)

For $t\to+\infty$ with $qE>0$, an [asymptotic expansion](../../../analysis.md#asymptotic-expansion) gives

$$
z(t)=ct-\frac{\mathcal E_0}{qE}+O(t^{-1}),
$$

so the longitudinal [velocity](../../../classical-mechanics.md#velocity) tends to the speed of light. More generally, its limiting sign is the sign of $qE$.

For small $t$, the [taylor series](../../../calculus.md#taylor-series) of the square root gives

$$
z(t)
=\frac{qEc^2}{2\mathcal E_0}t^2+O(t^4).
$$

In the nonrelativistic [limit](../../../calculus.md#limit-of-a-function) $\mathcal E_0\simeq mc^2$, this becomes

$$
z(t)\simeq\frac{qE}{2m}t^2
=\frac12at^2,
\qquad a=\frac{qE}{m}.
$$

The transverse motion is then uniform:

$$
\boxed{x(t)=\frac{p_0}{m}t}.
$$

Eliminating $t$ gives the nonrelativistic parabolic trajectory

$$
\boxed{
z(x)=\frac{qEm}{2p_0^2}x^2
}.
$$

## 17B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17b/a">a</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/a/solution">Solution</h4>

↑ **Parent:** [A](#17b/a)

Apply a one-step numerical method to the [scalar](../../../vector-space.md#scalar) test [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation)

$$
y'=\lambda y.
$$

If one step has the form

$$
y_{n+1}=R(z)y_n,
\qquad z=h\lambda,
$$

then $R$ is the [stability function](../../../numerical-analysis.md#stability-function) and the [linear stability domain](../../../numerical-analysis.md#linear-stability-domain) is

$$
\boxed{\mathcal S=\{z\in\mathbb C:|R(z)|\leq1\}}.
$$

The method is [A-stable](../../../numerical-analysis.md#a-stability) when

$$
\boxed{\{z:\operatorname{Re}z\leq0\}\subseteq\mathcal S},
$$

so it does not amplify any mode that the exact [differential equation](../../../differential-equation.md) does not amplify.

<h3 id="17b/b">b</h3>

↑ **Parent:** [17B](#17b)

<h4 id="17b/b/solution">Solution</h4>

↑ **Parent:** [B](#17b/b)

For the test equation $f(y)=\lambda y$, put $z=h\lambda$. The stage equations of this [implicit Runge-Kutta method](../../../numerical-analysis.md#implicit-runge-kutta-method) are

$$
\begin{pmatrix}
1-z/4&-z(1/4-a)\\
-z(1/4+a)&1-z/4
\end{pmatrix}
\begin{pmatrix}k_1\\k_2\end{pmatrix}
=\lambda y_n\begin{pmatrix}1\\1\end{pmatrix}.
$$

Substitution into the update gives the [stability function](../../../numerical-analysis.md#stability-function)

$$
R(z)=\frac{2+z+2a^2z^2}{2-z+2a^2z^2}.
$$

For $z=x+iy$, direct expansion gives

$$
\begin{aligned}
&|2-z+2a^2z^2|^2-|2+z+2a^2z^2|^2\\
&\hspace{35mm}=-8x(1+a^2|z|^2).
\end{aligned}
$$

This is nonnegative whenever $x\leq0$, and hence $|R(z)|\leq1$ throughout the closed left half-plane, provided the denominator has no zero there.

If $a=0$, the denominator vanishes only at $z=2$. If $a\ne0$, its zeros solve

$$
2a^2z^2-z+2=0.
$$

Real roots are positive, while a complex-conjugate pair has positive real part because the sum of the roots is $1/(2a^2)>0$. Thus there are no poles in the closed left half-plane for any real $a$. Therefore

$$
\boxed{a\in\mathbb R}
$$

is the complete set of [A-stable](../../../numerical-analysis.md#a-stability) parameters, as summarized by the [A-stability of a symmetric two-stage implicit Runge-Kutta family](../../../numerical-analysis.md#a-stability-of-a-symmetric-two-stage-implicit-runge-kutta-family).

## 18H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

**True.** If the [Markov chain](../../../markov-process.md#markov-chain) with [transition matrix](../../../markov-process.md#stochastic-matrix) $P$ is irreducible, then for every pair of states $i,j$ there is a path

$$
i=i_0,i_1,\ldots,i_m=j
$$

with $P_{i_{r-1}i_r}>0$ at every step. The support assumption gives $Q_{i_{r-1}i_r}>0$ for every edge of the same path. Thus every state can reach every other state under $Q$, so the second chain is also an [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain).

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

**True.** For a state $i$, let

$$
\mathcal R_P(i)=\{n\geq1:(P^n)_{ii}>0\}
$$

be its possible return times under $P$, and define $\mathcal R_Q(i)$ similarly. Every positive $P$-path is a positive $Q$-path, so

$$
\mathcal R_P(i)\subseteq\mathcal R_Q(i).
$$

The greatest common divisor of the larger set divides that of the smaller set. Since the latter is one by the assumed [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain) property, the former is also one. Hence every state is aperiodic under $Q$.

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/solution">Solution</h4>

↑ **Parent:** [C](#18h/c)

**False.** On the two-state space, take

$$
P=
\begin{pmatrix}1&0\\0&1\end{pmatrix},
\qquad
Q=
\begin{pmatrix}\tfrac12&\tfrac12\\0&1\end{pmatrix}.
$$

Every positive entry of $P$ remains positive in $Q$. Under $P$, both singleton states are closed [communicating classes](../../../markov-process.md#communicating-class), so neither state is a [transient state](../../../markov-process.md#transient-state). Under $Q$, however, state one eventually moves to the absorbing state two and can never return after doing so. State one is therefore transient.

<h3 id="18h/d">d</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/d/solution">Solution</h4>

↑ **Parent:** [D](#18h/d)

**False.** Again use two states, but now take

$$
P=
\begin{pmatrix}1&0\\0&1\end{pmatrix},
\qquad
Q=
\begin{pmatrix}\tfrac12&\tfrac12\\
\tfrac12&\tfrac12
\end{pmatrix}.
$$

The support condition holds. Under $P$, the [first return time](../../../markov-process.md#first-return-time) to state one is identically one, so $\mu_1=1$. Under $Q$, the chain is irreducible with [stationary distribution](../../../markov-process.md#stationary-distribution) $(1/2,1/2)$. The [mean recurrence time](../../../markov-process.md#mean-recurrence-time) formula gives

$$
\eta_1=\frac1{\pi_1}=2>1=\mu_1.
$$

**Thus enlarging transition support does not imply a smaller mean return time.**

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
