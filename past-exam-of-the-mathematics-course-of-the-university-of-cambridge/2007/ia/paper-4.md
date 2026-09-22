# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2007/PaperIA_4.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2007/PaperIA_4.pdf)

**Table of contents**

- [1E](#1e)
  - [i](#1e/i)
    - [Solution](#1e/i/solution)
  - [ii](#1e/ii)
    - [Solution](#1e/ii/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3C](#3c)
  - [Solution](#3c/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7E](#7e)
  - [Solution](#7e/solution)
- [8E](#8e)
  - [i](#8e/i)
    - [Solution](#8e/i/solution)
  - [ii](#8e/ii)
    - [Solution](#8e/ii/solution)
- [9C](#9c)
  - [i](#9c/i)
    - [Solution](#9c/i/solution)
  - [ii](#9c/ii)
    - [Solution](#9c/ii/solution)
- [10C](#10c)
  - [i](#10c/i)
    - [Solution](#10c/i/solution)
  - [ii](#10c/ii)
    - [Solution](#10c/ii/solution)
  - [iii](#10c/iii)
    - [Solution](#10c/iii/solution)
- [11C](#11c)
  - [Solution](#11c/solution)
- [12C](#12c)
  - [i](#12c/i)
    - [Solution](#12c/i/solution)
  - [ii](#12c/ii)
    - [Solution](#12c/ii/solution)
  - [iii](#12c/iii)
    - [Solution](#12c/iii/solution)
  - [iv](#12c/iv)
    - [Solution](#12c/iv/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/i">i</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/i/solution">Solution</h4>

↑ **Parent:** [I](#1e/i)

The [Euclidean algorithm](../../../number-theory.md#euclidean-algorithm) gives

$$
18=2\cdot7+4,\qquad 7=4+3,\qquad 4=3+1.
$$

Back-substitution supplies the [Bezout identity](../../../algebra.md#bezout-identity)

$$
1=4-3=2\cdot4-7=2(18-2\cdot7)-7=2\cdot18-5\cdot7.
$$

Thus one solution is $(x,y)=(-5,2)$. If $(x,y)$ is any solution, subtraction gives $7(x+5)+18(y-2)=0$. Since $7$ and $18$ are coprime, $18$ divides $x+5$. Write $x+5=18t$; substitution then gives $y-2=-7t$. Conversely these values satisfy the equation for every [integer](../../../number-theory.md#integer) $t$. Hence **all solutions** are

$$
\boxed{x=-5+18t,\qquad y=2-7t,\qquad t\in\mathbb Z.}
$$

<h3 id="1e/ii">ii</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1e/ii)

Factor the expression as $n^3-n=(n-1)n(n+1)$. One of three consecutive [integers](../../../number-theory.md#integer) is divisible by $3$, so $3\mid n^3-n$. If $n$ is odd, its neighbours $n-1$ and $n+1$ are consecutive even [integers](../../../number-theory.md#integer). One is divisible by $4$ and the other by $2$, so their product is divisible by $8$. Since $3$ and $8$ are [coprime integers](../../../number-theory.md#coprime-integers), their product divides the expression:

$$
\boxed{24\mid n^3-n\quad\text{for every odd integer }n.}
$$

The argument also includes negative odd [integers](../../../number-theory.md#integer) and the zero product at $n=\pm1$.

## 2E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

Define the [binomial coefficient](../../../combinatorics.md#binomial-coefficient) $\binom nk$ as the number of $k$-element subsets of an $n$-element set. Equivalently it is $n!/[k!(n-k)!]$: there are $n(n-1)\cdots(n-k+1)$ ordered lists of $k$ distinct elements, and each subset gives $k!$ such lists. The empty subset gives $\binom n0=1$.

Distinguish one element of the set. A $k$-element subset either omits it, giving $\binom{n-1}k$ possibilities, or contains it and chooses its other $k-1$ elements from the remaining set, giving $\binom{n-1}{k-1}$ possibilities. These cases are disjoint and exhaustive, proving [Pascal's identity](../../../combinatorics.md#pascal-s-rule):

$$
\boxed{\binom{n-1}k+\binom{n-1}{k-1}=\binom nk.}
$$

For the requested sum, fix $n\ge0$ and use [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on $k$. At $k=0$, both sides equal one. If the assertion holds at $k$, adding the next summand gives

$$
\sum_{j=0}^{k+1}\binom{n+j}j
=\binom{n+k+1}k+\binom{n+k+1}{k+1}
=\binom{n+k+2}{k+1},
$$

where the last equality is [Pascal's identity](../../../combinatorics.md#pascal-s-rule). Thus the induction proves the [hockey-stick identity](../../../combinatorics.md#hockey-stick-identity) for all nonnegative $n,k$:

$$
\boxed{\sum_{j=0}^k\binom{n+j}j=\binom{n+k+1}k.}
$$

## 3C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3c/solution">Solution</h3>

↑ **Parent:** [3C](#3c)

Take upward [velocity](../../../classical-mechanics.md#velocity) as positive, and consider the closed material system consisting of the rocket and the fuel it ejects during a short interval $dt$. Initially its mass and [momentum](../../../classical-mechanics.md#momentum) are $m$ and $mv$. Let $\delta m>0$ be the ejected mass, so the rocket's mass change is $dm=-\delta m$. At the end its [velocity](../../../classical-mechanics.md#velocity) is $v+dv$, while the ejected gas has inertial [velocity](../../../classical-mechanics.md#velocity) $v-u$ to first order; its downward relative [velocity](../../../classical-mechanics.md#velocity) need not be downward in the inertial frame.

The final total [momentum](../../../classical-mechanics.md#momentum), to first order, is

$$
(m-\delta m)(v+dv)+\delta m(v-u)=mv+m\,dv-u\,\delta m.
$$

Neglect air resistance and take the gravitational [acceleration](../../../classical-mechanics.md#acceleration) $g$ constant. The external gravitational impulse on this material system is $-mg\,dt$ to first order. [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) therefore gives $m\,dv-u\,\delta m=-mg\,dt$, or

$$
\boxed{m\frac{dv}{dt}=-u\frac{dm}{dt}-gm.}
$$

The positive thrust is $-u\dot m$ because fuel loss makes $\dot m<0$. Applying $d(mv)/dt$ to the rocket alone without accounting for the escaping [momentum](../../../classical-mechanics.md#momentum) would give the wrong equation.

For constant $u$ and positive mass, divide by $m$ and integrate from release at $t=0$:

$$
v(t)=-u\ln\frac{m(t)}{m_0}-gt.
$$

Thus the gravity-corrected [rocket equation](../../../classical-mechanics.md#rocket-equation) is equivalent to

$$
\boxed{m(t)=m_0\exp\left[-\frac{gt+v(t)}u\right].}
$$

## 4C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

The potential factors as $V=x^2(3-2x)$, so its zeros are $0$ and $3/2$, with a double zero at the origin. Its [derivatives](../../../calculus.md#derivative) are $V'=6x(1-x)$ and $V''=6-12x$. Thus there is a local minimum $(0,0)$, a local maximum $(1,1)$ and an inflection at $(1/2,1/2)$. The potential tends to $+\infty$ on the far left and $-\infty$ on the far right. These features determine the left-hand sketch.

Put $v=\dot x$. [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) gives the [phase plane](../../../dynamical-systems.md#phase-plane) system $\dot x=v$, $\dot v=-V'=6x(x-1)$. Its conserved [mechanical energy](../../../classical-mechanics.md#mechanical-energy) and trajectories are

$$
\boxed{E=\frac12v^2+3x^2-2x^3,\qquad
v=\pm\sqrt{2[E-V(x)]}.}
$$

The [linearization](../../../algebra.md#linearization) at $(0,0)$ has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\pm i\sqrt6$, and the surrounding energy curves are closed, so it is a [center equilibrium](../../../dynamical-systems.md#center-equilibrium). At $(1,0)$ the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\pm\sqrt6$, giving a [saddle equilibrium](../../../dynamical-systems.md#saddle-equilibrium). The figure shows the [cubic potential barrier phase portrait](../../../dynamical-systems.md#cubic-potential-barrier-phase-portrait); arrows point right when $v>0$ and left when $v<0$.

<a id="4c/image-cubic-potential-trapped-oscillations-escaping-trajectories-and-the-barrier-separatrix"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-4-potential-phase.png)

**[Figure 1](#4c/image-cubic-potential-trapped-oscillations-escaping-trajectories-and-the-barrier-separatrix). Cubic potential, trapped oscillations, escaping trajectories and the barrier separatrix**.

For **$0<E<1$**, there are three turning-point roots of $V(x)=E$. The two leftmost enclose a closed orbit around the origin: the particle oscillates between them. There is also a separate open component to the right of the third root, where an incoming particle turns and escapes to $+\infty$. The closed orbits run clockwise in the $(x,v)$ plane.

For **$E=1$**, the factorization $1-V(x)=(x-1)^2(2x+1)$ gives the [separatrix](../../../dynamical-systems.md#separatrix)

$$
v^2=2(x-1)^2(2x+1).
$$

The branch with $-1/2\le x<1$ is a [homoclinic orbit](../../../dynamical-systems.md#homoclinic-orbit): it leaves the saddle asymptotically, turns at $x=-1/2$ and returns asymptotically. On $x>1$, one branch approaches the saddle and the other departs towards infinity. Approaching the saddle takes infinite time. The saddle itself is also an [equilibrium](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) trajectory.

For **$E>1$**, the particle can cross the barrier. There is one left [turning point](../../../classical-mechanics.md#turning-point) below $-1/2$; an incoming particle passes through the well, turns on the left and escapes to the right. For **$E<0$**, only a right-hand open component exists, with its [turning point](../../../classical-mechanics.md#turning-point) beyond $3/2$. At **$E=0$**, the stationary centre coexists with a right-hand open trajectory turning at $3/2$. Thus negative energy does not imply trapping here: the cubic potential is unbounded below on the right.

## 5E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

For finite sets $A_1,\ldots,A_s$, the [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) states

$$
\left|\bigcup_{i=1}^sA_i\right|
=\sum_{\varnothing\ne J\subseteq\{1,\ldots,s\}}
(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.
$$

To prove it, consider an element belonging to exactly $d$ of the sets. If $d=0$, it contributes zero to both sides. If $d>0$, its contribution on the right is

$$
\sum_{j=1}^d(-1)^{j+1}\binom dj=1-(1-1)^d=1,
$$

which is its contribution to the union. Summing these contributions proves the formula.

For the keypad, a first digit zero cannot be entered. Define four families of valid codes: $A$ consists of all codes with no zero; $B$ consists of codes beginning with $2$; $C$ consists of $110b$ with $b\in\{1,\ldots,9\}$; and $D$ consists of $a110$ with $a\in\{1,\ldots,9\}$. They cover every valid code. Indeed, if the first digit is not $2$, a zero in the second position is impossible; a zero in the third requires the prefix $11$; a zero in the fourth requires the middle pair $11$. In the third-position case the last digit cannot also be zero. Hence the only remaining zero-containing possibilities are exactly $C$ and $D$.

Their cardinalities are

$$
|A|=9^4=6561,\quad |B|=10^3=1000,\quad |C|=9,\quad |D|=9.
$$

The only nonempty pairwise intersections are $A\cap B$, with $9^3=729$ codes, and $B\cap D=\{2110\}$, with one code. All triple and fourfold intersections are empty. Applying [inclusion-exclusion](../../../combinatorics.md#inclusion-exclusion-principle) therefore gives

$$
\boxed{6561+1000+9+9-729-1=6849\text{ enterable codes}.}
$$

The restriction concerns actual preceding keypresses. It cannot license two successive zeros unless the first-key condition is already satisfied.

## 6E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

We use these countability facts: the [integers](../../../number-theory.md#integer) are [countable](../../../set-theory.md#countable-set); a finite [Cartesian product](../../../set-theory.md#cartesian-product) of [countable sets](../../../set-theory.md#countable-set) is [countable](../../../set-theory.md#countable-set); a [countable](../../../set-theory.md#countable-set) union of [countable sets](../../../set-theory.md#countable-set) is [countable](../../../set-theory.md#countable-set); and every subset of a [countable set](../../../set-theory.md#countable-set) is [countable](../../../set-theory.md#countable-set). Finite products can be enumerated by listing index tuples in increasing maximum coordinate, and [countable](../../../set-theory.md#countable-set) unions by diagonal enumeration of pairs of indices.

Fix $d\ge1$. For each degree bound $D$, there are finitely many monomials $X_1^{\alpha_1}\cdots X_d^{\alpha_d}$ with $\alpha_1+\cdots+\alpha_d\le D$. An [integer](../../../number-theory.md#integer) [polynomial](../../../polynomial.md) of total degree at most $D$ is specified by an [integer](../../../number-theory.md#integer) coefficient for each of them, so these [polynomials](../../../polynomial.md) form a finite [Cartesian product](../../../set-theory.md#cartesian-product) of copies of $\mathbb Z$ and are [countable](../../../set-theory.md#countable-set). Every [polynomial](../../../polynomial.md) has some finite degree bound. Taking the union over $D=0,1,2,\ldots$ proves the [countability of integer polynomial rings](../../../set-theory.md#countability-of-integer-polynomial-rings):

$$
\boxed{\mathbb Z[X_1,\ldots,X_d]\text{ is countably infinite}.}
$$

It is infinite because it contains all [integer](../../../number-theory.md#integer) constant [polynomials](../../../polynomial.md).

For $d=1$, each nonzero [polynomial](../../../polynomial.md) has only finitely many real roots: repeated application of the [factor theorem](../../../polynomial.md#factor-theorem) bounds their number by its degree. The real [algebraic numbers](../../../algebra.md#algebraic-number) are the union of these finite root sets over the countably many nonzero [integer](../../../number-theory.md#integer) [polynomials](../../../polynomial.md). Thus they are [countable](../../../set-theory.md#countable-set). If the real [transcendental numbers](../../../algebra.md#transcendental-number) were [countable](../../../set-theory.md#countable-set) too, their union with the [algebraic numbers](../../../algebra.md#algebraic-number) would make $\mathbb R$ [countable](../../../set-theory.md#countable-set), contrary to the allowed uncountability assumption. Hence **there are uncountably many real [transcendental numbers](../../../algebra.md#transcendental-number)**.

To construct an [algebraically independent real sequence](../../../algebra.md#algebraically-independent-real-sequence), choose $x_1$ outside the [algebraic numbers](../../../algebra.md#algebraic-number). Suppose $x_1,\ldots,x_d$ already satisfy the required nonvanishing condition. For each nonzero $P\in\mathbb Z[X_1,\ldots,X_d,T]$, write

$$
P(X_1,\ldots,X_d,T)=\sum_{j=0}^sP_j(X_1,\ldots,X_d)T^j.
$$

At least one coefficient [polynomial](../../../polynomial.md) $P_j$ is nonzero, and the inductive hypothesis makes its value at $(x_1,\ldots,x_d)$ nonzero. Consequently $P(x_1,\ldots,x_d,T)$ is a nonzero one-variable [polynomial](../../../polynomial.md) and has only finitely many real roots. There are countably many choices of $P$, so the union of all these forbidden roots is [countable](../../../set-theory.md#countable-set). Choose $x_{d+1}$ outside it, which is possible because $\mathbb R$ is uncountable. This extends the nonvanishing condition to $d+1$. Recursion therefore gives

$$
\boxed{f(x_1,\ldots,x_d)\ne0\quad\text{for every }d\ge1
\text{ and nonzero }f\in\mathbb Z[X_1,\ldots,X_d].}
$$

In particular the chosen numbers are distinct, since a relation $X_i-X_j$ is forbidden. Clearing rational denominators shows that every finite initial segment consists of [algebraically independent elements](../../../algebra.md#algebraically-independent-elements) over $\mathbb Q$.

## 7E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7e/solution">Solution</h3>

↑ **Parent:** [7E](#7e)

A real [sequence](../../../real-analysis.md#sequence) $x_n$ converges to $l$ if, for every $\varepsilon>0$, there is an [integer](../../../number-theory.md#integer) $N$ such that $|x_n-l|<\varepsilon$ for every $n\ge N$. A [convergent series](../../../real-analysis.md#convergent-series) $\sum_{n=1}^\infty x_n$ is one whose partial sums $s_N=\sum_{n=1}^Nx_n$ converge to a finite real limit.

If $s_N\to s$, then $x_N=s_N-s_{N-1}\to s-s=0$. This necessary condition is the [term test for divergence](../../../real-analysis.md#term-test-for-divergence). Its converse fails: the [harmonic series](../../../real-analysis.md#harmonic-series) has terms $1/n\to0$ but diverges. For a direct proof, each block from $n=2^{j-1}+1$ to $2^j$ contains $2^{j-1}$ terms each at least $2^{-j}$, so contributes at least $1/2$. Infinitely many such blocks make the partial sums unbounded.

For the positive [sequences](../../../real-analysis.md#sequence) in the final request, the inequality makes $y_n$ decreasing and bounded below by zero. The [bounded monotone sequence theorem](../../../real-analysis.md#bounded-monotone-sequence-theorem) gives $y_n\to l\ge0$. Summing the decrements gives

$$
\frac12\sum_{n=1}^N\min(x_n,y_n)\le y_1-y_{N+1}\le y_1.
$$

Suppose $l>0$. Since $y_n\ge l$, this implies

$$
\sum_{n=1}^N\min(x_n,l)\le2y_1\quad\text{for every }N.
$$

But [clipping preserves divergence of a positive series](../../../real-analysis.md#clipping-preserves-divergence-of-a-positive-series): if infinitely many $x_n\ge l$, the clipped series has infinitely many terms equal to $l$; otherwise its tail equals the divergent tail of $\sum x_n$. Either case contradicts the displayed bound. Hence the only possible limit is

$$
\boxed{y_n\longrightarrow0.}
$$

This proves the [minimum-decrement convergence criterion](../../../real-analysis.md#minimum-decrement-convergence-criterion) without assuming that the divergent positive [sequence](../../../real-analysis.md#sequence) $x_n$ itself tends to zero.

## 8E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8e/i">i</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/i/solution">Solution</h4>

↑ **Parent:** [I](#8e/i)

If the [prime](../../../number-theory.md#prime-number) $p$ does not divide $x$, then $\gcd(p,x)=1$. The [Bezout identity](../../../algebra.md#bezout-identity) gives [integers](../../../number-theory.md#integer) $a,b$ with $ap+bx=1$. Multiplying by $y$ gives $apy+bxy=y$. If $p\mid xy$, both terms on the left are divisible by $p$, so $p\mid y$. Thus [Euclid lemma](../../../number-theory.md#euclid-lemma) holds:

$$
\boxed{p\mid xy\implies p\mid x\text{ or }p\mid y.}
$$

For completeness, existence in the [Fundamental theorem of arithmetic](../../../number-theory.md#fundamental-theorem-of-arithmetic) follows by strong induction on a positive [integer](../../../number-theory.md#integer) $n>1$. If $n$ is [prime](../../../number-theory.md#prime-number) there is nothing to prove; otherwise $n=ab$ with $1<a,b<n$, and the inductive [prime](../../../number-theory.md#prime-number) factorizations of $a,b$ give one for $n$. The [integer](../../../number-theory.md#integer) $1$ has the empty factorization.

For uniqueness, suppose $p_1\cdots p_r=q_1\cdots q_s$ are two [prime](../../../number-theory.md#prime-number) factorizations. Repeated application of [Euclid lemma](../../../number-theory.md#euclid-lemma) shows that $p_1$ divides some $q_j$. Both are [primes](../../../number-theory.md#prime-number), so they are equal. Reorder the second list, cancel this equal factor, and repeat. All factors must be matched, including their multiplicities. Thus **[prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) exists and is unique up to the order of its factors**. For nonzero negative [integers](../../../number-theory.md#integer) one also records the sign.

<h3 id="8e/ii">ii</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8e/ii)

The [Fermat-Euler theorem](../../../number-theory.md#euler-s-theorem) states that, for a positive [integer](../../../number-theory.md#integer) $q$ and an [integer](../../../number-theory.md#integer) $a$ coprime to $q$, $a^{\varphi(q)}\equiv1\pmod q$, where the [Euler totient function](../../../number-theory.md#euler-totient-function) $\varphi(q)$ counts residue classes coprime to $q$. The case $q=1$ is trivial. For $q>1$, let $r_1,\ldots,r_{\varphi(q)}$ be a [reduced residue system](../../../number-theory.md#reduced-residue-system). Multiplication by $a$ permutes it: equality of two resulting residues can be cancelled using the modular inverse of $a$, and the products remain coprime to $q$. Multiplying the residues before and after the permutation gives

$$
a^{\varphi(q)}r_1\cdots r_{\varphi(q)}\equiv r_1\cdots r_{\varphi(q)}\pmod q.
$$

Every factor on the right is a unit, so its product can be cancelled. This proves

$$
\boxed{a^{\varphi(q)}\equiv1\pmod q.}
$$

The [integer](../../../number-theory.md#integer) $359$ is [prime](../../../number-theory.md#prime-number): none of the [primes](../../../number-theory.md#prime-number) $2,3,5,7,11,13,17$ up to $\sqrt{359}<19$ divides it. Therefore $\varphi(359)=358$. Apply the theorem to $60$ and use the supplied congruence:

$$
10^{179}\equiv(60^2)^{179}=60^{358}\equiv1\pmod{359}.
$$

To connect this to individual digits rather than merely assert periodicity, use long-division remainders $r_0=1$ and

$$
10r_{n-1}=359a_n+r_n,\qquad0\le r_n<359.
$$

Induction gives $r_n\equiv10^n\pmod{359}$. Since $10$ is coprime to $359$, no remainder is zero. The congruence above therefore implies $r_{n+179}=r_n$ for every $n\ge0$, using the unique representative in $1,\ldots,358$. In particular

$$
a_{n+179}=\left\lfloor\frac{10r_{n+178}}{359}\right\rfloor
=\left\lfloor\frac{10r_{n-1}}{359}\right\rfloor=a_n.
$$

Hence

$$
\boxed{a_{n+179}=a_n\quad(n\ge1).}
$$

This is the mechanism of [decimal period from multiplicative order](../../../number-theory.md#decimal-period-from-multiplicative-order): the period divides $179$.

## 9C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9c/i">i</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/i/solution">Solution</h4>

↑ **Parent:** [I](#9c/i)

The relevant parameters are $a,h,g$ and the ring mass $m$, with dimensions length, length, length/time$^2$ and mass. The wire is fixed and smooth, so there is no additional friction parameter. Because $m$ is the only parameter carrying a mass dimension, it cannot enter a dimensionless group governing the period. Using $a$ and $g$ as the length and time scales, the independent dimensionless variables are $T\sqrt{g/a}$ and $h/a$. [Dimensional analysis](../../../physics.md#dimensional-analysis) therefore gives

$$
\boxed{T=\sqrt{\frac ag}\,G(h/a).}
$$

The physical mass cancellation also follows from the energy equation in part (ii), since kinetic and gravitational [potential energy](../../../classical-mechanics.md#potential-energy) are both proportional to $m$.

<h3 id="9c/ii">ii</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#9c/ii)

Along the [holonomic constraint](../../../classical-mechanics.md#holonomic-constraint) $z=x^2/(4a)$, we have $\dot z=x\dot x/(2a)$ and hence speed squared $(1+x^2/(4a^2))\dot x^2$. The smooth wire's [normal reaction](../../../classical-mechanics.md#normal-force) is perpendicular to the permitted [velocity](../../../classical-mechanics.md#velocity) and does no work. [Conservation of mechanical energy](../../../classical-mechanics.md#conservation-of-mechanical-energy), with release from rest at height $h$, gives

$$
\frac12m\left(1+\frac{x^2}{4a^2}\right)\dot x^2+\frac{mgx^2}{4a}=mgh.
$$

The [turning points](../../../classical-mechanics.md#turning-point) are $x=\pm x_0$ with $x_0=2\sqrt{ah}$. One full oscillation has twice the travel time between them:

$$
T=2\int_{-x_0}^{x_0}
\sqrt{\frac{1+x^2/(4a^2)}{2g[h-x^2/(4a)]}}dx.
$$

Set $x=x_0u$ and $\beta=h/a$. After cancelling the scale factors,

$$
T=2\sqrt{\frac{2a}{g}}\int_{-1}^1
\sqrt{\frac{1+\beta u^2}{1-u^2}}du,
$$

so the [bead on a parabolic wire](../../../classical-mechanics.md#bead-on-a-parabolic-wire) has

$$
\boxed{G(\beta)=2\sqrt2\int_{-1}^1\sqrt{\frac{1+\beta u^2}{1-u^2}}du.}
$$

For $\beta\ll1$, expand the numerator uniformly on $[-1,1]$:

$$
\sqrt{1+\beta u^2}=1+\frac12\beta u^2+O(\beta^2).
$$

The integrable endpoint weight gives $\int_{-1}^1(1-u^2)^{-1/2}du=\pi$ and $\int_{-1}^1u^2(1-u^2)^{-1/2}du=\pi/2$, for example by $u=\sin\theta$. Therefore the requested small-oscillation period is

$$
\boxed{T=2\pi\sqrt{\frac{2a}{g}}
\left[1+\frac{h}{4a}+O\left((h/a)^2\right)\right].}
$$

The leading frequency is $\sqrt{g/(2a)}$, and the first finite-amplitude correction increases the period. At $h=0$ the ring is stationary; the expression is the limiting period of nonzero small oscillations.

## 10C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10c/i">i</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/i/solution">Solution</h4>

↑ **Parent:** [I](#10c/i)

Dot [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) with $\dot{\boldsymbol r}$. The magnetic cross-product term is perpendicular to this [velocity](../../../classical-mechanics.md#velocity), so

$$
m\dot{\boldsymbol r}\cdot\ddot{\boldsymbol r}
=-k\boldsymbol r\cdot\dot{\boldsymbol r}
-e\dot{\boldsymbol r}\cdot(\dot{\boldsymbol r}\times\boldsymbol B)
=-k\boldsymbol r\cdot\dot{\boldsymbol r}.
$$

Thus

$$
\frac d{dt}\left(m|\dot{\boldsymbol r}|^2+k|\boldsymbol r|^2\right)=0,
$$

or

$$
\boxed{\frac12m|\dot{\boldsymbol r}|^2+\frac12k|\boldsymbol r|^2
=\mathrm{constant}.}
$$

The two halves are the [kinetic energy](../../../classical-mechanics.md#kinetic-energy) and the isotropic spring's [potential energy](../../../classical-mechanics.md#potential-energy). The expression in the question is twice their sum. The [Lorentz force](../../../electromagnetism.md#lorentz-force) changes the direction of motion but supplies no power, because it is perpendicular to [velocity](../../../classical-mechanics.md#velocity); this explains why the magnetic field does not appear in the conserved [mechanical energy](../../../classical-mechanics.md#mechanical-energy). The sign corresponds to charge $-e$.

<h3 id="10c/ii">ii</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10c/ii)

Write $\boldsymbol v=\dot{\boldsymbol r}$. The original PDF contains the cross product $\dot{\boldsymbol r}\times\boldsymbol r$; the TeX aid drops its [velocity](../../../classical-mechanics.md#velocity) dot. Since $\boldsymbol v\times\boldsymbol v=0$, differentiation and the equation of motion give

$$
\frac d{dt}\left[m(\boldsymbol v\times\boldsymbol r)\cdot\boldsymbol B\right]
=m(\ddot{\boldsymbol r}\times\boldsymbol r)\cdot\boldsymbol B
=-e[(\boldsymbol v\times\boldsymbol B)\times\boldsymbol r]\cdot\boldsymbol B.
$$

The radial restoring [force](../../../classical-mechanics.md#force) contributes no [torque](../../../classical-mechanics.md#torque). The vector triple-product identity yields

$$
[(\boldsymbol v\times\boldsymbol B)\times\boldsymbol r]\cdot\boldsymbol B
=B^2\boldsymbol v\cdot\boldsymbol r
-(\boldsymbol v\cdot\boldsymbol B)(\boldsymbol r\cdot\boldsymbol B).
$$

Meanwhile

$$
\frac d{dt}\left[\frac e2|\boldsymbol r\times\boldsymbol B|^2\right]
=e(\boldsymbol r\times\boldsymbol B)\cdot(\boldsymbol v\times\boldsymbol B)
=e\left[B^2\boldsymbol r\cdot\boldsymbol v
-(\boldsymbol r\cdot\boldsymbol B)(\boldsymbol v\cdot\boldsymbol B)\right].
$$

The [derivatives](../../../calculus.md#derivative) cancel, proving

$$
\boxed{m(\dot{\boldsymbol r}\times\boldsymbol r)\cdot\boldsymbol B
+\frac e2|\boldsymbol r\times\boldsymbol B|^2=\mathrm{constant}.}
$$

This is the [magnetic axial angular-momentum invariant](../../../classical-mechanics.md#magnetic-axial-angular-momentum-invariant). Its first term is the negative of the ordinary [angular momentum](../../../classical-mechanics.md#angular-momentum) projected on $\boldsymbol B$; retaining that sign is essential.

<h3 id="10c/iii">iii</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10c/iii)

Let $q(t)=\boldsymbol r(t)\cdot\boldsymbol B$. Since the field is constant, dotting the equation of motion with $\boldsymbol B$ eliminates the magnetic term:

$$
m\ddot q=-kq-e(\dot{\boldsymbol r}\times\boldsymbol B)\cdot\boldsymbol B=-kq.
$$

This is a [harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion) with frequency $\omega=\sqrt{k/m}$. Initially $q(0)=\boldsymbol r_0\cdot\boldsymbol B$ and $\dot q(0)=0$, because the particle starts at rest. Therefore

$$
\boxed{\boldsymbol r(t)\cdot\boldsymbol B
=(\boldsymbol r_0\cdot\boldsymbol B)\cos\left(\sqrt{k/m}\,t\right).}
$$

The magnetic [force](../../../classical-mechanics.md#force) modifies the transverse motion but not this projection. The formula also holds trivially when $\boldsymbol B=0$.

## 11C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11c/solution">Solution</h3>

↑ **Parent:** [11C](#11c)

For a fixed central gravitational source, the radial and transverse components of [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) in [polar coordinates](../../../calculus.md#polar-coordinates) are

$$
\ddot r-r\dot\theta^2=-\frac{GM}{r^2},\qquad
r\ddot\theta+2\dot r\dot\theta=0.
$$

The second equation gives $r^2\dot\theta=h$, the constant specific [angular momentum](../../../classical-mechanics.md#angular-momentum). Take $h>0$ by choosing the orientation of $\theta$, and put $u=1/r$. Writing $u'$ and $u''$ for [derivatives](../../../calculus.md#derivative) with respect to $\theta$,

$$
\dot r=-hu',\qquad\ddot r=-h^2u^2u'',\qquad
r\dot\theta^2=h^2u^3.
$$

Substituting into the radial equation and dividing by $-h^2u^2$ proves the [Binet equation](../../../classical-mechanics.md#binet-equation)

$$
\boxed{u''+u=\frac{GM}{h^2}=k.}
$$

At perihelion the [velocity](../../../classical-mechanics.md#velocity) is tangential. The [escape velocity](../../../classical-mechanics.md#escape-velocity) is $v_0=\sqrt{2GM/r_0}$, so $h=r_0v_0$ and $h^2=2GMr_0$. Consequently $k=1/(2r_0)$. The initial conditions are $u(0)=1/r_0$ and $u'(0)=0$. Solving the [linear ordinary differential equation](../../../differential-equation.md#linear-ordinary-differential-equation) gives the [parabolic Kepler orbit](../../../classical-mechanics.md#parabolic-trajectory)

$$
\boxed{u(\theta)=\frac{1+\cos\theta}{2r_0}
=\frac1{r_0}\cos^2(\theta/2),\qquad
r=r_0\sec^2(\theta/2).}
$$

Using [angular momentum](../../../classical-mechanics.md#angular-momentum) conservation again,

$$
\dot\theta=\frac h{r^2}=\frac h{r_0^2}\cos^4(\theta/2),
\qquad\boxed{\sec^4(\theta/2)\dot\theta=\frac h{r_0^2}.}
$$

On the outgoing branch $r=2r_0$ is first reached at $\theta=\pi/2$. Integrate from release at perihelion, using $w=\tan(\theta/2)$:

$$
t=\frac{r_0^2}{h}\int_0^{\pi/2}\sec^4(\theta/2)d\theta
=\frac{2r_0^2}{h}\int_0^1(1+w^2)dw
=\boxed{\frac{8r_0^2}{3h}.}
$$

More generally the same integral gives $t=(2r_0^2/h)(w+w^3/3)$, the [Barker equation](../../../classical-mechanics.md#barker-equation) for this parabolic orbit.

## 12C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12c/i">i</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/i/solution">Solution</h4>

↑ **Parent:** [I](#12c/i)

For constant particle masses define the [centre of mass](../../../classical-mechanics.md#center-of-mass) by $M\boldsymbol X=\sum_i m_i\boldsymbol r_i$, with $M=\sum_i m_i$. Summing [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) over all particles gives

$$
M\ddot{\boldsymbol X}=\sum_i\boldsymbol F_i^e+
\sum_{i<j}(\boldsymbol F_{ij}+\boldsymbol F_{ji}).
$$

Each pair of internal [forces](../../../classical-mechanics.md#force) cancels by [Newton's third law](../../../classical-mechanics.md#newton-s-third-law). Hence

$$
\boxed{M\ddot{\boldsymbol X}=\boldsymbol F^e,\qquad
\boldsymbol F^e=\sum_i\boldsymbol F_i^e.}
$$

Only the action-reaction condition is needed for this translation law; centrality of the internal [forces](../../../classical-mechanics.md#force) is needed for the [angular momentum](../../../classical-mechanics.md#angular-momentum) result in part (ii).

<h3 id="12c/ii">ii</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#12c/ii)

About a fixed inertial origin, the total [angular momentum](../../../classical-mechanics.md#angular-momentum) is $\boldsymbol L=\sum_i m_i\boldsymbol r_i\times\dot{\boldsymbol r}_i$. Differentiation gives

$$
\dot{\boldsymbol L}=\sum_i\boldsymbol r_i\times m_i\ddot{\boldsymbol r}_i,
$$

because $\dot{\boldsymbol r}_i\times\dot{\boldsymbol r}_i=0$. Separate the external and internal contributions. The combined [torque](../../../classical-mechanics.md#torque) of an internal pair is

$$
\boldsymbol r_i\times\boldsymbol F_{ij}
+\boldsymbol r_j\times\boldsymbol F_{ji}
=(\boldsymbol r_i-\boldsymbol r_j)\times\boldsymbol F_{ij}=0.
$$

The first equality uses [Newton's third law](../../../classical-mechanics.md#newton-s-third-law), and the second uses the given central-force condition. All internal torques therefore cancel, leaving

$$
\boxed{\frac{d\boldsymbol L}{dt}=\boldsymbol N,
\qquad\boldsymbol N=\sum_i\boldsymbol r_i\times\boldsymbol F_i^e.}
$$

An equal-and-opposite pair which is not central need not have zero combined [torque](../../../classical-mechanics.md#torque); this explains why both internal-force hypotheses matter.

<h3 id="12c/iii">iii</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#12c/iii)

Write $\boldsymbol r_i=\boldsymbol X+\boldsymbol r_i'$ and $\boldsymbol v_i=\boldsymbol V+\boldsymbol v_i'$, where $\boldsymbol V=\dot{\boldsymbol X}$. The definition of the [centre of mass](../../../classical-mechanics.md#center-of-mass) and its [derivative](../../../calculus.md#derivative) give

$$
\sum_i m_i\boldsymbol r_i'=0,\qquad
\sum_i m_i\boldsymbol v_i'=0.
$$

Expand the total [angular momentum](../../../classical-mechanics.md#angular-momentum):

$$
\begin{aligned}
\boldsymbol L
&=\sum_i m_i(\boldsymbol X+\boldsymbol r_i')\times(\boldsymbol V+\boldsymbol v_i')\\
&=M\boldsymbol X\times\boldsymbol V
+\boldsymbol X\times\sum_i m_i\boldsymbol v_i'
+\left(\sum_i m_i\boldsymbol r_i'\right)\times\boldsymbol V
+\sum_i m_i\boldsymbol r_i'\times\boldsymbol v_i'.
\end{aligned}
$$

The two middle terms vanish. Thus the [angular momentum decomposition about the centre of mass](../../../classical-mechanics.md#angular-momentum-decomposition-about-the-centre-of-mass) is

$$
\boxed{\boldsymbol L=M\boldsymbol X\times\boldsymbol V
+\sum_i m_i\boldsymbol r_i'\times\boldsymbol v_i'.}
$$

The first term is orbital [angular momentum](../../../classical-mechanics.md#angular-momentum) of the centre; the second is [angular momentum about the centre of mass](../../../classical-mechanics.md#angular-momentum-about-the-centre-of-mass).

<h3 id="12c/iv">iv</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#12c/iv)

Let $r=|\boldsymbol r_1-\boldsymbol r_2|$ and $\widehat{\boldsymbol r}=(\boldsymbol r_1-\boldsymbol r_2)/r$. A differentiable central [potential energy](../../../classical-mechanics.md#potential-energy) gives the internal [forces](../../../classical-mechanics.md#force)

$$
\boldsymbol F_{12}=-\nabla_{\boldsymbol r_1}U=-U'(r)\widehat{\boldsymbol r},\qquad
\boldsymbol F_{21}=-\nabla_{\boldsymbol r_2}U=+U'(r)\widehat{\boldsymbol r}.
$$

There are no external [forces](../../../classical-mechanics.md#force). Differentiating the total [kinetic energy](../../../classical-mechanics.md#kinetic-energy) and using [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) therefore gives

$$
\begin{aligned}
\frac{dT}{dt}
&=m_1\boldsymbol v_1\cdot\dot{\boldsymbol v}_1
+m_2\boldsymbol v_2\cdot\dot{\boldsymbol v}_2\\
&=\boldsymbol F_{12}\cdot\boldsymbol v_1+
\boldsymbol F_{21}\cdot\boldsymbol v_2\\
&=-U'(r)\widehat{\boldsymbol r}\cdot(\boldsymbol v_1-\boldsymbol v_2).
\end{aligned}
$$

Since $\dot r=\widehat{\boldsymbol r}\cdot(\boldsymbol v_1-\boldsymbol v_2)$, the last expression is $-U'(r)\dot r=-dU/dt$. Thus

$$
\boxed{\frac{dT}{dt}+\frac{dU}{dt}=0,\qquad T+U=\mathrm{constant}.}
$$

This conserves total [mechanical energy](../../../classical-mechanics.md#mechanical-energy), including the [kinetic energy](../../../classical-mechanics.md#kinetic-energy) of centre-of-mass motion, not merely the relative [kinetic energy](../../../classical-mechanics.md#kinetic-energy).

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
