# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperia_4_2024.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2024/paperia_4_2024.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
  - [i](#2e/i)
    - [Solution](#2e/i/solution)
  - [ii](#2e/ii)
    - [Solution](#2e/ii/solution)
  - [iii](#2e/iii)
    - [Solution](#2e/iii/solution)
  - [iv](#2e/iv)
    - [Solution](#2e/iv/solution)
- [3C](#3c)
  - [a](#3c/a)
    - [Solution](#3c/a/solution)
  - [b](#3c/b)
    - [Solution](#3c/b/solution)
- [4C](#4c)
  - [a](#4c/a)
    - [i](#4c/a/i)
      - [Solution](#4c/a/i/solution)
    - [ii](#4c/a/ii)
      - [Solution](#4c/a/ii/solution)
    - [iii](#4c/a/iii)
      - [Solution](#4c/a/iii/solution)
    - [iv](#4c/a/iv)
      - [Solution](#4c/a/iv/solution)
  - [b](#4c/b)
    - [Solution](#4c/b/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
  - [i](#5e/i)
    - [Solution](#5e/i/solution)
  - [ii](#5e/ii)
    - [Solution](#5e/ii/solution)
  - [iii](#5e/iii)
    - [Solution](#5e/iii/solution)
  - [iv](#5e/iv)
    - [Solution](#5e/iv/solution)
- [6E](#6e)
  - [i](#6e/i)
    - [Solution](#6e/i/solution)
  - [ii](#6e/ii)
    - [Solution](#6e/ii/solution)
- [7E](#7e)
  - [Solution](#7e/solution)
  - [a](#7e/a)
    - [i](#7e/a/i)
      - [Solution](#7e/a/i/solution)
    - [ii](#7e/a/ii)
      - [Solution](#7e/a/ii/solution)
  - [b](#7e/b)
    - [i](#7e/b/i)
      - [Solution](#7e/b/i/solution)
    - [ii](#7e/b/ii)
      - [Solution](#7e/b/ii/solution)
    - [iii](#7e/b/iii)
      - [Solution](#7e/b/iii/solution)
- [8E](#8e)
  - [a](#8e/a)
    - [Solution](#8e/a/solution)
  - [b](#8e/b)
    - [i](#8e/b/i)
      - [Solution](#8e/b/i/solution)
    - [ii](#8e/b/ii)
      - [Solution](#8e/b/ii/solution)
- [9C](#9c)
  - [a](#9c/a)
    - [Solution](#9c/a/solution)
  - [b](#9c/b)
    - [Solution](#9c/b/solution)
- [10C](#10c)
  - [i](#10c/i)
    - [Solution](#10c/i/solution)
  - [ii](#10c/ii)
    - [Solution](#10c/ii/solution)
  - [iii](#10c/iii)
    - [Solution](#10c/iii/solution)
  - [iv](#10c/iv)
    - [Solution](#10c/iv/solution)
- [11C](#11c)
  - [a](#11c/a)
    - [Solution](#11c/a/solution)
  - [b](#11c/b)
    - [i](#11c/b/i)
      - [Solution](#11c/b/i/solution)
    - [ii](#11c/b/ii)
      - [Solution](#11c/b/ii/solution)
  - [c](#11c/c)
    - [i](#11c/c/i)
      - [Solution](#11c/c/i/solution)
    - [ii](#11c/c/ii)
      - [Solution](#11c/c/ii/solution)
  - [d](#11c/d)
    - [Solution](#11c/d/solution)
- [12C](#12c)
  - [a](#12c/a)
    - [Solution](#12c/a/solution)
  - [b](#12c/b)
    - [Solution](#12c/b/solution)
  - [c](#12c/c)
    - [Solution](#12c/c/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

The [Wilson theorem](../../../number-theory.md#wilson-s-theorem) states that for a prime $p$,

$$
(p-1)!\equiv-1\pmod p.
$$

Indeed, every nonzero residue modulo $p$ has a unique multiplicative inverse. The only residues equal to their own inverses solve $x^2\equiv1\pmod p$, hence are $1$ and $-1$. Pairing every other residue with its distinct inverse leaves

$$
(p-1)!\equiv1\cdot(-1)\equiv-1\pmod p.
$$

The [Fermat little theorem](../../../number-theory.md#fermat-little-theorem) states that for prime $p$,

$$
a^p\equiv a\pmod p;
$$

equivalently, if $p\nmid a$, then $a^{p-1}\equiv1\pmod p$.

Wilson's theorem at $p=31$ gives

$$
30!=30\cdot29\cdot28!\equiv2\cdot28!\equiv-1\pmod{31},
$$

so $28!\equiv15\pmod{31}$. Also $729\equiv16\pmod{31}$, and therefore

$$
\boxed{28!\cdot729\equiv15\cdot16\equiv23\pmod{31}}.
$$

## 2E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

A relation on $S$ is a subset of $S\times S$. An equivalence relation is reflexive, symmetric, and transitive. Its equivalence class at $x$ is $[x]=\{y\in S:x\sim y\}$.

<h3 id="2e/i">i</h3>

↑ **Parent:** [2E](#2e)

<h4 id="2e/i/solution">Solution</h4>

↑ **Parent:** [I](#2e/i)

This is not an equivalence relation because it is not reflexive: $0\not\sim0$, since $0\cdot0\not>0$.

<h3 id="2e/ii">ii</h3>

↑ **Parent:** [2E](#2e)

<h4 id="2e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2e/ii)

The relation is reflexive and symmetric, but not transitive. For example,

$$
1\sim0,qquad0\sim-1,
$$

while $1\not\sim-1$. Hence it is not an equivalence relation.

<h3 id="2e/iii">iii</h3>

↑ **Parent:** [2E](#2e)

<h4 id="2e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2e/iii)

This is an equivalence relation: $x-x=0\in\mathbb Z$; if $x-y\in\mathbb Z$, then $y-x\in\mathbb Z$; and integer differences add. Its classes are

$$
\boxed{[x]=x+\mathbb Z},
$$

the cosets of $\mathbb Z$ in $\mathbb R$.

<h3 id="2e/iv">iv</h3>

↑ **Parent:** [2E](#2e)

<h4 id="2e/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2e/iv)

This relation is reflexive and transitive, but not symmetric: $1\sim0$ whereas $0\not\sim1$. It is therefore not an equivalence relation.

## 3C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3c/a">a</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/a/solution">Solution</h4>

↑ **Parent:** [A](#3c/a)

The [parallel axis theorem](../../../classical-mechanics.md#parallel-axis-theorem) says that for an axis through $x$, parallel to the centre-of-mass axis in direction $\hat d$,

$$
I_T(x)=I_T(x_T)+M_T|(x-x_T)\times\hat d|^2.
$$

Let

$$
\rho_A^2=|(x_A-x_C)\times\hat d|^2,
\qquad
\rho_B^2=|(x_B-x_C)\times\hat d|^2.
$$

Moments about the axis through $x_C$ add, so

$$
I_C(x_C)=I_A(x_A)+M_A\rho_A^2
+I_B(x_B)+M_B\rho_B^2.
$$

Using $M_A=M_C-M_B$ and solving gives

$$
\boxed{
M_B=\frac{I_C(x_C)-I_A(x_A)-I_B(x_B)-M_C\rho_A^2}
{\rho_B^2-\rho_A^2}}
$$

when the denominator is nonzero. In the degenerate equal-distance case, this inertia equation alone does not determine $M_B$; the centre-of-mass equation $M_Cx_C=M_Ax_A+M_Bx_B$ supplies the remaining information.

<h3 id="3c/b">b</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/b/solution">Solution</h4>

↑ **Parent:** [B](#3c/b)

For a lamina in the $xy$-plane,

$$
I_x=\int y^2\,dm,
\qquad I_y=\int x^2\,dm,
\qquad I_z=\int(x^2+y^2)\,dm,
$$

so the [perpendicular axis theorem](../../../classical-mechanics.md#perpendicular-axis-theorem) is immediately

$$
\boxed{I_z=I_x+I_y}.
$$

For the uniform ellipse, put $x=au$, $y=bv$, where $u^2+v^2\leq1$. Symmetry of the unit disk gives

$$
\frac1\pi\int_{u^2+v^2\leq1}u^2\,du\,dv
=\frac14,
$$

and the same for $v^2$. Hence

$$
\boxed{I_x=\frac{Mb^2}{4},\qquad
I_y=\frac{Ma^2}{4},\qquad
I_z=\frac M4(a^2+b^2)}.
$$

## 4C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4c/a">a</h3>

↑ **Parent:** [4C](#4c)

<h4 id="4c/a/i">i</h4>

↑ **Parent:** [A](#4c/a)

<h5 id="4c/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4c/a/i)

Set $c=1$. If $B$ is in the future lightcone of $A$ and $C$ in that of $B$, then

$$
t_B-t_A\geq|x_B-x_A|,
\qquad
t_C-t_B\geq|x_C-x_B|.
$$

Adding and using the triangle inequality gives

$$
t_C-t_A\geq|x_B-x_A|+|x_C-x_B|
\geq|x_C-x_A|.
$$

**Thus the statement is true.**

<h4 id="4c/a/ii">ii</h4>

↑ **Parent:** [A](#4c/a)

<h5 id="4c/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4c/a/ii)

**False.** Take

$$
A=(0,0),\qquad B=(1,1),\qquad C=(-1,1),
$$

with coordinates written as $(x,t)$. Both $B$ and $C$ lie on the future lightcone of $A$, but $B$ and $C$ are simultaneous and spatially separated, so neither is in the future lightcone of the other.

<h4 id="4c/a/iii">iii</h4>

↑ **Parent:** [A](#4c/a)

<h5 id="4c/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4c/a/iii)

**True.** The assumptions give

$$
t_B-t_A\geq|x_B-x_A|,
\qquad t_A-t_C\geq|x_A-x_C|.
$$

Adding and applying the triangle inequality proves

$$
t_B-t_C\geq|x_B-x_A|+|x_A-x_C|
\geq|x_B-x_C|,
$$

so $B$ is in the future lightcone of $C$.

<h4 id="4c/a/iv">iv</h4>

↑ **Parent:** [A](#4c/a)

<h5 id="4c/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4c/a/iv)

**False.** With $(x,t)$ coordinates, take

$$
A=(0,0),\qquad B=(1,1),\qquad C=(-1,1).
$$

Both separations from $A$ are lightlike, but $B-C=(2,0)$ is spacelike.

<h3 id="4c/b">b</h3>

↑ **Parent:** [4C](#4c)

<h4 id="4c/b/solution">Solution</h4>

↑ **Parent:** [B](#4c/b)

Again set $c=1$ and write

$$
X_A=x_C-x_A,\quad T_A=t_C-t_A,\qquad
X_B=x_C-x_B,\quad T_B=t_C-t_B.
$$

A boost of [velocity](../../../classical-mechanics.md#velocity) $v$ gives

$$
X_A'=\gamma(X_A-vT_A),\qquad
X_B'=\gamma(X_B-vT_B).
$$

Define

$$
D(v)=(X_A-vT_A)^2-(X_B-vT_B)^2.
$$

The hypothesis says $D(0)<0$. Put $\xi=x_B-x_A$ and $\tau=t_B-t_A$. Causality gives $\tau\geq|\xi|$, while $T_B\geq|X_B|$, and $T_A=T_B+\tau$, $X_A=X_B+\xi$. Therefore

$$
T_A^2+X_A^2-(T_B^2+X_B^2)
=2T_B\tau+2X_B\xi+\tau^2+\xi^2>0.
$$

But

$$
D(1)+D(-1)
=2\{T_A^2+X_A^2-(T_B^2+X_B^2)\}>0.
$$

Hence at least one of $D(1),D(-1)$ is positive. By continuity, $D(v)>0$ for some physical [velocity](../../../classical-mechanics.md#velocity) $|v|<1$ sufficiently close to that endpoint. In the corresponding inertial frame,

$$
|x_C'-x_A'|>|x_C'-x_B'|,
$$

as required.

## 5E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

The [Euler theorem](../../../number-theory.md#euler-theorem) states that if $\gcd(a,d)=1$, then

$$
a^{\phi(d)}\equiv1\pmod d.
$$

Let $r_1,\ldots,r_{\phi(d)}$ be the reduced residue classes modulo $d$. Multiplication by $a$ permutes them, so

$$
a^{\phi(d)}r_1\cdots r_{\phi(d)}
\equiv r_1\cdots r_{\phi(d)}\pmod d.
$$

Their product is a unit and may be cancelled, proving the theorem.

<h3 id="5e/i">i</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/i/solution">Solution</h4>

↑ **Parent:** [I](#5e/i)

A decimal integer is congruent modulo $3$ to its digit sum. Cyclic permutation does not change that sum. Hence every rotation of a multiple of $3$ is again divisible by $3$.

<h3 id="5e/ii">ii</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5e/ii)

Divisibility by $2$ or $5$ depends only on the final digit. As the digits are cyclically rotated, every digit appears in the final position. Thus every rotation is divisible by $d\in\{2,5\}$ exactly when every digit is divisible by $d$.

<h3 id="5e/iii">iii</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5e/iii)

As printed, the claim is false: $70$ is 7-cyclic-divisible because its rotations are $70$ and $07=7$, but its digits are not all equal to $7$ and its length is not a multiple of $6$.

The standard rotation argument proves the likely intended statement. If an $L$-digit integer and all its rotations are divisible by $7$, then for each leading digit $a$,

$$
10c_j(n)-c_{j+1}(n)=a(10^L-1)
$$

is divisible by $7$. The [multiplicative order](../../../number-theory.md#multiplicative-order) of $10$ modulo $7$ is $6$. If $6\nmid L$, then $7\nmid10^L-1$, forcing every digit $a$ to be divisible by $7$, hence to be either $0$ or $7$. Thus the valid conclusion is:

$$
\boxed{\text{either every digit is }0\text{ or }7,
\quad\text{or }6\mid L.}
$$

The counterexample shows why “all its digits are equal to 7” cannot replace the first alternative.

<h3 id="5e/iv">iv</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5e/iv)

Let

$$
l=\operatorname{ord}_p(10).
$$

By Fermat's little theorem, $l\mid p-1$. If the digit count $L$ is a multiple of $l$, then $10^L\equiv1\pmod p$. The [cyclic decimal divisibility](../../../number-theory.md#cyclic-decimal-divisibility) relation gives

$$
c_j(n)\equiv10^jn\pmod{10^L-1},
$$

and hence also modulo $p$. Since $p>7$ is coprime to $10$, every $10^j$ is a unit modulo $p$. Therefore

$$
p\mid c_j(n)\quad\Longleftrightarrow\quad p\mid n
$$

for every $j$. Since $c_0(n)=n$, this proves the required equivalence.

## 6E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6e/i">i</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/i/solution">Solution</h4>

↑ **Parent:** [I](#6e/i)

For $n=1$,

$$
F_2F_0-F_1^2=-1=(-1)^1.
$$

If $C_n=F_{n+1}F_{n-1}-F_n^2$, then the recurrence gives

$$
\begin{aligned}
C_{n+1}
&=F_{n+2}F_n-F_{n+1}^2\\
&=(F_{n+1}+F_n)F_n-F_{n+1}^2\\
&=F_n^2-F_{n+1}F_{n-1}=-C_n.
\end{aligned}
$$

Induction yields the [Fibonacci determinant identity](../../../real-analysis.md#fibonacci-determinant-identity) known as Cassini's identity:

$$
\boxed{F_{n+1}F_{n-1}-F_n^2=(-1)^n}.
$$

<h3 id="6e/ii">ii</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6e/ii)

For fixed $m,l$, set

$$
D_n=F_{n+l}F_{n+m}-F_nF_{n+m+l}.
$$

At $n=0$, $D_0=F_lF_m$. Applying the Fibonacci recurrence to every term and cancelling gives $D_{n+1}=-D_n$. Induction therefore proves

$$
\boxed{F_{n+l}F_{n+m}-F_nF_{n+m+l}
=(-1)^nF_mF_l}.
$$

Applying this identity to the relevant pairs of indices and using $F_{r+1}=F_r+F_{r-1}$ gives

$$
F_{j+k}^2-F_{j-k}^2=F_{2k}F_{2j}
$$

and

$$
F_{j+k+1}^2+F_{j-k}^2=F_{2k+1}F_{2j+1}.
$$

Thus, for $j\geq k\geq0$,

$$
\boxed{(F_{j+k}-F_{j-k})(F_{j+k}+F_{j-k})=F_{2k}F_{2j}}
$$

and

$$
\boxed{F_{j+k+1}^2+F_{j-k}^2=F_{2k+1}F_{2j+1}}.
$$

## 7E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7e/solution">Solution</h3>

↑ **Parent:** [7E](#7e)

For a nonempty set $S\subset\mathbb R$ bounded above, $\sup S$ is its least upper bound: every $s\in S$ satisfies $s\leq\sup S$, and every $u<\sup S$ fails to be an upper bound.

A [sequence](../../../real-analysis.md#sequence) $x_n$ converges to $x$ if for every $\varepsilon>0$ there is $N$ such that $n\geq N$ implies $|x_n-x|<\varepsilon$.

<h3 id="7e/a">a</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/a/i">i</h4>

↑ **Parent:** [A](#7e/a)

<h5 id="7e/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7e/a/i)

Every convergent [sequence](../../../real-analysis.md#sequence) is bounded. Conversely, let $(x_n)$ be increasing and bounded above, and set $L=\sup\{x_n:n\geq1\}$. For any $\varepsilon>0$, $L-\varepsilon$ is not an upper bound, so some $x_N>L-\varepsilon$. Monotonicity then gives

$$
L-\varepsilon<x_N\leq x_n\leq L
$$

for all $n\geq N$. Hence $|x_n-L|<\varepsilon$, proving the [monotone bounded sequence](../../../real-analysis.md#monotone-bounded-sequence) criterion.

<h4 id="7e/a/ii">ii</h4>

↑ **Parent:** [A](#7e/a)

<h5 id="7e/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7e/a/ii)

Let

$$
x_n=12-\frac{1000n^2+4}{1.1^n}.
$$

For $n\geq3$, the binomial theorem gives

$$
1.1^n=(1+0.1)^n
\geq\binom n3(0.1)^3
=\frac{n(n-1)(n-2)}{6000}.
$$

Consequently $(1000n^2+4)/1.1^n\to0$: given $\varepsilon>0$, the displayed rational upper bound is below $\varepsilon$ for all sufficiently large $n$. Thus, directly from the definition of convergence,

$$
\boxed{x_n\longrightarrow12}.
$$

<h3 id="7e/b">b</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/b/i">i</h4>

↑ **Parent:** [B](#7e/b)

<h5 id="7e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7e/b/i)

**Yes.** Put $\alpha=\sup S$ and $\beta=\sup T$. Every $s+t\leq\alpha+\beta$, so this is an upper bound. Given $\varepsilon>0$, choose $s\in S$ with $s>\alpha-\varepsilon/2$ and $t\in T$ with $t>\beta-\varepsilon/2$. Then $s+t>\alpha+\beta-\varepsilon$. Hence

$$
\boxed{\sup(S+T)=\sup S+\sup T}.
$$

<h4 id="7e/b/ii">ii</h4>

↑ **Parent:** [B](#7e/b)

<h5 id="7e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7e/b/ii)

**No.** Take $S=T=\{-2,-1\}$. Then

$$
\sup S=\sup T=-1,
\qquad(\sup S)(\sup T)=1,
$$

but $ST=\{1,2,4\}$ and therefore $\sup(ST)=4$.

<h4 id="7e/b/iii">iii</h4>

↑ **Parent:** [B](#7e/b)

<h5 id="7e/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7e/b/iii)

**No, even when every element of $S$ is positive.** Take

$$
S=\left\{\frac12\right\},\qquad T=\{1,2\}.
$$

Then $S^T=\{1/2,1/4\}$, so

$$
\sup(S^T)=\frac12,
\qquad
(\sup S)^{\sup T}=\left(\frac12\right)^2=\frac14.
$$

## 8E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8e/a">a</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/a/solution">Solution</h4>

↑ **Parent:** [A](#8e/a)

A set is [countable set](../../../set-theory.md#countable-set) if it is finite or admits an enumeration by natural numbers. If $A_n$ are countable, choose enumerations $a_{n,m}$. Since $\mathbb N^2$ is countable by diagonal enumeration, the array $(n,m)\mapsto a_{n,m}$ enumerates $\bigcup_nA_n$ after repetitions are removed. This proves that a [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets) is countable.

The integers are countable, so $\mathbb Z\times\mathbb N_{>0}$ is countable. Mapping $(p,q)$ to $p/q$ surjects onto $\mathbb Q$, hence $\mathbb Q$ is countable. The same diagonal argument shows that $A\times B$ is countable whenever $A,B$ are.

Finally, if the reals in $(0,1)$ had decimal expansions $x_1,x_2,\ldots$, choose a decimal whose $n$th digit differs from the $n$th digit of $x_n$, avoiding digits $0$ and $9$ to remove expansion ambiguity. This number differs from every listed number. The [Cantor diagonal argument](../../../set-theory.md#cantor-diagonal-argument) proves that $\mathbb R$ is uncountable.

<h3 id="8e/b">b</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/b/i">i</h4>

↑ **Parent:** [B](#8e/b)

<h5 id="8e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8e/b/i)

**No.** For every $m\in\mathbb R$, the line $y=mx$ contains the origin. These lines are distinct, so the uncountable family

$$
\{y=mx:m\in\mathbb R\}
$$

has nonempty common intersection.

<h4 id="8e/b/ii">ii</h4>

↑ **Parent:** [B](#8e/b)

<h5 id="8e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8e/b/ii)

**Yes.** The set $\mathbb Q^2$ is countable, hence the set of unordered pairs of distinct rational points is countable. Two distinct points determine at most one line. Mapping each such pair to its line therefore has countable image, and every line in the stated collection lies in that image. Thus the collection is countable.

## 9C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9c/a">a</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/a/solution">Solution</h4>

↑ **Parent:** [A](#9c/a)

The particle moves on a horizontal circle of radius

$$
r=L+a\sin\phi_1.
$$

If $T$ is the tension in the light rod, vertical and radial balance give

$$
T\cos\phi_1=mg,
\qquad
T\sin\phi_1=m\omega^2(L+a\sin\phi_1).
$$

Dividing eliminates both $T$ and $m$, yielding the [rotating conical pendulum with an offset pivot](../../../physics.md#rotating-conical-pendulum-with-an-offset-pivot) condition

$$
\boxed{
\omega=\sqrt{\frac{g\tan\phi_1}{L+a\sin\phi_1}}}.
$$

The ratio under the square root has units $T^{-2}$. The answer is independent of $m$; increasing $L$ increases the orbit radius and lowers the angular [velocity](../../../classical-mechanics.md#velocity) required at fixed $\phi_1$.

<h3 id="9c/b">b</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/b/solution">Solution</h4>

↑ **Parent:** [B](#9c/b)

The spring length is $a+x$, its tension is $kx$, and the orbit radius is

$$
r=L+(a+x)\sin\phi_2.
$$

Vertical balance first gives

$$
kx\cos\phi_2=mg,
\qquad
\boxed{x=\frac{mg}{k\cos\phi_2}}.
$$

Radial balance is

$$
kx\sin\phi_2=m\omega^2r.
$$

Using the vertical equation,

$$
\boxed{
\omega=\left[
\frac{g\tan\phi_2}
{L+\left(a+\dfrac{mg}{k\cos\phi_2}\right)\sin\phi_2}
\right]^{1/2}}.
$$

Unlike the rigid-rod result, this depends on $m$: a larger mass stretches the spring farther and changes the radius of the orbit.

## 10C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10c/i">i</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/i/solution">Solution</h4>

↑ **Parent:** [I](#10c/i)

A [central force](../../../physics.md#central-force) conserves [angular momentum](../../../classical-mechanics.md#angular-momentum)

$$
\ell=mr^2\dot\theta.
$$

Put $u=1/r$. Since $\dot\theta=\ell u^2/m$,

$$
\dot r=-\frac{\ell}{m}u',
\qquad
\ddot r=-\frac{\ell^2}{m^2}u^2u'',
\qquad
r\dot\theta^2=\frac{\ell^2}{m^2}u^3,
$$

where primes now denote [differentiation](../../../calculus.md#differentiation) with respect to $\theta$. Substitution into the radial equation gives the [Binet equation](../../../classical-mechanics.md#binet-equation)

$$
\boxed{
u''+u
=\frac{m}{\ell^2u^2}
\frac{dV}{dr}\bigg|_{r=1/u}}.
$$

<h3 id="10c/ii">ii</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10c/ii)

For $V=-km/r$, one has $dV/dr=kmu^2$, so

$$
u''+u=K,
\qquad K=\frac{km^2}{\ell^2}.
$$

After choosing the angular origin, the solution is

$$
u=K(1+e\cos\theta),
\qquad
r=\frac{p}{1+e\cos\theta},
\qquad p=\frac1K.
$$

For $0\leq e<1$, using $r=\sqrt{x^2+y^2}$ and $r+ex=p$ gives

$$
(1-e^2)\left(x+\frac{ep}{1-e^2}\right)^2+y^2
=\frac{p^2}{1-e^2}.
$$

This is an ellipse, with the force centre at one focus, as described by a [Kepler orbit](../../../classical-mechanics.md#kepler-orbit).

<h3 id="10c/iii">iii</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10c/iii)

For

$$
V(r)=-\frac{km}{r-r_0},
$$

Binet's equation becomes

$$
\boxed{
u''+u=\frac{K}{(1-r_0u)^2}},
\qquad K=\frac{km^2}{\ell^2},\qquad 0<u<\frac1{r_0}.
$$

A circular orbit has constant $u=u_c$ and therefore satisfies

$$
K=u_c(1-r_0u_c)^2.
$$

The right side has maximum $4/(27r_0)$ at $u_c=1/(3r_0)$. Thus there are two circular orbits when $0<K<4/(27r_0)$, one marginal orbit at equality, and none above it.

Writing $u=u_c+\eta$ and linearizing gives

$$
\eta''+\frac{1-3r_0u_c}{1-r_0u_c}\eta=0.
$$

**Hence the outer orbit $u_c<1/(3r_0)$, equivalently $r_c>3r_0$, is stable; the inner orbit is unstable. These are the circular-orbit branches of the [shifted inverse-radius potential](../../../classical-mechanics.md#shifted-inverse-radius-potential).**

<h3 id="10c/iv">iv</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#10c/iv)

To first order in $r_0$,

$$
\frac{K}{(1-r_0u)^2}=K(1+2r_0u)+O(r_0^2).
$$

The expanded orbit equation is therefore

$$
u''+\omega^2u=K,
\qquad
\omega^2=1-2Kr_0.
$$

Its required family of solutions is

$$
\boxed{
u(\theta)=X[1+A\cos(\omega\theta)]},
\qquad
\boxed{X=\frac{K}{1-2Kr_0},\quad
\omega=\sqrt{1-2Kr_0}},
$$

with any $0<A<1$. Successive periapses occur when $\omega\theta$ changes by $2\pi$, so their angular separation is

$$
\boxed{\Delta\theta=\frac{2\pi}{\sqrt{1-2Kr_0}}
=2\pi(1+Kr_0)+O(r_0^2)}.
$$

The periapsis advance per revolution is consequently $2\pi Kr_0+O(r_0^2)$.

## 11C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11c/a">a</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/a/solution">Solution</h4>

↑ **Parent:** [A](#11c/a)

With total mass $M=\sum_i m_i$, define

$$
R=\frac1M\sum_i m_ix_i,
\qquad
P=\sum_i m_i\dot x_i,
\qquad
L=\sum_i x_i\times m_i\dot x_i.
$$

The [angular momentum](../../../classical-mechanics.md#angular-momentum) about the centre of mass is

$$
L_{\rm CoM}=\sum_i(x_i-R)\times m_i(\dot x_i-\dot R).
$$

Expanding, using $\sum_i m_i(x_i-R)=0$ and $P=M\dot R$, gives

$$
\boxed{L_{\rm CoM}=L-R\times P}.
$$

<h3 id="11c/b">b</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/b/i">i</h4>

↑ **Parent:** [B](#11c/b)

<h5 id="11c/b/i/solution">Solution</h5>

↑ **Parent:** [I](#11c/b/i)

Every particle is initially at distance $R$ from the axis, so

$$
\boxed{I(0)=\sum_i m_iR^2=mR^2}.
$$

<h4 id="11c/b/ii">ii</h4>

↑ **Parent:** [B](#11c/b)

<h5 id="11c/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11c/b/ii)

Each freely moving particle has position, relative to its own initial radial and tangential unit [vectors](../../../vector-space.md#vector),

$$
x_i(t)=R,e_{r,i}+vt,e_{\theta,i}.
$$

Thus all particles lie on a circle of radius

$$
\boxed{R(t)=\sqrt{R^2+v^2t^2}}.
$$

Their [angular momenta](../../../classical-mechanics.md#angular-momentum) are constant and sum to

$$
\boxed{L=mRv,\hat z}.
$$

Since $I(t)=mR(t)^2$, the angular [velocity](../../../classical-mechanics.md#velocity) is

$$
\dot\theta=\frac{L}{I(t)}
=\frac{Rv}{R^2+v^2t^2}.
$$

With $\theta(0)=0$,

$$
\boxed{\theta(t)=\arctan\frac{vt}{R}}.
$$

This is the geometry of a [freely expanding rotating particle ring](../../../classical-mechanics.md#freely-expanding-rotating-particle-ring).

<h3 id="11c/c">c</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/c/i">i</h4>

↑ **Parent:** [C](#11c/c)

<h5 id="11c/c/i/solution">Solution</h5>

↑ **Parent:** [I](#11c/c/i)

For uniform surface density $m_0/(\pi R^2)$,

$$
I=\frac{m_0}{\pi R^2}
\int_0^{2\pi}\int_0^Rr^2(r\,dr\,d\theta)
=\boxed{\frac12m_0R^2}.
$$

<h4 id="11c/c/ii">ii</h4>

↑ **Parent:** [C](#11c/c)

<h5 id="11c/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11c/c/ii)

At time $t$, the remaining water has [angular momentum](../../../classical-mechanics.md#angular-momentum)

$$
L=\frac12mR^2\omega.
$$

During $dt$, the ejected mass is $-dm$, and its signed tangential speed in the inertial frame is $R\omega+u$. Conservation of [angular momentum](../../../classical-mechanics.md#angular-momentum) gives, to first order,

$$
0=d\left(\frac12mR^2\omega\right)
+(-dm)R(R\omega+u).
$$

After simplification, the [angular rocket equation](../../../classical-mechanics.md#angular-rocket-equation) is

$$
\boxed{m\dot\omega
=\dot m\left(\omega+\frac{2u}{R}\right)}.
$$

Here $u$ is signed relative to the direction of rotation; reversing the spray changes its sign.

<h3 id="11c/d">d</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/d/solution">Solution</h4>

↑ **Parent:** [D](#11c/d)

For $u=0$, the equation becomes

$$
\frac{\dot\omega}{\omega}=\frac{\dot m}{m},
$$

so $\omega/m$ is constant. With $m(t)=m_0-\mu t$,

$$
\omega(t)=\omega_0\frac{m_0-\mu t}{m_0}.
$$

It reaches zero when the water is exhausted, at

$$
\boxed{t_{\rm stop}=\frac{m_0}{\mu}}.
$$

## 12C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12c/a">a</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/a/solution">Solution</h4>

↑ **Parent:** [A](#12c/a)

The [four-momentum](../../../special-relativity.md#four-momentum) of a massive particle is

$$
P^\mu=(E/c,\mathbf p)=m\gamma(c,\mathbf v),
\qquad P^2=m^2c^2,
$$

while for a massless particle

$$
P^\mu=(E/c,\mathbf p),\qquad E=c|\mathbf p|,\qquad P^2=0.
$$

For $P_1=P_2+P_3$, invariance gives

$$
(P_1-P_2)^2=P_3^2.
$$

In the rest frame of particle 1, $P_1=(m_1c,0)$, so

$$
\boxed{E_2=\frac{m_1^2+m_2^2-m_3^2}{2m_1}c^2},
\qquad
\boxed{E_3=\frac{m_1^2+m_3^2-m_2^2}{2m_1}c^2},
$$

with $E_1=m_1c^2$. Equal and opposite final [momenta](../../../classical-mechanics.md#momentum) are real exactly when

$$
\boxed{m_1\geq m_2+m_3},
$$

the threshold condition for a [relativistic two-body decay](../../../special-relativity.md#relativistic-two-body-decay).

<h3 id="12c/b">b</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/b/solution">Solution</h4>

↑ **Parent:** [B](#12c/b)

At step $n$, the parent and daughter rest masses are

$$
m(R_n)=nM+m_0,
\qquad
m(Q)+m(R_{n-1})=m+(n-1)M+m_0.
$$

The decay is allowed when $M\geq m$, which holds because $M=\lambda m$ with $\lambda>1$. Hence all $N$ stages occur:

$$
R_N\longrightarrow R_0+NQ.
$$

The initial rest mass is $NM+m_0$ and the final rest mass is $Nm+m_0$. Thus

$$
\boxed{\Delta m=N(M-m)=Nm(\lambda-1)}
$$

of rest mass is converted into [kinetic energy](../../../classical-mechanics.md#kinetic-energy), corresponding to energy $Nm(\lambda-1)c^2$.

<h3 id="12c/c">c</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/c/solution">Solution</h4>

↑ **Parent:** [C](#12c/c)

[Momentum](../../../classical-mechanics.md#momentum) conservation is $P_A+P_B=P_C+P_D$. The diagonal bilinears are $P_a^2=m_a^2c^2$. The six off-diagonal ones are

$$
2P_A\cdot P_B=s-(m_A^2+m_B^2)c^2,
$$



$$
2P_A\cdot P_C=(m_A^2+m_C^2)c^2-t,
\qquad
2P_A\cdot P_D=(m_A^2+m_D^2)c^2-u,
$$



$$
2P_B\cdot P_C=(m_B^2+m_C^2)c^2-u,
\qquad
2P_B\cdot P_D=(m_B^2+m_D^2)c^2-t,
$$

and

$$
2P_C\cdot P_D=s-(m_C^2+m_D^2)c^2.
$$

These express every bilinear invariant through the [Mandelstam variables](../../../special-relativity.md#mandelstam-variables) and masses. Expanding $s+t+u$ and using [momentum](../../../classical-mechanics.md#momentum) conservation cancels all mixed products, leaving

$$
\boxed{s+t+u=(m_A^2+m_B^2+m_C^2+m_D^2)c^2}.
$$

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
