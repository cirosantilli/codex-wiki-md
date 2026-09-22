# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2008/PaperIA_4.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2008/PaperIA_4.pdf)

**Table of contents**

- [1D](#1d)
  - [i](#1d/i)
    - [Solution](#1d/i/solution)
  - [ii](#1d/ii)
    - [Solution](#1d/ii/solution)
  - [iii](#1d/iii)
    - [Solution](#1d/iii/solution)
  - [iv](#1d/iv)
    - [Solution](#1d/iv/solution)
- [2D](#2d)
  - [a](#2d/a)
    - [Solution](#2d/a/solution)
  - [b](#2d/b)
    - [Solution](#2d/b/solution)
- [3B](#3b)
  - [Solution](#3b/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5D](#5d)
  - [a](#5d/a)
    - [Solution](#5d/a/solution)
  - [b](#5d/b)
    - [Solution](#5d/b/solution)
  - [c](#5d/c)
    - [Solution](#5d/c/solution)
- [6D](#6d)
  - [a](#6d/a)
    - [Solution](#6d/a/solution)
  - [b](#6d/b)
    - [Solution](#6d/b/solution)
  - [c](#6d/c)
    - [Solution](#6d/c/solution)
- [7D](#7d)
  - [a](#7d/a)
    - [Solution](#7d/a/solution)
  - [b](#7d/b)
    - [Solution](#7d/b/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9B](#9b)
  - [Solution](#9b/solution)
- [10B](#10b)
  - [i](#10b/i)
    - [Solution](#10b/i/solution)
  - [ii](#10b/ii)
    - [Solution](#10b/ii/solution)
  - [Solution](#10b/solution)
- [11B](#11b)
  - [i](#11b/i)
    - [Solution](#11b/i/solution)
  - [ii](#11b/ii)
    - [Solution](#11b/ii/solution)
  - [Solution](#11b/solution)
- [12B](#12b)
  - [Solution](#12b/solution)

## 1D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1d/i">i</h3>

↑ **Parent:** [1D](#1d)

<h4 id="1d/i/solution">Solution</h4>

↑ **Parent:** [I](#1d/i)

**False.** Take $A=\{0\}$ and $B=C=\{0,1\}$, with $f(0)=0$ and $g=\operatorname{id}_B$. Then $f$ is an [injection](../../../algebra.md#injective-function) and $g$ is a [surjection](../../../algebra.md#surjective-function), but the [function composition](../../../algebra.md#function-composition) $g\circ f$ has [image of a function](../../../set-theory.md#image-of-a-function) $\{0\}$, so it is not a [surjection](../../../algebra.md#surjective-function) onto $C$.

<h3 id="1d/ii">ii</h3>

↑ **Parent:** [1D](#1d)

<h4 id="1d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1d/ii)

**True.** The [function composition](../../../algebra.md#function-composition) $j=g\circ f$ is an [injection](../../../algebra.md#injective-function): $j(a)=j(a')$ first implies $f(a)=f(a')$ by the [injectivity](../../../algebra.md#injective-function) of $g$, then $a=a'$ by the [injectivity](../../../algebra.md#injective-function) of $f$. Fix one $a_0\in A$, using the given nonemptiness, and define

$$
h(c)=\begin{cases}a,&c=j(a)\text{ for some }a\in A,\\a_0,&c\notin j(A).\end{cases}
$$

The first case is well defined because $j$ is an [injection](../../../algebra.md#injective-function). For every $a\in A$, $h(j(a))=a$. Thus this [left inverse](../../../function.md#left-inverse) satisfies $\boxed{h\circ g\circ f=\operatorname{id}_A}$, the [identity function](../../../function.md#identity-function) on $A$.

<h3 id="1d/iii">iii</h3>

↑ **Parent:** [1D](#1d)

<h4 id="1d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1d/iii)

**False.** Take $A=\{0,1\}$, $B=\{0\}$ and the [constant function](../../../function.md#constant-function) $f(a)=0$. For the [subsets](../../../set.md#subset) $X=\{0\}$ and $Y=\{1\}$, the [intersection](../../../set.md#set-intersection) $X\cap Y$ is empty, so $f(X\cap Y)=\varnothing$, whereas the [intersection](../../../set.md#set-intersection) of their [images of a function](../../../set-theory.md#image-of-a-function) is $f(X)\cap f(Y)=\{0\}$. In general the inclusion $f(X\cap Y)\subseteq f(X)\cap f(Y)$ holds, but a common image value can arise from different points of $X$ and $Y$.

<h3 id="1d/iv">iv</h3>

↑ **Parent:** [1D](#1d)

<h4 id="1d/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1d/iv)

**True.** For each $a\in A$, the definition of [preimage](../../../set-theory.md#preimage) gives

$$
a\in f^{-1}(Z\cap W)\iff f(a)\in Z\cap W\iff f(a)\in Z\text{ and }f(a)\in W\iff a\in f^{-1}(Z)\cap f^{-1}(W).
$$

Thus $\boxed{f^{-1}(Z\cap W)=f^{-1}(Z)\cap f^{-1}(W)}$. Unlike the corresponding statement for [images of a function](../../../set-theory.md#image-of-a-function), this [intersection](../../../set.md#set-intersection) identity requires no [injectivity](../../../algebra.md#injective-function).

## 2D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2d/a">a</h3>

↑ **Parent:** [2D](#2d)

<h4 id="2d/a/solution">Solution</h4>

↑ **Parent:** [A](#2d/a)

The [equivalence class](../../../set-theory.md#equivalence-class) of $x\in X$ is $[x]=\{y\in X:y\sim x\}$. By the reflexivity of the [equivalence relation](../../../set-theory.md#equivalence-relation), $x\in[x]$, so every [equivalence class](../../../set-theory.md#equivalence-class) is nonempty and their union is $X$.

Suppose $[x]\cap[z]\ne\varnothing$, and choose $w$ in this [intersection](../../../set.md#set-intersection). We have $w\sim x$ and $w\sim z$. Symmetry and transitivity give $x\sim z$. If $y\in[x]$, then $y\sim x\sim z$, so $y\in[z]$; interchanging $x,z$ proves the reverse inclusion. Thus two [equivalence classes](../../../set-theory.md#equivalence-class) are either identical or disjoint. **The distinct [equivalence classes](../../../set-theory.md#equivalence-class) therefore form a [set partition](../../../combinatorics.md#set-partition) of $X$.** This also covers $X=\varnothing$, whose family of [equivalence classes](../../../set-theory.md#equivalence-class) is empty.

<h3 id="2d/b">b</h3>

↑ **Parent:** [2D](#2d)

<h4 id="2d/b/solution">Solution</h4>

↑ **Parent:** [B](#2d/b)

For positive [integers](../../../number-theory.md#integer), $m/m=2^0$, establishing reflexivity. If $m/n=2^k$, then $n/m=2^{-k}$, establishing symmetry. If also $n/\ell=2^j$, then $m/\ell=2^{k+j}$, establishing transitivity. Hence this is an [equivalence relation](../../../set-theory.md#equivalence-relation).

Every positive [integer](../../../number-theory.md#integer) can be written uniquely as $m=2^r d$, where $r\geq0$ is an [integer](../../../number-theory.md#integer) and $d$ is an odd positive [integer](../../../number-theory.md#integer), its [odd part of a positive integer](../../../number-theory.md#odd-part-of-a-positive-integer). Existence follows by repeatedly dividing by two while the result is even; the process terminates because the positive [integers](../../../number-theory.md#integer) strictly decrease. For uniqueness, $2^r d=2^s e$ with $d,e$ odd would make one of $d,e$ even if $r\ne s$; therefore $r=s$ and $d=e$.

Multiplying by a power of two preserves the [odd part of a positive integer](../../../number-theory.md#odd-part-of-a-positive-integer), and two positive [integers](../../../number-theory.md#integer) with the same odd part have ratio a power of two. The [equivalence class](../../../set-theory.md#equivalence-class) indexed by odd $d$ is consequently $\{2^r d:r\geq0\}$. **The required representative set is $\boxed{A=\{1,3,5,\ldots\}}$.**

## 3B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3b/solution">Solution</h3>

↑ **Parent:** [3B](#3b)

Put $M=m_1+m_2$ and let $\mathbf R=(m_1\mathbf r_1+m_2\mathbf r_2)/M$ be the [center of mass](../../../classical-mechanics.md#center-of-mass). Applying [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) separately to the two [point masses](../../../classical-mechanics.md#point-mass) gives

$$
m_1\ddot{\mathbf r}_1=\mathbf f,\qquad m_2\ddot{\mathbf r}_2=-\mathbf f,\qquad M\ddot{\mathbf R}=0.
$$

Thus the [center of mass](../../../classical-mechanics.md#center-of-mass) has constant [velocity](../../../classical-mechanics.md#velocity), $\mathbf R(t)=\mathbf R(0)+t\dot{\mathbf R}(0)$. For the relative [position](../../../classical-mechanics.md#position) $\mathbf r=\mathbf r_1-\mathbf r_2$, subtraction gives

$$
\ddot{\mathbf r}=\left(\frac1{m_1}+\frac1{m_2}\right)\mathbf f,\qquad \boxed{\mu\ddot{\mathbf r}=\mathbf f},\qquad \mu=\frac{m_1m_2}{m_1+m_2}.
$$

Here $\mu$ is the [reduced mass](../../../classical-mechanics.md#reduced-mass); it converts the relative motion into a one-body [equation of motion](../../../classical-mechanics.md#equation-of-motion).

For the given linear [force](../../../classical-mechanics.md#force), the relative [position](../../../classical-mechanics.md#position) obeys [simple harmonic motion](../../../classical-mechanics.md#simple-harmonic-motion), $\ddot{\mathbf r}+\Omega^2\mathbf r=0$, where $\Omega^2=k/\mu$. The initial rest condition gives

$$
\mathbf r(t)=\mathbf r(0)\cos(\Omega t),\qquad |\mathbf r(0)|=d.
$$

For $d>0$, collision first occurs when the relative [position](../../../classical-mechanics.md#position) vanishes, namely when $\Omega t=\pi/2$. Therefore

$$
\boxed{t_{\rm collision}=\frac\pi2\sqrt{\frac{m_1m_2}{k(m_1+m_2)}}}.
$$

The separation $d$ cancels because the [frequency](../../../physics.md#frequency) of this [simple harmonic motion](../../../classical-mechanics.md#simple-harmonic-motion) is independent of its [amplitude](../../../physics.md#wave-amplitude).

## 4B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

Introduce $v=\dot x$. The [phase plane](../../../dynamical-systems.md#phase-plane) system for the [damped pendulum](../../../classical-mechanics.md#damped-pendulum) is

$$
\dot x=v,\qquad \dot v=-2kv-\omega^2\sin x.
$$

At an [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system), $v=0$ and $\sin x=0$, so all [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are $\boxed{(x,v)=(n\pi,0),\ n\in\mathbb Z}$. Angles identified modulo $2\pi$ give one downward and one upward [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system).

The [linearization of a dynamical system](../../../algebra.md#linearization-of-a-dynamical-system) at $(n\pi,0)$ has [Jacobian matrix](../../../calculus.md#jacobian-matrix) and [eigenvalues](../../../linear-operator-theory.md#eigenvalue)

$$
J_n=\begin{pmatrix}0&1\\-\omega^2(-1)^n&-2k\end{pmatrix},\qquad \lambda_\pm=-k\pm\sqrt{k^2-\omega^2(-1)^n}.
$$

When $n$ is even and $k>\omega$, both [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are real and strictly negative, since $0<\sqrt{k^2-\omega^2}<k$. These downward [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are **[stable nodes](../../../dynamical-systems.md#stable-node)**. When $n$ is even and $k<\omega$, the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $-k\pm i\sqrt{\omega^2-k^2}$, so the downward [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are **[stable foci](../../../dynamical-systems.md#stable-spiral)**, approached with decaying oscillations.

When $n$ is odd, $\sqrt{k^2+\omega^2}>k$, so one [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is positive and one is negative in either parameter range. Every upward [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is consequently an **unstable [saddle equilibrium](../../../dynamical-systems.md#saddle-equilibrium)**. All these [equilibrium points](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) are [hyperbolic equilibria](../../../dynamical-systems.md#hyperbolic-equilibrium-point) in the two requested cases, so their [linearization of a dynamical system](../../../algebra.md#linearization-of-a-dynamical-system) gives their local nonlinear classification.

## 5D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5d/a">a</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/a/solution">Solution</h4>

↑ **Parent:** [A](#5d/a)

A [set](../../../set.md) is countable if it admits an [injection](../../../algebra.md#injective-function) into the [natural numbers](../../../arithmetic.md#natural-number); this includes [finite sets](../../../set.md#finite-set) and the empty [set](../../../set.md). Use $\mathbb N_0=\{0,1,2,\ldots\}$ for the enumeration. The [Cantor pairing function](../../../set-theory.md#cantor-pairing-function)

$$
\Pi(i,j)=\frac{(i+j)(i+j+1)}2+j
$$

is a [bijection](../../../function.md#bijection) $\mathbb N_0^2\to\mathbb N_0$. Indeed, on the diagonal $i+j=s$, its values are the consecutive [integers](../../../number-theory.md#integer) from $s(s+1)/2$ through $s(s+1)/2+s$. These intervals are disjoint, and the next starts one beyond the preceding endpoint. Every nonnegative [integer](../../../number-theory.md#integer) therefore determines exactly one diagonal $s$, then exactly one $j$, and finally $i=s-j$. If one's convention starts the [natural numbers](../../../arithmetic.md#natural-number) at one, translate both coordinates by one. Thus **$\mathbb N\times\mathbb N$ is a [countable set](../../../set-theory.md#countable-set)**.

For [countable sets](../../../set-theory.md#countable-set) $X,Y$, choose [injections](../../../algebra.md#injective-function) $e_X:X\to\mathbb N_0$ and $e_Y:Y\to\mathbb N_0$. The map $(x,y)\mapsto\Pi(e_X(x),e_Y(y))$ is an [injection](../../../algebra.md#injective-function), proving their [Cartesian product](../../../set-theory.md#cartesian-product) is countable. Repeating this proves that every [finite Cartesian power of a countable set](../../../set-theory.md#finite-cartesian-power-of-a-countable-set) is countable.

For a sequence of [countable sets](../../../set-theory.md#countable-set) $X_n$, choose an [injection](../../../algebra.md#injective-function) $e_n:X_n\to\mathbb N_0$ for each $n$. For $x\in\bigcup_nX_n$, let $n(x)$ be the least index containing $x$. The map

$$
x\longmapsto\Pi\bigl(n(x),e_{n(x)}(x)\bigr)
$$

is an [injection](../../../algebra.md#injective-function): its value recovers $n(x)$ and then $x$. This proves the **[countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets) theorem**. Selecting all $e_n$ uses the usual [axiom of countable choice](../../../set-theory.md#axiom-of-countable-choice); if enumerations are already supplied, the construction itself needs no additional choices.

<h3 id="5d/b">b</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/b/solution">Solution</h4>

↑ **Parent:** [B](#5d/b)

For a [countable set](../../../set-theory.md#countable-set) $A$, the [polynomials](../../../polynomial.md) of [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) at most $d$ with coefficients in $A$ are described by coefficient tuples in $A^{d+1}$. The [finite Cartesian power of a countable set](../../../set-theory.md#finite-cartesian-power-of-a-countable-set) result makes this a [countable set](../../../set-theory.md#countable-set). Taking the union over $d\geq0$ shows there are only countably many such [polynomials](../../../polynomial.md) altogether; restricting to the nonzero [polynomials](../../../polynomial.md) preserves countability.

A nonzero [polynomial](../../../polynomial.md) of [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) $d$ has at most $d$ distinct [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial). To see the bound, a root $r$ gives the factorization $P(x)=(x-r)Q(x)$ by the [factor theorem](../../../polynomial.md#factor-theorem), and each other root is a root of $Q$, whose degree is $d-1$; induction starts with a nonzero constant, which has no roots. Thus $\phi(A)$ is a [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets), each of them finite, and is a [countable set](../../../set-theory.md#countable-set).

Starting with the given [countable set](../../../set-theory.md#countable-set) $A_0$, [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) now shows that every $A_n=\phi(A_{n-1})$ is countable. A final application of the [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets) theorem gives

$$
\boxed{\bigcup_{n=1}^{\infty}A_n\text{ is countable}.}
$$

This countability argument does not require that the sequence of [sets](../../../set.md) be increasing.

<h3 id="5d/c">c</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/c/solution">Solution</h4>

↑ **Parent:** [C](#5d/c)

To obtain a [countable closure under real polynomial roots](../../../set-theory.md#countable-closure-under-real-polynomial-roots), start with $B_0=\{1,\pi\}$ and explicitly retain previous elements at each stage:

$$
B_{n+1}=B_n\cup\phi(B_n),\qquad X=\bigcup_{n=0}^{\infty}B_n.
$$

Part (b) shows that $\phi$ takes [countable sets](../../../set-theory.md#countable-set) to [countable sets](../../../set-theory.md#countable-set); consequently all $B_n$ and then $X$ are countable by the [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets) theorem. Also $1,\pi\in X$.

For a nonzero [polynomial](../../../polynomial.md) $P(t)=c_0+\cdots+c_dt^d$ with all $c_j\in X$, choose stages $n_j$ containing the finitely many coefficients and put $N=\max_jn_j$. The inclusions $B_n\subseteq B_{n+1}$ ensure that every coefficient belongs to $B_N$. Every real [root of a polynomial](../../../polynomial.md#root-of-a-polynomial) $P$ therefore belongs to $\phi(B_N)\subseteq B_{N+1}\subseteq X$. **This [countable set](../../../set-theory.md#countable-set) $X$ has all the required properties.** Retaining $B_n$ explicitly avoids assuming the generally false inclusion $A\subseteq\phi(A)$: for example, $\phi(\{1\})$ does not contain $1$, since a nonzero [polynomial](../../../polynomial.md) all of whose coefficients are one is positive at $1$.

## 6D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6d/a">a</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/a/solution">Solution</h4>

↑ **Parent:** [A](#6d/a)

Let $d=\gcd(a,m)$. If the [linear congruence](../../../number-theory.md#linear-congruence) $ar\equiv b\pmod m$ holds, then $b=ar-ms$ for some [integer](../../../number-theory.md#integer) $s$, so the [greatest common divisor](../../../number-theory.md#greatest-common-divisor) $d$ divides $b$. Conversely, [Bézout's identity](../../../algebra.md#bezout-identity) gives [integers](../../../number-theory.md#integer) $u,v$ with $au+mv=d$. If $b=dj$, multiply this identity by $j$ to obtain $a(uj)\equiv b\pmod m$. Hence

$$
\boxed{ar\equiv b\pmod m\text{ has a solution}\iff d\mid b.}
$$

For the number of solutions, write $a=da'$, $m=dm'$ and $b=db'$. The [linear congruence](../../../number-theory.md#linear-congruence) becomes $a'r\equiv b'\pmod {m'}$, where $a',m'$ are [coprime integers](../../../number-theory.md#coprime-integers). Multiplication by $a'$ is invertible modulo $m'$ by [Bézout's identity](../../../algebra.md#bezout-identity), so the solutions form one [residue class](../../../number-theory.md#residue-class) $r\equiv r_0\pmod {m'}$. Modulo $m=dm'$, these are exactly

$$
\boxed{r_0,\ r_0+m',\ldots,r_0+(d-1)m'.}
$$

They are distinct: if two have the same [residue class](../../../number-theory.md#residue-class) modulo $m$, then $dm'$ divides $(j-\ell)m'$, forcing $d\mid j-\ell$; with $0\leq j,\ell<d$, this forces $j=\ell$. Every other solution differs from $r_0$ by a multiple of $m'$, so these exhaust the $d$ solutions.

Finally,

$$
b(m/d)\equiv0\pmod m\iff dm'\mid bm'\iff d\mid b.
$$

Combining this with the existence criterion gives the requested equivalent [modular congruence](../../../number-theory.md#modular-congruence).

<h3 id="6d/b">b</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/b/solution">Solution</h4>

↑ **Parent:** [B](#6d/b)

Take a generator $u$ of the [multiplicative group of a finite field](../../../algebra.md#multiplicative-group-of-a-finite-field) $\mathbb F_p^\times$, which has order $p-1$. Write $x=u^a$. Since any possible nonzero base is $y=u^r$, the condition of being a $k$th power is

$$
x=y^k\iff u^a=u^{kr}\iff kr\equiv a\pmod {p-1}.
$$

By part (a), this [linear congruence](../../../number-theory.md#linear-congruence) is soluble exactly when $d=\gcd(k,p-1)$ divides $a$. Meanwhile

$$
x^{(p-1)/d}=1\iff u^{a(p-1)/d}=1\iff (p-1)\mid a(p-1)/d\iff d\mid a.
$$

Thus the required test is

$$
\boxed{x\text{ is a }k\text{th power in }\mathbb F_p^\times\iff x^{(p-1)/d}\equiv1\pmod p.}
$$

The exponent [residue classes](../../../number-theory.md#residue-class) divisible by $d$ are $0,d,\ldots,p-1-d$, so there are exactly $(p-1)/d$ distinct nonzero $k$th powers. Equivalently, part (a) shows each value has exactly $d$ preimages under the power map.

<h3 id="6d/c">c</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/c/solution">Solution</h4>

↑ **Parent:** [C](#6d/c)

The [greatest common divisor](../../../number-theory.md#greatest-common-divisor) is

$$
\gcd(437,1012)=\gcd(19\cdot23,44\cdot23)=23,
$$

since $19$ and $44$ are [coprime integers](../../../number-theory.md#coprime-integers). Part (b) therefore gives $\boxed{1012/23=44}$ distinct $437$th powers in the nonzero [multiplicative group of a finite field](../../../algebra.md#multiplicative-group-of-a-finite-field) $\mathbb F_{1013}^\times$. If “powers mod $1013$” includes all [residue classes](../../../number-theory.md#residue-class), the additional value $0=0^{437}$ gives **$\boxed{45}$ values including zero**. The distinction is relevant because part (b) explicitly works in the nonzero group.

## 7D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7d/a">a</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/a/solution">Solution</h4>

↑ **Parent:** [A](#7d/a)

Suppose $x^2+y^2=0$ in the [field](../../../algebra.md#field) $F$. If $y\ne0$, division by $y^2$ gives $(x/y)^2=-1$, contrary to the hypothesis. Hence $y=0$ and then $x^2=0$; the absence of nonzero [zero divisors](../../../mathematics.md#zero-divisor) in a [field](../../../algebra.md#field) gives $x=0$. Therefore

$$
\boxed{x^2+y^2=0\Longrightarrow x=y=0.}
$$

For the stated operations on $F^2$, addition is an [abelian group](../../../group.md#abelian-group) operation: [associativity](../../../group.md#associative-property) and [commutativity](../../../algebra.md#commutativity) hold componentwise, its identity is $(0,0)$, and the negative of $(x,y)$ is $(-x,-y)$.

To check multiplication without omitting associativity, associate to each pair the [matrix](../../../vector-space.md#matrix)

$$
M(x,y)=\begin{pmatrix}x&-y\\y&x\end{pmatrix}.
$$

This is an [injection](../../../algebra.md#injective-function) into the two-by-two [matrices](../../../vector-space.md#matrix) over $F$, and direct [matrix multiplication](../../../vector-space.md#matrix-multiplication) gives

$$
M(x,y)M(z,w)=M(xz-yw,xw+yz).
$$

It also preserves addition. The [associativity](../../../group.md#associative-property) and distributivity of [matrix multiplication](../../../vector-space.md#matrix-multiplication) therefore imply the same laws for the pair multiplication. Its formula is symmetric in the pairs, so it is commutative. Its identity is $(1,0)$, which is different from $(0,0)$.

For a nonzero pair, the first result shows that $x^2+y^2\ne0$. Its multiplicative inverse is

$$
\boxed{(x,y)^{-1}=\left(\frac{x}{x^2+y^2},\frac{-y}{x^2+y^2}\right),}
$$

since multiplying $(x,y)$ by $(x,-y)$ gives $(x^2+y^2,0)$. This verifies every [field](../../../algebra.md#field) axiom, so **the given operations make $F^2$ a [field](../../../algebra.md#field)**. The embedded copy of $F$ is $\{(x,0):x\in F\}$; the element $(0,1)$ has square $(-1,0)$, describing a [quadratic extension](../../../algebra.md#quadratic-extension) of $F$.

<h3 id="7d/b">b</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/b/solution">Solution</h4>

↑ **Parent:** [B](#7d/b)

Suppose $x^2\equiv-1\pmod p$. Then $x\ne0$ modulo the [prime number](../../../number-theory.md#prime-number) $p$, so [Fermat's little theorem](../../../number-theory.md#fermat-little-theorem) gives $x^{p-1}\equiv1\pmod p$. But $p=4m+3$ makes $(p-1)/2=2m+1$ odd, and therefore

$$
x^{p-1}=(x^2)^{(p-1)/2}\equiv(-1)^{2m+1}=-1\pmod p.
$$

This contradicts $1\not\equiv-1\pmod p$, since $p$ is odd. Thus **$-1$ is not a [quadratic residue](../../../number-theory.md#quadratic-residue) modulo $p$**. Apply part (a) to the [finite field](../../../algebra.md#finite-field) $F=\mathbb F_p$: the pairs $F^2$ with the given operations form a [field](../../../algebra.md#field), and there are $p$ choices for each coordinate, so its [cardinality](../../../set-theory.md#cardinality) is $\boxed{p^2}$.

## 8D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

The key [telescoping series](../../../real-analysis.md#telescoping-series) identity is

$$
c_k=\frac{(q+k-1)q!}{(q+k)!}=\frac{q!}{(q+k-1)!}-\frac{q!}{(q+k)!}.
$$

For the requested [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction), when $n=1$ the proposed sum is $q/(q+1)=1-q!/(q+1)!$. If the identity holds for $n$, adding $c_{n+1}=q!/(q+n)!-q!/(q+n+1)!$ cancels its last term and yields $1-q!/(q+n+1)!$. Thus it holds for every $n\geq1$. Since $q!/(q+n)!\to0$ for fixed positive [integer](../../../number-theory.md#integer) $q$, the infinite [series](../../../real-analysis.md#series-mathematics) has sum $\boxed{1}$.

For the second [series](../../../real-analysis.md#series-mathematics), the integral digit condition is $0\leq a_n\leq n-1$, and in particular $a_1=0$. Its partial sums are increasing and satisfy

$$
0\leq\sum_{n=1}^N\frac{a_n}{n!}\leq\sum_{n=1}^N\frac{n-1}{n!}=1-\frac1{N!}\leq1.
$$

Thus the [bounded monotone sequence theorem](../../../real-analysis.md#bounded-monotone-sequence-theorem) proves convergence to a [real number](../../../arithmetic.md#real-number) $S\in[0,1]$. The same telescoping calculation gives, for every $N\geq1$,

$$
\sum_{n>N}\frac{n-1}{n!}=\frac1{N!},\qquad R_N:=N!\left(S-\sum_{n=1}^N\frac{a_n}{n!}\right)\in[0,1].
$$

If positive digits occur infinitely often, then every tail contains a positive term, so $R_N>0$. If $a_n\leq n-2$ occurs infinitely often, then every tail contains a digit smaller than its maximum. Indeed,

$$
1-R_N=N!\sum_{n>N}\frac{n-1-a_n}{n!}>0.
$$

Consequently the two conditions together give $0<R_N<1$ for every $N$. Were $S=A/B$ a [rational number](../../../number-theory.md#rational-number), with positive [integer](../../../number-theory.md#integer) $B$, choose $N\geq B$. Because $B\mid N!$, the number $N!S$ is an [integer](../../../number-theory.md#integer), as is $\sum_{n=1}^Na_nN!/n!$. Their difference $R_N$ would be an [integer](../../../number-theory.md#integer) strictly between zero and one, a contradiction.

Conversely, if positive digits occur only finitely often, then $S$ is a finite sum of [rational numbers](../../../number-theory.md#rational-number). If digits below their maximum occur only finitely often, then $a_n=n-1$ for every $n>N$ for some $N$, giving

$$
S=\sum_{n=1}^N\frac{a_n}{n!}+\frac1{N!}\in\mathbb Q.
$$

These are exactly the two ways the conjunction of infinitude conditions can fail. Hence the [irrationality criterion for factorial series](../../../real-analysis.md#irrationality-criterion-for-factorial-series) is proved in both directions: **$S$ is irrational exactly when both kinds of digit occur infinitely often.**

## 9B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9b/solution">Solution</h3>

↑ **Parent:** [9B](#9b)

During ejection, the remaining [mass](../../../classical-mechanics.md#mass) is $m(t)=m_o+m_w-Qt$, and the water is exhausted at $t_c=m_w/Q$. Consider the [momentum](../../../classical-mechanics.md#momentum) of the octopus and the small portion of water expelled during $dt$. Initially it is $mu$. At the end of this interval, the remaining body has [mass](../../../classical-mechanics.md#mass) $m-Q\,dt$ and [velocity](../../../classical-mechanics.md#velocity) $u+du$, while the expelled [mass](../../../classical-mechanics.md#mass) $Q\,dt$ has laboratory [velocity](../../../classical-mechanics.md#velocity) $u-V$, to first order. Hence the total final [momentum](../../../classical-mechanics.md#momentum) is

$$
(m-Q\,dt)(u+du)+Q\,dt(u-V)=mu+m\,du-QV\,dt+o(dt).
$$

The external [impulse](../../../classical-mechanics.md#impulse) from [quadratic drag](../../../fluid-mechanics.md#quadratic-drag) is $-\alpha u^2dt$. Equating this to the change in total [momentum](../../../classical-mechanics.md#momentum), and dividing by $dt$, proves the [equation of motion](../../../classical-mechanics.md#equation-of-motion)

$$
\boxed{m\frac{du}{dt}=QV-\alpha u^2.}
$$

The outgoing water's [momentum](../../../classical-mechanics.md#momentum) flux is essential: applying $d(mu)/dt$ to the remaining body alone would omit it.

For [dimensional analysis](../../../physics.md#dimensional-analysis), the independent physical inputs are $m_o,m_w,Q,V,\alpha$, with dimensions

$$
[m_o]=[m_w]=\mathsf M,\quad[Q]=\mathsf M\mathsf T^{-1},\quad[V]=\mathsf L\mathsf T^{-1},\quad[\alpha]=\mathsf M\mathsf L^{-1}.
$$

The scales $m_o$, $m_o/Q$ and $Vm_o/Q$ fix units of [mass](../../../classical-mechanics.md#mass), time and length. In these units, the only remaining independent [dimensionless variables](../../../mathematics.md#dimensionless-variable) are

$$
\boxed{\lambda=\frac{m_w}{m_o},\qquad\mu=\frac{\alpha V}{Q}.}
$$

For example, with $s=Qt/m_o$ and $w=u/V$, the [equation of motion](../../../classical-mechanics.md#equation-of-motion) becomes $(1+\lambda-s)\,dw/ds=1-\mu w^2$, with $w(0)=0$ and ejection ending at $s=\lambda$. Thus the dimensionless terminal value depends only on $\lambda,\mu$, proving $u_c=Vf(\lambda,\mu)$.

For its explicit value, put $m_0=m_o+m_w$ and $U=\sqrt{QV/\alpha}$. The initially stationary solution stays below $U$, since the [acceleration](../../../classical-mechanics.md#acceleration) vanishes at $U$ and is positive below it. [Separation of variables](../../../partial-differential-equation.md#separation-of-variables) gives

$$
\int_0^{u(t)}\frac{dv}{QV-\alpha v^2}=\int_0^t\frac{d\tau}{m_0-Q\tau}.
$$

The two integrals yield

$$
\frac{1}{\sqrt{\alpha QV}}\operatorname{artanh}\frac{u(t)}U=\frac1Q\log\frac{m_0}{m_0-Qt}.
$$

This is [constant mass-loss propulsion with quadratic drag](../../../classical-mechanics.md#constant-mass-loss-propulsion-with-quadratic-drag). At $t_c$, the remaining [mass](../../../classical-mechanics.md#mass) is $m_o$, giving

$$
\boxed{u_c=\sqrt{\frac{QV}{\alpha}}\tanh\left(\sqrt{\frac{\alpha V}{Q}}\log\frac{m_o+m_w}{m_o}\right)
=\frac{V}{\sqrt\mu}\tanh\bigl(\sqrt\mu\log(1+\lambda)\bigr).}
$$

Thus $f(\lambda,\mu)=\mu^{-1/2}\tanh(\sqrt\mu\log(1+\lambda))$, verifying the required dimensional form. The limit as drag tends to zero is $V\log(1+\lambda)$, the ordinary [rocket equation](../../../classical-mechanics.md#rocket-equation), while the positive-drag answer is below the [terminal velocity](../../../classical-mechanics.md#terminal-velocity) $U$.

## 10B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10b/i">i</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/i/solution">Solution</h4>

↑ **Parent:** [I](#10b/i)

Multiplying the tangential [equation of motion](../../../classical-mechanics.md#equation-of-motion) by $r$ gives

$$
\frac d{dt}(r^2\dot\theta)=r^2\ddot\theta+2r\dot r\dot\theta=0.
$$

Therefore $h=r^2\dot\theta$ is constant. It is the signed [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum); reverse the angular orientation if necessary to take $h>0$ for a nonradial [orbit](../../../dynamical-systems.md#orbit-dynamical-system). Set $u=1/r$ and denote differentiation with respect to $\theta$ by a prime. Then

$$
\dot\theta=hu^2,\qquad \dot r=-hu',\qquad \ddot r=-h^2u^2u'',\qquad r\dot\theta^2=h^2u^3.
$$

Substitution into the radial [equation of motion](../../../classical-mechanics.md#equation-of-motion) and division by $-h^2u^2$ give the [Binet equation](../../../classical-mechanics.md#binet-equation)

$$
u''+u=\frac{GM}{h^2}.
$$

Its general solution is $u=GM/h^2+A\cos\theta+B\sin\theta$. Write $A=(GM/h^2)e\cos\theta_0$ and $B=(GM/h^2)e\sin\theta_0$, where $e\geq0$. This produces the [Kepler orbit](../../../classical-mechanics.md#kepler-orbit)

$$
\boxed{\frac{h^2u}{GM}=1+e\cos(\theta-\theta_0).}
$$

Here $e$ is the [orbital eccentricity](../../../classical-mechanics.md#orbital-eccentricity), and $\theta_0$ points toward [periapsis](../../../classical-mechanics.md#periapsis) when $e>0$. Only portions with $u>0$ describe positive radial distances. The expression assumes $h\ne0$; a zero-[angular momentum](../../../classical-mechanics.md#angular-momentum) trajectory is radial and must be treated separately.

<h3 id="10b/ii">ii</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10b/ii)

Choose the [gravitational potential energy](../../../classical-mechanics.md#gravitational-energy) to vanish at infinity. The total [mechanical energy](../../../classical-mechanics.md#mechanical-energy) is

$$
E=\frac m2\bigl(\dot r^2+r^2\dot\theta^2\bigr)-\frac{GMm}{r}=\frac{mh^2}2\bigl((u')^2+u^2\bigr)-GMm\,u.
$$

Put $\gamma=GM/h^2$ and $\varphi=\theta-\theta_0$. From part (i), $u=\gamma(1+e\cos\varphi)$ and $u'=-\gamma e\sin\varphi$. Consequently

$$
(u')^2+u^2=\gamma^2\bigl(1+2e\cos\varphi+e^2\bigr),
$$

and the angular terms cancel against the [gravitational potential energy](../../../classical-mechanics.md#gravitational-energy):

$$
\boxed{E=\frac{mG^2M^2}{2h^2}(e^2-1).}
$$

For a nonradial [Kepler orbit](../../../classical-mechanics.md#kepler-orbit), negative, zero and positive [mechanical energy](../../../classical-mechanics.md#mechanical-energy) correspond respectively to $e<1$, $e=1$ and $e>1$.

<h3 id="10b/solution">Solution</h3>

↑ **Parent:** [10B](#10b)

At infinity, the meteorite's incoming asymptote has [speed](../../../classical-mechanics.md#speed) $V$ and perpendicular distance $b$ from the Earth’s centre. The magnitude of its [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) is the magnitude of $\mathbf r\times\mathbf v$. On the asymptote, this is $bV$, so [conservation of angular momentum](../../../classical-mechanics.md#conservation-of-angular-momentum) gives $\boxed{h=bV}$. Its [mechanical energy](../../../classical-mechanics.md#mechanical-energy) at infinity is $E=mV^2/2$. Comparing with part (ii) gives

$$
\boxed{e=\sqrt{1+\frac{b^2V^4}{G^2M^2}}}.
$$

For $b>0$ this [Kepler orbit](../../../classical-mechanics.md#kepler-orbit) is a [hyperbola](../../../geometry-and-topology.md#hyperbola). The smallest $r=1/u$ occurs at [periapsis](../../../classical-mechanics.md#periapsis), where $\cos(\theta-\theta_0)=1$. Thus

$$
\boxed{r_{\min}=\frac{b^2V^2}{GM(1+e)}=\frac{GM}{V^2}(e-1)
=\frac{\sqrt{G^2M^2+b^2V^4}-GM}{V^2}.}
$$

The middle equality follows by substituting $e^2-1=b^2V^4/(G^2M^2)$. A trajectory entering the Earth satisfies $r_{\min}<R$, equivalently

$$
e<1+\frac{RV^2}{GM}\iff b^2<R^2+\frac{2GMR}{V^2}.
$$

Therefore the sufficient collision condition is

$$
\boxed{b<\sqrt{R^2+\frac{2GMR}{V^2}}.}
$$

This is [gravitational focusing](../../../classical-mechanics.md#gravitational-focusing): [Newtonian gravity](../../../classical-mechanics.md#gravitational-acceleration) increases the collision radius measured at infinity. Equality is the ideal grazing trajectory, which touches the surface; a strict inequality penetrates it. For $b=0$ the incoming motion is radial and collides, with $r_{\min}=0$ as the limiting value of the above expression.

## 11B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11b/i">i</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/i/solution">Solution</h4>

↑ **Parent:** [I](#11b/i)

Let $\mathbf e'_1(t),\mathbf e'_2(t),\mathbf e'_3(t)$ be an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) fixed in the [rotating reference frame](../../../physics.md#rotating-reference-frame) $S'$. A small rotation through $\boldsymbol\omega\,dt$ changes each basis vector by $\boldsymbol\omega\times\mathbf e'_j\,dt$, so its derivative in the [inertial frame](../../../physics.md#inertial-frame) is

$$
\left(\frac{d\mathbf e'_j}{dt}\right)_S=\boldsymbol\omega\times\mathbf e'_j.
$$

Write the arbitrary [vector](../../../vector-space.md#vector) as $\mathbf a=\sum_j a_j(t)\mathbf e'_j(t)$. Differentiating the components and the moving basis separately gives

$$
\left(\frac{d\mathbf a}{dt}\right)_S=\sum_j\dot a_j\mathbf e'_j+\sum_j a_j\boldsymbol\omega\times\mathbf e'_j
=\left(\frac{d\mathbf a}{dt}\right)_{S'}+\boldsymbol\omega\times\mathbf a.
$$

This proves the **[rotating-frame derivative formula](../../../physics.md#rotating-frame-derivative-formula)**, including when the [angular velocity](../../../classical-mechanics.md#angular-velocity) varies with time.

<h3 id="11b/ii">ii</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11b/ii)

Use $D=(d/dt)_S$, $D'=(d/dt)_{S'}$, and $\mathbf v'=D'\mathbf r$. By the [rotating-frame derivative formula](../../../physics.md#rotating-frame-derivative-formula), $D\mathbf r=\mathbf v'+\boldsymbol\omega\times\mathbf r$. Apply the [product rule](../../../calculus.md#product-rule) for the [cross product](../../../vector-space.md#cross-product) and the same [rotating-frame derivative formula](../../../physics.md#rotating-frame-derivative-formula) again:

$$
D^2\mathbf r=D\mathbf v'+(D\boldsymbol\omega)\times\mathbf r+\boldsymbol\omega\times D\mathbf r.
$$

We have $D\mathbf v'=D'\mathbf v'+\boldsymbol\omega\times\mathbf v'$ and $D\boldsymbol\omega=D'\boldsymbol\omega$, since $\boldsymbol\omega\times\boldsymbol\omega=0$. Therefore

$$
\boxed{D^2\mathbf r=D'^2\mathbf r+2\boldsymbol\omega\times D'\mathbf r+(D'\boldsymbol\omega)\times\mathbf r+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf r).}
$$

Rearranging this identity into an [equation of motion in a rotating frame](../../../classical-mechanics.md#equation-of-motion-in-a-rotating-frame) produces the apparent [Coriolis acceleration](../../../physics.md#coriolis-acceleration), [Euler acceleration](../../../physics.md#euler-acceleration) and [centrifugal acceleration](../../../physics.md#centrifugal-acceleration), with signs opposite to their corresponding terms on the right of this inertial [acceleration](../../../classical-mechanics.md#acceleration) identity. No translational term is needed because the two origins coincide.

<h3 id="11b/solution">Solution</h3>

↑ **Parent:** [11B](#11b)

Let $\Omega$ be the Earth's [angular velocity](../../../classical-mechanics.md#angular-velocity) magnitude. Use the local east, north and upward unit [vectors](../../../vector-space.md#vector) $\mathbf e_E,\mathbf e_N,\mathbf e_U$, with $\mathbf e_E\times\mathbf e_N=\mathbf e_U$. At latitude $\lambda$, the Earth's [angular velocity](../../../classical-mechanics.md#angular-velocity) and the train's ground-relative [velocity](../../../classical-mechanics.md#velocity) are

$$
\boldsymbol\Omega=\Omega\cos\lambda\,\mathbf e_N+\Omega\sin\lambda\,\mathbf e_U,\qquad \mathbf v'=V\mathbf e_N.
$$

Thus the east component of the [Coriolis force](../../../physics.md#coriolis-force) is

$$
-2m\boldsymbol\Omega\times\mathbf v'=2m\Omega V\sin\lambda\,\mathbf e_E.
$$

For a north–south track, the train has no eastward [acceleration](../../../classical-mechanics.md#acceleration) relative to Earth. Its path curvature lies in the local north–vertical plane. The [centrifugal acceleration](../../../physics.md#centrifugal-acceleration) and [Newtonian gravity](../../../classical-mechanics.md#gravitational-acceleration) also lie in that plane, and the Earth's constant [angular velocity](../../../classical-mechanics.md#angular-velocity) gives no [Euler acceleration](../../../physics.md#euler-acceleration). Hence the sideways [force](../../../classical-mechanics.md#force) from the track must cancel the eastward [Coriolis force](../../../physics.md#coriolis-force):

$$
\boxed{\mathbf F_{\rm track,side}=-2m\Omega V\sin\lambda\,\mathbf e_E.}
$$

**Its magnitude is $2m\Omega V\sin\lambda$, and its direction is west** in the Northern hemisphere. The eastward tendency is the apparent [Coriolis force](../../../physics.md#coriolis-force); the requested track [force](../../../classical-mechanics.md#force) has the opposite direction.

## 12B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12b/solution">Solution</h3>

↑ **Parent:** [12B](#12b)

Let $\rho=3m/(4\pi R_0^3)$ be the uniform [mass density](../../../fluid-mechanics.md#density). In [spherical coordinates](../../../calculus.md#spherical-coordinate-system) $(r,\vartheta,\phi)$ with the chosen diameter as polar axis, the squared perpendicular distance to that axis is $r^2\sin^2\vartheta$. The [moment of inertia](../../../classical-mechanics.md#moment-of-inertia) is therefore

$$
I=\rho\int_0^{R_0}r^4\,dr\int_0^\pi\sin^3\vartheta\,d\vartheta\int_0^{2\pi}d\phi
=\frac{8\pi\rho R_0^5}{15}=\boxed{\frac25mR_0^2}.
$$

This derives the [moment of inertia of a uniform solid sphere](../../../classical-mechanics.md#moment-of-inertia-of-a-uniform-solid-sphere) about any central axis by [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry).

Put $a=R_1-R_0$. The [center of mass](../../../classical-mechanics.md#center-of-mass) follows the circle of radius $a$, with [position](../../../classical-mechanics.md#position) $\mathbf r_C=a(\sin\theta,-\cos\theta)$. Let $\mathbf e_r=(\sin\theta,-\cos\theta)$ and $\mathbf e_\theta=(\cos\theta,\sin\theta)$. Its [velocity](../../../classical-mechanics.md#velocity) is $a\dot\theta\mathbf e_\theta$, and the contact point is displaced from the [center of mass](../../../classical-mechanics.md#center-of-mass) by $R_0\mathbf e_r$. With positive spin [angular velocity](../../../classical-mechanics.md#angular-velocity) $\Omega_s$ counterclockwise, its contact-point [velocity](../../../classical-mechanics.md#velocity) is

$$
\mathbf v_{\rm contact}=a\dot\theta\mathbf e_\theta+\Omega_s\mathbf e_z\times R_0\mathbf e_r
=(a\dot\theta+R_0\Omega_s)\mathbf e_\theta.
$$

The cylinder is fixed, so [rolling without slipping](../../../classical-mechanics.md#rolling-without-slipping) requires this [velocity](../../../classical-mechanics.md#velocity) to vanish. Consequently $\Omega_s=-a\dot\theta/R_0$. If instead the spin angle $\psi$ is positive clockwise, opposite to increasing $\theta$, then the printed positive-coefficient convention is

$$
\boxed{\dot\psi=\frac{R_1-R_0}{R_0}\dot\theta.}
$$

The spin and orbital rotation have opposite directions when both are measured about the same oriented axis; the [angular speed](../../../classical-mechanics.md#angular-speed) is $a|\dot\theta|/R_0$. This specifies the sign convention in the printed expression.

The instantaneous contact point is at rest, so the [normal reaction](../../../classical-mechanics.md#normal-force) and [static friction](../../../classical-mechanics.md#static-friction) do no work. [Conservation of energy](../../../physics.md#conservation-of-energy) equates the loss of [gravitational potential energy](../../../classical-mechanics.md#gravitational-energy) from release to the total [kinetic energy](../../../classical-mechanics.md#kinetic-energy):

$$
mg a(\cos\theta-\cos\alpha)=\frac12ma^2\dot\theta^2+\frac12I\left(\frac a{R_0}\dot\theta\right)^2
=\frac7{10}ma^2\dot\theta^2.
$$

On the descent from $0<\alpha<\pi/2$, $\theta$ decreases, so

$$
\dot\theta=-\sqrt{\frac{10g}{7a}(\cos\theta-\cos\alpha)}.
$$

Integrating $dt=-d\theta/|\dot\theta|$ from release to the bottom gives

$$
\boxed{T_R=\sqrt{\frac{7(R_1-R_0)}{10g}}\int_0^\alpha\frac{d\theta}{\sqrt{\cos\theta-\cos\alpha}}.}
$$

The integral is finite: at the release point its denominator is asymptotic to $\sqrt{\sin\alpha\,(\alpha-\theta)}$. Contact is maintained, since the inward radial [equation of motion](../../../classical-mechanics.md#equation-of-motion) gives the positive [normal reaction](../../../classical-mechanics.md#normal-force) $N=m(g\cos\theta+a\dot\theta^2)$ throughout this range.

For frictionless sliding, the [normal reaction](../../../classical-mechanics.md#normal-force) passes through the sphere's centre and produces no [torque](../../../classical-mechanics.md#torque); [Newtonian gravity](../../../classical-mechanics.md#gravitational-acceleration) also exerts no central [torque](../../../classical-mechanics.md#torque). With initial zero spin, the sphere remains nonrotating. All the lost [gravitational potential energy](../../../classical-mechanics.md#gravitational-energy) becomes translational [kinetic energy](../../../classical-mechanics.md#kinetic-energy), so

$$
\frac12ma^2\dot\theta^2=mga(\cos\theta-\cos\alpha),\qquad
\boxed{T_S=\sqrt{\frac{R_1-R_0}{2g}}\int_0^\alpha\frac{d\theta}{\sqrt{\cos\theta-\cos\alpha}}=\sqrt{\frac57}\,T_R.}
$$

A hollow spherical shell of the same [mass](../../../classical-mechanics.md#mass) and radius places its material farther from the centre, giving a larger [moment of inertia](../../../classical-mechanics.md#moment-of-inertia). Under [rolling without slipping](../../../classical-mechanics.md#rolling-without-slipping), a given centre [speed](../../../classical-mechanics.md#speed) therefore requires more rotational [kinetic energy](../../../classical-mechanics.md#kinetic-energy); the same gravitational drop yields a smaller [speed](../../../classical-mechanics.md#speed). **Replacing the solid sphere by a hollow shell increases $T_R$ and leaves $T_S$ unchanged.** The sliding case remains nonrotating and has the same [center of mass](../../../classical-mechanics.md#center-of-mass) path and gravitational drop. This is the general comparison for [rolling inside a fixed circular cylinder](../../../classical-mechanics.md#rolling-inside-a-fixed-circular-cylinder).

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
