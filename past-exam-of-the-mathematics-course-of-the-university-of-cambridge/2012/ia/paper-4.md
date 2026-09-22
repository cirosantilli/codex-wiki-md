# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2012/PaperIA_4.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2012/PaperIA_4.pdf)

**Table of contents**

- [1D](#1d)
  - [i](#1d/i)
    - [Solution](#1d/i/solution)
  - [ii](#1d/ii)
    - [Solution](#1d/ii/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
  - [i](#2d/i)
    - [Solution](#2d/i/solution)
  - [ii](#2d/ii)
    - [Solution](#2d/ii/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5D](#5d)
  - [i](#5d/i)
    - [Solution](#5d/i/solution)
  - [ii](#5d/ii)
    - [Solution](#5d/ii/solution)
  - [iii](#5d/iii)
    - [Solution](#5d/iii/solution)
  - [Solution](#5d/solution)
- [6D](#6d)
  - [Solution](#6d/solution)
- [7D](#7d)
  - [i](#7d/i)
    - [Solution](#7d/i/solution)
  - [ii](#7d/ii)
    - [Solution](#7d/ii/solution)
  - [iii](#7d/iii)
    - [Solution](#7d/iii/solution)
  - [iv](#7d/iv)
    - [Solution](#7d/iv/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9B](#9b)
  - [a](#9b/a)
    - [Solution](#9b/a/solution)
  - [b](#9b/b)
    - [Solution](#9b/b/solution)
- [10B](#10b)
  - [a](#10b/a)
    - [Solution](#10b/a/solution)
  - [b](#10b/b)
    - [Solution](#10b/b/solution)
- [11B](#11b)
  - [a](#11b/a)
    - [Solution](#11b/a/solution)
  - [b](#11b/b)
    - [Solution](#11b/b/solution)
  - [c](#11b/c)
    - [Solution](#11b/c/solution)
- [12B](#12b)
  - [a](#12b/a)
    - [Solution](#12b/a/solution)
  - [b](#12b/b)
    - [Solution](#12b/b/solution)

## 1D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1d/i">i</h3>

↑ **Parent:** [1D](#1d)

<h4 id="1d/i/solution">Solution</h4>

↑ **Parent:** [I](#1d/i)

Use the [Euclidean algorithm](../../../number-theory.md#euclidean-algorithm): $23=18+5$, $18=3\cdot5+3$, $5=3+2$, and $3=2+1$. Back-substitution gives the [Bezout identity](../../../algebra.md#bezout-identity) $1=9\cdot18-7\cdot23$. Multiplying by $101$ gives one solution of the [linear Diophantine equation](../../../number-theory.md#linear-diophantine-equation), and shifting the coefficients by multiples of $(23,-18)$ reduces it to

$$
\boxed{x=12,\qquad y=-5.}
$$

Indeed, $18\cdot12+23(-5)=216-115=101$. More generally all solutions are $x=12+23k$, $y=-5-18k$, $k\in\mathbb Z$: subtracting this particular solution gives $18(x-12)=-23(y+5)$, and the [coprime integers](../../../number-theory.md#coprime-integers) $18,23$ [force](../../../classical-mechanics.md#force) $23\mid(x-12)$.

<h3 id="1d/ii">ii</h3>

↑ **Parent:** [1D](#1d)

<h4 id="1d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1d/ii)

Write $x=3+18k$. The second [modular congruence](../../../number-theory.md#modular-congruence) becomes $18k\equiv-1\pmod{23}$. The [Bezout identity](../../../algebra.md#bezout-identity) above says that $9$ is the inverse of $18$ modulo $23$, so $k\equiv-9\equiv14\pmod{23}$. Therefore

$$
\boxed{x=255,\qquad x\equiv255\pmod{414}.}
$$

The checks are $255=18\cdot14+3=23\cdot11+2$. The [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) explains uniqueness modulo $18\cdot23=414$, since the moduli are [coprime integers](../../../number-theory.md#coprime-integers).

## 2D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

An [equivalence relation](../../../set-theory.md#equivalence-relation) $R$ on $X$ is a [reflexive relation](../../../set-theory.md#reflexive-relation) ($xRx$), a [symmetric relation](../../../set-theory.md#symmetric-relation) ($xRy\Rightarrow yRx$), and a [transitive relation](../../../set-theory.md#transitive-relation) ($xRy$, $yRz\Rightarrow xRz$). Its [equivalence class](../../../set-theory.md#equivalence-class) at $x$ is $[x]_R=\{y\in X:xRy\}$. Because $R$ is a [reflexive relation](../../../set-theory.md#reflexive-relation), every class is nonempty and every $x$ belongs to its own class, so the classes cover $X$. If $[x]_R$ and $[z]_R$ share an element $y$, symmetry and [transitivity](../../../set-theory.md#transitive-relation) give $xRz$. For every $w\in[x]_R$, [transitivity](../../../set-theory.md#transitive-relation) then gives $zRw$, so $[x]_R\subseteq[z]_R$; exchanging $x,z$ gives equality. Thus distinct classes are disjoint. **The equivalence classes form a [set partition](../../../combinatorics.md#set-partition) of $X$.** On the [empty set](../../../set.md#empty-set), the empty family is the corresponding partition.

<h3 id="2d/i">i</h3>

↑ **Parent:** [2D](#2d)

<h4 id="2d/i/solution">Solution</h4>

↑ **Parent:** [I](#2d/i)

**The intersection is always an [equivalence relation](../../../set-theory.md#equivalence-relation).** Both component relations contain $(x,x)$, so $V$ is a [reflexive relation](../../../set-theory.md#reflexive-relation). If $xVy$, both relations relate $x$ to $y$, and symmetry in each gives $yVx$. If $xVy$ and $yVz$, [transitivity](../../../set-theory.md#transitive-relation) in each component gives both $xRz$ and $xSz$, hence $xVz$. This is the [intersection of equivalence relations](../../../set-theory.md#intersection-of-equivalence-relations); the same argument works for any family of such relations.

<h3 id="2d/ii">ii</h3>

↑ **Parent:** [2D](#2d)

<h4 id="2d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2d/ii)

**The union need not be an [equivalence relation](../../../set-theory.md#equivalence-relation)**, because [transitivity](../../../set-theory.md#transitive-relation) can mix the two relations. Take $X=\{1,2,3\}$. Let $R$ have [equivalence classes](../../../set-theory.md#equivalence-class) $\{1,2\}$ and $\{3\}$, and $S$ have classes $\{1\}$ and $\{2,3\}$. Then $1W2$ and $2W3$, but neither component relates $1$ to $3$, so $1W3$ fails. The [union of equivalence relations](../../../set-theory.md#union-of-equivalence-relations) is reflexive and symmetric; it is precisely [transitivity](../../../set-theory.md#transitive-relation) that may fail.

## 3B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

By [Newton's third law](../../../classical-mechanics.md#newton-s-third-law), the [force](../../../classical-mechanics.md#force) on the second particle is $-F_{12}$. For $M=m_1+m_2$ and [centre of mass](../../../classical-mechanics.md#center-of-mass) $R=(m_1r_1+m_2r_2)/M$, [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) gives $M\ddot R=F_{12}-F_{12}=0$. Thus

$$
\boxed{R(t)=R(0)+t\dot R(0).}
$$

The centre moves on a straight line with constant [velocity](../../../classical-mechanics.md#velocity); zero [velocity](../../../classical-mechanics.md#velocity) is allowed. For the relative position $r=r_1-r_2$, subtraction of the two equations gives

$$
\ddot r=\left(\frac1{m_1}+\frac1{m_2}\right)F_{12}(r),\qquad
\boxed{\mu\ddot r=F_{12}(r),\quad\mu=\frac{m_1m_2}{m_1+m_2}.}
$$

Hence the [two-body problem](../../../classical-mechanics.md#two-body-problem) reduces to a single particle of [reduced mass](../../../classical-mechanics.md#reduced-mass) $\mu$, together with the elementary centre motion. Reconstruct the positions as $r_1=R+(m_2/M)r$, $r_2=R-(m_1/M)r$.

**Yes: the two equal [masses](../../../classical-mechanics.md#mass) can follow the same fixed circle in diametrically opposite positions.** Put the stationary [centre of mass](../../../classical-mechanics.md#center-of-mass) at the circle's center and choose tangential [velocities](../../../classical-mechanics.md#velocity) with the same sense of rotation. If the circle has radius $a$, the separation is $2a$ and the mutual gravitational [force](../../../classical-mechanics.md#force) is directed toward that center, with magnitude $Gm^2/(4a^2)$. The [circular orbit](../../../classical-mechanics.md#circular-orbit) condition is $ma\omega^2=Gm^2/(4a^2)$, so an [equal-mass circular binary](../../../classical-mechanics.md#equal-mass-circular-binary) has

$$
\boxed{\omega^2=\frac{Gm}{4a^3}.}
$$

These initial data maintain the opposite positions and give the same constant [angular speed](../../../classical-mechanics.md#angular-speed) for both particles.

## 4B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

For $0<v<c$, the [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) with coincident origins is

$$
\boxed{t'=\gamma\left(t-\frac{vx}{c^2}\right),\qquad x'=\gamma(x-vt),\quad\gamma=(1-v^2/c^2)^{-1/2}.}
$$

For two simultaneous events in $S$, $\Delta t=0$, so $\Delta t'=-\gamma v\Delta x/c^2$. Distinct spatial positions therefore generally give different times in the boosted frame: this is [relativity of simultaneity](../../../special-relativity.md#relativity-of-simultaneity).

Choose the emission events at $(t,x)=(0,0)$ and $(0,d)$. After emission, the [photon](../../../quantum-mechanics.md#photon) world lines are $x=ct$ and $x=d+ct$. Applying the [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) to either gives

$$
x'-ct'=\gamma(1+v/c)(x-ct).
$$

Thus the two [photons](../../../quantum-mechanics.md#photon) move at [speed](../../../classical-mechanics.md#speed) $c$ in $S'$ on parallel lines whose intercepts differ by $\gamma(1+v/c)d$. Measuring their positions at the same $t'$ after both emissions gives the [photon separation under a collinear Lorentz boost](../../../special-relativity.md#photon-separation-under-a-collinear-lorentz-boost):

$$
\boxed{\Delta x'=\gamma(1+v/c)d=d\sqrt{\frac{c+v}{c-v}}.}
$$

This separation is constant. It is not the contracted distance between the stationary sources: the two emission events are not simultaneous in $S'$, and one [photon](../../../quantum-mechanics.md#photon) has already moved when the other is emitted.

## 5D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5d/i">i</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/i/solution">Solution</h4>

↑ **Parent:** [I](#5d/i)

Take $fg=f\circ g$. **The assertion can fail on an [infinite set](../../../set.md#infinite-set).** On $X=\mathbb N_0$, [set](../../../set.md) $g(n)=n+1$, $f(0)=0$, and $f(n)=n-1$ for $n\geq1$. Then $f(g(n))=n$ for every $n$, but $g(f(0))=1\ne0$. Thus a [right inverse](../../../function.md#right-inverse) need not be a [left inverse](../../../function.md#left-inverse).

**On a [finite set](../../../set.md#finite-set) it is always true.** From $fg=\operatorname{id}_X$, $g$ is an [injection](../../../algebra.md#injective-function): equality of two $g$-values gives equality after applying $f$. An injective self-map of a finite [set](../../../set.md) is a [bijection](../../../function.md#bijection). Composing $fg=\operatorname{id}_X$ with $g^{-1}$ shows $f=g^{-1}$, and hence $gf=\operatorname{id}_X$. This includes the empty [set](../../../set.md).

<h3 id="5d/ii">ii</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5d/ii)

**It can be false even on a two-element [finite set](../../../set.md#finite-set).** On $X=\{0,1\}$, let $f$ and $g$ both be the constant [map](../../../function.md#function-class) with value $0$. Then $fg=g$, but $f(1)=0\ne1$. In general the equation says exactly that $f$ fixes the image $g(X)$; it says nothing about other points. If $g$ happens to be a [surjection](../../../algebra.md#surjective-function), it does [force](../../../classical-mechanics.md#force) $f$ to be the [identity map](../../../function.md#identity-function), but finiteness alone does not ensure this. The empty [set](../../../set.md) and a singleton have only one self-map, so the assertion is trivially true on those [sets](../../../set.md).

<h3 id="5d/iii">iii</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5d/iii)

**It can be false even on a two-element [finite set](../../../set.md#finite-set).** The same constant [maps](../../../function.md#function-class) $f=g=0$ on $\{0,1\}$ satisfy $fg=f$, while $g\ne\operatorname{id}_X$. Indeed, a constant $f$ makes $fg=f$ for every $g$. If $f$ were an [injection](../../../algebra.md#injective-function), one could cancel it pointwise to conclude $g(x)=x$, but finiteness alone supplies no such hypothesis. As before, the assertion is trivial on the empty [set](../../../set.md) or a singleton.

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

The final property concerns a [pointwise periodic self-map](../../../function.md#pointwise-periodic-self-map). Such a [map](../../../function.md#function-class) is a [bijection](../../../function.md#bijection): each point has a predecessor in its finite cycle, giving surjectivity; if $f(x)=f(y)$, choose a common multiple $N$ of periods of $x,y$ and apply $f^{N-1}$ to get $x=y$. Its finite cycles are therefore disjoint.

If $X$ is finite, choose the [least common multiple](../../../number-theory.md#least-common-multiple) of the finitely many cycle lengths. This positive [integer](../../../number-theory.md#integer) $N$ gives $f^N=\operatorname{id}_X$. The empty [set](../../../set.md) satisfies the property with $N=1$.

Conversely, in the usual [set](../../../set.md) theory with choice, every infinite $X$ contains a [countably infinite set](../../../set-theory.md#countably-infinite-set). Divide such a subset into disjoint finite blocks $B_j$ of sizes $j+1$, $j\geq1$, make $f$ a cyclic permutation on each block, and fix every other point. Every point returns to itself, but an identity iterate would have to be divisible by every block length $j+1$. No positive [integer](../../../number-theory.md#integer) has that property: take a block longer than that [integer](../../../number-theory.md#integer). Thus the [uniform period criterion for pointwise periodic maps](../../../function.md#uniform-period-criterion-for-pointwise-periodic-maps) gives

$$
\boxed{X\text{ has the property exactly when }X\text{ is finite}.}
$$

The [axiom of choice](../../../set-theory.md#axiom-of-choice) assumption is stated here because extracting a countably infinite subset of an arbitrary infinite [set](../../../set.md) is not an unrestricted theorem in [set](../../../set.md) theory without choice.

## 6D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6d/solution">Solution</h3>

↑ **Parent:** [6D](#6d)

[Fermat's little theorem](../../../number-theory.md#fermat-little-theorem) says that for a prime $p$ and $p\nmid a$, $a^{p-1}\equiv1\pmod p$; equivalently $a^p\equiv a\pmod p$ for every [integer](../../../number-theory.md#integer) $a$. The [Wilson theorem](../../../number-theory.md#wilson-s-theorem) says $(p-1)!\equiv-1\pmod p$ for a prime $p$ (and, conversely, this congruence characterizes primes among [integers](../../../number-theory.md#integer) greater than one).

For $p=2$, $x=1$ is a [square root of minus one modulo a prime](../../../number-theory.md#square-root-of-minus-one-modulo-a-prime). If $p$ is odd and $x^2\equiv-1$, [Fermat's little theorem](../../../number-theory.md#fermat-little-theorem) gives

$$
1\equiv x^{p-1}=(-1)^{(p-1)/2}\pmod p,
$$

so $(p-1)/2$ is even and $p\equiv1\pmod4$. Conversely, put $h=(p-1)/2$. Pairing $j$ with $p-j$ in the [factorial](../../../combinatorics.md#factorial) gives $(p-1)!\equiv(-1)^h(h!)^2$. For $p\equiv1\pmod4$, $h$ is even, so the [Wilson theorem](../../../number-theory.md#wilson-s-theorem) yields $(h!)^2\equiv-1$. Thus

$$
\boxed{p=2\text{ or }p\equiv1\pmod4,}
$$

and in the latter case $x=h!$ supplies a solution.

For the [multiplicative order](../../../number-theory.md#multiplicative-order) assertion, divide $k$ by $d$: $k=qd+r$, $0\leq r<d$. Since $x^d\equiv1$ and $x^k\equiv1$, it follows that $x^r\equiv1$. Minimality of the positive order excludes $0<r<d$, hence $r=0$ and

$$
\boxed{d\mid k.}
$$

In particular $d\mid p-1$ by [Fermat's little theorem](../../../number-theory.md#fermat-little-theorem). Negative $k$, if included, are handled by the same division using the modular inverse of $x$.

A [Fermat number](../../../number-theory.md#fermat-number) in the paper has $n\geq1$. If a prime $p$ divides $F_n=2^{2^n}+1$, it is odd and $2^{2^n}\equiv-1\pmod p$. Squaring gives $2^{2^{n+1}}\equiv1$, so the order $d$ divides $2^{n+1}$. It does not divide $2^n$, since $-1\ne1$ modulo an odd prime. Every divisor of $2^{n+1}$ is a power of two, so the only possibility is

$$
\boxed{\operatorname{ord}_p(2)=2^{n+1}.}
$$

If two different [Fermat numbers](../../../number-theory.md#fermat-number) shared a [prime factor](../../../number-theory.md#prime-factor), the same element $2$ modulo that prime would have two different orders. This is impossible, proving pairwise [coprimality](../../../number-theory.md#coprime-integers). Also $2^{n+1}\mid p-1$, so for $n\geq1$ every such prime is $1$ modulo $4$. No prime $3$ modulo $4$ can occur.

A prime $1$ modulo $4$ need not occur: take **$p=13$**. It is prime, $2^6=64\equiv-1\pmod{13}$, and $2^4\equiv3\ne1$. Since the order divides $12$, the first congruence excludes every divisor of $6$ and the second excludes $4$; hence the order is $12$. This is not a power of two, so $13$ is not a [prime divisor of a Fermat number](../../../number-theory.md#prime-divisor-of-a-fermat-number). The index restriction matters: the conventional extra number $F_0=3$ is outside the paper's positive-$n$ family.

## 7D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7d/i">i</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/i/solution">Solution</h4>

↑ **Parent:** [I](#7d/i)

If $q=\sqrt2+\sqrt3$ were a [rational number](../../../number-theory.md#rational-number), then $q^2=5+2\sqrt6$ would make $\sqrt6$ rational. Write $\sqrt6=a/b$ in lowest terms. Then $a^2=6b^2$, which is impossible by [unique factorization](../../../algebra.md#unique-factorization-in-an-integral-domain): the exponent of the prime $2$ is even on the left and odd on the right. Therefore

$$
\boxed{\sqrt2+\sqrt3
otin\mathbb Q.}
$$

<h3 id="7d/ii">ii</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7d/ii)

The [exponential function](../../../calculus.md#exponential-function) series gives [Euler's number](../../../calculus.md#e-mathematical-constant) $e=\sum_{k=0}^{\infty}1/k!$. Suppose $e=a/b$ with [integers](../../../number-theory.md#integer) $a,b$ and $b>0$. Choose $n\geq\max(b,2)$. Since $b$ divides $n!$, the number

$$
N=n!\left(e-\sum_{k=0}^n\frac1{k!}\right)
$$

is an [integer](../../../number-theory.md#integer). But its positive tail satisfies

$$
0<N=\sum_{j=1}^{\infty}\frac{n!}{(n+j)!}
<\sum_{j=1}^{\infty}\frac1{(n+1)^j}=\frac1n<1.
$$

The inequality is strict because the factors after the first exceed $n+1$ when $j\geq2$. No [integer](../../../number-theory.md#integer) lies strictly between zero and one. This proves the [irrationality of e](../../../calculus.md#irrationality-of-e):

$$
\boxed{e
otin\mathbb Q.}
$$

<h3 id="7d/iii">iii</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7d/iii)

For $P(x)=x^3+4x-7$, the [derivative](../../../calculus.md#derivative) $P'(x)=3x^2+4$ is positive everywhere, so the [mean value theorem](../../../calculus.md#mean-value-theorem) makes $P$ strictly increasing. Since a [polynomial](../../../polynomial.md) is a [continuous function](../../../calculus.md#continuous-function), the [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) and the values $P(1)=-2$, $P(2)=9$ locate its unique real root in $(1,2)$. By the [rational root theorem](../../../mathematics.md#rational-root-theorem), a rational root of a monic [integer](../../../number-theory.md#integer) polynomial must be an [integer](../../../number-theory.md#integer). There is no [integer](../../../number-theory.md#integer) in $(1,2)$, so **the unique real root is an [irrational number](../../../algebra.md#irrational-number)**. The denominator part of that theorem also follows directly: if $a/b$ in lowest terms were a root, $a^3+4ab^2-7b^3=0$ would [force](../../../classical-mechanics.md#force) $b\mid a^3$, hence $b=1$.

<h3 id="7d/iv">iv</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#7d/iv)

If $\log_2 3=a/b$ were a [rational number](../../../number-theory.md#rational-number), choose positive [integers](../../../number-theory.md#integer) $a,b$ because $\log_2 3>0$. Exponentiation gives $2^a=3^b$, but the left side is even and the right side is odd. Thus

$$
\boxed{\log_2 3
otin\mathbb Q.}
$$

This is the basic [irrational logarithm criterion](../../../calculus.md#irrational-logarithm-criterion): a rational logarithm would [force](../../../classical-mechanics.md#force) positive [integer](../../../number-theory.md#integer) powers of its base and argument to coincide.

## 8D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

First apply the [Cantor theorem](../../../set.md#cantor-s-theorem) by diagonalization. If an [injection](../../../algebra.md#injective-function) $j:\mathcal P(\mathbb R)\to\mathbb R$ existed, it would define a [surjection](../../../algebra.md#surjective-function) $h:\mathbb R\to\mathcal P(\mathbb R)$ by the unique inverse value on $j$'s image, and by $h(x)=\varnothing$ elsewhere. The [set](../../../set.md) $D=\{x\in\mathbb R:x\notin h(x)\}$ cannot equal $h(a)$ for any $a$, since $a\in D$ would be equivalent to $a\notin D$. This contradicts surjectivity. **There is no injection from the power [set](../../../set.md) of the real line into the real line.**

For the opposite type of encoding, let $b(x)=\tfrac12+\pi^{-1}\arctan x$, an injective [map](../../../function.md#function-class) from $\mathbb R$ to $(0,1)$. Give $b(x)$ its canonical [binary expansion](../../../arithmetic.md#binary-expansion), choosing the terminating expansion with trailing zeros whenever two expansions exist. If the binary digits of $b(x),b(y)$ are $a_j,b_j$, define a [real-number pairing by separated digits](../../../algebra.md#real-number-pairing-by-separated-digits):

$$
H(x,y)=\sum_{j\geq1}\left(\frac{2a_j}{3^{2j-1}}+\frac{2b_j}{3^{2j}}\right).
$$

This uses ternary digits only $0,2$, alternating the two input digit sequences. If two outputs first differ at ternary position $k$, that difference has magnitude $2\cdot3^{-k}$, while every later digit together contributes at most $\sum_{j>k}2\cdot3^{-j}=3^{-k}$. Their outputs therefore differ. The digits recover both binary sequences, hence both inputs. Neither output endpoint $0$ nor $1$ occurs because the input numbers lie strictly between zero and one. Thus **$H$ is an injection from $\mathbb R^2$ into $(0,1)\subset\mathbb R$**. The ternary construction avoids an unjustified decimal-interleaving argument at ambiguous expansions.

For a [finite modification of the identity on the real line](../../../function.md#finite-modification-of-the-identity-on-the-real-line), let $D_f=\{x:f(x)\ne x\}$ have size $n$, and sort it uniquely as $x_1<\cdots<x_n$. Its finite record is $(x_1,f(x_1),\ldots,x_n,f(x_n))$. It determines $f$ completely, with the identity used outside the recorded points. Repeatedly applying the pairing $H$ gives an [injection](../../../algebra.md#injective-function) $H_k:\mathbb R^k\to(0,1)$ for every positive finite $k$: take $H_1=b$ and $H_k(t_1,\ldots,t_k)=H(t_1,H_{k-1}(t_2,\ldots,t_k))$. Encode $f$ by

$$
J(f)=\begin{cases}1/2,&n=0,\\ n+H_{2n}(x_1,f(x_1),\ldots,x_n,f(x_n)),&n\geq1.\end{cases}
$$

Different lengths occupy disjoint intervals $(n,n+1)$, and within a fixed length the record is recoverable. Hence

$$
\boxed{\text{There is an injection }X\to\mathbb R.}
$$

Indeed the cardinality is exactly that of $\mathbb R$: the [functions](../../../function.md) that alter only $0$, assigning it an arbitrary real value, give an injection in the other direction, and the [Cantor-Schröder-Bernstein theorem](../../../set-theory.md#cantor-schroder-bernstein-theorem) applies.

## 9B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9b/a">a</h3>

↑ **Parent:** [9B](#9b)

<h4 id="9b/a/solution">Solution</h4>

↑ **Parent:** [A](#9b/a)

A [central force](../../../physics.md#central-force) has no angular component, so the supplied polar acceleration formula and [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) give $d(r^2\dot\theta)/dt=0$. Thus $l=r^2\dot\theta$ is the conserved [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum). For a nonradial orbit, $l\ne0$ allows $\theta$ to be used as a parameter. With $u=1/r$ and a prime denoting $d/d\theta$,

$$
\dot r=-u^{-2}u'\dot\theta=-lu',\qquad\ddot r=-lu''\dot\theta=-l^2u^2u''.
$$

Also $r\dot\theta^2=l^2u^3$. The radial equation $\ddot r-r\dot\theta^2=-f(r)$ therefore becomes the [Binet equation](../../../classical-mechanics.md#binet-equation)

$$
\boxed{l^2u^2(u''+u)=f(1/u).}
$$

For a purely radial trajectory $l=0$, the angular parameter is unavailable, and one instead uses the direct radial equation. The orbit in part (b) is nonradial.

<h3 id="9b/b">b</h3>

↑ **Parent:** [9B](#9b)

<h4 id="9b/b/solution">Solution</h4>

↑ **Parent:** [B](#9b/b)

Set $\theta=0$ initially and choose its positive sense to agree with the initial tangential motion. The inward radial component is $\dot r(0)=-4\cos(\pi/3)=-2$, while the tangential [speed](../../../classical-mechanics.md#speed) is $4\sin(\pi/3)=2\sqrt3$. Hence

$$
\boxed{l=2\sqrt3,\quad u(0)=1,\quad u'(0)=1/\sqrt3.}
$$

Substitution in the [Binet equation](../../../classical-mechanics.md#binet-equation) gives $12(u''+u)=3+9u$, or $u''+u/4=1/4$. This is an [orbit equation for combined inverse-square and inverse-cube attraction](../../../classical-mechanics.md#orbit-equation-for-combined-inverse-square-and-inverse-cube-attraction). Solving the constant-coefficient equation and applying both initial conditions gives

$$
\boxed{u(\theta)=1+\frac2{\sqrt3}\sin(\theta/2).}
$$

On $0\leq\theta\leq2\pi$, the sine is nonnegative, so $r$ stays finite and positive. At $\theta=2\pi$, $u=1$, hence $r=1$ and the particle is back at its original spatial position after one revolution. But $u'(2\pi)=-1/\sqrt3$, so its radial [velocity](../../../classical-mechanics.md#velocity) is now $+2$, rather than the original $-2$. **The return is not a periodic return in position and [velocity](../../../classical-mechanics.md#velocity).**

After that revolution, the first zero of $u$ is at $\theta=8\pi/3$, where $\sin(\theta/2)=-\sqrt3/2$. The physical branch therefore has $r\to\infty$ as $\theta\uparrow8\pi/3$; it must not be continued into negative $u$. Since $dt/d\theta=1/(lu^2)$ and $u$ has a simple zero, reaching infinity takes infinite time. As a check, the specific [potential energy](../../../classical-mechanics.md#potential-energy) is $\Phi(r)=-3/r-9/(2r^2)$ and the conserved energy per unit [mass](../../../classical-mechanics.md#mass) is $4^2/2+\Phi(1)=1/2$, giving escape [speed](../../../classical-mechanics.md#speed) $1$ at infinity, also obtained from $-lu'(8\pi/3)=1$.

## 10B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10b/a">a</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/a/solution">Solution</h4>

↑ **Parent:** [A](#10b/a)

Apply the [rotating-frame derivative formula](../../../physics.md#rotating-frame-derivative-formula) first to $r$, then to $v'= [dr/dt]_{S'}$. Since the [angular velocity](../../../classical-mechanics.md#angular-velocity) is constant in either frame,

$$
\left[\frac{dr}{dt}\right]_S=v'+\omega\times r,
$$



$$
\boxed{\left[\frac{d^2r}{dt^2}\right]_S=\left[\frac{d^2r}{dt^2}\right]_{S'}+2\omega\times v'+\omega\times(\omega\times r).}
$$

The two apparent [forces](../../../classical-mechanics.md#force) in the rotating equation are the [Coriolis force](../../../physics.md#coriolis-force) and the [centrifugal acceleration](../../../physics.md#centrifugal-acceleration) multiplied by [mass](../../../classical-mechanics.md#mass). Thus

$$
m\left[\frac{dv'}{dt}\right]_{S'}=-\nabla\phi+G-2m\omega\times v'-m\omega\times(\omega\times r).
$$

Set $\phi_{\rm eff}=\phi-\tfrac m2|\omega\times r|^2$. The supplied gradient identity gives $\nabla\phi_{\rm eff}=\nabla\phi+m\omega\times(\omega\times r)$. Taking the scalar product with $v'$ removes $G$, since it is orthogonal to $v'$, and removes the [Coriolis force](../../../physics.md#coriolis-force). Therefore the [energy balance in a uniformly rotating frame](../../../physics.md#energy-balance-in-a-uniformly-rotating-frame) is

$$
\boxed{\frac{d}{dt}\left(\frac m2|v'|^2+\phi-\frac m2|\omega\times r|^2\right)=\left(\frac{\partial\phi}{\partial t}\right)_{r'}.}
$$

**The displayed quantity is conserved when the potential is stationary in the rotating coordinates.** This includes a static inertial potential invariant under rotations about the chosen axis, such as vertical gravity in part (b). If the word conservative only means a time-independent inertial potential, that extra rotational invariance is needed; a conservative [force](../../../classical-mechanics.md#force) alone does not imply the claimed conservation.

For an explicit counterexample to that unrestricted interpretation, take unit [mass](../../../classical-mechanics.md#mass), an inertial [force](../../../classical-mechanics.md#force) $F=e_x$, $\phi=-x$, no $G$, rotation $\omega=\omega e_z$, and inertial trajectory $r(t)=(t^2/2,1,0)$ with initial [velocity](../../../classical-mechanics.md#velocity) zero. It satisfies [Newton's second law](../../../classical-mechanics.md#newton-s-second-law). Substituting $v'=\dot r-\omega\times r$ into the proposed energy gives $E=\omega t$, which is not constant for nonzero rotation. The qualified conservation law above is the one used for the hoop.

<h3 id="10b/b">b</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/b/solution">Solution</h4>

↑ **Parent:** [B](#10b/b)

In the [rotating-hoop bead](../../../physics.md#rotating-hoop-bead) problem, use a signed angle in the hoop plane from the downward vertical. The gravitational [potential energy](../../../classical-mechanics.md#potential-energy) is $-mga\cos\theta$, the rotating-frame [speed](../../../classical-mechanics.md#speed) is $a\dot\theta$, and the distance from the rotation axis is $a\sin\theta$. The [centrifugal potential](../../../physics.md#centrifugal-potential) gives

$$
E=\frac{ma^2}{2}\dot\theta^2-mga\cos\theta-\frac{m\omega^2a^2}{2}\sin^2\theta.
$$

Gravity is stationary in these rotating coordinates, and the frictionless constraint does no work. Projecting the rotating equation along the hoop, or differentiating its effective potential in the one-dimensional [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation), gives

$$
\boxed{\ddot\theta+\left(\frac ga-\omega^2\cos\theta\right)\sin\theta=0.}
$$

If $\omega^2>g/a$, the two off-axis positions are

$$
\boxed{\theta=\pm\theta_0,\qquad\theta_0=\arccos\left(\frac{g}{a\omega^2}\right).}
$$

Their unsigned angle to the downward vertical is the same; they lie on opposite sides of the hoop. The second [derivative](../../../calculus.md#derivative) of the effective potential there is $m\omega^2a^2\sin^2\theta_0>0$. Equivalently, writing $\theta=\theta_0+\delta$ gives to first order

$$
\ddot\delta+\omega^2\sin^2\theta_0\,\delta=0.
$$

The same holds at $-\theta_0$. Thus **both equilibria are stable**, with small-oscillation angular frequency $|\omega|\sin\theta_0$.

## 11B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11b/a">a</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/a/solution">Solution</h4>

↑ **Parent:** [A](#11b/a)

The [parallel axis theorem](../../../classical-mechanics.md#parallel-axis-theorem) says that for an axis through a body's [centre of mass](../../../classical-mechanics.md#center-of-mass) and a parallel axis at perpendicular distance $d$,

$$
\boxed{I=I_{\rm cm}+Md^2,}
$$

where $M$ is the total [mass](../../../classical-mechanics.md#mass). The displacement is the distance between the two parallel axes; neither axis may be arbitrary in place of the center-of-mass axis. Expanding the squared distances of [mass](../../../classical-mechanics.md#mass) elements gives this formula, since the cross term integrates to zero at the [centre of mass](../../../classical-mechanics.md#center-of-mass).

<h3 id="11b/b">b</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/b/solution">Solution</h4>

↑ **Parent:** [B](#11b/b)

The [moment of inertia](../../../classical-mechanics.md#moment-of-inertia) of the uniform disc about its central perpendicular axis is

$$
I_O=\int_0^a r^2\frac{m}{\pi a^2}2\pi r\,dr=\frac12ma^2.
$$

The [parallel axis theorem](../../../classical-mechanics.md#parallel-axis-theorem) gives $I_A=I_O+ma^2=3ma^2/2$. For angle $\beta$ from the downward resting position, the gravitational [torque](../../../classical-mechanics.md#torque) is $-mga\sin\beta$, so $I_A\ddot\beta=-mga\sin\beta$. Linearizing at $\beta=0$ gives $\ddot\beta+(2g/(3a))\beta=0$. Thus the [uniform disc pivoted at its rim](../../../physics.md#uniform-disc-pivoted-at-its-rim) is a [physical pendulum](../../../physics.md#physical-pendulum) with period

$$
\boxed{T=2\pi\sqrt{\frac{3a}{2g}}.}
$$

<h3 id="11b/c">c</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/c/solution">Solution</h4>

↑ **Parent:** [C](#11b/c)

Measure a signed angle $\theta$ from the upward radius $A\to O$ in the direction of falling. With $I_A=3ma^2/2$, gravitational [torque](../../../classical-mechanics.md#torque) gives

$$
\boxed{\ddot\theta=\frac{2g}{3a}\sin\theta.}
$$

There is an idealization in the release condition: **exactly upright and exactly at rest is an unstable equilibrium, so the exact ideal solution stays there.** Uniqueness of this smooth equation with $\theta(0)=\dot\theta(0)=0$ prevents spontaneous departure. The usual falling calculation means an infinitesimal disturbance, with its energy tending to that of the upright rest state. For that limiting [separatrix](../../../dynamical-systems.md#separatrix) motion, conservation of [mechanical energy](../../../classical-mechanics.md#mechanical-energy) gives

$$
\frac12I_A\dot\theta^2=mga(1-\cos\theta),\qquad
\boxed{\dot\theta^2=\frac{4g}{3a}(1-\cos\theta).}
$$

On the branch with increasing angle, $\dot\theta=\sqrt{8g/(3a)}\sin(\theta/2)$ for $0<\theta<2\pi$; the opposite branch has the opposite [angular velocity](../../../classical-mechanics.md#angular-velocity). The nontrivial limiting motion approaches the upright position only as $t\to-\infty$, because $dt/d\theta$ has a logarithmically divergent integral near zero.

Let $e_r$ point from $A$ toward $O$, and $e_\theta$ in the direction of increasing angle, so $e_r=\sin\theta\,e_x+\cos\theta\,e_z$ and $e_\theta=\cos\theta\,e_x-\sin\theta\,e_z$. The [centre of mass](../../../classical-mechanics.md#center-of-mass) acceleration on the limiting falling branch is

$$
\boxed{a_O=-\frac{4g}{3}(1-\cos\theta)e_r+\frac{2g}{3}\sin\theta\,e_\theta.}
$$

Gravity has components $-mg\cos\theta\,e_r+mg\sin\theta\,e_\theta$. Applying [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) to the whole disc gives

$$
\boxed{R=\frac{mg}{3}(7\cos\theta-4)e_r-\frac{mg}{3}\sin\theta\,e_\theta.}
$$

The signed component parallel to the radius, positive from $A$ toward $O$, is the required $mg(7\cos\theta-4)/3$. This same radial formula is consistent at the exact stationary upright state, where $\theta=0$, $a_O=0$, and $R=mg e_z$; nonzero falling angles require the limiting-release interpretation just stated.

## 12B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12b/a">a</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/a/solution">Solution</h4>

↑ **Parent:** [A](#12b/a)

Use [metric signature](../../../topology.md#metric-signature) $(+---)$, as required by the sign of the scalar product in this question. For a massive particle, the [four-momentum](../../../special-relativity.md#four-momentum) is

$$
\boxed{P=(E/c,p)=m\gamma(c,v),\qquad\gamma=(1-|v|^2/c^2)^{-1/2}.}
$$

For a [photon](../../../quantum-mechanics.md#photon) of positive frequency $\nu$ and direction $e$, the [Planck constant](../../../quantum-mechanics.md#planck-constant) gives $E=h\nu$ and

$$
\boxed{K=\left(\frac{h\nu}{c},\frac{h\nu}{c}e\right),\qquad K^2=0.}
$$

A [future-pointing timelike four-vector](../../../special-relativity.md#future-pointing-timelike-four-vector) $P=(P^0,p)$ has $P^0>|p|$ and $P^0>0$ in this signature. The ordinary Euclidean [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) yields

$$
P_1\cdot P_2=P_1^0P_2^0-p_1\cdot p_2\geq P_1^0P_2^0-|p_1||p_2|>0.
$$

This is stronger than the requested nonnegative inequality. For an electron and a positron of rest [mass](../../../classical-mechanics.md#mass) $m>0$, their future-pointing timelike [four-momenta](../../../special-relativity.md#four-momentum) have $P_1^2=P_2^2=m^2c^2$. Thus

$$
(P_1+P_2)^2=2m^2c^2+2P_1\cdot P_2>0,
$$

which cannot equal the null norm of a single [photon](../../../quantum-mechanics.md#photon). **[Four-momentum conservation](../../../special-relativity.md#four-momentum-conservation) forbids spontaneous [photon](../../../quantum-mechanics.md#photon) decay into an electron-positron pair in vacuum.** An external body or field able to exchange momentum would be a different system.

<h3 id="12b/b">b</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/b/solution">Solution</h4>

↑ **Parent:** [B](#12b/b)

For $u>0$, take the initial electron direction as the longitudinal axis and put $\beta=u/c$. Incoming [four-momentum conservation](../../../special-relativity.md#four-momentum-conservation) gives

$$
h(\nu_1+\nu_2)=mc^2(\gamma+1),\qquad
\frac hc(\nu_1e_1+\nu_2e_2)=m\gamma u\,\hat u.
$$

The transverse components must cancel. In the noncollinear case the two transverse directions are opposite, and $\nu_1\sin\theta_1=\nu_2\sin\theta_2$. Hence the ratio of longitudinal momentum times $c$ to energy is

$$
\frac{\gamma\beta}{\gamma+1}
=\frac{\nu_1\cos\theta_1+\nu_2\cos\theta_2}{\nu_1+\nu_2}
=\frac{\sin(\theta_1+\theta_2)}{\sin\theta_1+\sin\theta_2}.
$$

Writing $s=(\theta_1+\theta_2)/2$ and $d=(\theta_1-\theta_2)/2$, the last ratio is $\cos s/\cos d$. It also equals $(1+\cos(\theta_1+\theta_2))/(\cos\theta_1+\cos\theta_2)$ whenever that denominator is nonzero. Since $\gamma^2\beta^2=\gamma^2-1$, the [angular relation for two-photon electron-positron annihilation](../../../special-relativity.md#angular-relation-for-two-photon-electron-positron-annihilation) is

$$
\boxed{\frac{1+\cos(\theta_1+\theta_2)}{\cos\theta_1+\cos\theta_2}
=\frac{\gamma\beta}{\gamma+1}
=\sqrt{\frac{\gamma-1}{\gamma+1}}.}
$$

The positive root follows from $u>0$. For noncollinear emission the positive momentum-to-energy ratio ensures $\cos s>0$, and $|d|<\pi/2$ ensures the stated denominator is positive.

The printed quotient needs a qualification for exactly collinear [photons](../../../quantum-mechanics.md#photon). The allowed configuration $\theta_1=0$, $\theta_2=\pi$ has positive frequencies

$$
h\nu_{1,2}=\frac{mc^2}{2}\left[(\gamma+1)\pm\gamma\beta\right],
$$

which obey both conservation equations, but the printed left side is $0/0$. Thus the quotient holds for noncollinear angles, or as its appropriate noncollinear limit. The undivided identity

$$
1+\cos(\theta_1+\theta_2)
=\sqrt{\frac{\gamma-1}{\gamma+1}}(\cos\theta_1+\cos\theta_2)
$$

remains true in the collinear case, where both sides vanish. The limit $u=0$ similarly requires care because the initial direction is then undefined and the [photons](../../../quantum-mechanics.md#photon) are antiparallel.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
