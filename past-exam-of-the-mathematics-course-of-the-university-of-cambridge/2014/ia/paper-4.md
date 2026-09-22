# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2014/PaperIA_4.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2014/PaperIA_4.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3C](#3c)
  - [Solution](#3c/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
- [6E](#6e)
  - [i](#6e/i)
    - [Solution](#6e/i/solution)
  - [ii](#6e/ii)
    - [Solution](#6e/ii/solution)
  - [iii](#6e/iii)
    - [Solution](#6e/iii/solution)
  - [iv](#6e/iv)
    - [Solution](#6e/iv/solution)
- [7E](#7e)
  - [i](#7e/i)
    - [Solution](#7e/i/solution)
  - [ii](#7e/ii)
    - [Solution](#7e/ii/solution)
  - [iii](#7e/iii)
    - [Solution](#7e/iii/solution)
- [8E](#8e)
  - [i](#8e/i)
    - [Solution](#8e/i/solution)
  - [ii](#8e/ii)
    - [Solution](#8e/ii/solution)
- [9C](#9c)
  - [Solution](#9c/solution)
- [10C](#10c)
  - [Solution](#10c/solution)
- [11C](#11c)
  - [Solution](#11c/solution)
- [12C](#12c)
  - [Solution](#12c/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

The [Euclidean algorithm](../../../number-theory.md#euclidean-algorithm) gives

$$
203=147+56,\quad147=2\cdot56+35,\quad56=35+21,\quad35=21+14,\quad21=14+7,\quad14=2\cdot7.
$$

Thus the [greatest common divisor](../../../number-theory.md#greatest-common-divisor) is **$d=7$**. The [extended Euclidean algorithm](../../../number-theory.md#extended-euclidean-algorithm) reverses these divisions:

$$
7=21-14=2\cdot21-35=2\cdot56-3\cdot35=8\cdot56-3\cdot147=8\cdot203-11\cdot147.
$$

This supplies the [Bezout identity](../../../algebra.md#bezout-identity) with $x=8$, $y=-11$.

To obtain [all solutions of a linear Diophantine equation](../../../number-theory.md#all-solutions-of-a-linear-diophantine-equation), subtract this particular solution from any other and divide by $7$. The result is $29(x-8)+21(y+11)=0$. Since $29$ and $21$ are [coprime integers](../../../number-theory.md#coprime-integers), $21$ divides $x-8$, giving

$$
\boxed{x=8+21t,\qquad y=-11-29t,\qquad t\in\mathbb Z.}
$$

Every displayed pair satisfies the original [linear Diophantine equation](../../../number-theory.md#linear-diophantine-equation), so the parametrization is exhaustive.

For the [modular arithmetic](../../../number-theory.md#modular-arithmetic) calculation, $21\cdot18=378\equiv1\pmod{29}$, so $18$ is the [modular inverse](../../../number-theory.md#modular-multiplicative-inverse) of $21$. Multiplication gives $n\equiv25\cdot18\equiv15\pmod{29}$. The admissible [integers](../../../number-theory.md#integer) are $15+29t$ for $0\leq t\leq68$, ending at $1987$; the next is $2016$. **There are $\boxed{69}$ such integers.**

## 2E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

For [integers](../../../number-theory.md#integer) $0\leq k\leq n$, define the [binomial coefficient](../../../combinatorics.md#binomial-coefficient) by

$$
\binom nk=\frac{n!}{k!(n-k)!},\qquad0!=1.
$$

Here the [factorial](../../../combinatorics.md#factorial) $n!$ is the product of the positive [integers](../../../number-theory.md#integer) up to $n$. This also counts the $k$-element [subsets](../../../set.md#subset) of an $n$-element [set](../../../set.md): an ordered choice has $n!/(n-k)!$ possibilities, and each [subset](../../../set.md#subset) is ordered in $k!$ ways.

Directly from the [factorial](../../../combinatorics.md#factorial) definition, when $0\leq k<n$,

$$
\binom nk+\binom n{k+1}
=\frac{n!(k+1)+n!(n-k)}{(k+1)!(n-k)!}
=\frac{(n+1)!}{(k+1)!(n-k)!}
=\boxed{\binom{n+1}{k+1}}.
$$

This is [Pascal's identity](../../../combinatorics.md#pascal-s-rule).

The required [hockey-stick identity](../../../combinatorics.md#hockey-stick-identity) follows by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on $m$, with $n\geq0$ fixed. For $m=0$, both sides are $1$. If it holds at $m$, adding the next [binomial coefficient](../../../combinatorics.md#binomial-coefficient) and using [Pascal's identity](../../../combinatorics.md#pascal-s-rule) gives

$$
\sum_{k=0}^{m+1}\binom{n+k}k
=\binom{n+m+1}m+\binom{n+m+1}{m+1}
=\binom{n+m+2}{m+1}.
$$

Therefore **for every $n,m\geq0$**,

$$
\boxed{\sum_{k=0}^m\binom{n+k}k=\binom{n+m+1}m.}
$$

## 3C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3c/solution">Solution</h3>

↑ **Parent:** [3C](#3c)

In classical [charged particle in a uniform magnetic field](../../../electromagnetism.md#charged-particle-in-a-uniform-magnetic-field) motion, the [Lorentz force](../../../electromagnetism.md#lorentz-force) and [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) give

$$
m\dot{\mathbf v}=q\mathbf v\times\mathbf B.
$$

Assume $\mathbf B\ne0$ and choose an orthonormal coordinate system with $\mathbf B=B\mathbf e_z$, $B=|\mathbf B|$. Write $\Omega=qB/m$, retaining the sign of the [electric charge](../../../electromagnetism.md#electric-charge). The [velocity](../../../classical-mechanics.md#velocity) equations are

$$
\dot v_x=\Omega v_y,\qquad\dot v_y=-\Omega v_x,\qquad\dot v_z=0.
$$

Thus the parallel [velocity](../../../classical-mechanics.md#velocity) is constant, and the perpendicular [velocity](../../../classical-mechanics.md#velocity) rotates at constant [angular frequency](../../../classical-mechanics.md#angular-frequency). Choosing the time origin and perpendicular axes conveniently gives

$$
v_x=v_\perp\cos\Omega t,\qquad v_y=-v_\perp\sin\Omega t,\qquad v_z=v_\parallel.
$$

Integrating the [velocity](../../../classical-mechanics.md#velocity), one obtains

$$
x=x_c+\frac{v_\perp}{\Omega}\sin\Omega t,\qquad y=y_c+\frac{v_\perp}{\Omega}\cos\Omega t,\qquad z=z_0+v_\parallel t.
$$

The first two coordinates describe a [circle](../../../topology.md#circle) of radius $mv_\perp/(|q|B)$, while the third advances uniformly. This is [helical motion in a uniform magnetic field](../../../electromagnetism.md#helical-motion-in-a-uniform-magnetic-field): the [helix](../../../topology.md#helix) has **axis parallel to $\mathbf B$** through the [guiding centre](../../../electromagnetism.md#guiding-center). Its [cyclotron frequency](../../../quantum-theory.md#cyclotron-frequency) is

$$
\boxed{\omega_c=\frac{|q|B}{m}},
$$

and its signed [angular velocity](../../../classical-mechanics.md#angular-velocity) vector about that axis is $-q\mathbf B/m$. The minus sign follows from the ordering $\mathbf v\times\mathbf B$ in the [Lorentz force](../../../electromagnetism.md#lorentz-force). The [helix](../../../topology.md#helix) degenerates to a [circle](../../../topology.md#circle) when $v_\parallel=0$ and to a straight line when $v_\perp=0$. If $q=0$ or $B=0$, there is only straight-line motion. In a relativistic extension with fixed [Lorentz factor](../../../special-relativity.md#lorentz-factor) $\gamma$, the frequency becomes $|q|B/(\gamma m)$; the classical result above uses $m\mathbf v$ as [momentum](../../../classical-mechanics.md#momentum).

## 4C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

A [four-vector](../../../special-relativity.md#four-vector) is a collection of four components $A^\mu=(A^0,\mathbf A)$ that transforms by the same [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) as $(ct,\mathbf x)$. Use the [metric signature](../../../topology.md#metric-signature) $(-,+,+,+)$. The [Lorentzian inner product](../../../general-relativity.md#lorentzian-inner-product) is

$$
A\cdot B=-A^0B^0+A^1B^1+A^2B^2+A^3B^3.
$$

A nonzero [four-vector](../../../special-relativity.md#four-vector) is a [timelike vector](../../../general-relativity.md#timelike-vector), [null vector](../../../special-relativity.md#null-vector) or [spacelike vector](../../../general-relativity.md#spacelike-vector) according as $A\cdot A$ is negative, zero or positive. Reversing the [metric signature](../../../topology.md#metric-signature) reverses the signs used to name these three classes, without changing their geometric meaning.

For a frame moving at [speed](../../../classical-mechanics.md#speed) $v$ along the positive $x$ axis, write $\beta=v/c$ and use the [Lorentz factor](../../../special-relativity.md#lorentz-factor) $\gamma=(1-\beta^2)^{-1/2}$. The component [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) is

$$
\boxed{A'^0=\gamma(A^0-\beta A^1),\quad A'^1=\gamma(A^1-\beta A^0),\quad A'^2=A^2,\quad A'^3=A^3.}
$$

Expanding the first two squares gives

$$
-(A'^0)^2+(A'^1)^2=\gamma^2(1-\beta^2)\bigl(-(A^0)^2+(A^1)^2\bigr)=-(A^0)^2+(A^1)^2.
$$

The other two components are unchanged, so $A'\cdot A'=A\cdot A$. Consequently **a [timelike vector](../../../general-relativity.md#timelike-vector) remains timelike under a [Lorentz transformation](../../../special-relativity.md#lorentz-transformation)**.

For a nonzero [null vector](../../../special-relativity.md#null-vector), $|\mathbf A|=|A^0|$ and $A^0\ne0$. Set $a=A^0$ and $\hat{\mathbf n}=\mathbf A/a$. Then $|\hat{\mathbf n}|=1$ and $A=a(1,\hat{\mathbf n})$. If the zero [four-vector](../../../special-relativity.md#four-vector) is included among [null vectors](../../../special-relativity.md#null-vector), take $a=0$ and any [unit vector](../../../vector-space.md#unit-vector).

For two future-pointing [null vectors](../../../special-relativity.md#null-vector), write $A=a(1,\hat{\mathbf n})$ and $B=b(1,\hat{\mathbf m})$ with $a,b>0$. The [sum of future-pointing null vectors](../../../special-relativity.md#sum-of-future-pointing-null-vectors) satisfies

$$
(A+B)\cdot(A+B)=-2ab\bigl(1-\hat{\mathbf n}\cdot\hat{\mathbf m}\bigr)\leq0,
$$

because the ordinary [inner product](../../../linear-algebra.md#inner-product) of two [unit vectors](../../../vector-space.md#unit-vector) is at most one. **The sum is null if their spatial directions coincide, and timelike otherwise.** Its positive time component makes the sum nonzero and future-pointing.

## 5E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

A real [sequence](../../../real-analysis.md#sequence) $(x_n)$ has [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) $x$ when

$$
\forall\varepsilon>0\ \exists N\in\mathbb N\ \forall n\geq N:\quad |x_n-x|<\varepsilon.
$$

A [series](../../../real-analysis.md#series-mathematics) $\sum_{n\geq1}x_n$ is a [convergent series](../../../real-analysis.md#convergent-series) with sum $s$ when its [partial sums](../../../real-analysis.md#partial-sum) $S_N=\sum_{n=1}^Nx_n$ have [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) $s$.

For the first [comparison test for series](../../../real-analysis.md#comparison-test-for-series), either of the two allowed bounds implies $0<x_n\leq a_n+b_n$. Hence

$$
0<\sum_{n=1}^Nx_n\leq\sum_{n=1}^{\infty}a_n+\sum_{n=1}^{\infty}b_n<\infty.
$$

The [partial sums](../../../real-analysis.md#partial-sum) form a [monotone bounded sequence](../../../real-analysis.md#monotone-bounded-sequence), so they converge. **The [series](../../../real-analysis.md#series-mathematics) $\sum x_n$ is convergent.**

For the exponent $2$, use $1/n^2\leq1/[n(n-1)]=1/(n-1)-1/n$ for $n\geq2$. The resulting [telescoping series](../../../real-analysis.md#telescoping-series) bounds every [partial sum](../../../real-analysis.md#partial-sum) by $2$, proving that the [series](../../../real-analysis.md#series-mathematics) converges by the [monotone bounded sequence](../../../real-analysis.md#monotone-bounded-sequence) property. To prove divergence of the [harmonic series](../../../real-analysis.md#harmonic-series), group the terms with $2^j<n\leq2^{j+1}$: their sum is at least $2^j/2^{j+1}=1/2$. Thus its [partial sums](../../../real-analysis.md#partial-sum) are unbounded. If $\alpha\leq1$, then $n^{-\alpha}\geq n^{-1}$, so the [comparison test for series](../../../real-analysis.md#comparison-test-for-series) proves

$$
\boxed{\sum_{n\geq1}n^{-2}<\infty,\qquad\sum_{n\geq1}n^{-\alpha}=\infty\quad(\alpha\leq1).}
$$

For the weighted square assumption, the finite-dimensional [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives, for every $N$,

$$
\sum_{n=1}^Nx_n=\sum_{n=1}^N(nx_n)\frac1n
\leq\left(\sum_{n=1}^Nn^2x_n^2\right)^{1/2}\left(\sum_{n=1}^N\frac1{n^2}\right)^{1/2}
\leq\left(\sum_{n\geq1}n^2x_n^2\right)^{1/2}\left(\sum_{n\geq1}n^{-2}\right)^{1/2}<\infty.
$$

Again the positive [partial sums](../../../real-analysis.md#partial-sum) form a [monotone bounded sequence](../../../real-analysis.md#monotone-bounded-sequence). This is the [weighted square roots of a summable sequence](../../../real-analysis.md#weighted-square-roots-of-a-summable-sequence) argument, with $a_n=n^2x_n^2$. **The weighted square condition implies $\sum x_n<\infty$.**

**The converse is false.** Take $x_n=n^{-3/2}$. Each block $2^j\leq n<2^{j+1}$ contributes at most $2^j2^{-3j/2}=2^{-j/2}$, and the resulting [geometric series](../../../real-analysis.md#geometric-series) converges. But $n^2x_n^2=1/n$, whose [harmonic series](../../../real-analysis.md#harmonic-series) diverges. This proves the counterexample without assuming the full [P-series](../../../real-analysis.md#p-series) criterion.

## 6E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6e/i">i</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/i/solution">Solution</h4>

↑ **Parent:** [I](#6e/i)

The [Fermat-Euler theorem](../../../number-theory.md#euler-s-theorem) states that, for an [integer](../../../number-theory.md#integer) $N\geq2$ and any [integer](../../../number-theory.md#integer) $a$ [coprime](../../../number-theory.md#coprime-integers) to $N$,

$$
\boxed{a^{\varphi(N)}\equiv1\pmod N,}
$$

where the [Euler totient function](../../../number-theory.md#euler-totient-function) $\varphi(N)$ counts the [residue classes](../../../number-theory.md#residue-class) [coprime](../../../number-theory.md#coprime-integers) to $N$.

Let $r_1,\ldots,r_{\varphi(N)}$ be representatives of these [residue classes](../../../number-theory.md#residue-class). Multiplication by $a$ gives a [permutation](../../../combinatorics.md#permutation) of them: each $ar_i$ remains [coprime](../../../number-theory.md#coprime-integers) to $N$, and $ar_i\equiv ar_j$ implies $r_i\equiv r_j$ by cancellation using the [modular inverse](../../../number-theory.md#modular-multiplicative-inverse) of $a$. Multiplying all the resulting [modular congruences](../../../number-theory.md#modular-congruence) yields

$$
a^{\varphi(N)}r_1\cdots r_{\varphi(N)}\equiv r_1\cdots r_{\varphi(N)}\pmod N.
$$

The product is itself [coprime](../../../number-theory.md#coprime-integers) to $N$, so it has a [modular inverse](../../../number-theory.md#modular-multiplicative-inverse) and can be canceled. This proves the [Fermat-Euler theorem](../../../number-theory.md#euler-s-theorem). For $N=1$, the congruence is trivial; no separate argument is needed.

<h3 id="6e/ii">ii</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6e/ii)

For the [odd prime](../../../number-theory.md#odd-prime) $p$, the [Fermat-Euler theorem](../../../number-theory.md#euler-s-theorem) gives $x^{p-1}\equiv1\pmod p$. Therefore the [residue class](../../../number-theory.md#residue-class) $z=x^{(p-1)/2}$ obeys $(z-1)(z+1)\equiv0\pmod p$. Since a [prime number](../../../number-theory.md#prime-number) dividing a product divides one of its factors,

$$
\boxed{x^{(p-1)/2}\equiv1\text{ or }-1\pmod p.}
$$

If $x$ is a [quadratic residue](../../../number-theory.md#quadratic-residue), choose $y$ with $y^2\equiv x\pmod p$. Then $y$ is nonzero modulo $p$, and [Fermat's little theorem](../../../number-theory.md#fermat-little-theorem) gives

$$
\boxed{x^{(p-1)/2}\equiv y^{p-1}\equiv1\pmod p.}
$$

This proves the [quadratic residue](../../../number-theory.md#quadratic-residue) direction of [Euler's criterion](../../../number-theory.md#euler-s-criterion).

<h3 id="6e/iii">iii</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6e/iii)

Suppose $x$ is a [quadratic nonresidue](../../../number-theory.md#quadratic-nonresidue). On the nonzero [residue classes](../../../number-theory.md#residue-class) modulo $p$, define the [involution](../../../group-theory.md#involution)

$$
T(a)=xa^{-1}.
$$

It is an [involution](../../../group-theory.md#involution) because $T(T(a))=a$. A fixed point would satisfy $a^2=x$, which is excluded by the [quadratic nonresidue](../../../number-theory.md#quadratic-nonresidue) hypothesis. Thus it partitions the $p-1$ classes into $(p-1)/2$ disjoint pairs $\{a,xa^{-1}\}$, each with product $x$. Consequently

$$
\prod_{a=1}^{p-1}a\equiv x^{(p-1)/2}\pmod p.
$$

Now evaluate the same product by pairing every class with its own [modular inverse](../../../number-theory.md#modular-multiplicative-inverse). The only classes equal to their [modular inverses](../../../number-theory.md#modular-multiplicative-inverse) solve $(a-1)(a+1)=0$ and hence are $1$ and $-1$. All other pairs have product one. The complete product is therefore $-1$, so

$$
\boxed{x^{(p-1)/2}\equiv-1\pmod p.}
$$

Together with the preceding part, this is [Euler's criterion](../../../number-theory.md#euler-s-criterion); the pairing argument establishes the converse without assuming it.

<h3 id="6e/iv">iv</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6e/iv)

[Fermat's little theorem](../../../number-theory.md#fermat-little-theorem) reduces the exponent modulo $22$ because $23$ is a [prime number](../../../number-theory.md#prime-number) and $5$ is [coprime](../../../number-theory.md#coprime-integers) to it. Compute $5^2\equiv3\pmod{22}$, then $5^4\equiv9\pmod{22}$ and $5^5\equiv45\equiv1\pmod{22}$. Thus $5^5=22k+1$ for an [integer](../../../number-theory.md#integer) $k$, and

$$
\boxed{5^{5^5}=5^{22k+1}\equiv(5^{22})^k5\equiv5\pmod{23}.}
$$

The exponent is $5^5=3125$, rather than an iterated left-associated power.

## 7E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7e/i">i</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/i/solution">Solution</h4>

↑ **Parent:** [I](#7e/i)

A [set](../../../set.md) is a [countable set](../../../set-theory.md#countable-set) if it admits an [injective function](../../../algebra.md#injective-function) into the [natural numbers](../../../arithmetic.md#natural-number); this includes [finite sets](../../../set.md#finite-set) and [countably infinite sets](../../../set-theory.md#countably-infinite-set). A [countably infinite set](../../../set-theory.md#countably-infinite-set) can be listed by a [bijection](../../../function.md#bijection) from $\mathbb N$.

Let $Z$ be the [set](../../../set.md) of infinite [binary sequences](../../../real-analysis.md#bitstream). Suppose it were countable and list all its members as $s^{(1)},s^{(2)},\ldots$, writing $s^{(j)}_n$ for the $n$th entry of row $j$. A finite listing could be repeated to make such a list as well. Define the [binary sequence](../../../real-analysis.md#bitstream) $y$ by $y_n=1-s^{(n)}_n$. It differs from the $n$th row in coordinate $n$, for every $n$. Thus it belongs to $Z$ but is missing from the list, a contradiction. **The [set](../../../set.md) $Z$ is uncountable**, by [Cantor's diagonal argument](../../../set-theory.md#cantor-s-diagonal-argument).

<h3 id="7e/ii">ii</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7e/ii)

Use $\mathbb N=\{1,2,\ldots\}$. If a [bijection](../../../function.md#bijection) $f:\mathbb N\to\mathbb N$ maps $S$ onto the even [natural numbers](../../../arithmetic.md#natural-number), its restriction is a [bijection](../../../function.md#bijection) from $S$ onto an infinite [set](../../../set.md). Moreover, its restriction to the [complement](../../../set.md#complement-of-a-set) of $S$ maps onto the odd [natural numbers](../../../arithmetic.md#natural-number). Both [sets](../../../set.md) are therefore infinite.

Conversely, suppose that $S$ and its [complement](../../../set.md#complement-of-a-set) are infinite. Applying the [increasing enumeration of an infinite subset of natural numbers](../../../set-theory.md#increasing-enumeration-of-an-infinite-subset-of-natural-numbers) to each gives

$$
S=\{s_1<s_2<\cdots\},\qquad\mathbb N\setminus S=\{t_1<t_2<\cdots\}.
$$

For completeness, successively choose the least unused member. The process never stops because the [set](../../../set.md) is infinite, and it lists every member: an omitted member would have infinitely many selected [natural numbers](../../../arithmetic.md#natural-number) below it, which is impossible. Define

$$
\boxed{f(s_j)=2j,\qquad f(t_j)=2j-1.}
$$

This is [injective](../../../algebra.md#injective-function) on each list, their images are disjoint, and together their images cover $\mathbb N$. Thus it is a [bijection](../../../function.md#bijection) and maps $S$ onto $2\mathbb N$. **Both infinitude conditions are necessary and sufficient.** If a convention includes zero in $\mathbb N$, index each list from zero and use $2j$, $2j+1$ instead.

<h3 id="7e/iii">iii</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#7e/iii)

Use [uncountability by interleaving prescribed binary coordinates](../../../real-analysis.md#uncountability-by-interleaving-prescribed-binary-coordinates). For each arbitrary [binary sequence](../../../real-analysis.md#bitstream) $b=(b_k)_{k\geq1}$, define another [binary sequence](../../../real-analysis.md#bitstream) by

$$
x_{3k-2}=0,\qquad x_{3k-1}=a_{3k-1},\qquad x_{3k}=b_k\quad(k\geq1).
$$

There are infinitely many zero coordinates, namely $3k-2$, so $x\in X$. There are also infinitely many coordinates agreeing with the prescribed [binary expansion](../../../arithmetic.md#binary-expansion), namely $3k-1$, so $x\in Y$. The coordinates $3k$ recover $b$, making this map an [injection](../../../algebra.md#injective-function) of the [uncountable set](../../../set-theory.md#uncountable-set) of all [binary sequences](../../../real-analysis.md#bitstream) into $Y$. If $Y$ were a [countable set](../../../set-theory.md#countable-set), composing with an [injection](../../../algebra.md#injective-function) into $\mathbb N$ would make all [binary sequences](../../../real-analysis.md#bitstream) countable, contrary to part (i). **Therefore $\boxed{Y\text{ is uncountable}.}$** The construction works for every prescribed [binary sequence](../../../real-analysis.md#bitstream) $(a_n)$; no special distribution property of the digits of $\sqrt2$ is needed.

## 8E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8e/i">i</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/i/solution">Solution</h4>

↑ **Parent:** [I](#8e/i)

For [finite sets](../../../set.md#finite-set) $A_1,\ldots,A_r$, the [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) states

$$
\boxed{\left|\bigcup_{i=1}^rA_i\right|=\sum_{\varnothing\ne J\subseteq\{1,\ldots,r\}}(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.}
$$

To prove it, count the contribution of one element. If it belongs to exactly $q\geq1$ of the [sets](../../../set.md), it is counted by $\binom qk$ intersections of size $k$. Its total weight is

$$
\sum_{k=1}^q(-1)^{k+1}\binom qk=1-(1-1)^q=1,
$$

using the [binomial theorem](../../../combinatorics.md#binomial-theorem). An element belonging to none contributes zero. Summing these weights gives the [cardinality](../../../set-theory.md#cardinality) of the union and proves the [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle). Equivalently, within a finite ambient [set](../../../set.md) $U$, the number avoiding every $A_i$ is the sum over all $J$, with sign $(-1)^{|J|}$ and the empty intersection interpreted as $U$.

<h3 id="8e/ii">ii</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8e/ii)

In the ambient [set](../../../set.md) of all $n^n$ [functions](../../../function.md) from $\mathbb Z/n\mathbb Z$ to itself, let $A_j$ be the forbidden event $f(j)-f(j-1)\equiv j\pmod n$. Apply the avoidance form of the [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) from part (i).

For a proper [subset](../../../set.md#subset) $J$ of the $n$ [cyclic difference constraints](../../../combinatorics.md#cyclic-difference-constraints), with $|J|=k<n$, the selected edges form disjoint paths around the cycle, including isolated vertices. There are $n-k$ components. On each component, choosing one value of $f$ arbitrarily determines all the other values by the prescribed differences. No consistency condition occurs because the cycle has been broken. Therefore

$$
\left|\bigcap_{j\in J}A_j\right|=n^{n-k}\qquad(k<n).
$$

This also works for $n=2$, whose two directed constraints use the same pair of vertices: any single constraint leaves one freely chosen value.

If all $n$ constraints hold, summing them around the cycle gives the necessary condition

$$
0\equiv\sum_{j=0}^{n-1}j=\frac{n(n-1)}2\pmod n.
$$

It holds when $n$ is odd and fails when $n$ is even, the latter sum being congruent to $n/2$. When it holds, choose $f(0)$ in $n$ ways and determine every other value; the final constraint is then consistent. Thus the full intersection has size $F=n$ for odd $n$ and $F=0$ for even $n$.

There are $\binom nk$ [subsets](../../../set.md#subset) of size $k$. By the [binomial theorem](../../../combinatorics.md#binomial-theorem),

$$
|X|=\sum_{k=0}^{n-1}(-1)^k\binom nk n^{n-k}+(-1)^nF
=(n-1)^n+(-1)^n(F-1).
$$

Hence **the number of admissible [functions](../../../function.md) is**

$$
\boxed{|X|=\begin{cases}(n-1)^n+1-n,&n\text{ odd},\\(n-1)^n-1,&n\text{ even}.\end{cases}}
$$

## 9C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9c/solution">Solution</h3>

↑ **Parent:** [9C](#9c)

First apply [momentum conservation](../../../classical-mechanics.md#momentum-conservation) to the rocket and the infinitesimal amount of expelled gas. During $dt$, the exhaust [mass](../../../classical-mechanics.md#mass) is $\alpha\,dt$ and its inertial [velocity](../../../classical-mechanics.md#velocity), to first order, is $v-u$. With no dust, the momentum balance is

$$
mv=(m-\alpha\,dt)(v+dv)+\alpha\,dt(v-u)+o(dt).
$$

It gives the [rocket equation](../../../classical-mechanics.md#rocket-equation) **$\boxed{m\dot v=\alpha u}$**, while $\dot m=-\alpha$.

For a [dust-collecting rocket](../../../classical-mechanics.md#dust-collecting-rocket), the incoming dust [mass](../../../classical-mechanics.md#mass) is $\beta v\,dt$ with zero initial [momentum](../../../classical-mechanics.md#momentum). The same balance has rocket [mass](../../../classical-mechanics.md#mass) $m+(\beta v-\alpha)dt$ after the interval, so

$$
mv=\bigl(m+(\beta v-\alpha)dt\bigr)(v+dv)+\alpha\,dt(v-u)+o(dt).
$$

Consequently

$$
\boxed{\dot m=\beta v-\alpha,\qquad m\dot v=\alpha u-\beta v^2.}
$$

The second term in the [acceleration](../../../classical-mechanics.md#acceleration) equation accounts for the [momentum](../../../classical-mechanics.md#momentum) required to bring collected dust up to rocket [speed](../../../classical-mechanics.md#speed).

Set $\lambda=\sqrt{\alpha/(\beta u)}$ and $V=\lambda u$, so $\alpha u=\beta V^2$. As long as the engines operate and $0\leq v<V$, the [velocity](../../../classical-mechanics.md#velocity) increases and time can be eliminated:

$$
\frac{d\log m}{dv}=\frac{v-\lambda^2u}{V^2-v^2}
=-\frac{\lambda-1}{2(V-v)}-\frac{\lambda+1}{2(V+v)}.
$$

Integrating from $v=0$, $m=m_0$, gives

$$
\log\frac m{m_0}=\frac{\lambda-1}{2}\log\frac{V-v}{V}-\frac{\lambda+1}{2}\log\frac{V+v}{V}.
$$

Thus the required [mass](../../../classical-mechanics.md#mass)–[velocity](../../../classical-mechanics.md#velocity) relation is

$$
\boxed{m=\lambda m_0u\sqrt{\frac{(\lambda u-v)^{\lambda-1}}{(\lambda u+v)^{\lambda+1}}}.}
$$

If $\lambda>1$, this formula would give $m\to0$ as $v\to V^-$. In this interval, $\dot m=\beta(v-\lambda^2u)<0$. A real rocket retains positive body [mass](../../../classical-mechanics.md#mass) even after its fuel is gone, and collected dust only increases that residual [mass](../../../classical-mechanics.md#mass). It therefore cannot follow this branch all the way to zero [mass](../../../classical-mechanics.md#mass): **its fuel must run out while $v<\lambda u$**. Indeed the hypothetical time integral $dt/dv=m/[\beta(V^2-v^2)]$ is integrable at $V$ when $\lambda>1$, so even the formal zero-mass endpoint would occur at finite time.

If $0<\lambda<1$, the same relation instead gives $m\to\infty$ as $v\to V^-$. The [mass](../../../classical-mechanics.md#mass) first decreases, reaches its minimum at $v=\lambda^2u$, and then increases because dust arrives faster than fuel is expelled. The time integral now diverges at $V$: under indefinitely maintained thrust, **$v$ approaches $\lambda u$ asymptotically while stored dust grows without bound**. At that limiting [speed](../../../classical-mechanics.md#speed), thrust $\alpha u$ balances the dust-loading term $\beta v^2$, and $\dot m\to\beta u\lambda(1-\lambda)>0$. This is the physical reason the total rocket [mass](../../../classical-mechanics.md#mass) no longer signals fuel exhaustion. A rocket with a finite initial fuel supply still runs out at finite time $t=M_{\rm fuel}/\alpha$ and before reaching $V$; increasing total [mass](../../../classical-mechanics.md#mass) does not create new fuel.

## 10C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10c/solution">Solution</h3>

↑ **Parent:** [10C](#10c)

For any [vector](../../../vector-space.md#vector) $\mathbf a$, differentiating its components and the rotating basis gives the [rotating-frame derivative formula](../../../physics.md#rotating-frame-derivative-formula)

$$
\left(\frac{d\mathbf a}{dt}\right)_S=\left(\frac{d\mathbf a}{dt}\right)_{S'}+\boldsymbol\omega\times\mathbf a.
$$

Apply it twice to the [position](../../../classical-mechanics.md#position) $\mathbf x$, with constant [angular velocity](../../../classical-mechanics.md#angular-velocity) $\boldsymbol\omega$. The inertial [acceleration](../../../classical-mechanics.md#acceleration) is

$$
\mathbf a_S=\ddot{\mathbf x}+2\boldsymbol\omega\times\dot{\mathbf x}+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x),
$$

where dots denote rotating-frame derivatives. [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) therefore becomes

$$
\boxed{m\ddot{\mathbf x}=\mathbf F-2m\boldsymbol\omega\times\dot{\mathbf x}-m\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x).}
$$

The last terms are the [Coriolis force](../../../physics.md#coriolis-force) and the force corresponding to [centrifugal acceleration](../../../physics.md#centrifugal-acceleration).

For the [particle on a uniformly rotating inclined plane](../../../physics.md#particle-on-a-uniformly-rotating-inclined-plane), choose orthonormal vectors $\mathbf e_1$ along the horizontal $\xi$ axis and $\mathbf e_2$ up the slope, and set $\mathbf e_3=\mathbf e_1\times\mathbf e_2$, the upward [normal vector](../../../differential-geometry.md#normal-vector). Then $\mathbf e_z=\sin\theta\,\mathbf e_2+\cos\theta\,\mathbf e_3$ and

$$
\mathbf x=\xi\mathbf e_1+\eta\mathbf e_2,\qquad\boldsymbol\omega=\omega\mathbf e_z,\qquad\mathbf F=-mg\mathbf e_z+N\mathbf e_3.
$$

Here $N$ is the [normal reaction](../../../classical-mechanics.md#normal-force). The marble is modeled as the smooth sliding particle specified by the printed equations, without an additional rolling constraint. The rotating-frame [Coriolis acceleration](../../../physics.md#coriolis-acceleration) and [centrifugal acceleration](../../../physics.md#centrifugal-acceleration) are respectively

$$
-2\boldsymbol\omega\times\dot{\mathbf x}=2\omega\dot\eta\cos\theta\,\mathbf e_1-2\omega\dot\xi\cos\theta\,\mathbf e_2+2\omega\dot\xi\sin\theta\,\mathbf e_3,
$$



$$
-\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x)=\omega^2\xi\mathbf e_1+\omega^2\eta\cos^2\theta\,\mathbf e_2-\omega^2\eta\sin\theta\cos\theta\,\mathbf e_3.
$$

The normal rotating-frame [acceleration](../../../classical-mechanics.md#acceleration) is zero, so the [normal reaction](../../../classical-mechanics.md#normal-force) is not generally $mg\cos\theta$; it satisfies

$$
N=m\bigl(g\cos\theta-2\omega\dot\xi\sin\theta+\omega^2\eta\sin\theta\cos\theta\bigr).
$$

Projecting the same equation onto the two tangential axes gives exactly

$$
\boxed{\ddot\xi=\omega^2\xi+2\omega\dot\eta\cos\theta,\qquad\ddot\eta=\omega^2\eta\cos^2\theta-2\omega\dot\xi\cos\theta-g\sin\theta.}
$$

Multiply the equations by $\dot\xi$ and $\dot\eta$ and add. The [Coriolis force](../../../physics.md#coriolis-force) terms cancel, as expected because this force does no work relative to the rotating frame. The [normal reaction](../../../classical-mechanics.md#normal-force) also does no work along the plane. The conserved quantity is **rotating-frame [kinetic energy](../../../classical-mechanics.md#kinetic-energy) plus gravitational and [centrifugal potential](../../../physics.md#centrifugal-potential) energy**:

$$
\boxed{E'=\frac m2(\dot\xi^2+\dot\eta^2)+mg\eta\sin\theta-\frac{m\omega^2}{2}(\xi^2+\eta^2\cos^2\theta)=\text{constant}.}
$$

This need not be the conserved inertial [energy](../../../classical-mechanics.md#energy), since the externally driven rotating plane can exchange energy with the particle.

## 11C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11c/solution">Solution</h3>

↑ **Parent:** [11C](#11c)

The area element in [plane polar coordinates](../../../classical-mechanics.md#plane-polar-coordinates) is $r\,dr\,d\theta$. Thus the axial [moment of inertia](../../../classical-mechanics.md#moment-of-inertia) is

$$
I_0=\int_0^{2\pi}\int_0^a r^2\rho_0(a-r)r\,dr\,d\theta
=2\pi\rho_0\left[\frac{ar^4}{4}-\frac{r^5}{5}\right]_0^a
=\boxed{\frac{\pi\rho_0a^5}{10}}.
$$

For the removed material, the angular width is $2\pi/13$, and

$$
\int_{a/2}^a r^3(a-r)\,dr=\frac{13a^5}{320}.
$$

Its [moment of inertia](../../../classical-mechanics.md#moment-of-inertia) is therefore $I_{\rm cut}=\pi\rho_0a^5/160$, leaving

$$
I=I_0-I_{\rm cut}=\frac{3\pi\rho_0a^5}{32}.
$$

The [torque](../../../classical-mechanics.md#torque) equation $I\dot\Omega=\tau$ gives constant [angular acceleration](../../../classical-mechanics.md#angular-acceleration), so the time to reach the prescribed [angular speed](../../../classical-mechanics.md#angular-speed) from rest is

$$
\boxed{t=\frac{I\Omega}{\tau}=\frac{3\pi\rho_0a^5\Omega}{32\tau}.}
$$

To find the [centre of mass after removing material](../../../classical-mechanics.md#centre-of-mass-after-removing-material), let $\mathbf e_1$ point along the bisector of the missing sector in the disc. The original disc has zero first [mass](../../../classical-mechanics.md#mass) moment about its centre. The missing sector has zero transverse first moment by reflection symmetry, while its component along $\mathbf e_1$ is

$$
Q_{\rm cut}=\rho_0\int_{a/2}^a r^2(a-r)\,dr\int_{-\pi/13}^{\pi/13}\cos\theta\,d\theta
=\frac{11\rho_0a^4}{96}\sin\frac\pi{13},
$$

because the radial integral is $11a^4/192$. The remaining first moment is $-Q_{\rm cut}\mathbf e_1$. Dividing by the given [mass](../../../classical-mechanics.md#mass) $k\rho_0a^3$ gives the body-fixed [centre of mass](../../../classical-mechanics.md#center-of-mass)

$$
\boxed{\mathbf R=-\frac{11a}{96k}\sin\frac\pi{13}\,\mathbf e_1.}
$$

It lies away from the missing sector. In the inertial frame, let $t_*$ be the moment the applied [torque](../../../classical-mechanics.md#torque) stops and let $\psi=\psi_*+\Omega(t-t_*)$ give the orientation of that sector's bisector. Then, with $d=11a\sin(\pi/13)/(96k)$,

$$
\mathbf R(t)=-d(\cos\psi,\sin\psi,0),\qquad\boxed{\ddot{\mathbf R}=-\Omega^2\mathbf R}.
$$

The [centre of mass](../../../classical-mechanics.md#center-of-mass) has inward [centripetal acceleration](../../../classical-mechanics.md#centripetal-acceleration) of magnitude $\Omega^2d$. **The required real [force](../../../classical-mechanics.md#force) is the constraint reaction exerted by the fixed rod and its support**. Its horizontal resultant is $k\rho_0a^3\ddot{\mathbf R}$; a zero applied axial [torque](../../../classical-mechanics.md#torque) does not imply a zero resultant [force](../../../classical-mechanics.md#force).

## 12C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12c/solution">Solution</h3>

↑ **Parent:** [12C](#12c)

For a massive particle of [rest mass](../../../special-relativity.md#invariant-mass) $m$, its [four-momentum](../../../special-relativity.md#four-momentum) is $P^\mu=mU^\mu=(E/c,\mathbf p)$, where the [four-velocity](../../../special-relativity.md#four-velocity) is $U^\mu=\gamma(c,\mathbf v)$, $E=\gamma mc^2$ and $\mathbf p=\gamma m\mathbf v$. With [metric signature](../../../topology.md#metric-signature) $(-,+,+,+)$, $P\cdot P=-m^2c^2$. A [photon](../../../quantum-mechanics.md#photon) has [four-momentum](../../../special-relativity.md#four-momentum) $(E/c,(E/c)\hat{\mathbf n})$, a future-pointing [null vector](../../../special-relativity.md#null-vector). [Four-momentum conservation](../../../special-relativity.md#four-momentum-conservation) states that the total incoming and outgoing [four-momenta](../../../special-relativity.md#four-momentum) agree for an isolated interaction; this includes both [energy](../../../classical-mechanics.md#energy) and [momentum conservation](../../../classical-mechanics.md#momentum-conservation) in every inertial frame.

Take the incoming [photon](../../../quantum-mechanics.md#photon) direction as $x$. Its [energy](../../../classical-mechanics.md#energy) is $\hbar\omega=\mu mc^2$, so the total initial [four-momentum](../../../special-relativity.md#four-momentum) is

$$
P=mc(1+\mu,\mu,0,0),\qquad -P\cdot P=m^2c^2(1+2\mu).
$$

The [invariant mass](../../../special-relativity.md#invariant-mass) available after [photon absorption](../../../quantum-mechanics.md#photon-absorption) is therefore $M=m\sqrt{1+2\mu}$. In the [centre-of-momentum frame](../../../special-relativity.md#center-of-momentum-frame), the two equal daughters have opposite [momenta](../../../classical-mechanics.md#momentum). Their total [energy](../../../classical-mechanics.md#energy) is at least their combined [rest energy](../../../special-relativity.md#rest-energy) $2\alpha mc^2$, with equality precisely when both daughters have zero [momentum](../../../classical-mechanics.md#momentum) in that frame. Thus the [mass threshold after photon absorption](../../../special-relativity.md#mass-threshold-after-photon-absorption) is

$$
\boxed{\alpha_{\max}=\frac12\sqrt{1+2\mu}.}
$$

The bound is attainable kinematically by taking each daughter [four-momentum](../../../special-relativity.md#four-momentum) equal to $P/2$; each then has the required [rest mass](../../../special-relativity.md#invariant-mass). It immediately gives **$\alpha_{\max}\to1/2$ as $\mu\to0$**.

At this threshold both daughters move with the [centre-of-momentum frame](../../../special-relativity.md#center-of-momentum-frame). The common laboratory [velocity](../../../classical-mechanics.md#velocity) follows from $\mathbf v=c\mathbf P/P^0$:

$$
\boxed{v=\frac{c\mu}{1+\mu}=\frac{c}{1+\mu^{-1}}.}
$$

For $\mu=0$, its continuous limiting value is zero. At smaller allowed daughter [rest masses](../../../special-relativity.md#invariant-mass), some of the [centre-of-momentum energy](../../../special-relativity.md#centre-of-momentum-energy) appears as their relative [kinetic energy](../../../classical-mechanics.md#kinetic-energy), so their [four-momenta](../../../special-relativity.md#four-momentum) need not be $P/2$.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
