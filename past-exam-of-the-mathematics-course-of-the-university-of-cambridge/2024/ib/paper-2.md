# Paper 2

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperib_2_2024.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperib_2_2024.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
  - [i](#1e/i)
    - [Solution](#1e/i/solution)
  - [ii](#1e/ii)
    - [Solution](#1e/ii/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5D](#5d)
  - [Solution](#5d/solution)
- [6H](#6h)
  - [i](#6h/i)
    - [Solution](#6h/i/solution)
  - [ii](#6h/ii)
    - [Solution](#6h/ii/solution)
  - [iii](#6h/iii)
    - [Solution](#6h/iii/solution)
  - [iv](#6h/iv)
    - [Solution](#6h/iv/solution)
- [7H](#7h)
  - [a](#7h/a)
    - [Solution](#7h/a/solution)
  - [b](#7h/b)
    - [Solution](#7h/b/solution)
- [8G](#8g)
  - [a](#8g/a)
    - [Solution](#8g/a/solution)
  - [b](#8g/b)
    - [Solution](#8g/b/solution)
- [9E](#9e)
  - [a](#9e/a)
    - [Solution](#9e/a/solution)
  - [b](#9e/b)
    - [Solution](#9e/b/solution)
- [10F](#10f)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
- [11G](#11g)
  - [a](#11g/a)
    - [Solution](#11g/a/solution)
  - [b](#11g/b)
    - [Solution](#11g/b/solution)
  - [c](#11g/c)
    - [Solution](#11g/c/solution)
  - [d](#11g/d)
    - [Solution](#11g/d/solution)
- [12B](#12b)
  - [Solution](#12b/solution)
- [13C](#13c)
  - [Solution](#13c/solution)
- [14B](#14b)
  - [Solution](#14b/solution)
- [15A](#15a)
  - [i](#15a/i)
    - [Solution](#15a/i/solution)
  - [ii](#15a/ii)
    - [Solution](#15a/ii/solution)
  - [iii](#15a/iii)
    - [Solution](#15a/iii/solution)
  - [iv](#15a/iv)
    - [Solution](#15a/iv/solution)
  - [v](#15a/v)
    - [Solution](#15a/v/solution)
  - [vi](#15a/vi)
    - [Solution](#15a/vi/solution)
- [16C](#16c)
  - [Solution](#16c/solution)
- [17D](#17d)
  - [a](#17d/a)
    - [Solution](#17d/a/solution)
  - [b](#17d/b)
    - [Solution](#17d/b/solution)
  - [c](#17d/c)
    - [Solution](#17d/c/solution)
- [18H](#18h)
  - [Solution](#18h/solution)

## 1E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

The [Eisenstein criterion](../../../commutative-algebra.md#eisenstein-criterion) says that a primitive [polynomial](../../../polynomial.md)

$$
f(X)=a_nX^n+\cdots+a_0\in\mathbb Z[X]
$$

is irreducible if there is a prime $p$ such that

$$
p\nmid a_n,
\qquad
p\mid a_i\quad(0\leq i<n),
\qquad
p^2\nmid a_0.
$$

By the [Gauss lemma for polynomials](../../../commutative-algebra.md#gauss-lemma-for-polynomials), irreducibility over $\mathbb Q$ and over $\mathbb Z$ agree for primitive [polynomials](../../../polynomial.md).

<h3 id="1e/i">i</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/i/solution">Solution</h4>

↑ **Parent:** [I](#1e/i)

Let

$$
P_n(X)=1+X+\cdots+X^{n-1}.
$$

If $n=ab$ with $a,b>1$, then

$$
P_n(X)=\left(1+X+\cdots+X^{a-1}\right)
\left(1+X^a+\cdots+X^{a(b-1)}\right),
$$

so $P_n$ is reducible.

Conversely, let $n=p$ be prime. Translation by one is an automorphism of $\mathbb Z[X]$, and

$$
P_p(X+1)=\frac{(X+1)^p-1}{X}
=\sum_{k=1}^p\binom pkX^{k-1}.
$$

Its leading coefficient is one, every lower coefficient is divisible by $p$, and its constant coefficient is $p$, which is not divisible by $p^2$. The [Eisenstein criterion](../../../commutative-algebra.md#eisenstein-criterion) proves that $P_p(X+1)$ is irreducible, hence so is $P_p(X)$. Therefore the [geometric-sum irreducibility criterion](../../../commutative-algebra.md#geometric-sum-irreducibility-criterion) is

$$
\boxed{1+X+\cdots+X^{n-1}\text{ is irreducible in }\mathbb Z[X]
\Longleftrightarrow n\text{ is prime}}.
$$

<h3 id="1e/ii">ii</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1e/ii)

Regard

$$
F=X^2+Y^2-1
$$

as a monic quadratic in $X$ over $\mathbb Q[Y]$. By the [Gauss lemma for polynomials](../../../commutative-algebra.md#gauss-lemma-for-polynomials), reducibility in $\mathbb Q[X,Y]$ would imply reducibility in $\mathbb Q(Y)[X]$, so $1-Y^2$ would be a square in $\mathbb Q(Y)$. This is impossible: its zero at $Y=1$ has odd order one, whereas every zero or pole of a square in a rational-function field has even order. Hence

$$
\boxed{X^2+Y^2-1\text{ is irreducible over }\mathbb Q}.
$$

The same [odd-valuation obstruction to a rational-function square](../../../commutative-algebra.md#odd-valuation-obstruction-to-a-rational-function-square) works over every field of characteristic different from two, since the zeros $Y=1$ and $Y=-1$ are then distinct. It does not work over every field. In characteristic two,

$$
X^2+Y^2-1=(X+Y+1)^2,
$$

so the [polynomial](../../../polynomial.md) is reducible.

## 2F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

A map $h:X\to X$ is a contraction if there is a constant $q<1$ such that

$$
d(hx,hy)\leq qd(x,y)
$$

for every $x,y\in X$.

The [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) states that a contraction of a nonempty complete metric space has a unique fixed point, and that the iterates from every starting point converge to it. To prove this, choose $x_0\in X$ and put $x_{n+1}=h(x_n)$. Then

$$
d(x_{n+1},x_n)\leq q^nd(x_1,x_0),
$$

so, for $m>n$,

$$
d(x_m,x_n)\leq\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus $(x_n)$ is Cauchy and converges, by completeness, to some $x_*$. A contraction is continuous, so

$$
h(x_*)=\lim_nh(x_n)=\lim_nx_{n+1}=x_*.
$$

If $y_*$ is another fixed point, then

$$
d(x_*,y_*)\leq qd(x_*,y_*),
$$

forcing $x_*=y_*$.

For the Newton map

$$
g(x)=x-\frac{f(x)}{f'(x)},
$$

one has $g(r)=r$ and

$$
g'(x)=\frac{f(x)f''(x)}{f'(x)^2},
\qquad
\boxed{g'(r)=0}.
$$

On the given neighbourhood,

$$
|g'(x)|\leq\frac{M|f(x)|}{\delta^2}.
$$

Since $f(r)=0$, choose a closed interval $U'$ centred at $r$ and contained in $U$ so small that $M|f(x)|/\delta^2\leq1/2$ there. Then

$$
|g(x)-r|\leq\frac12|x-r|,
$$

so $g(U')\subseteq U'$ and $g$ is a contraction on the complete interval $U'$. The [local contraction proof for Newton iteration](../../../analysis.md#local-contraction-proof-for-newton-iteration) therefore shows that $r$ is the unique fixed point of $g$ on $U'$.

## 3B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

Multiplication by $(1-x^2)^{-1/2}$ puts the equation in [Sturm-Liouville theory](../../../analysis.md#sturm-liouville-theory) form:

$$
\boxed{
\frac d{dx}\left(\sqrt{1-x^2}\,T_n'\right)
+\frac{n^2}{\sqrt{1-x^2}}T_n=0}.
$$

Multiply the equations for $T_n,T_m$ by $T_m,T_n$, subtract and integrate. The boundary term vanishes because $\sqrt{1-x^2}=0$ at both endpoints and the [polynomial](../../../polynomial.md) [derivatives](../../../calculus.md#derivative) are bounded. Therefore, for $n^2\ne m^2$,

$$
\boxed{
\int_{-1}^1\frac{T_n(x)T_m(x)}{\sqrt{1-x^2}}\,dx=0}.
$$

This is the usual [Chebyshev polynomial](../../../numerical-analysis.md#chebyshev-polynomial) orthogonality.

Differentiating the original equation and writing $U_n=T_n'$ gives

$$
\boxed{(1-x^2)U_n''-3xU_n'+(n^2-1)U_n=0}.
$$

Its self-adjoint form is

$$
\boxed{
\frac d{dx}\left((1-x^2)^{3/2}U_n'\right)
+(n^2-1)\sqrt{1-x^2}\,U_n=0}.
$$

The same subtraction argument now yields, for $n^2\ne m^2$,

$$
\boxed{
\int_{-1}^1U_n(x)U_m(x)\sqrt{1-x^2}\,dx=0}.
$$

These two relations form the [Chebyshev derivative Sturm-Liouville pair](../../../numerical-analysis.md#chebyshev-derivative-sturm-liouville-pair).

## 4C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

Vanishing net [charge density](../../../electromagnetism.md#charge-density) does not require vanishing current. Positive and negative charge carriers can cancel in [charge density](../../../electromagnetism.md#charge-density) while their oppositely directed motions add to a nonzero current. Charge conservation only requires

$$
\partial_t\rho+\nabla\cdot J=0;
$$

for magnetostatics this becomes $\nabla\cdot J=0$.

Because $\nabla\cdot B=0$, one may introduce a [magnetic vector potential](../../../electromagnetism.md#magnetic-vector-potential) with

$$
B=\nabla\times A.
$$

It is not unique: $A+\nabla\chi$ gives the same field for any [scalar](../../../vector-space.md#scalar) $\chi$.

For the stated current,

$$
\nabla\cdot J=0,
$$

so it is consistent with stationary charge conservation. Direct calculation gives

$$
\nabla\times J
=\lambda J_0(\sin\lambda z,\cos\lambda z,0)
=\lambda J.
$$

Thus $J$ is a [Beltrami field](../../../electromagnetism.md#beltrami-field). For $\lambda\ne0$, choose

$$
\boxed{B=\frac{\mu_0}{\lambda}J}.
$$

Then $\nabla\cdot B=0$ and $\nabla\times B=\mu_0J$. A convenient Coulomb-gauge potential is

$$
\boxed{A=\frac{\mu_0}{\lambda^2}J},
$$

since $\nabla\times A=B$ and $\nabla\cdot A=0$. [Gradient](../../../calculus.md#gradient) gauge terms may of course be added.

If $\lambda=0$, the current is the constant field $J=(0,J_0,0)$. The formulas involving $1/\lambda$ do not apply; one valid choice is

$$
\boxed{B=(0,0,-\mu_0J_0x),
\qquad
A=\left(0,-\frac12\mu_0J_0x^2,0\right).}
$$

## 5D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

Writing the [velocity](../../../classical-mechanics.md#velocity) as $(u,v)=(y,ax)$ gives

$$
\partial_xu+\partial_yv=0,
$$

so the flow is incompressible. With the convention

$$
u=\psi_y,
\qquad
v=-\psi_x,
$$

a stream [function](../../../function.md) is

$$
\boxed{\psi(x,y)=\frac12(y^2-ax^2)}.
$$

The [streamlines](../../../fluid-mechanics.md#streamline) are its level sets. For $a>0$, they are the hyperbolas

$$
y^2-ax^2=\text{constant},
$$

with separatrices $y=\pm\sqrt a\,x$ and a saddle at the origin. For $a<0$, they are concentric ellipses

$$
y^2+|a|x^2=\text{constant},
$$

traversed clockwise. This is the [streamline classification of a planar linear saddle or centre](../../../fluid-mechanics.md#streamline-classification-of-a-planar-linear-saddle-or-centre).

The [scalar](../../../vector-space.md#scalar) [vorticity](../../../fluid-mechanics.md#vorticity) is

$$
\partial_xv-\partial_yu=a-1.
$$

Hence the flow is irrotational exactly when

$$
\boxed{a=1}.
$$

Then $(u,v)=(y,x)=\nabla\phi$, and a [velocity potential](../../../fluid-mechanics.md#velocity-potential) is

$$
\boxed{\phi(x,y)=xy+\text{constant}}.
$$

## 6H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6h/i">i</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/i/solution">Solution</h4>

↑ **Parent:** [I](#6h/i)

Writing $p_j$ for the probability of face $j$, the hypotheses are

$$
\boxed{H_0:p_1=\cdots=p_6=\frac16}
$$

against

$$
\boxed{H_1:\text{at least one }p_j\ne\frac16}.
$$

<h3 id="6h/ii">ii</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6h/ii)

For observed counts $O_j$ and null expected counts $E_j=np_j$, the [Pearson chi-squared goodness-of-fit test](../../../statistical-modelling.md#pearson-chi-squared-goodness-of-fit-test) uses

$$
X^2=\sum_{j=1}^k\frac{(O_j-E_j)^2}{E_j}.
$$

When the null cell probabilities are specified and the expected counts grow, its limiting null distribution is

$$
\boxed{X^2\ \xrightarrow{d}\ \chi^2_{k-1}}.
$$

Here $k=6$, so the [limit](../../../calculus.md#limit-of-a-function) is $\chi^2_5$.

<h3 id="6h/iii">iii</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6h/iii)

Under fairness every expected count is $90/6=15$. Therefore

$$
\begin{aligned}
X^2
&=\frac{(20-15)^2+(15-15)^2+(12-15)^2
+(17-15)^2+(9-15)^2+(17-15)^2}{15}\\
&=\frac{25+0+9+4+36+4}{15}
=\boxed{5.2}.
\end{aligned}
$$

<h3 id="6h/iv">iv</h3>

↑ **Parent:** [6H](#6h)

<h4 id="6h/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6h/iv)

The asymptotic p-value is the upper-tail probability

$$
\boxed{\mathbb P(\chi^2_5\geq5.2)=1-F_{\chi^2_5}(5.2)}.
$$

Numerically this is approximately $0.392$, so the data provide little evidence against fairness.

## 7H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="7h/a">a</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/a/solution">Solution</h4>

↑ **Parent:** [A](#7h/a)

Use multipliers $\lambda,\mu\geq0$ for

$$
x_1+x_2-c\leq0,
\qquad
\sqrt{x_2}-d\leq0.
$$

At an interior point in the nonnegative quadrant, the [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) are

$$
\log x_1+1+\lambda=0,
$$



$$
-1+\lambda+\frac{\mu}{2\sqrt{x_2}}=0,
$$

with complementary slackness for the two constraints.

For $c=3/e^2$ and $d=2/e$, the square-root constraint is inactive at the answer, so $\mu=0$. The second stationarity equation gives $\lambda=1$, and the first gives $x_1=e^{-2}$. The sum constraint is active, hence

$$
\boxed{x_1=\frac1{e^2},
\qquad
x_2=\frac2{e^2}}.
$$

Indeed, $\sqrt{x_2}=\sqrt2/e<2/e$. The minimum value is

$$
\boxed{-\frac4{e^2}}.
$$

<h3 id="7h/b">b</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/b/solution">Solution</h4>

↑ **Parent:** [B](#7h/b)

Now $d=1/e$, and both constraints are active. Therefore

$$
x_2=\frac1{e^2},
\qquad
x_1=c-x_2=\frac2{e^2}.
$$

The first stationarity equation gives

$$
\lambda=1-\log2>0,
$$

and the second gives

$$
\mu=\frac{2\log2}{e}>0.
$$

Thus all multiplier and complementary-slackness conditions hold, and

$$
\boxed{x_1=\frac2{e^2},
\qquad
x_2=\frac1{e^2}},
$$

with minimum value

$$
\boxed{\frac{2\log2-5}{e^2}}.
$$

The observation is that lowering $d$ activates the second constraint and moves the optimum to the intersection of the two active boundaries. Rewriting $\sqrt{x_2}\leq d$ as $x_2\leq d^2$ shows that the feasible set is convex, while $x_1\log x_1-x_2$ is convex. Hence the [active-set transition in capped resource allocation](../../../mathematical-optimization.md#active-set-transition-in-capped-resource-allocation) and the KKT candidates above give the unique global minima, not merely local stationary points.

## 8G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="8g/a">a</h3>

↑ **Parent:** [8G](#8g)

<h4 id="8g/a/solution">Solution</h4>

↑ **Parent:** [A](#8g/a)

The characteristic [polynomial](../../../polynomial.md) is

$$
\chi_A(t)=\det(tI-A).
$$

To prove triangularizability, use induction on $n$. The result is immediate for $n=1$. Over $\mathbb C$, $\chi_A$ has a root $\lambda$, so $A$ has an [eigenvector](../../../linear-operator-theory.md#eigenvector) $v_1$. Extend it to a [basis](../../../vector-space.md#basis). In this [basis](../../../vector-space.md#basis),

$$
[A]=\begin{pmatrix}\lambda&*\\0&B\end{pmatrix}.
$$

By induction, a change among the remaining $n-1$ [basis](../../../vector-space.md#basis) [vectors](../../../vector-space.md#vector) makes $B$ upper triangular. Thus the [triangularization over an algebraically closed field](../../../linear-operator-theory.md#triangularization-over-an-algebraically-closed-field) gives

$$
\boxed{A\text{ is similar to an upper-triangular matrix}}.
$$

The minimal [polynomial](../../../polynomial.md) $m_A$ is the monic [polynomial](../../../polynomial.md) of least degree satisfying $m_A(A)=0$. To establish existence without quoting the Cayley-Hamilton theorem, let $T$ be an upper-triangular [matrix](../../../vector-space.md#matrix) similar to $A$, with diagonal entries $\lambda_1,\ldots,\lambda_n$, and put

$$
V_k=\operatorname{span}\{e_1,\ldots,e_k\}.
$$

Then

$$
(T-\lambda_kI)V_k\subseteq V_{k-1}.
$$

The factors $T-\lambda_kI$ commute, so applying all of them successively lowers the invariant flag to zero:

$$
\prod_{k=1}^n(T-\lambda_kI)=0.
$$

Similarity gives the same [polynomial](../../../polynomial.md) identity for $A$. Hence a nonzero monic annihilating [polynomial](../../../polynomial.md) of degree $n$ exists, and a least-degree one exists.

If $m$ and $\widetilde m$ were two monic annihilating [polynomials](../../../polynomial.md) of the same least degree, then $m-\widetilde m$ would be an annihilating [polynomial](../../../polynomial.md) of smaller degree unless it were zero. Thus the minimal [polynomial](../../../polynomial.md) is unique, and the [minimal polynomial bound from a triangular invariant flag](../../../linear-operator-theory.md#minimal-polynomial-bound-from-a-triangular-invariant-flag) gives

$$
\boxed{\deg m_A\leq n}.
$$

<h3 id="8g/b">b</h3>

↑ **Parent:** [8G](#8g)

<h4 id="8g/b/solution">Solution</h4>

↑ **Parent:** [B](#8g/b)

The [eigenvalue](../../../linear-operator-theory.md#eigenvalue) equation $D_rf=\lambda f$ is

$$
f(x+r)=(1+\lambda)f(x).
$$

If $\lambda=-1$, this forces $f(x+r)=0$ for every $x$, hence $f=0$, so $-1$ is not an [eigenvalue](../../../linear-operator-theory.md#eigenvalue). If $c=1+\lambda\ne0$, choose arbitrary values on representatives of the cosets of $r\mathbb Z$ and extend by

$$
f(t+kr)=c^kf(t),
\qquad k\in\mathbb Z.
$$

This produces nonzero eigenfunctions. Choosing [functions](../../../function.md) supported on distinct cosets gives infinitely many linearly independent eigenfunctions. Therefore

$$
\boxed{\operatorname{spec}_{\rm point}(D_r)=\mathbb R\setminus\{-1\}},
$$

and every eigenspace is infinite-dimensional.

Direct expansion gives

$$
D_rD_sf(x)=f(x+r+s)-f(x+r)-f(x+s)+f(x),
$$

which is symmetric in $r,s$. Hence

$$
\boxed{D_rD_s=D_sD_r}.
$$

Suppose a degree-$n$ [polynomial](../../../polynomial.md) $p$ were a sum of $n$ periodic [functions](../../../function.md),

$$
p=f_1+\cdots+f_n,
\qquad D_{r_i}f_i=0,
\quad r_i\ne0.
$$

Apply the commuting product $D_{r_1}\cdots D_{r_n}$. Every term on the right is killed by its corresponding factor, whereas for leading coefficient $a_n$ the [mixed finite difference of a polynomial](../../../linear-operator-theory.md#mixed-finite-difference-of-a-polynomial) gives

$$
D_{r_1}\cdots D_{r_n}p
=n!a_n\prod_{i=1}^nr_i\ne0.
$$

This contradiction proves

$$
\boxed{p\text{ cannot be a sum of }n\text{ periodic functions}}.
$$

## 9E

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="9e/a">a</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/a/solution">Solution</h4>

↑ **Parent:** [A](#9e/a)

An [ideal](../../../commutative-algebra.md#ideal) of $R/I$ has the form $J/I$ for an [ideal](../../../commutative-algebra.md#ideal) $J\supseteq I$ of $R$. If $R$ is Noetherian, write

$$
J=(a_1,\ldots,a_k).
$$

Then

$$
J/I=(a_1+I,\ldots,a_k+I),
$$

so every [ideal](../../../commutative-algebra.md#ideal) of $R/I$ is finitely generated. Hence

$$
\boxed{R/I\text{ is Noetherian}}.
$$

The [Hilbert basis theorem](../../../algebra.md#hilbert-basis-theorem) states that $R[X]$ is Noetherian whenever $R$ is Noetherian. The integers form a principal [ideal](../../../commutative-algebra.md#ideal) domain, so every [ideal](../../../commutative-algebra.md#ideal) of $\mathbb Z$ has one generator and $\mathbb Z$ is Noetherian. It follows that $\mathbb Z[X]$ is Noetherian.

For a nonsquare integer $d$, evaluation at $\sqrt d$ gives

$$
\mathbb Z[X]\longrightarrow\mathbb Z[\sqrt d],
\qquad X\longmapsto\sqrt d.
$$

It is surjective and its kernel is $(X^2-d)$. Therefore

$$
\boxed{\mathbb Z[\sqrt d]\cong\mathbb Z[X]/(X^2-d)}
$$

 is Noetherian by the quotient result. This is the [noetherianity of a quadratic integer order](../../../algebra.md#noetherianity-of-a-quadratic-integer-order).

<h3 id="9e/b">b</h3>

↑ **Parent:** [9E](#9e)

<h4 id="9e/b/solution">Solution</h4>

↑ **Parent:** [B](#9e/b)

The coefficient condition says precisely that every nonconstant monomial has positive powers of both variables. Thus

$$
R=K+XYK[X,Y].
$$

If $c+XYf$ and $d+XYg$ lie in $R$, so do their sum and their product

$$
cd+XY(cg+df+XYfg),
$$

so $R$ is a subring of $K[X,Y]$.

For $n\geq1$, let

$$
I_n=(XY,XY^2,\ldots,XY^n)_R.
$$

Then $I_n\subseteq I_{n+1}$. The containment is strict because $XY^{n+1}\notin I_n$: multiplying a generator $XY^j$ by an element of $R$ produces either a [scalar](../../../vector-space.md#scalar) multiple of $XY^j$, or terms divisible by $X^2$. It cannot produce the monomial $XY^{n+1}$ when $j\leq n$. Hence

$$
I_1\subsetneq I_2\subsetneq I_3\subsetneq\cdots
$$

is a strictly increasing [ideal](../../../commutative-algebra.md#ideal) chain. The [constant-plus-ideal non-Noetherian subring](../../../algebra.md#constant-plus-ideal-non-noetherian-subring) therefore satisfies

$$
\boxed{R\text{ is not Noetherian}}.
$$

## 10F

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

A topological space is compact if every open cover has a finite subcover. It is Hausdorff if every pair of distinct points has disjoint open neighbourhoods.

Let $Y$ be closed in compact $X$, and let $\{U_i\}$ be an open cover of $Y$ by sets open in $X$. Adding the [open set](../../../topology.md#open-set) $X\setminus Y$ gives a cover of $X$, which has a finite subcover. Removing $X\setminus Y$ leaves a finite subcover of $Y$. Thus every closed subspace of a [compact space](../../../topology.md#compact-space) is compact.

Now let $A,B$ be disjoint closed subsets of a compact Hausdorff space. They are compact. For each $a\in A$ and $b\in B$, choose disjoint [open sets](../../../topology.md#open-set) $U_{a,b}\ni a$ and $V_{a,b}\ni b$. Fixing $a$, finitely many $V_{a,b_j}$ cover $B$. Put

$$
U_a=\bigcap_jU_{a,b_j},
\qquad
V_a=\bigcup_jV_{a,b_j}.
$$

Then $U_a$ contains $a$, $V_a$ contains $B$, and they are disjoint. Finitely many $U_{a_i}$ cover $A$. Therefore

$$
U=\bigcup_iU_{a_i},
\qquad
V=\bigcap_iV_{a_i}
$$

are disjoint open neighbourhoods of $A$ and $B$. This proves the [normality of a compact Hausdorff space](../../../topology.md#normality-of-a-compact-hausdorff-space).

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

Let $X$ be compact Hausdorff, let $x\in X$, and let $U$ be a neighbourhood of $x$. Choose an open $O$ with $x\in O\subseteq U$. Apply the separation result from part (a) to the disjoint closed sets $\{x\}$ and $X\setminus O$. There is an open $V\ni x$ whose closure lies in $O$. Then

$$
K=\overline V
$$

is compact, contains the neighbourhood $V$ of $x$, and lies in $U$. Thus $X$ is locally compact.

Conversely, suppose $X$ is locally compact Hausdorff and $A\cap K$ is closed in every compact $K\subseteq X$. For $x\notin A$, choose a compact neighbourhood $K$ of $x$ and an [open set](../../../topology.md#open-set) $U$ with

$$
x\in U\subseteq K.
$$

Since $A\cap K$ is closed in $K$, there is an [open set](../../../topology.md#open-set) $W\subseteq X$ such that

$$
K\setminus(A\cap K)=K\cap W.
$$

Then $U\cap W$ is an open neighbourhood of $x$ disjoint from $A$. Thus $X\setminus A$ is open and

$$
\boxed{A\text{ is closed}}.
$$

This is the [compactly detected closed-set theorem in a locally compact Hausdorff space](../../../topology.md#compactly-detected-closed-set-theorem-in-a-locally-compact-hausdorff-space).

## 11G

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="11g/a">a</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/a/solution">Solution</h4>

↑ **Parent:** [A](#11g/a)

If $(x,y)\sim(x+a,y+b)$ in the torus, then

$$
\widetilde\pi(x+a,y+b)=(2x+2a,y+b).
$$

This is Klein-equivalent to $(2x,y)$ by taking $(c,d)=(2a,b)$. Hence $\widetilde\pi$ descends to a well-defined continuous map

$$
\pi:T^2\to K,
\qquad
\pi([x,y])=[2x,y].
$$

The deck [group](../../../group.md) of the Klein bottle has an index-two [subgroup](../../../group.md#subgroup) consisting of transformations with even $c$; it is generated by translations $(x,y)\mapsto(x+2,y)$ and $(x,y)\mapsto(x,y+1)$. This is exactly the image under $\widetilde\pi$ of the torus deck lattice. Therefore the [orientation double cover of the Klein bottle](../../../topology.md#orientation-double-cover-of-the-klein-bottle) has two sheets:

$$
\boxed{\pi:T^2\to K\text{ is }2:1}.
$$

<h3 id="11g/b">b</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/b/solution">Solution</h4>

↑ **Parent:** [B](#11g/b)

For $T^2$, take the unit square $[0,1]\times[0,1]$. Identify

$$
(0,y)\sim(1,y),
\qquad
(x,0)\sim(x,1),
$$

so both pairs of opposite edges have matching directions.

For $K$, take $[0,1]\times[-1/2,1/2]$. Identify

$$
(x,-1/2)\simeq(x,1/2)
$$

with matching directions, and

$$
(0,y)\simeq(1,-y)
$$

with reversed directions. These equations specify the arrows on the two fundamental-domain drawings.

<h3 id="11g/c">c</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/c/solution">Solution</h4>

↑ **Parent:** [C](#11g/c)

In the Klein fundamental square from part (b), the following straight lines project to the required closed geodesics:

$$
\gamma_1(t)=[t,0],
\qquad0\leq t\leq1;
$$

this is the one-sided horizontal core, and cutting along it leaves a Möbius strip.

Take

$$
\gamma_2(t)=[0,t-1/2],
\qquad0\leq t\leq1;
$$

this is a two-sided vertical geodesic, and cutting along it leaves a cylinder.

Finally take

$$
\gamma_3(t)=[2t,t],
\qquad0\leq t\leq1.
$$

Its endpoints differ by the deck translation $(2,1)$, so it is closed. The parameters $t=1/4$ and $t=3/4$ represent the same Klein-bottle point through an odd-$c$ glide reflection, and no other interior pair does. Thus its image has exactly one transverse self-intersection. This is the [flat Klein-bottle geodesic model](../../../topology.md#flat-klein-bottle-geodesic-model).

<h3 id="11g/d">d</h3>

↑ **Parent:** [11G](#11g)

<h4 id="11g/d/solution">Solution</h4>

↑ **Parent:** [D](#11g/d)

A loop whose Klein deck transformation has odd $c$ has one closed lift to the orientation double cover; one with even $c$ has two. Thus the preimage of $\gamma_1$ contains one closed geodesic, while those of $\gamma_2$ and $\gamma_3$ contain two each.

In the torus unit square, representatives are

$$
\widetilde\gamma_1(t)=[t,0],
$$

which maps twice around $\gamma_1$;

$$
\widetilde\gamma_{2,1}(t)=[0,t],
\qquad
\widetilde\gamma_{2,2}(t)=[1/2,t];
$$

and

$$
\widetilde\gamma_{3,1}(t)=[t,t],
\qquad
\widetilde\gamma_{3,2}(t)=[t,1/2-t].
$$

All coordinates are taken modulo one. Hence the requested numbers are

$$
\boxed{1,\quad 2,\quad 2}.
$$

The two diagonal lifts of $\gamma_3$ meet over its self-intersection point but remain distinct closed geodesics.

## 12B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="12b/solution">Solution</h3>

↑ **Parent:** [12B](#12b)

For $0<a<2$, the beta-integral evaluation gives

$$
I(a)=\int_0^\infty\frac{x^{a-1}}{1+x^2}\,dx
=\frac\pi2\csc\frac{\pi a}{2}.
$$

[Differentiation](../../../calculus.md#differentiation) under the [integral](../../../calculus.md#integral) sign near $a=1$ is justified by domination at zero and infinity. Therefore

$$
I^{(4)}(1)=\int_0^\infty\frac{(\log x)^4}{1+x^2}\,dx.
$$

Writing $a=1+t$ gives

$$
I(1+t)=\frac\pi2\sec\frac{\pi t}{2}.
$$

Since

$$
\sec z=1+\frac{z^2}{2}+\frac{5z^4}{24}+O(z^6),
$$

the [logarithmic moments of the Cauchy kernel](../../../complex-analysis.md#logarithmic-moments-of-the-cauchy-kernel) yield

$$
\boxed{
\int_0^\infty\frac{(\log x)^4}{1+x^2}\,dx
=\frac{5\pi^5}{32}}.
$$

The same expansion gives $I''(1)=\pi^3/8$, agreeing with the supplied identity.

## 13C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="13c/solution">Solution</h3>

↑ **Parent:** [13C](#13c)

For a variation $y+\varepsilon\eta$,

$$
\left.\frac d{d\varepsilon}I[y+\varepsilon\eta]\right|_{\varepsilon=0}
=\int_0^{x_0}\left(F_y\eta+F_{y'}\eta'\right)dx.
$$

Integration by parts gives

$$
\delta I=\left[F_{y'}\eta\right]_0^{x_0}
+\int_0^{x_0}\left(F_y-\frac d{dx}F_{y'}\right)\eta\,dx.
$$

For fixed endpoints, $\eta(0)=\eta(x_0)=0$. The [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) therefore gives the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation)

$$
\boxed{\frac d{dx}F_{y'}-F_y=0}.
$$

A solution makes the first variation vanish for every admissible variation, so it is a stationary candidate; whether it is a minimum or maximum is decided by higher variations. If endpoint values are free, $\eta$ is arbitrary there, and the boundary term instead vanishes under the natural conditions

$$
\boxed{F_{y'}(0)=F_{y'}(x_0)=0}.
$$

Thus the same Euler-Lagrange solution is stationary for all free-endpoint variations. These are the [natural boundary conditions for a free endpoint](../../../analysis.md#natural-boundary-conditions-for-a-free-endpoint).

For

$$
F=y'^2+z'^2+2yz,
$$

the two equations are

$$
\boxed{y''=z,\qquad z''=y}.
$$

Set $u=y+z$ and $v=y-z$. Then

$$
u''=u,
\qquad
v''=-v.
$$

The conditions $y(0)=z(0)=0$ give

$$
u=A\sinh x,
\qquad
v=B\sin x,
$$

and hence the most general solution is

$$
\boxed{
y=\frac12(A\sinh x+B\sin x),
\qquad
z=\frac12(A\sinh x-B\sin x)}.
$$

Free conditions at $x_0$ are $y'(x_0)=z'(x_0)=0$. Adding and subtracting them gives

$$
A\cosh x_0=0,
\qquad
B\cos x_0=0.
$$

Thus $A=0$. The zero solution exists for every $x_0$, while nonzero solutions exist precisely when

$$
\boxed{x_0=\left(k+\frac12\right)\pi,
\qquad k=0,1,2,\ldots}.
$$

For those values they form the one-parameter family

$$
\boxed{y=C\sin x,
\qquad z=-C\sin x},
$$

where $C$ is arbitrary. This is the [free-endpoint normal mode of a coupled variational functional](../../../analysis.md#free-endpoint-normal-mode-of-a-coupled-variational-functional).

## 14B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="14b/solution">Solution</h3>

↑ **Parent:** [14B](#14b)

The convolution is

$$
(f*g)(x)=\int_{-\infty}^{\infty}f(x-y)g(y)\,dy.
$$

We claim that the $n$-fold convolution is

$$
\boxed{
F_n(x)=
\begin{cases}
\dfrac{x^{n-1}}{(n-1)!}e^{-x},&x\geq0,\\
0,&x<0.
\end{cases}}
$$

This is true for $n=1$. If it holds for $n-1$ and $x\geq0$, then

$$
\begin{aligned}
F_n(x)
&=\int_0^x e^{-(x-y)}
\frac{y^{n-2}e^{-y}}{(n-2)!}\,dy\\
&=\frac{e^{-x}}{(n-2)!}\int_0^xy^{n-2}\,dy
=\frac{x^{n-1}e^{-x}}{(n-1)!},
\end{aligned}
$$

and the convolution vanishes for $x<0$. This is the [gamma density from repeated exponential convolution](../../../fourier-analysis.md#gamma-density-from-repeated-exponential-convolution).

The Fourier transform is

$$
\boxed{
\widehat F_n(k)=\frac1{(n-1)!}
\int_0^\infty x^{n-1}e^{-(1+ik)x}\,dx
=\frac1{(1+ik)^n}}.
$$

The [convolution theorem](../../../fourier-analysis.md#convolution-theorem) states

$$
\boxed{\widehat{f*g}(k)=\widehat f(k)\widehat g(k)}.
$$

Indeed, Fubini and $u=x-y$ give

$$
\begin{aligned}
\widehat{f*g}(k)
&=\int\!\int e^{-ikx}f(x-y)g(y)\,dy\,dx\\
&=\int\!\int e^{-ik(u+y)}f(u)g(y)\,du\,dy
=\widehat f(k)\widehat g(k).
\end{aligned}
$$

Since $\widehat F(k)=(1+ik)^{-1}$, induction immediately verifies

$$
\widehat F_n=(\widehat F)^n=(1+ik)^{-n}.
$$

For [Parseval identity](../../../fourier-analysis.md#parseval-identity), take $g(x)=\overline{f(-x)}$. Then

$$
(f*g)(0)=\int_{-\infty}^{\infty}|f(x)|^2\,dx,
\qquad
\widehat g(k)=\overline{\widehat f(k)}.
$$

Using Fourier inversion at zero, which follows from the supplied delta identity,

$$
(f*g)(0)=\frac1{2\pi}\int_{-\infty}^{\infty}
\widehat{f*g}(k)\,dk,
$$

and the convolution theorem gives

$$
\boxed{
\int_{-\infty}^{\infty}|f(x)|^2\,dx
=\frac1{2\pi}\int_{-\infty}^{\infty}|\widehat f(k)|^2\,dk}.
$$

Apply this to $F_{n+1}$. Since

$$
\int_0^\infty|F_{n+1}(x)|^2dx
=\frac1{(n!)^2}\int_0^\infty x^{2n}e^{-2x}\,dx
=\frac{(2n)!}{2^{2n+1}(n!)^2},
$$

one obtains the [Even rational Parseval integral](../../../fourier-analysis.md#even-rational-parseval-integral)

$$
\boxed{
\int_{-\infty}^{\infty}\frac{dk}{(1+k^2)^{n+1}}
=\frac{\pi(2n)!}{2^{2n}(n!)^2}
=\frac\pi{4^n}\binom{2n}{n}}.
$$

## 15A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="15a/i">i</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/i/solution">Solution</h4>

↑ **Parent:** [I](#15a/i)

For a test [wavefunction](../../../quantum-mechanics.md#wave-function) $f$,

$$
[x,p_x]f
=x(-i\hbar f')+i\hbar(xf)'
=i\hbar f.
$$

Thus the [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) is

$$
\boxed{[x,p_x]=i\hbar I}.
$$

<h3 id="15a/ii">ii</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#15a/ii)

The time-dependent [Schrödinger equation](../../../physics.md#schrodinger-equation) is

$$
\boxed{i\hbar\frac{\partial\psi}{\partial t}=H\psi}.
$$

<h3 id="15a/iii">iii</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#15a/iii)

Differentiating $\langle O\rangle=\langle\psi|O|\psi\rangle$ and using the [Schrödinger equation](../../../physics.md#schrodinger-equation) and its adjoint gives the [Ehrenfest theorem](../../../quantum-mechanics.md#ehrenfest-theorem)

$$
\boxed{
\frac d{dt}\langle O\rangle
=\frac1{i\hbar}\langle[O,H]\rangle
+\left\langle\frac{\partial O}{\partial t}\right\rangle}.
$$

<h3 id="15a/iv">iv</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#15a/iv)

Using $[A,BC]=[A,B]C+B[A,C]$ and $[x,p_x]=i\hbar I$,

$$
\boxed{[x,p_x^2]=2i\hbar p_x},
\qquad
\boxed{[x^2,p_x]=2i\hbar x}.
$$

<h3 id="15a/v">v</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/v/solution">Solution</h4>

↑ **Parent:** [V](#15a/v)

With $L=xp_y-yp_x$, the canonical commutators give

$$
[L,x]=i\hbar y,
\quad
[L,y]=-i\hbar x,
\quad
[L,p_x]=i\hbar p_y,
\quad
[L,p_y]=-i\hbar p_x.
$$

It follows that

$$
[L,x^2+y^2]=0,
\qquad
[L,p_x^2+p_y^2]=0.
$$

Therefore rotational symmetry of the isotropic oscillator gives

$$
\boxed{[L,H]=0}.
$$

<h3 id="15a/vi">vi</h3>

↑ **Parent:** [15A](#15a)

<h4 id="15a/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#15a/vi)

In polar coordinates, $z=re^{i\phi}$ and

$$
L=-i\hbar\frac{\partial}{\partial\phi}.
$$

Consequently

$$
L\psi=\hbar\psi,
\qquad
L\psi^*=-\hbar\psi^*.
$$

The two states are orthogonal. They are degenerate energy eigenstates, so their coefficients acquire the same overall time-dependent phase; equivalently, $[L,H]=0$ makes $\langle L\rangle$ constant. For the normalized state

$$
\frac{\sqrt5}{3}\psi+\frac23\psi^*,
$$

the [angular momentum of a complex-coordinate Gaussian state](../../../quantum-mechanics.md#angular-momentum-of-a-complex-coordinate-gaussian-state) is therefore

$$
\boxed{
\langle L\rangle_t
=\frac59\hbar-\frac49\hbar
=\frac\hbar9},
\qquad t>0.
$$

## 16C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="16c/solution">Solution</h3>

↑ **Parent:** [16C](#16c)

A gauge transformation is

$$
\boxed{A_\mu\longmapsto A_\mu+\partial_\mu\chi}.
$$

Because [partial derivatives](../../../calculus.md#partial-derivative) commute, the added contribution to $F_{\mu\nu}$ is

$$
\partial_\mu\partial_\nu\chi-\partial_\nu\partial_\mu\chi=0,
$$

so the [electromagnetic field tensor](../../../electromagnetism.md#electromagnetic-field-tensor) is gauge invariant.

Define

$$
E=-\nabla\Phi-\partial_tA,
\qquad
B=\nabla\times A.
$$

Since $\partial_0=c^{-1}\partial_t$ and $A_0=-\Phi/c$,

$$
\boxed{F_{0i}=-\frac{E_i}{c},
\qquad
F_{i0}=\frac{E_i}{c},
\qquad
F_{ij}=\epsilon_{ijk}B_k}.
$$

The identity

$$
\partial_\lambda F_{\mu\nu}
+\partial_\mu F_{\nu\lambda}
+\partial_\nu F_{\lambda\mu}=0
$$

follows directly from $F=dA$. Its spatial and mixed components are

$$
\nabla\cdot B=0,
\qquad
\nabla\times E=-\partial_tB.
$$

For the other two equations define the four-current

$$
\boxed{j^\mu=(c\rho,J)}.
$$

Then $\partial_\nu F^{0\nu}=\mu_0j^0$ gives

$$
\nabla\cdot E=\mu_0c^2\rho=\frac\rho{\epsilon_0},
$$

and $\partial_\nu F^{i\nu}=\mu_0j^i$ gives

$$
\nabla\times B-\frac1{c^2}\partial_tE=\mu_0J.
$$

This is the [Covariant Maxwell equation with the minus-plus-plus-plus metric](../../../electromagnetism.md#covariant-maxwell-equation-with-the-minus-plus-plus-plus-metric).

Using

$$
F^{\rho\sigma}F_{\rho\sigma}
=2\left(B^2-\frac{E^2}{c^2}\right),
$$

one finds

$$
\boxed{
T^{00}=\frac1{2\mu_0}
\left(B^2+\frac{E^2}{c^2}\right)
=\frac12\left(\frac{B^2}{\mu_0}+\epsilon_0E^2\right)}.
$$

This is the electromagnetic energy density.

For a null [vector](../../../vector-space.md#vector), the trace term in $T^{\mu\nu}k_\mu k_\nu$ vanishes. Put

$$
q^\rho=k_\mu F^{\mu\rho}.
$$

Antisymmetry gives $q\cdot k=0$. A [vector](../../../vector-space.md#vector) orthogonal to a null [vector](../../../vector-space.md#vector) has nonnegative Minkowski norm, so

$$
T^{\mu\nu}k_\mu k_\nu=\frac1{\mu_0}q^\rho q_\rho\geq0.
$$

Explicitly, in a frame with $k^\mu=\kappa(1,1,0,0)$,

$$
q^2=\kappa^2\left[
\left(B_3-\frac{E_2}{c}\right)^2
+\left(B_2+\frac{E_3}{c}\right)^2
\right].
$$

Hence the [null energy condition for the electromagnetic field](../../../electromagnetism.md#null-energy-condition-for-the-electromagnetic-field) is strict whenever the contraction is nonzero:

$$
\boxed{T^{\mu\nu}k_\mu k_\nu>0}.
$$

## 17D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="17d/a">a</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/a/solution">Solution</h4>

↑ **Parent:** [A](#17d/a)

For the test equation $y'=\lambda y$, write one numerical step as

$$
y_{n+1}=R(h\lambda)y_n.
$$

The [linear stability domain](../../../numerical-analysis.md#linear-stability-domain) is

$$
\mathcal S=\{z\in\mathbb C:|R(z)|\leq1\}.
$$

A method is A-stable when $\{z:\Re z\leq0\}\subseteq\mathcal S$.

Forward Euler has $R(z)=1+z$, so

$$
\boxed{\mathcal S_{\rm FE}=\{z:|1+z|\leq1\}}.
$$

This disk does not contain the whole left half-plane, so forward Euler is not A-stable. Backward Euler has $R(z)=(1-z)^{-1}$, so

$$
\boxed{\mathcal S_{\rm BE}=\{z:|1-z|\geq1\}}.
$$

It contains the left half-plane, and backward Euler is A-stable.

<h3 id="17d/b">b</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/b/solution">Solution</h4>

↑ **Parent:** [B](#17d/b)

A differential equation is stiff when it contains rapidly decaying modes on time scales much shorter than those of interest, forcing an explicit method to take very small steps for stability rather than accuracy.

Here

$$
\det(\lambda I-M)=\lambda^2+101\lambda+100
=(\lambda+1)(\lambda+100),
$$

so the decay rates are $1$ and $100$. For a negative real [eigenvalue](../../../linear-operator-theory.md#eigenvalue), forward Euler requires

$$
|1+h\lambda|\leq1,
$$

therefore the fast mode imposes

$$
\boxed{0<h\leq\frac2{100}=0.02}.
$$

For backward Euler the amplification factors are

$$
\frac1{1-h\lambda}=\frac1{1+h|\lambda|},
$$

whose [moduli](../../../complex-analysis.md#modulus) are at most one for every $h\geq0$. Thus

$$
\boxed{\text{backward Euler has no stability upper bound on }h}.
$$

This is the [stiff two-mode linear system](../../../numerical-analysis.md#stiff-two-mode-linear-system).

<h3 id="17d/c">c</h3>

↑ **Parent:** [17D](#17d)

<h4 id="17d/c/solution">Solution</h4>

↑ **Parent:** [C](#17d/c)

From the same value $y_n$, the two trial steps are

$$
y_F=(I+hM)y_n,
\qquad
 y_B=(I-hM)^{-1}y_n.
$$

The exact step and the two approximations expand as

$$
\begin{aligned}
e^{hM}y_n&=\left(I+hM+\frac12h^2M^2+O(h^3)\right)y_n,\\
y_F&=(I+hM)y_n,\\
y_B&=\left(I+hM+h^2M^2+O(h^3)\right)y_n.
\end{aligned}
$$

Thus their leading local errors have opposite signs, and the [Milne device for forward and backward Euler](../../../numerical-analysis.md#milne-device-for-forward-and-backward-euler) estimates either magnitude by

$$
\boxed{E_n=\frac12\lVert y_B-y_F\rVert
=\frac12h^2\lVert M^2y_n\rVert+O(h^3)}.
$$

Use backward Euler as the accepted step because it is A-stable. Reject a trial if $E_n$ exceeds the prescribed local tolerance; otherwise accept $y_B$ and choose, with a safety factor $s<1$,

$$
\boxed{h_{\rm new}=s h
\left(\frac{\mathrm{tol}}{E_n}\right)^{1/2}}.
$$

The small steps resolve the initial fast transient. Once its amplitude has decayed, the error estimator permits much larger steps, while the accepted backward-Euler evolution remains stable. This controls the error without paying the forward-Euler stability restriction throughout the integration.

## 18H

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="18h/solution">Solution</h3>

↑ **Parent:** [18H](#18h)

If the urn contains $g$ green balls, it contains $g+2$ red balls: both update rules preserve the difference $R-G=2$. Until absorption at $g=0$, the green count is therefore a birth-death chain with

$$
p_g=\mathbb P(g\to g-1)=\frac{g}{2g+2},
\qquad
q_g=\mathbb P(g\to g+1)=\frac{g+2}{2g+2}.
$$

The [function](../../../function.md)

$$
h(g)=\frac1{g+1}
$$

is harmonic, since

$$
p_gh(g-1)+q_gh(g+1)
=\frac1{2(g+1)}+\frac1{2(g+1)}=h(g).
$$

Let $\tau_0$ and $\tau_N$ be the hitting times of $0$ and $N$. The [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale), applied to the bounded stopped martingale $h(G_{n\wedge\tau_0\wedge\tau_N})$, gives

$$
h(m)=\mathbb P_m(\tau_0<\tau_N)
+\frac1{N+1}\mathbb P_m(\tau_N<\tau_0).
$$

Solving,

$$
\mathbb P_m(\tau_0<\tau_N)
=\frac{N-m}{N(m+1)}.
$$

Letting $N\to\infty$, the events on the left increase to eventual termination. The [harmonic hitting probability for the balanced-difference urn](../../../markov-process.md#harmonic-hitting-probability-for-the-balanced-difference-urn) is therefore

$$
\boxed{\mathbb P(\text{the process terminates})=\frac1{m+1}}.
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
