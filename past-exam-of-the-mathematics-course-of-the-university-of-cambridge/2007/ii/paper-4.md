# Paper 4

↑ **Parent:** [Ii](../ii.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2007/PaperII_4.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2007/PaperII_4.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3G](#3g)
  - [Solution](#3g/solution)
- [4G](#4g)
  - [Solution](#4g/solution)
- [5I](#5i)
  - [Solution](#5i/solution)
- [6B](#6b)
  - [Solution](#6b/solution)
- [7E](#7e)
  - [i](#7e/i)
    - [Solution](#7e/i/solution)
  - [ii](#7e/ii)
    - [Solution](#7e/ii/solution)
  - [iii](#7e/iii)
    - [Solution](#7e/iii/solution)
  - [Solution](#7e/solution)
- [8B](#8b)
  - [i](#8b/i)
    - [Solution](#8b/i/solution)
  - [ii](#8b/ii)
    - [Solution](#8b/ii/solution)
- [9C](#9c)
  - [a](#9c/a)
    - [Solution](#9c/a/solution)
  - [b](#9c/b)
    - [Solution](#9c/b/solution)
- [10A](#10a)
  - [Solution](#10a/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
  - [i](#11f/i)
    - [Solution](#11f/i/solution)
  - [ii](#11f/ii)
    - [Solution](#11f/ii/solution)
- [12G](#12g)
  - [Solution](#12g/solution)
- [13I](#13i)
  - [Solution](#13i/solution)
- [14E](#14e)
  - [i](#14e/i)
    - [Solution](#14e/i/solution)
  - [ii](#14e/ii)
    - [Solution](#14e/ii/solution)
- [15C](#15c)
  - [Solution](#15c/solution)
- [16G](#16g)
  - [Solution](#16g/solution)
- [17H](#17h)
  - [Solution](#17h/solution)
- [18F](#18f)
  - [Solution](#18f/solution)
- [19H](#19h)
  - [Solution](#19h/solution)
- [20H](#20h)
  - [Solution](#20h/solution)
- [21H](#21h)
  - [Solution](#21h/solution)
- [22G](#22g)
  - [Solution](#22g/solution)
- [23F](#23f)
  - [Solution](#23f/solution)
- [24H](#24h)
  - [i](#24h/i)
    - [Solution](#24h/i/solution)
  - [ii](#24h/ii)
    - [Solution](#24h/ii/solution)
- [25J](#25j)
  - [a](#25j/a)
    - [Solution](#25j/a/solution)
  - [b](#25j/b)
    - [Solution](#25j/b/solution)
  - [c](#25j/c)
    - [Solution](#25j/c/solution)
  - [d](#25j/d)
    - [Solution](#25j/d/solution)
- [26J](#26j)
  - [a](#26j/a)
    - [Solution](#26j/a/solution)
  - [b](#26j/b)
    - [Solution](#26j/b/solution)
  - [c](#26j/c)
    - [Solution](#26j/c/solution)
  - [d](#26j/d)
    - [Solution](#26j/d/solution)
  - [e](#26j/e)
    - [Solution](#26j/e/solution)
- [27I](#27i)
  - [Solution](#27i/solution)
- [28J](#28j)
  - [Solution](#28j/solution)
- [29I](#29i)
  - [Solution](#29i/solution)
- [30A](#30a)
  - [Solution](#30a/solution)
- [31B](#31b)
  - [Solution](#31b/solution)
- [32D](#32d)
  - [Solution](#32d/solution)
- [33A](#33a)
  - [Solution](#33a/solution)
- [34D](#34d)
  - [Solution](#34d/solution)
- [35E](#35e)
  - [Solution](#35e/solution)
- [36A](#36a)
  - [Solution](#36a/solution)
- [37B](#37b)
  - [i](#37b/i)
    - [Solution](#37b/i/solution)
  - [ii](#37b/ii)
    - [Solution](#37b/ii/solution)
  - [iii](#37b/iii)
    - [Solution](#37b/iii/solution)
  - [iv](#37b/iv)
    - [Solution](#37b/iv/solution)
- [38C](#38c)
  - [Solution](#38c/solution)
- [39C](#39c)
  - [a](#39c/a)
    - [Solution](#39c/a/solution)
  - [b](#39c/b)
    - [Solution](#39c/b/solution)

## 1F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

Let $p_1,\ldots,p_a$ be the [primes](../../../number-theory.md#prime-number) not exceeding $\sqrt x$, where $a=\pi(\sqrt x)$, and let $\Phi(x,a)$ count integers $1\leq n\leq x$ divisible by none of these primes. Every surviving integer other than $1$ is prime: a composite integer at most $x$ has a prime factor at most its square root. Conversely, the surviving primes are exactly those between $\sqrt x$ and $x$. Thus the [Legendre prime-counting formula](../../../number-theory.md#legendre-prime-counting-formula) is

$$
\boxed{\pi(x)=\Phi(x,\pi(\sqrt x))+\pi(\sqrt x)-1\quad(x\geq1).}
$$

By [inclusion-exclusion](../../../combinatorics.md#inclusion-exclusion-principle),

$$
\Phi(x,a)=\sum_{S\subseteq\{1,\ldots,a\}}(-1)^{|S|}
\left\lfloor\frac{x}{\prod_{i\in S}p_i}\right\rfloor,
$$

where the empty product is one. To cover literally every positive real $x$, replace the subtraction of $1$ by $\mathbf1_{\{x\geq1\}}$: for $0<x<1$, both counts are zero and there is no surviving integer $1$.

For $x=48$, the sieving primes are $2,3,5$. The surviving count is $48-(24+16+9)+(8+4+3)-1=13$. Consequently

$$
\boxed{\pi(48)=13+3-1=15.}
$$

## 2F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

The two-dimensional [Brouwer fixed-point theorem](../../../topological-analysis.md#brouwer-fixed-point-theorem) states that every continuous map from a closed filled triangle to itself has a fixed point. Use the triangle $\Delta=\{x\in\mathbb R^3:x_i\geq0,\ \sum_i x_i=1\}$, which lies in a two-dimensional affine plane. Strict positivity of the matrix entries ensures $(Ax)_i>0$ for every $x\in\Delta$. Therefore

$$
T(x)=\frac{Ax}{\sum_i(Ax)_i}
$$

is a continuous self-map of $\Delta$, in fact into its interior. Its fixed point $x$ satisfies $Ax=\lambda x$, where $\lambda=\sum_i(Ax)_i>0$. Since $x=T(x)$ lies in the interior, **$A$ has an [eigenvector](../../../linear-operator-theory.md#eigenvector) all of whose entries are strictly positive**. This is [positive matrix eigenvector from simplex normalization](../../../topological-analysis.md#positive-matrix-eigenvector-from-simplex-normalization); it uses strict positivity, not merely nonnegative entries.

## 3G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3g/solution">Solution</h3>

↑ **Parent:** [3G](#3g)

For a Euclidean circle with centre $c$ and radius $r$, two distinct finite points are inverse when they lie on the same ray from $c$ and their distances from $c$ have product $r^2$. Points on the circle are fixed, and $c$ and infinity are inverse to each other. In complex coordinates this uniquely defines [inversion in a circle](../../../group-theory.md#inversion-in-a-circle) by

$$
I_\Gamma(z)=c+\frac{r^2}{\overline z-\overline c}.
$$

Uniqueness follows from the ray and product conditions, including the specified centre–infinity pair; the formula also gives $I_\Gamma^2=\operatorname{id}$. A circle through infinity is a straight line in the complex plane; its inversion is reflection in that line, fixing infinity. For a line through $c$ with direction angle $\theta$, its formula is $c+e^{2i\theta}\overline{z-c}$.

Thus every inversion is an anti-[Möbius transformation](../../../group-theory.md#mobius-transformation), of the form $(a\overline z+b)/(c\overline z+d)$ with nonzero determinant. If $J(z)=\overline z$, write such an inversion as $M\circ J$ with $M$ a [Möbius transformation](../../../group-theory.md#mobius-transformation). Since $J\circ M\circ J$ is the Möbius transformation with conjugated coefficients, the product of two inversions is $M_1\circ(J\circ M_2\circ J)$, hence Möbius. Pairing consecutive inversions proves **every composition of an even number of inversions is a Möbius transformation**.

## 4G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4g/solution">Solution</h3>

↑ **Parent:** [4G](#4g)

A binary [linear-feedback shift register](../../../coding-theory.md#linear-feedback-shift-register) stores $L$ bits, shifts them at each clock step, and inserts a fixed linear combination over $\mathbb F_2$ of the stored bits. Its output obeys a recurrence $s_n+c_1s_{n-1}+\cdots+c_Ls_{n-L}=0$. Write its connection [polynomial](../../../polynomial.md) as $C(D)=1+c_1D+\cdots+c_LD^L$; the corresponding monic [feedback polynomial](../../../coding-theory.md#feedback-polynomial) is $z^LC(z^{-1})$.

The [Berlekamp-Massey algorithm](../../../coding-theory.md#berlekamp-massey-algorithm) maintains the shortest recurrence fitting the observed prefix. Initialize $C=B=1$, length $L=0$, displacement $m=1$, and previous nonzero discrepancy $b=1$. At symbol $n$, calculate $d=s_n+\sum_{j=1}^Lc_js_{n-j}$. If $d=0$, increase $m$. If $d\ne0$, save $T=C$ and replace $C$ by $C-(d/b)D^mB$. If $2L\leq n$, replace $L$ by $n+1-L$, $B$ by $T$, $b$ by $d$, and $m$ by $1$; otherwise only increase $m$. In the binary field subtraction equals addition. The shifted previous discrepancy [polynomial](../../../polynomial.md) cancels the current discrepancy while preserving earlier equations. A failed recurrence of length $L$ at position $n$ requires a corrected length at least $n+1-L$ when this exceeds $L$, explaining the length update. Thus the algorithm recovers the shortest compatible register; a known bound $L$ and at least $2L$ output symbols suffice to identify its minimal recurrence.

For the printed twelve-bit prefix, the nonzero discrepancies occur at positions $n=0,1,2,5,6,7$ (indexing from zero). The successive updated pairs $(L,C)$ are

$$
(1,1+D),\quad(1,1),\quad(2,1+D^2),\quad(4,1+D^2+D^3),\quad(4,1+D+D^2),\quad(4,1+D+D^4).
$$

All remaining discrepancies vanish. Therefore

$$
\boxed{s_n=s_{n-1}+s_{n-4}\quad(n\geq4),\qquad
z^4+z^3+1\text{ is the shortest compatible feedback polynomial}.}
$$

The first four observed bits are the fill. Length four is necessary: a length-three recurrence would need to hold already at $n=3$ and no such recurrence fits the prefix. Indeed the equations at $n=3,4,5$ force $c_2=1$, $c_1+c_3=0$, $c_1+c_3=1$, a contradiction. Finite observations cannot rule out longer nonminimal registers.

## 5I

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5i/solution">Solution</h3>

↑ **Parent:** [5I](#5i)

The normal-model [log-likelihood](../../../statistical-modelling.md#log-likelihood) is $-\frac n2\log\sigma^2-\|Y-X\beta\|^2/(2\sigma^2)$ up to a constant. Differentiating gives the [maximum-likelihood estimators](../../../statistical-modelling.md#maximum-likelihood-estimator)

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY,\qquad
\widehat\sigma^2=\frac1n\|Y-X\widehat\beta\|^2.}
$$

Let $P=X(X^TX)^{-1}X^T$. The fitted component $P\varepsilon$ and residual $(I-P)\varepsilon$ are orthogonal jointly normal projections and hence independent. Therefore

$$
\widehat\beta\sim N_p(\beta,\sigma^2(X^TX)^{-1}),\qquad
\frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-p},
\qquad \widehat\beta\ \text{and}\ \widehat\sigma^2\text{ are independent}.
$$

The prediction error $\widetilde y-y^*=x^{*T}(\widehat\beta-\beta)-\varepsilon^*$ is normal with mean zero and variance $\sigma^2\tau^2$, and is independent of the residual variance estimate. Dividing by the independent estimated standard deviation yields

$$
\boxed{\frac{\widetilde y-y^*}{\widetilde\sigma\tau}\sim t_{n-p}.}
$$

Thus the [prediction interval in a normal linear model](../../../statistical-inference.md#prediction-interval-in-a-normal-linear-model) is

$$
\boxed{\widetilde y\ \pm\ t_{n-p,1-\alpha/2}\,\widetilde\sigma
\sqrt{1+x^{*T}(X^TX)^{-1}x^*}.}
$$

The extra $1$ includes the new observation's independent noise; omitting it would give a confidence interval for its conditional mean instead.

## 6B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6b/solution">Solution</h3>

↑ **Parent:** [6B](#6b)

The terms $u$ and $\alpha v$ represent intrinsic exponential population growth. The losses $-uv$ and $-\alpha uv$ describe competition between the species; $-\epsilon_1u^2$ and $-\alpha\epsilon_2v^2$ describe crowding within each species. The positive constant $\alpha$ sets the relative time scale of the second population.

The four [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) in the nonnegative quadrant are

$$
(0,0),\quad (1/\epsilon_1,0),\quad(0,1/\epsilon_2),\quad
(u_*,v_*)=\left(\frac{1-\epsilon_2}{1-\epsilon_1\epsilon_2},
\frac{1-\epsilon_1}{1-\epsilon_1\epsilon_2}\right).
$$

The last follows by solving $\epsilon_1u+v=1$ and $u+\epsilon_2v=1$ and is strictly positive under the assumptions. The [Jacobian matrix](../../../calculus.md#jacobian-matrix) is

$$
J=\begin{pmatrix}1-v-2\epsilon_1u&-u\\-\alpha v&\alpha(1-u-2\epsilon_2v)\end{pmatrix}.
$$

At the origin its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1,\alpha>0$, so it is unstable. At the first single-species equilibrium they are $-1$ and $\alpha(1-1/\epsilon_1)<0$; at the second they are $1-1/\epsilon_2<0$ and $-\alpha$. Both are asymptotically stable. At coexistence,

$$
J_* =\begin{pmatrix}-\epsilon_1u_*&-u_*\\-\alpha v_*&-\alpha\epsilon_2v_*\end{pmatrix},
\qquad \det J_* =\alpha u_*v_*(\epsilon_1\epsilon_2-1)<0.
$$

Thus **coexistence is a saddle; either species-only equilibrium is stable, and extinction is unstable**. The saddle's stable manifold separates the competing basins of attraction.

## 7E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7e/i">i</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/i/solution">Solution</h4>

↑ **Parent:** [I](#7e/i)

Choose binary expansions $x=0.b_1b_2\ldots$ that do not end in an infinite string of ones. The [doubling map](../../../dynamical-systems.md#dyadic-transformation) deletes the first digit: $F(x)=0.b_2b_3\ldots$. Given $x$ and any neighbourhood of it, choose $N$ sufficiently large that its binary cylinder of length $N$ is small enough, and choose a point $y$ sharing that prefix but with a prescribed tail. After $N$ shifts, the tail of $y$ may be chosen arbitrarily in $[0,1)$. Choose it close to zero or close to one, whichever is at distance more than $1/3$ from $F^N(x)$. Then $|x-y|\leq2^{-N}$ but $|F^N(x)-F^N(y)|>1/3$. Hence **the map has sensitive dependence on initial conditions**, with a uniform separation constant. At dyadic endpoints the cylinder sharing the chosen terminating expansion still contains points arbitrarily close to the endpoint.

<h3 id="7e/ii">ii</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7e/ii)

Every nonempty relatively open interval contains a binary cylinder whose points share a finite prefix. Given nonempty open sets $U,V$, choose such a cylinder $C\subset U$ of length $N$. After $N$ binary shifts, $F^N(C)$ contains $[0,1)$ with the usual half-open cylinder convention. In particular, some point of $C$ maps into $V$. Thus **$F$ is topologically transitive**: $F^N(U)\cap V\ne\varnothing$. Equivalently, concatenate a prefix placing the point in $U$ with a tail placing its $N$th iterate in $V$.

<h3 id="7e/iii">iii</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7e/iii)

Given a binary cylinder with finite prefix $b_1\ldots b_N$, repeat a finite block beginning with that prefix indefinitely. The resulting binary sequence is periodic under the shift and represents a [periodic point of an interval map](../../../dynamical-systems.md#periodic-point-of-an-interval-map) of $F$ in the cylinder. If the given prefix consists entirely of ones, append a zero to the block so that its value is less than one; this still preserves the prefix. Since cylinders can be taken inside any nonempty open interval, **periodic points are dense**.

<h3 id="7e/solution">Solution</h3>

↑ **Parent:** [7E](#7e)

A point fixed by $F^4$ satisfies $(2^4-1)x\in\mathbb Z$, so $x=j/15$ for $0\leq j\leq14$. The points with period dividing two are $0,1/3,2/3$, corresponding to $j=0,5,10$. All other twelve points have least period four. Multiplication by two modulo fifteen groups them into the three cycles

$$
\boxed{(1/15,2/15,4/15,8/15),\quad
(3/15,6/15,12/15,9/15),\quad
(7/15,14/15,13/15,11/15).}
$$

This exhausts the requested four-cycles. The displayed order is the dynamical order, and cyclic changes of the starting point describe the same cycle.

## 8B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8b/i">i</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/i/solution">Solution</h4>

↑ **Parent:** [I](#8b/i)

For the Euler integral to converge directly, assume $\operatorname{Re}b>0$ and $\operatorname{Re}(c-b)>0$. At zero it is the [beta function](../../../complex-analysis.md#beta-function) $B(b,c-b)=\Gamma(b)\Gamma(c-b)/\Gamma(c)$. The normalization is therefore

$$
\boxed{K=\frac{\Gamma(c)}{\Gamma(b)\Gamma(c-b)}.}
$$

Outside these initial parameter conditions the [hypergeometric function](../../../complex-analysis.md#hypergeometric-function) is defined by analytic continuation wherever the parameters permit it.

<h3 id="8b/ii">ii</h3>

↑ **Parent:** [8B](#8b)

<h4 id="8b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8b/ii)

For $|z|<1$, differentiation under the convergent Euler integral gives

$$
F^{(n)}(a,b;c;0)=K(a)_n\int_0^1t^{b+n-1}(1-t)^{c-b-1}\,dt
=\frac{(a)_n(b)_n}{(c)_n},
$$

where $(a)_n=a(a+1)\cdots(a+n-1)$ and $(a)_0=1$ are [Pochhammer symbols](../../../combinatorics.md#rising-factorial). Thus its [Taylor series](../../../calculus.md#taylor-series) is

$$
F(a,b;c;z)=\sum_{n=0}^{\infty}\frac{(a)_n(b)_n}{(c)_n n!}z^n,
$$

which is symmetric in $a,b$. In the common region of parameter convergence for the two Euler integrals, this proves equality near zero. The [identity theorem](../../../complex-analysis.md#identity-theorem) extends it throughout their common principal slit domain, and parameter continuation gives the usual identity wherever both sides are defined:

$$
\boxed{F(a,b;c;z)=F(b,a;c;z).}
$$

## 9C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9c/a">a</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/a/solution">Solution</h4>

↑ **Parent:** [A](#9c/a)

Assume the spheroid is homogeneous, as implicit in the stated moments. Put $s=\sqrt{1-e^2}$ and map a uniform solid sphere by $(X_1,X_2,X_3)\mapsto(X_1,X_2,sX_3)$, preserving total mass by adjusting density. For the sphere, symmetry and its moment $2Ma^2/5$ give $\int X_i^2\,dm=Ma^2/5$ for each coordinate. The transformed squared-coordinate integrals are consequently $Ma^2/5,Ma^2/5,s^2Ma^2/5$. Reflection symmetry makes the off-diagonal inertia entries vanish. Thus

$$
\boxed{I_1=I_2=\frac{Ma^2}{5}(1+s^2)=\frac25Ma^2(1-e^2/2),
\qquad I_3=\frac25Ma^2.}
$$

The original PDF gives the correct solid-sphere factor $2/5$, rather than the converted TeX's $2/3$.

<h3 id="9c/b">b</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/b/solution">Solution</h4>

↑ **Parent:** [B](#9c/b)

Put $I=I_1=I_2$. The third of the [Euler equations for a torque-free rigid body](../../../classical-mechanics.md#euler-equations-for-a-torque-free-rigid-body) gives $\dot\omega_3=0$. The first two become $\dot\omega_1=-\Omega\omega_2$, $\dot\omega_2=\Omega\omega_1$, where

$$
\Omega=\frac{I_3-I}{I}\omega_3=\frac{e^2}{2-e^2}\omega_3.
$$

Therefore $\omega_1+i\omega_2=C e^{i\Omega t}$. In body coordinates, $L_1+iL_2=I C e^{i\Omega t}$ and $L_3=I_3\omega_3$ is constant. **The [angular momentum](../../../classical-mechanics.md#angular-momentum) precesses about the body symmetry axis**, with period

$$
\boxed{P=\frac{2\pi}{|\Omega|}=\frac{2\pi(2-e^2)}{e^2|\omega_3|}.}
$$

For positive $\omega_3$ this is the printed expression. In the inertial frame the torque-free [angular momentum](../../../classical-mechanics.md#angular-momentum) is constant; the precession here is its changing representation in the rotating body frame. If $e=0$ or $\omega_3=0$, this body-frame precession rate is zero.

## 10A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10a/solution">Solution</h3>

↑ **Parent:** [10A](#10a)

Here $H=\dot a/a=2/(3t)$, so the perturbation equation becomes $\ddot\delta+(4/3t)\dot\delta-(2/3t^2)\delta=0$. A trial $t^s$ gives $s(s-1)+(4/3)s-2/3=0$, with roots $2/3,-1$. Thus

$$
\boxed{\delta_k(t)=C_k t^{2/3}+D_k t^{-1}.}
$$

The pure growing mode obeys $\delta_k(t)/\delta_k(t_i)=a(t)/a(t_i)$; for generic data the decaying component eventually becomes negligible, though the growing-mode normalization must be determined from both initial data.

With $a(t_0)=1$, the physical wavelength is $2\pi a(t)/k$. Equating it to the [Hubble radius](../../../cosmology.md#hubble-radius) $c/H=3ct/2$, and using $k_0=2\pi H_0/c$, gives

$$
\frac{k_0}{k}\left(\frac{t_k}{t_0}\right)^{2/3}
=\frac{t_k}{t_0},\qquad
\boxed{t_k/t_0=(k_0/k)^3.}
$$

Growing-mode evolution from crossing to today multiplies the perturbation amplitude by $(t_0/t_k)^{2/3}=(k/k_0)^2$. Hence the supplied horizon-crossing variance gives

$$
\boxed{P(k)=\frac{A}{k^3}\left(\frac{k}{k_0}\right)^4
=\frac{A}{k_0^4}k.}
$$

This conclusion uses the stated matter-dominated growing-mode approximation over the relevant evolution, rather than an additional radiation-era transfer function.

## 11F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

Reduce the [polynomial](../../../polynomial.md) modulo $p$, obtaining a nonzero degree-$d$ [polynomial](../../../polynomial.md) over the field $\mathbb F_p$. If $a$ is a root, [polynomial](../../../polynomial.md) division gives $\bar f(X)=(X-a)h(X)$. Any different root $b$ is a root of $h$, because $b-a\ne0$ is invertible. Induction on degree therefore proves **there are at most $d$ distinct roots modulo $p$**.

Every nonzero residue is a root of $X^{p-1}-1$ by [Fermat's little theorem](../../../number-theory.md#fermat-little-theorem). The difference between this monic [polynomial](../../../polynomial.md) and the product over all its $p-1$ nonzero roots has degree at most $p-2$, yet has $p-1$ roots. The root bound forces it to vanish identically over $\mathbb F_p$. Thus all coefficients of the corresponding integer [polynomial](../../../polynomial.md) are divisible by $p$.

For the requested failure modulo $p^2$, take $p=7$: $6!+1=721=7\cdot103$, and $103$ is not divisible by seven. Hence **the prime-square strengthening fails**, even though some special primes do satisfy it.

<h3 id="11f/i">i</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/i/solution">Solution</h4>

↑ **Parent:** [I](#11f/i)

Compare constant terms in the [polynomial](../../../polynomial.md) identity proved above. The constant term of $X^{p-1}-1$ is $-1$, while that of the product is $(-1)^{p-1}(p-1)!$. For odd $p$, this gives $(p-1)!\equiv-1\pmod p$. For $p=2$, the same conclusion holds because $1\equiv-1\pmod2$. Thus [Wilson's theorem](../../../number-theory.md#wilson-s-theorem) follows:

$$
\boxed{(p-1)!+1\equiv0\pmod p.}
$$

<h3 id="11f/ii">ii</h3>

↑ **Parent:** [11F](#11f)

<h4 id="11f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11f/ii)

For odd $p$, pair the terms with denominators $j$ and $p-j$. Since both denominators are coprime to $p$,

$$
\frac1j+\frac1{p-j}=\frac{p}{j(p-j)}
$$

has numerator divisible by $p$ and denominator not divisible by $p$. Summing these $(p-1)/2$ pairs over a common denominator coprime to $p$ gives a numerator divisible by $p$. Cancelling common factors cannot remove a factor $p$, since none occurs in the denominator. Therefore **the numerator of $u_p$ in lowest terms is divisible by $p$**. Equivalently, inversion permutes the nonzero residues and $\sum_{j=1}^{p-1}j^{-1}\equiv\sum_{j=1}^{p-1}j\equiv0\pmod p$.

## 12G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12g/solution">Solution</h3>

↑ **Parent:** [12G](#12g)

A [Kleinian group](../../../topological-group.md#kleinian-group) is a discrete subgroup of $\operatorname{PSL}_2(\mathbb C)$, acting as orientation-preserving hyperbolic isometries of $\mathbb H^3$ and as Möbius transformations of its boundary sphere. Its limit set consists of the accumulation points on the boundary of an orbit $Gx$ with $x\in\mathbb H^3$; it is independent of that interior base point and is closed. A nonidentity parabolic transformation is conjugate to $z\mapsto z+c$, $c\ne0$. Its iterates on the upper half-space tend to its unique fixed boundary point, infinity in these coordinates. Consequently **every parabolic fixed point belongs to the limit set**.

The displayed matrix has determinant one, trace two, and is not the identity because $a\ne0$. Its fixed-point equation is $a(z-w)^2=0$, so it has exactly the double fixed point $w$. It is therefore parabolic, and **its fixed point is $w$**.

The determinant-one Gaussian-integer matrices form a subgroup of $\operatorname{SL}_2(\mathbb C)$. They are discrete because their entries lie in a discrete lattice: a matrix sufficiently near the identity has every entry equal to the corresponding identity entry. Passing through the quotient by $\{\pm I\}$ preserves discreteness, so their Möbius transformations form a Kleinian group.

For $w=n/r$, $n=p+iq$ and $r\ne0$, set $a=r^2$. This gives the [Gaussian-integer parabolic construction](../../../topological-group.md#gaussian-integer-parabolic-construction)

$$
\boxed{T\ \leftrightarrow\ \begin{pmatrix}1+rn&-n^2\\r^2&1-rn\end{pmatrix}.}
$$

All entries lie in $\mathbb Z[i]$, the determinant is one, and its parabolic fixed point is $n/r=w$. The points with nonzero $p,q,r$ are dense in the finite complex plane, and their closure on the sphere includes infinity. Since the limit set is closed and contains all these parabolic fixed points, **the limit set is the whole Riemann sphere**.

## 13I

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="13i/solution">Solution</h3>

↑ **Parent:** [13I](#13i)

Use the [exponential dispersion family](../../../exponential-family.md#exponential-dispersion-model) convention $f(y)=\exp\{[y\theta-b(\theta)]/\phi+c(y,\phi)\}$. For the [Gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution), take

$$
\phi=\alpha^{-1},\qquad \theta=-\lambda/\alpha<0,
\qquad b(\theta)=-\log(-\theta),
$$



$$
c(y,\phi)=(\alpha-1)\log y+\alpha\log\alpha-\log\Gamma(\alpha).
$$

Substitution reproduces the gamma density exactly. Differentiating its normalization with respect to $\theta$ yields $\mathbb EY=b'(\theta)$ and $\operatorname{Var}Y=\phi b''(\theta)$: the first identity follows from zero mean score, and differentiation again gives the variance. Therefore

$$
\boxed{\mathbb EY=\alpha/\lambda,\qquad\operatorname{Var}Y=\alpha/\lambda^2.}
$$

The [canonical link function](../../../statistical-modelling.md#canonical-link-function) is $g(\mu)=\theta=-1/\mu$. Some conventions reverse the sign and call $1/\mu$ the reciprocal link; this only reverses the regression coefficients. We retain the genuine natural parameter $\theta=-1/\mu$.

In the [Gamma regression with canonical link](../../../statistical-modelling.md#gamma-regression-with-canonical-link), $\eta_i=x_i^T\beta<0$ and $\mu_i=-1/\eta_i$. Differentiating the independent-observation log-likelihood gives

$$
\boxed{U(\beta)=\phi^{-1}X^T(y-\mu),\qquad
I(\beta)=\phi^{-1}X^T\operatorname{diag}(\mu_i^2)X.}
$$

Here $d\mu_i/d\eta_i=\mu_i^2$, so the negative Hessian equals this information matrix. [Fisher scoring](../../../statistical-modelling.md#scoring-algorithm) or Newton iteration is

$$
\beta_{\rm new}=\beta+I(\beta)^{-1}U(\beta),
$$

with the means and information recalculated at each iteration; damping can preserve $X\beta<0$ and increase the likelihood. Full column rank makes the information positive definite for positive means.

The saturated model has mean $y_i$. Subtracting fitted from saturated log-likelihood yields the unscaled [deviance](../../../exponential-family.md#exponential-family-deviance)

$$
\boxed{D=2\sum_i\left[\frac{y_i-\widehat\mu_i}{\widehat\mu_i}
-\log\frac{y_i}{\widehat\mu_i}\right].}
$$

Twice the actual log-likelihood ratio is $D/\phi$. In particular, the printed parenthetical $\widehat\mu=X\widehat\beta$ is incorrect for this nonidentity link: **$X\widehat\beta$ estimates $\eta$, and $\widehat\mu_i=-1/(x_i^T\widehat\beta)$**.

## 14E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="14e/i">i</h3>

↑ **Parent:** [14E](#14e)

<h4 id="14e/i/solution">Solution</h4>

↑ **Parent:** [I](#14e/i)

The fixed-point equation is $x[ax^2+bx+\mu-1]=0$. Thus

$$
\boxed{x=0,\qquad x_\pm=\frac{-b\pm\sqrt{b^2+4a(1-\mu)}}{2a}}
$$

when the discriminant is nonnegative. At zero the multiplier is $F'(0)=\mu$, so it is linearly stable for $-1<\mu<1$ and unstable for $|\mu|>1$. At a nonzero fixed point, eliminate $\mu$ to obtain the branch and its multiplier:

$$
\mu=1-bx-ax^2,\qquad M=1+bx+2ax^2.
$$

The branch is stable precisely when $-2<x(b+2ax)<0$. These formulas specify stability throughout the diagram, including any extra flip points outside the region requested.

If $b=0$ and $a>0$, the two nonzero branches $x=\pm\sqrt{(1-\mu)/a}$ exist for $\mu<1$ and have multiplier $3-2\mu>1$. Thus $\mu=1$ is a subcritical [pitchfork bifurcation](../../../dynamical-systems.md#pitchfork-bifurcation-normal-form). If $b\ne0$, the branch through zero has $x\sim(1-\mu)/b$ and $M\sim2-\mu$; its stability exchanges with zero at $\mu=1$, a [transcritical bifurcation](../../../dynamical-systems.md#transcritical-bifurcation). The two nonzero roots meet at

$$
\mu_{\rm sn}=1+b^2/(4a),\qquad x_{\rm sn}=-b/(2a),
$$

where $M=1$. The graph of $\mu(x)$ has nonzero second derivative $-2a$, proving a [saddle-node bifurcation](../../../dynamical-systems.md#saddle-node-bifurcation). At zero and $\mu=-1$, the multiplier is $-1$, indicating a [period-doubling bifurcation](../../../dynamical-systems.md#period-doubling-bifurcation); generically its nondegeneracy coefficient is $a+b^2$. If $a+b^2=0$, necessarily $b\ne0$ here, composition at $\mu=-1$ instead gives $F^2(x)-x=4b^4x^5+O(x^6)$. For $\delta=\mu+1>0$ small, the leading return equation is $-2\delta x+4b^4x^5=0$, producing a two-cycle with leading amplitudes $x\sim\pm[\delta/(2b^4)]^{1/4}$. Its return multiplier is $1+8\delta+o(\delta)>1$. Thus this special case still has a flip bifurcation, but it is degenerate and subcritical rather than the generic cubic normal form.

For $a,b>0$, the fold lies above $\mu=1$. Between it and the transcritical point, the branch $-b/(2a)<x<0$ is stable provided its multiplier remains above $-1$, while the other branch is unstable. For $a,b<0$, the fold lies below $\mu=1$: immediately above it the branch $x<-b/(2a)$ is stable and the branch between $-b/(2a)$ and zero is unstable; the branch crossing zero becomes stable for $\mu>1$. All these statements are subject to the displayed exact multiplier criterion if the diagram is extended. The sketch uses representative parameter values and stops before additional flips, as stipulated.

<a id="14e/i/image-fixed-point-branches-and-stability-for-three-representative-cubic-maps-with-folds-transcritical-or-pitchfork-crossings-and-the-origin-flip"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4-fixed-point-bifurcations.png)

**[Figure 1](#14e/i/image-fixed-point-branches-and-stability-for-three-representative-cubic-maps-with-folds-transcritical-or-pitchfork-crossings-and-the-origin-flip). Fixed-point branches and stability for three representative cubic maps, with folds, transcritical or pitchfork crossings, and the origin flip**.

<h3 id="14e/ii">ii</h3>

↑ **Parent:** [14E](#14e)

<h4 id="14e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#14e/ii)

Separate fixed points from roots of $F^2(x)=x$. Fixed points are zero, and $\pm\sqrt{\mu-1}$ for $\mu\geq1$. The remaining factors in the given factorization yield first $x^2=\mu+1$. For $\mu>-1$ these form the symmetric two-cycle $\{\sqrt{\mu+1},-\sqrt{\mu+1}\}$ because $F(x)=-x$. Its multiplier is $(-2\mu-3)^2>1$, so **this cycle is always unstable**.

The quartic factor gives $s^2-\mu s+1=0$ for $s=x^2$, hence $s_\pm=(\mu\pm\sqrt{\mu^2-4})/2$. Positive roots require $\mu\geq2$. At $\mu=2$ they give the fixed points $\pm1$, not genuine cycles. For $\mu>2$, $s_+s_-=1$ and $F(\sqrt{s_+})=\sqrt{s_-}$, giving exactly two additional cycles:

$$
\boxed{\{\sqrt{s_+},\sqrt{s_-}\},\qquad
\{-\sqrt{s_+},-\sqrt{s_-}\}.}
$$

There are therefore at most three two-cycles. For either of the latter two, its multiplier is

$$
(\mu-3s_+)(\mu-3s_-)
=(s_--2s_+)(s_+-2s_-)=9-2\mu^2.
$$

Thus **they are stable for $2<\mu<\sqrt5$ and unstable for $\mu>\sqrt5$**, with a flip at $\sqrt5$. The nonzero fixed points have multiplier $3-2\mu$, hence are stable for $1<\mu<2$. Zero is stable for $-1<\mu<1$. At $\mu=1$ there is a supercritical pitchfork; at $\mu=2$ both nonzero fixed points lose stability to these two-cycles. The symmetric unstable cycle terminates at zero at the subcritical flip $\mu=-1$. These are the [cubic map period-two branches](../../../dynamical-systems.md#cubic-map-period-two-branches).

<a id="14e/ii/image-fixed-points-and-all-three-two-cycle-branches-of-x-maps-to-x-times-mu-minus-x-squared-with-stable-branches-solid-and-unstable-branches-dashed"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4-two-cycle-bifurcations.png)

**[Figure 2](#14e/ii/image-fixed-points-and-all-three-two-cycle-branches-of-x-maps-to-x-times-mu-minus-x-squared-with-stable-branches-solid-and-unstable-branches-dashed). Fixed points and all three two-cycle branches of x maps to x times (mu minus x squared), with stable branches solid and unstable branches dashed**.

Beyond $\sqrt5$ one expects period-four branches and further period doublings, potentially a cascade toward chaotic behaviour. This local argument does not claim that every larger parameter is chaotic; periodic windows and escape may also occur.

## 15C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="15c/solution">Solution</h3>

↑ **Parent:** [15C](#15c)

The [Hamilton equations](../../../classical-mechanics.md#hamilton-s-equations) are $\dot q=p/m$ and $\dot p=-V_q$. Applying the chain rule to $H(q,p,\lambda(t))$, their two phase-space contributions cancel, giving $\dot H=V_\lambda\dot\lambda=H_\lambda\dot\lambda$.

For fixed $\lambda$, a closed periodic orbit of energy $E$ has $p=\pm\sqrt{2m(E-V)}$. Thus its [action variable](../../../classical-mechanics.md#action-variable) is

$$
I(E,\lambda)=\frac1{2\pi}\oint p\,dq
=\frac{\sqrt{2m}}{2\pi}\oint\pm\sqrt{E-V(q,\lambda)}\,dq.
$$

The sign matches the direction on each half of the orbit, making the enclosed phase-plane area positive. Since $dq=\dot q\,dt=p\,dt/m$, differentiating under the integral gives

$$
\boxed{I_E=\frac1{2\pi}\oint\frac m p\,dq=\frac\tau{2\pi},
\qquad I_\lambda=-\frac1{2\pi}\oint V_\lambda\,dt.}
$$

For slowly varying $\lambda$, the exact energy equation averaged over a nearly frozen cycle gives $d\langle H\rangle/dt=\langle V_\lambda\rangle\dot\lambda$ to the retained adiabatic order. Using $E=\langle H\rangle$, the two chain-rule terms therefore cancel:

$$
\frac{dI}{dt}=\frac\tau{2\pi}\langle V_\lambda\rangle\dot\lambda
-\frac1{2\pi}\oint V_\lambda\,dt\,\dot\lambda=0.
$$

Here the angle brackets differentiate the explicit parameter dependence along the frozen cycle, not an independently chosen family of energies. **The action is an adiabatic invariant**, with errors beyond the slow-cycle approximation.

For $V=\lambda q^{2n}$, scale $q=(E/\lambda)^{1/(2n)}s$. Then

$$
I=\frac{2\sqrt{2m}}\pi E^{(n+1)/(2n)}\lambda^{-1/(2n)}
\int_0^1\sqrt{1-s^{2n}}\,ds.
$$

The integral is a positive constant depending only on $n$. Constancy of $I$ gives $E^{n+1}/\lambda$ constant, hence

$$
\boxed{\langle H\rangle=C\lambda^{1/(n+1)}.}
$$

## 16G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="16g/solution">Solution</h3>

↑ **Parent:** [16G](#16g)

A binary relation $R$ on a set is a [well-founded relation](../../../set-theory.md#well-founded-relation) if every nonempty subset has an $R$-minimal member, that is, a member with no predecessor inside that subset. Here write $xRy$ when $x\in f(y)$.

Suppose $R$ is well-founded and fix any $g:\mathcal P(b)\to b$. Call a partial function $h:D\to b$ consistent if $D$ is downward closed under $R$ and $h(y)=g(\{h(x):x\in f(y)\})$ for $y\in D$. Two consistent partial functions agree on their common domain: otherwise the set of points where they disagree has a minimal member, all of whose predecessors are in both domains and agree, so applying $g$ gives agreement at that member as well, a contradiction. Thus the union of all consistent partial functions is itself a function $h:D\to b$, on a downward-closed domain, and remains consistent. This union is a set, because every such graph is a subset of $a\times b$.

If $D\ne a$, choose a minimal member $y$ of $a\setminus D$. All predecessors of $y$ lie in $D$, so extend $h$ to $y$ by the prescribed value $g(\{h(x):x\in f(y)\})$. The enlarged domain remains downward closed and consistent, contradicting the union's maximality. Hence $D=a$. The same minimal-disagreement argument proves uniqueness. This establishes the required recursion directly, without invoking an unproved [well-founded recursion](../../../set-theory.md#well-founded-recursion) theorem.

Conversely, if $R$ is not well-founded, choose a nonempty $S\subset a$ such that each $y\in S$ has a predecessor in $S$. Let $T$ be all points reachable from $S$ by a finite chain of upward $R$ steps, including $S$. Then

$$
y\in T\quad\Longleftrightarrow\quad f(y)\cap T\ne\varnothing.
$$

For a point reached by a nonempty chain, its preceding point is in $T$; for a point of $S$, use its predecessor in $S$. The converse follows by appending the final step to a chain. Choose $b=\{0,1\}$ and $g(B)=1$ if $1\in B$, zero otherwise. Both $h_0\equiv0$ and $h_1=\mathbf1_T$ satisfy the required recursion, and they differ because $S\ne\varnothing$. This contradicts recursiveness. Therefore **$f$ is recursive exactly when its predecessor relation is well-founded**, the characterization of a [recursive powerset mapping](../../../set-theory.md#recursive-powerset-mapping).

## 17H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="17h/solution">Solution</h3>

↑ **Parent:** [17H](#17h)

Let $d_v$ be the vertex degrees and let $r_{ij}$ count common neighbours of distinct vertices. Count unoriented length-two paths by their centre or endpoints:

$$
P_2=\sum_v\binom{d_v}{2}=\sum_{i<j}r_{ij}.
$$

If no four-cycle occurs, $r_{ij}\leq1$, so $P_2\leq\binom n2$. By [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), $P_2\geq\frac12[(2m)^2/n-2m]$. Solving $4m^2-2nm\leq n^2(n-1)$ gives

$$
\boxed{m\leq\frac n4(1+\sqrt{4n-3}).}
$$

If $m\geq n(n-1)/4$, the same bound and monotonicity of $2m^2/n-m$ in this range give $P_2\geq n(n-1)(n-3)/8$ (the small $n$ cases are immediate). Every pair of common neighbours supplies a four-cycle, counted twice through its two opposite vertex pairs, so [four-cycle counting by common neighbours](../../../graph-theory.md#four-cycle-counting-by-common-neighbours) gives

$$
C_4(G)=\frac12\sum_{i<j}\binom{r_{ij}}2.
$$

Let $N=\binom n2$ and $\bar r=P_2/N\geq(n-3)/4$. Convexity of $r(r-1)/2$ gives $C_4\geq(N/2)\binom{\bar r}2$. For $n\geq7$, this function is increasing on the needed range, giving

$$
\boxed{C_4(G)\geq\frac12\binom n2\binom{(n-3)/4}{2}.}
$$

For $3\leq n\leq6$ the printed right-hand side is nonpositive and the conclusion is trivial. **At $n=2$ the printed cycle bound is false**: a single edge meets the edge hypothesis but has no four-cycles, while the right-hand side is $5/64>0$. Thus this particular bound needs the intended $n\geq3$ restriction; the other counting statements above do not have this defect.

On four chosen vertices there are three distinct cycle subgraphs, each present with probability $2^{-4}$ in the stated random graph. Extra edges do not destroy these subgraphs. Therefore

$$
\boxed{\mathbb EC_4=\frac3{16}\binom n4.}
$$

For positive expectation, [Markov inequality](../../../probability-inequality.md#markov-inequality) gives

$$
P(C_4\leq(1+2\epsilon)\mathbb EC_4)
\geq1-\frac1{1+2\epsilon}
=\frac{2\epsilon}{1+2\epsilon}\geq\epsilon
$$

when $0<\epsilon<1/2$. If $n<4$, the cycle count is identically zero and the requested event has probability one.

## 18F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="18f/solution">Solution</h3>

↑ **Parent:** [18F](#18f)

The squared Vandermonde product defining the [polynomial discriminant](../../../galois-theory.md#polynomial-discriminant) is symmetric in all roots. By the fundamental theorem of [symmetric polynomials](../../../polynomial.md#symmetric-polynomial), it is a [polynomial](../../../polynomial.md) in the elementary symmetric functions, which are the signed coefficients of the monic [polynomial](../../../polynomial.md). Hence it is a [polynomial](../../../polynomial.md) function of those coefficients over the base field.

For $f=X^3+pX+q$, $\Delta(f)=-\operatorname{Res}(f,f')$. Eliminating the two leading rows in the Sylvester determinant reduces the resultant to

$$
\operatorname{Res}(f,f')=\det\begin{pmatrix}-2p&-3q&0\\0&-2p&-3q\\3&0&p\end{pmatrix}
=4p^3+27q^2.
$$

Thus

$$
\boxed{\Delta(X^3+pX+q)=-4p^3-27q^2.}
$$

For $X^3-3X+1$, the only possible rational roots are $\pm1$, and neither is a root. The cubic is therefore irreducible, so its [Galois group](../../../galois-theory.md#galois-group) is a transitive subgroup of $S_3$. Its discriminant is $81=9^2$. The Vandermonde product changes sign under odd permutations, and its square being a rational square implies that the product itself is rational; hence all Galois permutations are even. The only transitive subgroup of $A_3$ is $A_3$ itself. Consequently, writing $L$ for its splitting field,

$$
\boxed{\operatorname{Gal}(L/\mathbb Q)\cong C_3.}
$$

## 19H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="19h/solution">Solution</h3>

↑ **Parent:** [19H](#19h)

We consider finite-dimensional continuous complex representations of [SU(2)](../../../topological-group.md#su-2-group). Its maximal [torus](../../../topology.md#torus) is $\operatorname{diag}(e^{i\theta},e^{-i\theta})$. The [irreducible representations](../../../representation-theory.md#irreducible-representation) are

$$
\boxed{V_n=\operatorname{Sym}^n(\mathbb C^2),\qquad n=0,1,2,\ldots,\qquad \dim V_n=n+1.}
$$

They may be realized as homogeneous [polynomials](../../../polynomial.md) of degree $n$ in two variables, with the induced linear substitution action. Their [torus](../../../topology.md#torus) weights are $n,n-2,\ldots,-n$, each once. The centre $-I$ acts by $(-1)^n$, so precisely the even-$n$ representations descend to [SO(3)](../../../linear-algebra.md#so-3-group). In physics $n=2j$ labels integral or half-integral spin $j$.

Here is a classification argument. Average any positive definite Hermitian form over the compact group using normalized [Haar measure](../../../measure-theory.md#haar-measure). The averaged form is invariant, so the orthogonal complement of an [invariant subspace](../../../representation-theory.md#invariant-subspace) is invariant. Repeatedly splitting gives complete reducibility. Differentiate an [irreducible representation](../../../representation-theory.md#irreducible-representation) and complexify to the [Lie algebra](../../../lie-algebra.md) $\mathfrak{sl}_2$, with generators $H,E,F$ satisfying $[H,E]=2E$, $[H,F]=-2F$, and $[E,F]=H$. [Torus](../../../topology.md#torus) periodicity gives integer $H$-weights. Choose a vector $v$ of maximal weight $n$; then $Ev=0$. Induction on $k$ using the commutators gives

$$
EF^kv=k(n-k+1)F^{k-1}v.
$$

The chain terminates: if $F^{p}v\ne0$ and $F^{p+1}v=0$, the displayed formula forces $n=p\geq0$. The vectors $v,Fv,\ldots,F^nv$ have distinct weights, span an invariant subrepresentation, and hence span the [irreducible representation](../../../representation-theory.md#irreducible-representation). Their generator action agrees with $\operatorname{Sym}^n\mathbb C^2$. Invariance under the [Lie algebra](../../../lie-algebra.md) is equivalent to invariance under the connected group, completing the classification. Conversely, a nonzero [invariant subspace](../../../representation-theory.md#invariant-subspace) of a [symmetric power](../../../linear-algebra.md#symmetric-power) contains a weight vector by projection onto [torus](../../../topology.md#torus) weights. Raising it to the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) and then lowering generates every monomial, proving that the [symmetric power](../../../linear-algebra.md#symmetric-power) is irreducible.

The character on the [torus](../../../topology.md#torus) is

$$
\chi_n(\theta)=\sum_{k=0}^n e^{i(n-2k)\theta}
=\frac{\sin((n+1)\theta)}{\sin\theta},
$$

with the endpoints interpreted by continuity. Every representation has a unique decomposition $V\cong\bigoplus_{n\geq0}m_nV_n$. Its multiplicities can be computed from character inner products,

$$
\boxed{m_n=\int_{\mathrm{SU}(2)}\chi_V(g)\overline{\chi_n(g)}\,dg
=\frac2\pi\int_0^\pi\chi_V(\theta)\chi_n(\theta)\sin^2\theta\,d\theta.}
$$

The sine orthogonality directly verifies orthonormality of the irreducible characters. Alternatively, if $w_k$ is the dimension of the weight-$k$ subspace, the weight lists give $w_n=m_n+m_{n+2}+\cdots$, so **$m_n=w_n-w_{n+2}$** for $n\geq0$. This gives a constructive decomposition from [torus](../../../topology.md#torus) weights. In particular, multiplying weight characters yields the [Clebsch-Gordan decomposition](../../../quantum-mechanics.md#clebsch-gordan-decomposition) $V_m\otimes V_n\cong V_{m+n}\oplus V_{m+n-2}\oplus\cdots\oplus V_{|m-n|}$. Arbitrary unitary Hilbert-space representations of this compact group similarly decompose into Hilbert [direct sums](../../../vector-space.md#direct-sum) of these finite-dimensional irreducibles; the finite-dimensional statement above is the standard representation-theory setting.

## 20H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="20h/solution">Solution</h3>

↑ **Parent:** [20H](#20h)

Since $\mathcal O=\mathbb Z[\theta]$, reduction gives $\mathcal O/p\mathcal O\cong\mathbb F_p[X]/(\bar g)$. The maximal ideals of this quotient are precisely those generated by the distinct irreducible factors $\bar g_i$. Their inverse images are therefore

$$
\boxed{\mathfrak p_i=(p,g_i(\theta)),}
$$

the distinct [prime ideals](../../../commutative-algebra.md#prime-ideal) above $p$. In fact $\mathcal O/\mathfrak p_i\cong\mathbb F_p[X]/(\bar g_i)$ is a field of size $p^{\deg\bar g_i}$. Every prime containing $p$ arises this way; independence of the choice of lift $g_i$ follows because another lift differs by a multiple of $p$.

To prove the ideal factorization, set $J=\prod_i\mathfrak p_i^{e_i}$. A generator of the product either contains a factor $p$, and hence lies in $p\mathcal O$, or is the product $\prod_i g_i(\theta)^{e_i}$. The latter also lies in $p\mathcal O$, since its [polynomial](../../../polynomial.md) reduces to $\bar g$ and $g(\theta)=0$. Thus $J\subset p\mathcal O$. The [ideal norm](../../../algebraic-number-theory.md#ideal-norm) is multiplicative for nonzero ideals in the [ring of integers](../../../algebraic-number-theory.md#ring-of-integers); hence

$$
N(J)=\prod_i p^{e_i\deg\bar g_i}=p^{\deg g}
=N(p\mathcal O).
$$

Equal finite indices together with the containment imply equality. Therefore

$$
\boxed{p\mathcal O=\prod_i\mathfrak p_i^{e_i}.}
$$

This proves the [Dedekind factorization theorem](../../../algebraic-number-theory.md#dedekind-factorization-theorem) in the stated monogenic case by containment and norms, rather than assuming the desired factorization.

## 21H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="21h/solution">Solution</h3>

↑ **Parent:** [21H](#21h)

Cut the second circle factor at $p,q$. This divides the [torus](../../../topology.md#torus) into two annuli whose boundary circles are exactly the two collapsed circles. Collapsing each [annulus](../../../topology.md#annulus-mathematics)'s two boundaries separately produces a two-sphere; the two spheres then share their two poles. In particular, the two collapsed circles give two distinct vertices, not a single common collapsed point.

For an explicit [cellular homology](../../../homology.md#cellular-chain-complex) calculation, each suspended circle contributes one edge from the first vertex to the second and one two-cell attached with zero cellular boundary. Thus $C_0\cong\mathbb Z^2$, $C_1\cong\mathbb Z^2$, $C_2\cong\mathbb Z^2$, with no higher cells. Both edges have boundary $v_q-v_p$, so $\partial_1$ has rank one and kernel generated by the difference of the edges. Each two-cell's attaching loop traverses its edge in opposite directions, so $\partial_2=0$. Consequently the [homology of a torus with two parallel circles collapsed](../../../homology.md#homology-of-a-torus-with-two-parallel-circles-collapsed) is

$$
\boxed{H_0\cong\mathbb Z,\quad H_1\cong\mathbb Z,\quad
H_2\cong\mathbb Z^2,\quad H_k=0\ (k\geq3).}
$$

Collapsing either connecting edge as a maximal tree also exhibits the [homotopy](../../../algebraic-topology.md#homotopy) type $S^1\vee S^2\vee S^2$.

## 22G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="22g/solution">Solution</h3>

↑ **Parent:** [22G](#22g)

For a bounded operator on a complex [Banach space](../../../banach-space.md), the [resolvent set](../../../functional-analysis.md#resolvent-set-of-an-operator) is $\rho(T)=\{\lambda:\lambda I-T\text{ is bijective with bounded inverse}\}$, and the [resolvent operator](../../../functional-analysis.md#resolvent-of-an-operator) is $R_T(\lambda)=(\lambda I-T)^{-1}$. The [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) is its complement $\sigma(T)=\mathbb C\setminus\rho(T)$; the [point spectrum](../../../linear-operator-theory.md#point-spectrum) consists of $\lambda$ with $\ker(\lambda I-T)\ne0$. For a real Banach space these definitions use its complexification.

If $|\lambda|>\|T\|$, the norm-convergent [Neumann series](../../../banach-algebra.md#neumann-series) gives $R_T(\lambda)=\lambda^{-1}\sum_{n\geq0}(T/\lambda)^n$, so the spectrum is bounded. If $\lambda_0\in\rho(T)$, factor

$$
\lambda I-T=(\lambda_0I-T)[I+(\lambda-\lambda_0)R_T(\lambda_0)].
$$

The second factor is invertible by a Neumann series whenever $|\lambda-\lambda_0|\|R_T(\lambda_0)\|<1$. Thus the resolvent set is open and **the spectrum is closed and bounded**.

The point spectrum need not be closed. On $\ell^2$, define $Te_n=e_n/n$. Every $1/n$ is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue), but zero is not: $Tx=0$ forces every coordinate of $x$ to vanish. No other [eigenvalues](../../../linear-operator-theory.md#eigenvalue) occur, so $\sigma_p(T)=\{1/n:n\geq1\}$ is not closed.

Finally, if $T$ is self-adjoint and $Tv=\lambda v$, $v\ne0$, then $\langle Tv,v\rangle$ is real and equals $\lambda\|v\|^2$ under the convention linear in the first argument. Therefore **every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of a self-adjoint operator is real**.

## 23F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="23f/solution">Solution</h3>

↑ **Parent:** [23F](#23f)

Take an open neighbourhood $\widetilde U$ on which $p$ is one-to-one and a homeomorphism onto its image. By [invariance of domain](../../../topology.md#invariance-of-domain) for topological surfaces, that image is open. Shrink $\widetilde U$ so the image lies in a complex chart $(V,z)$ of $R$, and use $z\circ p$ as a chart of $\widetilde R$. These charts cover $\widetilde R$. On any overlap their transition is the transition between the original charts of $R$, restricted to an open set, so is holomorphic with holomorphic inverse. They define the desired [complex structure](../../../complex-geometry.md#complex-structure), and in these charts $p$ is locally the identity. Thus **$p$ is holomorphic**. The openness supplied by invariance of domain is important when the hypothesis is phrased only as a homeomorphism onto the image.

Let $f:\mathbb C\to Y$ be holomorphic and let $\pi:\mathbb D\to Y$ be the stated covering. Choose a lift of $f(0)$. The covering-space lifting theorem says that a map from a simply connected, locally path-connected domain has a unique lift after fixing this initial point: lift paths from zero, and [homotopy](../../../algebraic-topology.md#homotopy) lifting makes their endpoint independent of path. Since $\mathbb C$ is simply connected, this constructs $\widetilde f:\mathbb C\to\mathbb D$ with $\pi\circ\widetilde f=f$. On a small neighbourhood, the lift is a biholomorphic local inverse of $\pi$ composed with $f$, so it is holomorphic. Its modulus is less than one, and [Liouville theorem](../../../complex-analysis.md#liouville-theorem) therefore makes it constant. Hence **every holomorphic map $\mathbb C\to Y$ is constant**.

## 24H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="24h/i">i</h3>

↑ **Parent:** [24H](#24h)

<h4 id="24h/i/solution">Solution</h4>

↑ **Parent:** [I](#24h/i)

A [geodesic](../../../riemannian-geometry.md#geodesic) with affine parameter is a curve whose velocity is parallel along itself, $\nabla_{\dot\gamma}\dot\gamma=0$. Its energy on a fixed parameter interval is $E(\gamma)=\frac12\int\langle\dot\gamma,\dot\gamma\rangle\,dt$. For a smooth fixed-endpoint variation with variation field $V$, metric compatibility and the torsion-free connection give

$$
\delta E=\int\langle\nabla_tV,\dot\gamma\rangle\,dt
=[\langle V,\dot\gamma\rangle]_{t_0}^{t_1}
-\int\langle V,\nabla_t\dot\gamma\rangle\,dt.
$$

The endpoint term vanishes. Thus a [geodesic](../../../riemannian-geometry.md#geodesic) is a critical point; conversely, vanishing for every interior variation field implies $\nabla_t\dot\gamma=0$. **Affinely parametrized [geodesics](../../../riemannian-geometry.md#geodesic) are precisely the fixed-endpoint energy critical points.**

<h3 id="24h/ii">ii</h3>

↑ **Parent:** [24H](#24h)

<h4 id="24h/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#24h/ii)

Write $s=U(u)+V(v)>0$. The [geodesic](../../../riemannian-geometry.md#geodesic) energy density $E=\tfrac12s(\dot u^2+\dot v^2)$ is constant, because an affine [geodesic](../../../riemannian-geometry.md#geodesic) has constant speed. Its [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) give, with $p=s\dot u$,

$$
\dot p=\frac12U'(u)(\dot u^2+\dot v^2)=\frac{E U'(u)}s.
$$

The requested expression is

$$
K=s(V\dot u^2-U\dot v^2)=p^2-2EU.
$$

Differentiate, using $\dot u=p/s$ and $\dot E=0$:

$$
\dot K=2p\dot p-2EU'\dot u
=2p\frac{EU'}s-2EU'\frac p s=0.
$$

Therefore **$K$ is independent of the affine parameter**, the [Liouville metric geodesic integral](../../../riemannian-geometry.md#liouville-metric-geodesic-integral). The assumption of affine parametrization is the standard [geodesic](../../../riemannian-geometry.md#geodesic) convention here.

## 25J

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="25j/a">a</h3>

↑ **Parent:** [25J](#25j)

<h4 id="25j/a/solution">Solution</h4>

↑ **Parent:** [A](#25j/a)

A measurable set is invariant when $\theta^{-1}A=A$, or modulo a null set in the measure-theoretic version. A measurable function is invariant when $f\circ\theta=f$, similarly almost everywhere if appropriate. The map is a [measure-preserving transformation](../../../measure-theory.md#measure-preserving-transformation) when $\mu(\theta^{-1}A)=\mu(A)$ for every measurable set. A measure-preserving map is [ergodic](../../../measure-theory.md#ergodicity) when every invariant measurable set has measure zero or has null complement. On a finite positive measure space, normalize the measure to obtain the equivalent probability-space definition.

<h3 id="25j/b">b</h3>

↑ **Parent:** [25J](#25j)

<h4 id="25j/b/solution">Solution</h4>

↑ **Parent:** [B](#25j/b)

As printed, **$\theta_1(x)=1+x$ is not a self-map of $[0,1]$**, so it is not an ergodic transformation of the specified space. No reduction modulo one is stated; if it were imposed it would instead be the identity, also nonergodic.

The map $\theta_2(x)=x^2$ is not Lebesgue measure-preserving: the inverse image of $[0,1/4]$ is $[0,1/2]$, of a different measure. It also has nontrivial invariant sets if ergodicity is defined using invariant sets alone. For example,

$$
A=\{0<x<1:\ \{\log_2(-\log x)\}\in[0,1/2)\}
$$

is invariant under squaring because the logarithm inside the fractional part increases by one. Both it and its complement contain intervals of positive length, so their measures are positive. Thus **$\theta_2$ is not ergodic under either convention**.

Reflection $\theta_3(x)=1-x$ preserves Lebesgue measure, but $[0,1/4]\cup[3/4,1]$ is invariant of measure $1/2$, so it is not ergodic. Finally $\theta_4$ exchanges the two equally weighted atoms. The only invariant subsets are the empty and full sets, hence **$\theta_4$ is ergodic** despite having period two.

<h3 id="25j/c">c</h3>

↑ **Parent:** [25J](#25j)

<h4 id="25j/c/solution">Solution</h4>

↑ **Parent:** [C](#25j/c)

The [Birkhoff ergodic theorem](../../../measure-theory.md#birkhoff-ergodic-theorem) says that for a measure-preserving transformation on a finite measure space and $f\in L^1$, the averages $A_nf=n^{-1}\sum_{k=0}^{n-1}f\circ\theta^k$ converge almost everywhere to an invariant integrable function $f^*$. This limit is the conditional expectation of $f$ given the invariant sigma-algebra, and $\int f^*\,d\mu=\int f\,d\mu$. If the transformation is ergodic and $\mu(E)>0$, then $f^*$ equals the constant $\mu(E)^{-1}\int f\,d\mu$ almost everywhere.

<h3 id="25j/d">d</h3>

↑ **Parent:** [25J](#25j)

<h4 id="25j/d/solution">Solution</h4>

↑ **Parent:** [D](#25j/d)

Since the measure is finite and $f$ is bounded, $f\in L^1$. By [Birkhoff ergodic theorem](../../../measure-theory.md#birkhoff-ergodic-theorem), $A_nf\to f^*$ almost everywhere. If $|f|\leq M$, then $|A_nf|\leq M$ and therefore $|f^*|\leq M$ almost everywhere. For any finite $p\geq1$,

$$
|A_nf-f^*|^p\leq(2M)^p,
$$

and this constant is integrable because $\mu(E)<\infty$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives $\int|A_nf-f^*|^p\,d\mu\to0$. Thus **the ergodic averages converge in every $L^p$, $1\leq p<\infty$**, without assuming ergodicity.

## 26J

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="26j/a">a</h3>

↑ **Parent:** [26J](#26j)

<h4 id="26j/a/solution">Solution</h4>

↑ **Parent:** [A](#26j/a)

The nonzero off-diagonal rates are

$$
(c,r,b)\to(c+1,r,b):\lambda,
\quad(c,r,b)\to(c-1,r+1,b):\mu c,
$$



$$
(c,r,b)\to(c,r-1,b+1):\mu r,
\quad(c,r,b)\to(c,r,b-1):\mu b,
$$

with a transition involving a negative coordinate omitted. These represent arrival, the two metamorphoses, and death. The diagonal generator entry is consequently **$-(\lambda+\mu(c+r+b))$**, so the holding rate is $\lambda+\mu n$.

<h3 id="26j/b">b</h3>

↑ **Parent:** [26J](#26j)

<h4 id="26j/b/solution">Solution</h4>

↑ **Parent:** [B](#26j/b)

Put $\rho=\lambda/\mu$. The proposed stationary probability is the product

$$
\boxed{\pi(c,r,b)=e^{-3\rho}\frac{\rho^c}{c!}\frac{\rho^r}{r!}\frac{\rho^b}{b!}.}
$$

It sums to one. Divide the balance equation at $(c,r,b)$ by this probability. Incoming immigration from $(c-1,r,b)$ contributes $\lambda c/\rho=\mu c$; incoming first metamorphosis from $(c+1,r-1,b)$ contributes $\mu(c+1)r/(c+1)=\mu r$; the next metamorphosis contributes $\mu b$; incoming death from $(c,r,b+1)$ contributes $\mu(b+1)\rho/(b+1)=\lambda$. Their sum is precisely the outgoing rate. Missing boundary terms contribute zero, as the corresponding coordinate is zero. Thus $\pi Q=0$.

For $\lambda,\mu>0$ the chain is irreducible: with positive probability all current insects progress and die before another arrival, and from the empty state specified finite arrivals and stage transitions can reach any state. It is nonexplosive, since only finitely many Poisson arrivals occur in a finite interval and each individual makes at most three stage/death transitions. The existence of this normalized stationary law for an irreducible nonexplosive chain implies positive recurrence and uniqueness of the stationary probability law. “Only solution” here means only probability solution; the homogeneous equation itself also admits zero and scalar multiples.

<h3 id="26j/c">c</h3>

↑ **Parent:** [26J](#26j)

<h4 id="26j/c/solution">Solution</h4>

↑ **Parent:** [C](#26j/c)

The three stage counts are independent Poisson variables of mean $\rho$ under the product law. Hence

$$
\boxed{P(N=n)=e^{-3\rho}\frac{(3\rho)^n}{n!}.}
$$

Dividing the joint law by this mass gives

$$
\boxed{P(C=c,R=r,B=b\mid N=n)
=\frac{n!}{c!r!b!}\left(\frac13\right)^n,\quad c+r+b=n.}
$$

Thus the conditional stage composition is multinomial with equal stage probabilities.

<h3 id="26j/d">d</h3>

↑ **Parent:** [26J](#26j)

<h4 id="26j/d/solution">Solution</h4>

↑ **Parent:** [D](#26j/d)

The chain is **positive recurrent**, by irreducibility, nonexplosion, and the normalized stationary probability law established above. In particular it is neither null recurrent nor transient. The positive arrival and stage rates are understood in the population model.

<h3 id="26j/e">e</h3>

↑ **Parent:** [26J](#26j)

<h4 id="26j/e/solution">Solution</h4>

↑ **Parent:** [E](#26j/e)

Treat each arriving caterpillar as one customer in an [M-G-infinity queue](../../../queueing-theory.md#general-service-infinite-server-queue), with arrival rate $\lambda$ and service time equal to the sum of its three independent exponential stage lifetimes. This is an Erlang distribution of shape three and rate $\mu$, of mean $3/\mu$. Poisson arrivals independently retained according to whether their service has ended give, in stationarity, a Poisson number in service with mean

$$
\lambda\int_0^\infty P(S>s)\,ds=\lambda\mathbb ES=3\lambda/\mu.
$$

This is exactly the marginal law of $N$ found above. Each individual remains in service across both metamorphoses; counting a fresh service arrival at each stage would be incorrect.

## 27I

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="27i/solution">Solution</h3>

↑ **Parent:** [27I](#27i)

Assume a common support, a differentiable likelihood, and dominated differentiation under the integrals. The [score function](../../../statistical-modelling.md#informant-function) $S_\theta=\partial_\theta\log f(X;\theta)$ has mean zero. Its second moment is the [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) $I(\theta)$. If $T$ is unbiased, differentiation of $\mathbb E_\theta T=\theta$ gives $\mathbb E_\theta(TS_\theta)=1$, hence $\operatorname{Cov}_\theta(T,S_\theta)=1$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) yields

$$
\boxed{\operatorname{Var}_\theta(T)\geq I(\theta)^{-1},}
$$

the [Cramér-Rao lower bound](../../../statistical-modelling.md#cramer-rao-bound), assuming positive finite information.

Equality holds precisely when the centred estimator and score are linearly dependent almost surely. The covariance fixes the factor, giving $S_\theta=I(\theta)(T-\theta)$. If the same unbiased estimator is efficient for every parameter on a regular interval, integrate this identity in $\theta$:

$$
\log f(x;\theta)=A(\theta)T(x)-B(\theta)+C(x),
\qquad A'=I,\quad B'=\theta I.
$$

Exponentiation gives $f(x;\theta)=h(x)\exp(A(\theta)T(x)-B(\theta))$, an [exponential family](../../../exponential-family.md). This proves [efficient unbiased estimator implies exponential family](../../../statistical-inference.md#efficient-unbiased-estimator-implies-exponential-family) under the stated common-support regularity, rather than asserting it for nonregular support-dependent models.

## 28J

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="28j/solution">Solution</h3>

↑ **Parent:** [28J](#28j)

In the [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model), the stock follows geometric Brownian motion $dS=\mu S\,dt+\sigma S\,dW$, with constant volatility, and a risk-free account earns constant rate $r$. Frictionless continuous self-financing trading and no arbitrage lead to risk-neutral drift $r$. With $\tau=T-t$, risk-neutral lognormality gives

$$
\boxed{V(t,s)=e^{-r\tau}\Phi(d_2),\qquad
 d_2=\frac{\log(s/K)+(r-\sigma^2/2)\tau}{\sigma\sqrt\tau}.}
$$

This is the [Black-Scholes digital option formula](../../../mathematical-finance.md#black-scholes-digital-option-formula), obtained by discounting $P(S_T>K)$, not the stock-weighted probability of an ordinary call. Differentiation gives the [Delta hedge](../../../mathematical-finance.md#delta-hedge)

$$
\boxed{\Delta(t,s)=\frac{e^{-r\tau}\varphi(d_2)}{s\sigma\sqrt\tau},}
$$

where $\Phi,\varphi$ are the standard [normal distribution](../../../probability-theory.md#normal-distribution) and density. At fixed $s\ne K$, the density term decays faster than $\tau^{-1/2}$ grows, so delta tends to zero. At $s=K$, $d_2\to0$ and $\Delta\sim[K\sigma\sqrt{2\pi\tau}]^{-1}$ diverges. Thus a narrowing, increasingly large delta spike forms around the strike. The terminal payoff is discontinuous: frequent large hedge adjustments near the strike, transaction costs, jumps, discrete trading, and small model or price errors make practical replication difficult. A fixed path avoiding the strike and the at-the-strike limit need not behave alike.

## 29I

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="29i/solution">Solution</h3>

↑ **Parent:** [29I](#29i)

Let $P=\mathbb E\Delta_n^2$ in equilibrium, with $\Delta_n=X_n-\widehat X_n$. The innovation is $Z_{n+1}=Y_{n+1}-\widehat X_n=\Delta_n+\eta_{n+1}$. The given filter gives

$$
\Delta_{n+1}=(1-H)\Delta_n+\varepsilon_{n+1}-H\eta_{n+1}.
$$

Orthogonality to the new innovation requires $(1-H)P-H=0$, hence $H=P/(P+1)$. Since the variables are jointly Gaussian, this orthogonality is independence. Stationary variance gives $P=(1-H)^2P+1+H^2=P/(P+1)+1$, so

$$
P^2-P-1=0,\qquad P=(1+\sqrt5)/2,
\qquad \boxed{H=(\sqrt5-1)/2.}
$$

The added process noise reflects the fact that the new observation concerns $X_n$, not $X_{n+1}$.

For the control calculation choose a quadratic value coefficient $R>0$. Conditional minimization of $x^2+u^2+R\mathbb E[(x+u+\varepsilon)^2]$ gives $K=R/(1+R)$ and the Riccati equation $R=1+R-R^2/(1+R)$, hence $R^2=R+1$. Separation replaces $x$ by its conditional estimate, giving

$$
\boxed{K=R/(1+R)=H=(\sqrt5-1)/2.}
$$

To determine the average cost without solving an additional state covariance, complete the square:

$$
x^2+u^2+R\mathbb E[X_{n+1}^2-x^2\mid x,u]
=R+(1+R)(u+Kx)^2.
$$

With $u=-K\widehat X_n$, the final square is $K^2\Delta_n^2$. In equilibrium the expected telescoping value term is zero, so the minimal cost is

$$
\boxed{\bar J=R+(1+R)K^2P=1+\sqrt5.}
$$

The identity also proves optimality: conditional mean minimization of the square uniquely selects the stated control. Here $1-K\in(0,1)$ ensures stable closed-loop estimates, making the equilibrium averaging valid. This is the [Scalar delayed-observation LQG regulator](../../../control-theory.md#scalar-delayed-observation-lqg-regulator).

## 30A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="30a/solution">Solution</h3>

↑ **Parent:** [30A](#30a)

For a $C^2$ function, let $M(r)=(4\pi)^{-1}\int_{S^2}u(y+r\omega)\,d\omega$ be its spherical mean. Differentiation and the [divergence theorem](../../../calculus.md#divergence-theorem) give

$$
M'(r)=\frac1{4\pi r^2}\int_{\partial B(y,r)}\partial_nu\,dS
=\frac1{4\pi r^2}\int_{B(y,r)}\Delta u\,dx.
$$

If $u$ is harmonic, this derivative is zero; since $M(0)=u(y)$ by continuity, **every spherical mean equals the value at the centre**. Integrating $4\pi r^2M(r)$ over $0<r<R$ gives the same statement for the volume mean on a ball. This proves the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions).

If $u$ is subharmonic, $\Delta u\geq0$, so $M'(r)\geq0$. Thus

$$
\boxed{u(y)\leq\frac1{|\partial B(y,R)|}\int_{\partial B(y,R)}u\,dS,
\qquad u(y)\leq\frac1{|B(y,R)|}\int_{B(y,R)}u\,dx.}
$$

These are the corresponding mean value inequalities. A [subharmonic function](../../../partial-differential-equation.md#subharmonic-function) has the maximum principle on a ball: apply the second-derivative test to $u+\epsilon|x-y|^2$, whose Laplacian is strictly positive and hence cannot have an interior maximum, then let $\epsilon\downarrow0$.

For $w=|\phi|^2$, the given equation says $\Delta\phi=iV\phi$. Since $V$ is real,

$$
\Delta w=2|\nabla\phi|^2+2\operatorname{Re}(\overline\phi\Delta\phi)
=2|\nabla\phi|^2\geq0.
$$

The subharmonic maximum principle gives $w(x)\leq\max_{\partial B}w$ throughout the ball. Taking square roots yields

$$
\boxed{\sup_{B(y,R)}|\phi|\leq\sup_{\partial B(y,R)}|\phi|.}
$$

No sign condition on the real potential $V$ is needed.

## 31B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="31b/solution">Solution</h3>

↑ **Parent:** [31B](#31b)

Away from the turning points, the [Liouville–Green approximation](../../../analysis.md#wkb-approximation) gives in the allowed region

$$
\psi\sim q^{-1/4}\left[A\cos\left(\lambda\int_a^x\sqrt q\,ds\right)
+B\sin\left(\lambda\int_a^x\sqrt q\,ds\right)\right].
$$

The bound-state condition discards the growing exponential in each forbidden region, leaving

$$
\psi_L\sim C_L(-q)^{-1/4}\exp\left[-\lambda\int_x^a\sqrt{-q}\,ds\right],\qquad
\psi_R\sim C_R(-q)^{-1/4}\exp\left[-\lambda\int_b^x\sqrt{-q}\,ds\right].
$$

These approximations require variation slow compared with the local wavelength, and must be replaced near $a,b$ by Airy approximations.

Near $a$, set $z=-\lambda^{2/3}q'(a)^{1/3}(x-a)$. The local differential equation becomes $\psi_{zz}-z\psi=0$. Decay on the left selects [Airy function](../../../differential-equation.md#airy-function) $\operatorname{Ai}(z)$ rather than its growing companion. Comparing the supplied asymptotics across the turning point yields

$$
\psi\sim2C_Lq^{-1/4}\cos\left(S_a(x)-\frac\pi4\right),
\qquad S_a(x)=\lambda\int_a^x\sqrt q\,ds.
$$

At $b$, use $z=\lambda^{2/3}[-q'(b)]^{1/3}(x-b)$; decay on the right similarly yields $2C_Rq^{-1/4}\cos(S_b(x)-\pi/4)$, where $S_b=\lambda\int_x^b\sqrt q\,ds$. Let $J=S_a+S_b=\lambda\int_a^b\sqrt q\,ds$. The left expression has equal cosine and sine coefficients in the variable $S_a$; the right expression has those coefficients proportional to $\cos(J-\pi/4)$ and $\sin(J-\pi/4)$. They can describe the same nonzero wave only when $J-\pi/4=\pi/4+n\pi$. Therefore the [WKB quantization condition](../../../analysis.md#wkb-quantization-condition) is

$$
\boxed{\lambda\int_a^b\sqrt{q(x)}\,dx=(n+\tfrac12)\pi,
\qquad n=0,1,2,\ldots.}
$$

The two simple turning points contribute the two quarter-phase shifts, giving the half-integer correction.

## 32D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="32d/solution">Solution</h3>

↑ **Parent:** [32D](#32d)

The [Pauli matrices](../../../algebra.md#pauli-matrices) obey $(\mathbf n\cdot\boldsymbol\sigma)^2=I$. Expanding the exponential into even and odd powers gives the [time-evolution operator](../../../quantum-mechanics.md#time-evolution-operator)

$$
\boxed{U(t)=e^{-iHt/\hbar}
=I\cos(\gamma Bt/2)+i\mathbf n\cdot\boldsymbol\sigma\sin(\gamma Bt/2).}
$$

For orthogonal states the identity contribution vanishes, so the transition probability is $|\langle\chi'|\mathbf n\cdot\boldsymbol\sigma|\chi\rangle|^2\sin^2(\gamma Bt/2)$. For spin up to spin down in a static field $(B_x,0,B_z)$, only $\sigma_x$ has the required matrix element. Hence

$$
\boxed{P_{\uparrow\to\downarrow}(t)=\frac{B_x^2}{B_x^2+B_z^2}
\sin^2\left(\frac{\gamma\sqrt{B_x^2+B_z^2}\,t}{2}\right).}
$$

For the weak rotating transverse field, take $H_0=-\hbar\gamma B_z\sigma_z/2$. The unperturbed energies give $E_\downarrow-E_\uparrow=\hbar\gamma B_z$. The perturbation matrix element is $\langle\downarrow|V(t)|\uparrow\rangle=-\hbar\gamma A e^{i\alpha t}/2$. Thus first-order perturbation theory gives

$$
a_\downarrow(t)=\frac{i\gamma A}{2}\int_0^t e^{i(\gamma B_z+\alpha)s}\,ds
=\frac{\gamma A}{2\Omega}(e^{i\Omega t}-1),\qquad \Omega=\gamma B_z+\alpha.
$$

Squaring its magnitude yields

$$
\boxed{P_{\uparrow\to\downarrow}\approx
\left(\frac{\gamma A}{\gamma B_z+\alpha}\right)^2
\sin^2\left(\frac{(\gamma B_z+\alpha)t}{2}\right).}
$$

The hypothesis is $|\gamma A|\ll|\Omega|$, excluding resonance. At $\alpha=0$ this is the leading weak-$A$ expansion of the exact static-field formula with $B_x=A$. For extremely long times, a small higher-order frequency correction can accumulate phase, so first-order perturbation is not a uniform approximation on arbitrarily long time scales.

## 33A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="33a/solution">Solution</h3>

↑ **Parent:** [33A](#33a)

Label the two displacements in cell $n$ by $u_n,v_n$, with cell length $2a$. Choose the $K$ spring within a cell and the $G$ spring between cells. The equations are

$$
m\ddot u_n=-(K+G)u_n+Kv_n+Gv_{n-1},\qquad
m\ddot v_n=-(K+G)v_n+Ku_n+Gu_{n+1}.
$$

A [Bloch wave](../../../quantum-theory.md#bloch-state) $(u_n,v_n)=(u,v)e^{i(2aqn-\omega t)}$ gives a two-by-two [eigenvalue](../../../linear-operator-theory.md#eigenvalue) problem, whose determinant is

$$
(K+G-m\omega^2)^2-(K+Ge^{-2iaq})(K+Ge^{2iaq})=0.
$$

Thus the [alternating-spring chain dispersion relation](../../../statistical-physics.md#alternating-spring-chain-dispersion-relation) is

$$
\boxed{\omega_\pm^2(q)=\frac{K+G\pm\sqrt{K^2+G^2+2KG\cos(2aq)}}m.}
$$

Periodic boundaries require $e^{2iaqN}=1$, so $q=\pi j/(Na)$ modulo $\pi/a$. There are $N$ distinct wavenumbers in the [Brillouin zone](../../../quantum-theory.md#brillouin-zone) $-\pi/(2a)\leq q<\pi/(2a)$ and two branches, accounting for $2N$ modes. The minus branch is acoustic, with zero frequency and in-phase motion at the centre; the plus branch is optical, with opposite cell displacements.

Expanding the square root near zero gives

$$
\boxed{\omega_-(q)\sim a\sqrt{\frac{2KG}{m(K+G)}}|q|,\qquad
\omega_+(q)\sim\sqrt{\frac{2(K+G)}m}
\left[1-\frac{KG a^2q^2}{2(K+G)^2}\right].}
$$

At the zone boundary the square root is $K-G$, so the acoustic maximum is $\sqrt{2G/m}$ and the optical minimum is $\sqrt{2K/m}$. The frequency gap is therefore

$$
\boxed{\Delta\omega=\sqrt{2K/m}-\sqrt{2G/m}.}
$$

Quantizing each harmonic mode gives [phonons](../../../statistical-physics.md#phonon), bosonic excitations of energy $\hbar\omega_\pm(q)$ and crystal momentum $\hbar q$ defined modulo a reciprocal lattice vector. Their [group velocity](../../../wave-equation.md#group-velocity) is $d\omega/dq$; acoustic [phonons](../../../statistical-physics.md#phonon) carry long-wavelength sound, while optical [phonons](../../../statistical-physics.md#phonon) have a nonzero centre frequency. There is one longitudinal polarization per branch here, and [phonon](../../../statistical-physics.md#phonon) number is not conserved in thermal equilibrium.

## 34D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="34d/solution">Solution</h3>

↑ **Parent:** [34D](#34d)

A fixed-axis diatomic molecule has one bond-stretch vibrational coordinate $q$, reduced mass $m_r$, and angular frequency $\omega$. In the classical harmonic approximation its internal [Hamiltonian](../../../classical-mechanics.md#hamiltonian) is $p^2/(2m_r)+m_r\omega^2q^2/2$. The phase-space contribution per molecule is

$$
z_{\rm vib}=\frac1h\int_{\mathbb R^2}
\exp\left[-\frac{p^2/(2m_r)+m_r\omega^2q^2/2}{kT}\right]dp\,dq
=\boxed{\frac{2\pi kT}{h\omega}=\frac{kT}{\hbar\omega}.}
$$

The Gaussian integrals cancel the reduced mass. Extending the small bond displacement to the whole real line is the usual harmonic approximation. There is no rotational factor because the molecular orientation is fixed.

For $N$ identical dilute molecules of total mass $M$ in volume $V$, translation supplies $V(2\pi MkT/h^2)^{3/2}$. Including indistinguishability gives

$$
Z=\frac1{N!}\left[V\left(\frac{2\pi MkT}{h^2}\right)^{3/2}
\frac{kT}{\hbar\omega}\right]^N.
$$

Using Stirling's approximation and defining $Q=(V/N)(2\pi MkT/h^2)^{3/2}kT/(\hbar\omega)$,

$$
\boxed{F=-NkT(\log Q+1),\qquad S=-F_T=Nk(\log Q+7/2).}
$$

The $7/2$ is $1+5/2$: the logarithm contains $T^{5/2}$, combining three translational quadratic degrees with two vibrational ones. This is a classical result, valid when vibration is thermally classical rather than quantum frozen.

## 35E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="35e/solution">Solution</h3>

↑ **Parent:** [35E](#35e)

Replace $\varphi$ by $\varphi+\epsilon\eta$, with $\eta$ vanishing on the boundary, and differentiate the action at zero. Integrate the derivative of $\eta$ by parts:

$$
\delta S=\int\left[\frac{\partial\mathcal L}{\partial\varphi}\eta+
\frac{\partial\mathcal L}{\partial\varphi_{,a}}\partial_a\eta\right]d^4x
=\int\left[\frac{\partial\mathcal L}{\partial\varphi}
-\partial_a\frac{\partial\mathcal L}{\partial\varphi_{,a}}\right]\eta\,d^4x.
$$

The coefficient of $\eta$ is the [functional derivative](../../../calculus-of-variations.md#functional-derivative) $\delta S/\delta\varphi$.

For the electromagnetic action, $\delta F_{ab}=\partial_a\delta A_b-\partial_b\delta A_a$. Antisymmetry combines these terms and integration by parts gives

$$
\delta S=\int\left[\mu_0^{-1}\partial_aF^{ab}-J^b\right]\delta A_b\,d^4x.
$$

Thus the inhomogeneous [Maxwell equations](../../../electromagnetism.md#maxwell-equations) are $\partial_aF^{ab}=\mu_0J^b$. The definition of $F$ also gives the homogeneous equations $\partial_{[a}F_{bc]}=0$, equivalently $\partial_a\widetilde F^{ab}=0$. These are the two four-vector Maxwell systems.

Unrestricted variation of the alternative component-gradient action instead gives $\Box A^b=\mu_0J^b$. This is equivalent to the first Maxwell system only when supplemented by the [Lorenz gauge](../../../electromagnetism.md#lorenz-gauge-condition) $\partial_aA^a=0$, because

$$
\partial_aF^{ab}=\Box A^b-\partial^b(\partial_aA^a).
$$

The alternative action is not by itself gauge-invariant; the additional condition must be supplied consistently, not silently omitted.

Expand the tensor square: $F^{ab}F_{ab}=2[\partial^bA^a\partial_bA_a-\partial^bA^a\partial_aA_b]$. Hence

$$
S-\widehat S=\frac1{2\mu_0}\int\partial^bA^a\partial_aA_b\,d^4x.
$$

Integrating this cross term by parts twice expresses its integral as a boundary term plus $\int(\partial_aA^a)^2\,d^4x$. Under Lorenz gauge it is therefore purely a boundary term. With fixed or vanishing boundary contributions, **the two actions have the same variational equations once the additional gauge condition is included**. This is the [Lorenz-gauge reduction of the electromagnetic action](../../../electromagnetism.md#lorenz-gauge-reduction-of-the-electromagnetic-action).

## 36A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="36a/solution">Solution</h3>

↑ **Parent:** [36A](#36a)

Vary the curve by $\delta x^c$, fixing endpoints. Integration by parts in the kinetic functional gives its Euler-Lagrange equations

$$
\frac d{d\lambda}(2g_{cb}\dot x^b)-\partial_cg_{ab}\dot x^a\dot x^b=0.
$$

Multiplying by $g^{cd}/2$ and symmetrizing the velocity product gives

$$
\boxed{\ddot x^d+\Gamma^d_{ab}\dot x^a\dot x^b=0,\qquad
\Gamma^d_{ab}=\tfrac12g^{dc}(\partial_ag_{bc}+\partial_bg_{ac}-\partial_cg_{ab}).}
$$

There is no term proportional to $\dot x$ from parameter reparametrization, so this is the affine [geodesic equation](../../../riemannian-geometry.md#geodesic-equation).

In units $c=1$, the static spherical vacuum metric is Schwarzschild with $f(r)=1-2GM/r$. For example, starting from $-e^{2\Phi}dt^2+e^{2\Lambda}dr^2+r^2d\Omega^2$, the vacuum radial equations give $[r(1-e^{-2\Lambda})]'=0$ and $\Phi'+\Lambda'=0$. Asymptotic flatness and the Newtonian mass fix $e^{2\Phi}=e^{-2\Lambda}=1-2GM/r$, giving the displayed metric. Time and azimuthal coordinates are cyclic in its [geodesic](../../../riemannian-geometry.md#geodesic) Lagrangian, so

$$
\boxed{f\dot t=E,\qquad r^2\dot\phi=h.}
$$

Normalize the velocity norm to $-k$, with $k=1$ for proper-time parametrized massive motion and $k=0$ for null motion. In the equatorial plane this gives $\dot r^2+f(k+h^2/r^2)=E^2$. For a nonradial orbit, $h\ne0$ and $u=1/r$ imply $\dot r=-h\,du/d\phi$. Therefore

$$
\boxed{(u')^2+fu^2=-\frac{k}{h^2}f+\frac{E^2}{h^2}.}
$$

Differentiating with $f=1-2GMu$ yields

$$
\boxed{u''+u=\frac{kGM}{h^2}+3GMu^2.}
$$

It extends across isolated turning points by continuity. The original PDF's later $f=1-GMu$ is inconsistent with this claimed equation: that choice gives $u''+u=kGM/(2h^2)+(3GM/2)u^2$. The intended Schwarzschild factor is **$1-2GMu$**, which we retain.

For massive motion put $\ell=h^2/(GM)$. The Newtonian solution is $u_0=(1+e\cos\phi)/\ell$. The resonant cosine forcing in $3GMu_0^2$ is $6GMe\cos\phi/\ell^2$, producing the secular correction $3GMe\phi\sin\phi/\ell^2$. Resumming it into a shifted phase gives the precessing-ellipse approximation

$$
\boxed{u\approx\ell^{-1}[1+e\cos(\alpha\phi)],\qquad
\alpha=1-3GM/\ell.}
$$

For finite eccentricity there are also bounded corrections of this same small order: one particular correction is $3GM(1+e^2/2)/\ell^2-GMe^2\cos(2\phi)/(2\ell^2)$, besides adjustable homogeneous terms. Thus the simple displayed ellipse captures the secular precession rather than the complete first-order shape correction. Consecutive periapses are separated by $2\pi/\alpha$, so the [Schwarzschild perihelion precession](../../../general-relativity.md#schwarzschild-perihelion-precession) per radial orbit is approximately **$6\pi GM/\ell$**, forward in the direction of motion.

## 37B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="37b/i">i</h3>

↑ **Parent:** [37B](#37b)

<h4 id="37b/i/solution">Solution</h4>

↑ **Parent:** [I](#37b/i)

The steady [Stokes equations](../../../stokes-flow.md#stokes-equation) are $-\nabla p+\mu\nabla^2\mathbf u=0$, $\nabla\cdot\mathbf u=0$. Taking the curl gives $\nabla^2\boldsymbol\omega=0$. For an axisymmetric azimuthal component $\omega\mathbf e_\phi$, the vector Laplacian's azimuthal component is $(\nabla^2-1/(R^2\sin^2\theta))\omega$. Expanding the derivatives shows

$$
\left(\nabla^2-\frac1{R^2\sin^2\theta}\right)\frac{F}{R\sin\theta}
=\frac1{R\sin\theta}D^2F.
$$

With $\omega=-D^2\Psi/(R\sin\theta)$, the vorticity equation consequently gives **$D^4\Psi=0$**. This derives the streamfunction equation from momentum rather than treating the scalar vorticity component as an ordinary scalar [harmonic function](../../../partial-differential-equation.md#harmonic-function).

<h3 id="37b/ii">ii</h3>

↑ **Parent:** [37B](#37b)

<h4 id="37b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#37b/ii)

For $\Psi=f(R)\sin^2\theta$, the angular operator gives $D^2\Psi=(f''-2f/R^2)\sin^2\theta$. If $f=AR+B/R$, then $D^2\Psi=-2A\sin^2\theta/R$, which is annihilated by $D^2$, verifying the differential equation. The supplied curl formula gives

$$
u_R=2\left(\frac A R+\frac B{R^3}\right)\cos\theta,
\qquad u_\theta=-\left(\frac A R-\frac B{R^3}\right)\sin\theta.
$$

Both decay at infinity. At $R=a$, no slip requires $u_R=U\cos\theta$, $u_\theta=-U\sin\theta$, so $2(A/a+B/a^3)=U$ and $A/a-B/a^3=U$. Therefore

$$
\boxed{A=3Ua/4,\qquad B=-Ua^3/4.}
$$

This is the decaying translating-sphere solution in the laboratory frame; in the body frame one would additionally include the uniform flow at infinity.

<h3 id="37b/iii">iii</h3>

↑ **Parent:** [37B](#37b)

<h4 id="37b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#37b/iii)

Substitution gives

$$
\boxed{u_R=U\left(\frac{3a}{2R}-\frac{a^3}{2R^3}\right)\cos\theta,
\qquad u_\theta=-U\left(\frac{3a}{4R}+\frac{a^3}{4R^3}\right)\sin\theta,
\qquad u_\phi=0.}
$$

Rotational symmetry about the translation axis forbids a transverse force. Linearity of the Stokes equations and boundary conditions makes the force linear in $U$; dissipation makes the force on the translating sphere oppose its motion. Thus **the drag is axial and proportional to $U$**, without computing the stress integral. Dimensional analysis further gives scale $\mu aU$; the exact single-sphere coefficient is $6\pi$.

<h3 id="37b/iv">iv</h3>

↑ **Parent:** [37B](#37b)

<h4 id="37b/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#37b/iv)

For side-by-side spheres, reflection in the vertical mid-plane exchanges the spheres while preserving their common velocity, so their axial drags are equal. For vertically aligned spheres, reflection in the horizontal mid-plane exchanges them and reverses velocity; applying linearity to reverse all velocities back restores the original problem and again gives equal axial drag. These are symmetries of the exact two-sphere Stokes problem.

At a distant side-by-side centre, the leading flow produced by one sphere is $3aU/(4b)$ in the direction of translation. On its axis it is $3aU/(2b)$. This ambient entrainment lowers the relative velocity of the other sphere. Using [Stokes drag law](../../../stokes-flow.md#stokes-s-law) with that relative velocity gives the [mutual drag reduction of two distant translating spheres](../../../stokes-flow.md#mutual-drag-reduction-of-two-distant-translating-spheres):

$$
\boxed{D_{\rm side}=6\pi\mu aU\left[1-\frac{3a}{4b}+O((a/b)^2)\right],}
$$



$$
\boxed{D_{\rm axial}=6\pi\mu aU\left[1-\frac{3a}{2b}+O((a/b)^2)\right].}
$$

The feedback of the corrected force into the other sphere's flow enters at the next order. If the coefficient $6\pi$ is needed directly from the preceding solution, its pressure anomaly is $p=3\mu Ua\cos\theta/(2R^2)$. At the surface the traction components are $t_R=-3\mu U\cos\theta/(2a)$ and $t_\theta=3\mu U\sin\theta/(2a)$; their axial projection is the constant $-3\mu U/(2a)$. Integrating over $4\pi a^2$ gives the single-sphere force $-6\pi\mu aU\mathbf e_z$, as used above.

## 38C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="38c/solution">Solution</h3>

↑ **Parent:** [38C](#38c)

For a plane acoustic wave propagating along $\widehat{\mathbf k}$, the linear momentum equation and dispersion $\omega=c_0k$ give $\widetilde p=\rho_0c_0u_\parallel$ and $\mathbf u=u_\parallel\widehat{\mathbf k}$. Therefore the instantaneous acoustic intensity is

$$
\boxed{\widetilde p\,\mathbf u=\rho_0c_0|\mathbf u|^2\widehat{\mathbf k}.}
$$

For harmonic complex amplitudes the time average instead has the factor one half, $\langle\mathbf I\rangle=\tfrac12\rho_0c_0|\widehat{\mathbf u}|^2\widehat{\mathbf k}$.

For a radial velocity potential, set $v=r\phi$. The spherical wave equation reduces to $v_{tt}=c_0^2v_{rr}$, so

$$
\boxed{\phi(r,t)=\frac{F(t-r/c_0)+G(t+r/c_0)}r.}
$$

No incoming radiation from infinity means $G=0$. Linearizing the moving-surface condition at $r=a$ gives $\phi_r(a,t)=i\omega a\epsilon e^{i\omega t}$, with real parts understood. Write the outgoing solution as $\phi=A e^{i\omega(t-(r-a)/c_0)}/r$. Its radial derivative at $a$ is $-A(1+i\omega a/c_0)e^{i\omega t}/a^2$. Therefore the [outgoing acoustic field of a pulsating sphere](../../../linear-acoustics.md#outgoing-acoustic-field-of-a-pulsating-sphere) is

$$
\boxed{\phi(r,t)=\operatorname{Re}\left\{-\frac{i\omega a^3\epsilon}{1+i\omega a/c_0}
\frac{e^{i\omega(t-(r-a)/c_0)}}r\right\}.}
$$

In the far field the velocity amplitude has magnitude $(\omega/c_0)|A|/r$. Multiply its average plane-wave intensity by the spherical area to obtain the [mean acoustic power of a pulsating sphere](../../../linear-acoustics.md#mean-acoustic-power-of-a-pulsating-sphere):

$$
\boxed{\langle P\rangle=\frac{2\pi\rho_0\omega^2}{c_0}|A|^2
=\frac{2\pi\rho_0\epsilon^2a^6\omega^4}{c_0[1+(\omega a/c_0)^2]}.}
$$

This is positive outward radiated power, evaluated to leading quadratic order in the small real displacement amplitude.

## 39C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="39c/a">a</h3>

↑ **Parent:** [39C](#39c)

<h4 id="39c/a/solution">Solution</h4>

↑ **Parent:** [A](#39c/a)

Because $S w=ce_1$ with $c\ne0$, the similarity transform satisfies $\widehat A e_1=\lambda_1e_1$. Thus its first column is $(\lambda_1,0,\ldots,0)^T$ and it has block form $\begin{pmatrix}\lambda_1&*\\0&B\end{pmatrix}$. Taking the determinant gives $\det(zI-\widehat A)=(z-\lambda_1)\det(zI-B)$. Similarity preserves the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial). Hence **the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $A$, with algebraic multiplicities, are $\lambda_1$ and those of $B$**.

<h3 id="39c/b">b</h3>

↑ **Parent:** [39C](#39c)

<h4 id="39c/b/solution">Solution</h4>

↑ **Parent:** [B](#39c/b)

The two independent columns of $V$ remain independent after multiplication by invertible $S$. Since $R=SV$ has zeros below the second row, its leading two-by-two triangular block is invertible. Hence the image under $S$ of the [invariant subspace](../../../representation-theory.md#invariant-subspace) is exactly $\operatorname{span}(e_1,e_2)$. This coordinate plane is invariant under $\widehat A=SAS^{-1}$, forcing the bottom-left block to vanish:

$$
\widehat A=\begin{pmatrix}B&C\\0&D\end{pmatrix}.
$$

The block determinant factors $\det(zI-\widehat A)=\det(zI-B)\det(zI-D)$. Therefore **the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $A$ are exactly those of the indicated two-by-two and $(n-2)$-by-$(n-2)$ blocks**, counted with algebraic multiplicity. No diagonalizability assumption is needed.

## ↑ Ancestors (8)

1. [Ii](../ii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
