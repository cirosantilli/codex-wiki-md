# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2021/paperia_4_2021.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2021/paperia_4_2021.pdf)

**Table of contents**

- [1E](#1e)
  - [i](#1e/i)
    - [Solution](#1e/i/solution)
  - [ii](#1e/ii)
    - [Solution](#1e/ii/solution)
  - [iii](#1e/iii)
    - [Solution](#1e/iii/solution)
- [2E](#2e)
  - [i](#2e/i)
    - [Solution](#2e/i/solution)
  - [ii](#2e/ii)
    - [Solution](#2e/ii/solution)
  - [iii](#2e/iii)
    - [Solution](#2e/iii/solution)
- [3C](#3c)
  - [Solution](#3c/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5E](#5e)
  - [a](#5e/a)
    - [i](#5e/a/i)
      - [Solution](#5e/a/i/solution)
    - [ii](#5e/a/ii)
      - [Solution](#5e/a/ii/solution)
  - [b](#5e/b)
    - [Solution](#5e/b/solution)
- [6E](#6e)
  - [a](#6e/a)
    - [i](#6e/a/i)
      - [Solution](#6e/a/i/solution)
    - [ii](#6e/a/ii)
      - [Solution](#6e/a/ii/solution)
  - [b](#6e/b)
    - [Solution](#6e/b/solution)
- [7E](#7e)
  - [a](#7e/a)
    - [Solution](#7e/a/solution)
  - [b](#7e/b)
    - [i](#7e/b/i)
      - [Solution](#7e/b/i/solution)
    - [ii](#7e/b/ii)
      - [Solution](#7e/b/ii/solution)
  - [c](#7e/c)
    - [Solution](#7e/c/solution)
  - [d](#7e/d)
    - [i](#7e/d/i)
      - [Solution](#7e/d/i/solution)
    - [ii](#7e/d/ii)
      - [Solution](#7e/d/ii/solution)
- [8E](#8e)
  - [a](#8e/a)
    - [Solution](#8e/a/solution)
  - [b](#8e/b)
    - [i](#8e/b/i)
      - [Solution](#8e/b/i/solution)
    - [ii](#8e/b/ii)
      - [Solution](#8e/b/ii/solution)
  - [c](#8e/c)
    - [i](#8e/c/i)
      - [Solution](#8e/c/i/solution)
    - [ii](#8e/c/ii)
      - [Solution](#8e/c/ii/solution)
- [9C](#9c)
  - [Solution](#9c/solution)
- [10C](#10c)
  - [a](#10c/a)
    - [Solution](#10c/a/solution)
  - [b](#10c/b)
    - [Solution](#10c/b/solution)
  - [c](#10c/c)
    - [i](#10c/c/i)
      - [Solution](#10c/c/i/solution)
    - [ii](#10c/c/ii)
      - [Solution](#10c/c/ii/solution)
    - [iii](#10c/c/iii)
      - [Solution](#10c/c/iii/solution)
- [11C](#11c)
  - [i](#11c/i)
    - [Solution](#11c/i/solution)
  - [ii](#11c/ii)
    - [Solution](#11c/ii/solution)
  - [iii](#11c/iii)
    - [Solution](#11c/iii/solution)
- [12C](#12c)
  - [Solution](#12c/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/i">i</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/i/solution">Solution</h4>

↑ **Parent:** [I](#1e/i)

This can fail. Let $X=\{1\}$ and $Y=\{a,b\}$, put $f(1)=a$, and let $g(a)=g(b)=1$. Then the [function composition](../../../algebra.md#function-composition) $g\circ f$ is the [identity function](../../../function.md#identity-function) on $X$, hence is a [surjective function](../../../algebra.md#surjective-function), although $f$ is not surjective.

<h3 id="1e/ii">ii</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1e/ii)

This is always true. If $f(x_1)=f(x_2)$, then

$$
(g\circ f)(x_1)=g(f(x_1))=g(f(x_2))=(g\circ f)(x_2).
$$

The assumed [injectivity](../../../algebra.md#injective-function) of $g\circ f$ gives $x_1=x_2$, so $f$ is injective.

<h3 id="1e/iii">iii</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1e/iii)

This can fail in the same example as in part (i): $g\circ f$ is injective on the singleton $X$, but $g(a)=g(b)$.

For the final count, $g\circ f=\operatorname{id}_X$ forces $f$ to be injective. There are

$$
n(n-1)\cdots(n-m+1)=\frac{n!}{(n-m)!}
$$

such [functions](../../../function.md) $f$. Once $f$ is chosen, $g$ is forced on the $m$ elements of $f(X)$ and has $m$ independent choices at each of the other $n-m$ elements of $Y$. Hence the number of pairs is

$$
\boxed{\frac{n!}{(n-m)!}m^{n-m}.}
$$

## 2E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2e/i">i</h3>

↑ **Parent:** [2E](#2e)

<h4 id="2e/i/solution">Solution</h4>

↑ **Parent:** [I](#2e/i)

The [Fibonacci recurrence](../../../real-analysis.md#fibonacci-number) gives

$$
a_{n+1}=\frac{F_{n+2}}{F_{n+1}}
=1+\frac{F_n}{F_{n+1}}=1+\frac1{a_n}.
$$

The map $x\mapsto1+1/x$ is strictly decreasing for $x>0$. Since $a_3=2\geq a_1=1$, applying this decreasing map reverses each inequality and proves by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) that

$$
(-1)^na_{n+2}\leq(-1)^na_n.
$$

Taking even $n$ shows $a_{2n+2}\leq a_{2n}$, so $(a_{2n})$ is a [decreasing sequence](../../../real-analysis.md#monotone-sequence).

<h3 id="2e/ii">ii</h3>

↑ **Parent:** [2E](#2e)

<h4 id="2e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2e/ii)

The stated formula is [Cassini's identity](../../../real-analysis.md#fibonacci-determinant-identity). It holds for $n=1$, and the recurrence gives

$$
F_{n+3}F_{n+1}-F_{n+2}^2
=F_{n+1}^2-F_{n+2}F_n,
$$

which is the negative of the expression at index $n$. This proves the identity by induction.

Consequently

$$
a_{n+1}-a_n
=\frac{F_{n+2}F_n-F_{n+1}^2}{F_{n+1}F_n}
=\frac{(-1)^{n+1}}{F_{n+1}F_n}.
$$

The positive [Fibonacci numbers](../../../real-analysis.md#fibonacci-number) tend to [infinity](../../../mathematics.md#infinity), so this difference tends to zero.

<h3 id="2e/iii">iii</h3>

↑ **Parent:** [2E](#2e)

<h4 id="2e/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2e/iii)

Part (i) also shows that the odd subsequence is increasing and the even subsequence is decreasing. Each odd term is below the adjacent even term, so both are [bounded monotone sequences](../../../real-analysis.md#monotone-bounded-sequence) and therefore have limits. Part (ii) says their difference tends to zero, so those limits coincide. Interlacing the two subsequences proves that $(a_n)$ has that common [limit](../../../real-analysis.md#convergent-sequence).

## 3C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3c/solution">Solution</h3>

↑ **Parent:** [3C](#3c)

Let $M(t)=m_0-\alpha t$ be the trolley's remaining [mass](../../../classical-mechanics.md#mass). During $dt$, the expelled mass $-dM$ has ground-frame [velocity](../../../classical-mechanics.md#velocity) $v+u$. Conservation of [momentum](../../../classical-mechanics.md#momentum) gives, to first order,

$$
Mv=(M+dM)(v+dv)+(-dM)(v+u),
$$

and hence $M\,dv=u\,dM$. Integration yields the [rocket equation](../../../classical-mechanics.md#rocket-equation)

$$
v-v_0=u\log\frac{M}{m_0}.
$$

At the stopping time, $M=m_0e^{-v_0/u}$. Therefore the time spent ejecting gas is

$$
\boxed{\frac{m_0}{\alpha}\left(1-e^{-v_0/u}\right)}.
$$

## 4C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

Writing $x_i=(x_i,y_i,z_i)$, rotation about the $z$-axis gives particle $i$ the [speed](../../../classical-mechanics.md#speed) $\omega\sqrt{x_i^2+y_i^2}$. Its [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is therefore $m_i\omega^2(x_i^2+y_i^2)/2$, so

$$
T=\frac12I\omega^2,
\qquad
I=\sum_{i=1}^Nm_i(x_i^2+y_i^2).
$$

This is the defining mass sum for the [moment of inertia](../../../classical-mechanics.md#moment-of-inertia) about the $z$-axis.

For the uniform cuboid, the [mass density](../../../fluid-mechanics.md#density) is $\rho=M/(8abc)$ and

$$
I=\rho\int_{-a}^a\int_{-b}^b\int_{-c}^c(x^2+y^2)\,dz\,dy\,dx
=\boxed{\frac M3(a^2+b^2)}.
$$

## 5E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5e/a">a</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/a/i">i</h4>

↑ **Parent:** [A](#5e/a)

<h5 id="5e/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5e/a/i)

Define the [binomial coefficient](../../../combinatorics.md#binomial-coefficient) $\binom nr$ as the number of $r$-element [subsets](../../../set.md#subset) of an $n$-element set, equivalently as $n!/[r!(n-r)!]$. Partitioning the $r$-element subsets of $\{1,\ldots,n+1\}$ according to whether they contain $n+1$ proves [Pascal's identity](../../../combinatorics.md#pascal-s-rule)

$$
\binom{n+1}r=\binom nr+\binom n{r-1}.
$$

Thus the [forward difference operator](../../../finite-difference.md#forward-difference-operator) satisfies

$$
\boxed{(\delta f_r)(n)=\binom{n+1}r-\binom nr=\binom n{r-1}=f_{r-1}(n).}
$$

<h4 id="5e/a/ii">ii</h4>

↑ **Parent:** [A](#5e/a)

<h5 id="5e/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5e/a/ii)

We use induction on $k$. If $k=0$, then $\delta f=0$, so the integer-valued function $f$ is constant. For $k>0$, the integer-valued function $\delta f$ satisfies $\delta^k(\delta f)=0$. By induction it is an integer linear combination of

$$
\binom n{k-1},\binom n{k-2},\ldots,\binom n1,1.
$$

Part (i) shows that replacing each $\binom nr$ by $\binom n{r+1}$ gives an integer-valued [discrete antiderivative](../../../finite-difference.md#discrete-antiderivative). Subtracting the resulting integer linear combination from $f$ leaves a function with zero forward difference, hence an integer constant. This gives

$$
f(n)=c_0\binom nk+c_1\binom n{k-1}+\cdots+c_{k-1}\binom n1+c_k
$$

with every $c_j\in\mathbb Z$.

<h3 id="5e/b">b</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/b/solution">Solution</h4>

↑ **Parent:** [B](#5e/b)

The [binomial theorem](../../../combinatorics.md#binomial-theorem) states

$$
(x+y)^n=\sum_{r=0}^n\binom nrx^ry^{n-r}.
$$

The required sum is the coefficient of $x^n$ in

$$
(1-x)^n(1+x)^n=(1-x^2)^n.
$$

There is no $x^n$ term when $n$ is [odd](../../../number-theory.md#odd-number). When $n$ is [even](../../../number-theory.md#even-number), the relevant term has exponent $2(n/2)=n$ and coefficient $(-1)^{n/2}\binom n{n/2}$. Hence

$$
\sum_{r=0}^n(-1)^r\binom nr^2
=\begin{cases}
0,&n\text{ odd},\\
(-1)^{n/2}\binom n{n/2},&n\text{ even}.
\end{cases}
$$

## 6E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6e/a">a</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/a/i">i</h4>

↑ **Parent:** [A](#6e/a)

<h5 id="6e/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6e/a/i)

The [Euclidean algorithm](../../../number-theory.md#euclidean-algorithm) repeatedly replaces a pair $(a,b)$ by $(b,a-qb)$ without changing its [greatest common divisor](../../../number-theory.md#greatest-common-divisor). Reversing the divisions expresses $\gcd(a,b)$ as an integer linear combination $\alpha a+\beta b$, which is [Bézout's identity](../../../algebra.md#bezout-identity).

Here $3=3(15)-2(21)$, and therefore

$$
1=12\cdot3-35=36(15)-24(21)-35.
$$

One solution is $(x,y,z)=(36,-24,-1)$. It is not unique: for every $t\in\mathbb Z$, $(x,y,z)=(36+7t,-24-5t,-1)$ is another solution.

<h4 id="6e/a/ii">ii</h4>

↑ **Parent:** [A](#6e/a)

<h5 id="6e/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6e/a/ii)

Because $\gcd(m,n)=1$, choose $u,v\in\mathbb Z$ with $um+vn=1$ by [Bézout's identity](../../../algebra.md#bezout-identity). Then

$$
c=avn+bum
$$

satisfies $c\equiv a\pmod m$ and $c\equiv b\pmod n$. Any two simultaneous solutions differ by a multiple of both coprime integers and hence by a multiple of $mn$. This proves the two-modulus [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem).

The three congruences reduce to

$$
x\equiv2\pmod5,
\qquad x\equiv3\pmod7,
\qquad x\equiv1\pmod3.
$$

The first two give $x\equiv17\pmod{35}$; imposing the last gives

$$
\boxed{x\equiv52\pmod{105}}.
$$

<h3 id="6e/b">b</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/b/solution">Solution</h4>

↑ **Parent:** [B](#6e/b)

The [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) says that the size of a finite union is the alternating sum of the sizes of all nonempty intersections of its constituent sets.

For each [prime number](../../../number-theory.md#prime-number) $p\mid n$, let $A_p$ consist of the tuples for which $p$ divides every $x_i$. Exactly $(n/p)^r$ tuples lie in $A_p$, and for distinct primes $p_1,\ldots,p_j\mid n$, exactly $(n/(p_1\cdots p_j))^r$ lie in their intersection. A tuple has greatest common divisor greater than one with $n$ exactly when it belongs to some $A_p$. Inclusion-exclusion therefore gives the [Jordan totient function](../../../number-theory.md#jordan-s-totient-function)

$$
\phi_r(n)
=n^r\sum_{S\subseteq\{p:p\mid n\}}(-1)^{|S|}\prod_{p\in S}p^{-r}
=\boxed{n^r\prod_{p\mid n}(1-p^{-r})}.
$$

## 7E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7e/a">a</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/a/solution">Solution</h4>

↑ **Parent:** [A](#7e/a)

This is an infinite [binary expansion](../../../arithmetic.md#binary-expansion) with digits in $\{0,1\}$. If the usual expansion of $\alpha$ has infinitely many $1$ digits, list their positions as $b_1<b_2<\cdots$. If it terminates with a final term $2^{-k}$, replace that term by

$$
2^{-k}=\sum_{j=k+1}^{\infty}2^{-j};
$$

this also covers every [dyadic rational](../../../arithmetic.md#dyadic-rational). For $\alpha=1$, use $b_n=n$. Thus every $\alpha\in(0,1]$ has the required form.

The representation by an infinite strictly increasing sequence is unique. If two sequences first differ at exponent $k$, one sum contains $2^{-k}$ and the other does not. The latter's entire possible tail is at most $\sum_{j>k}2^{-j}=2^{-k}$, while the former has $2^{-k}$ plus its own nonempty tail, so the sums cannot agree.

<h3 id="7e/b">b</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/b/i">i</h4>

↑ **Parent:** [B](#7e/b)

<h5 id="7e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7e/b/i)

For $M=\max\{|s|,|t|,1\}$, factorization of a difference of powers gives

$$
|s^j-t^j|
=|s-t|\left|\sum_{l=0}^{j-1}s^{j-1-l}t^l\right|
\leq jM^{j-1}|s-t|.
$$

Consequently the [polynomial](../../../polynomial.md) $f$ obeys the [Lipschitz bound](../../../real-analysis.md#lipschitz-bound)

$$
\boxed{|f(s)-f(t)|\leq A M^{d-1}|s-t|,
\qquad
A=\sum_{j=1}^dj|\alpha_j|.}
$$

<h4 id="7e/b/ii">ii</h4>

↑ **Parent:** [B](#7e/b)

<h5 id="7e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7e/b/ii)

Since $p/q$ is not a root, $q^df(p/q)$ is a nonzero [integer](../../../number-theory.md#integer), and hence

$$
|f(p/q)|\geq q^{-d}.
$$

Moreover $0<\theta-p/q<1$ implies $|p/q|<|\theta|+1$. Applying part (i) to $s=\theta$, $t=p/q$, and using $f(\theta)=0$ gives

$$
q^{-d}\leq A(|\theta|+1)^{d-1}\left|\theta-\frac pq\right|.
$$

Rearrangement proves

$$
\boxed{\theta-\frac pq\geq
\frac1A\left(\frac1{|\theta|+1}\right)^{d-1}\frac1{q^d}}.
$$

This is the core estimate behind the [Liouville approximation theorem](../../../number-theory.md#liouville-approximation-theorem).

<h3 id="7e/c">c</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/c/solution">Solution</h4>

↑ **Parent:** [C](#7e/c)

Let

$$
\alpha_N=\sum_{n=1}^N2^{-n!}=\frac{p_N}{q_N},
\qquad q_N=2^{N!}.
$$

The tail satisfies

$$
0<\alpha-\alpha_N<2\,2^{-(N+1)!}.
$$

For every fixed positive [integer](../../../number-theory.md#integer) $d$, this is smaller than $q_N^{-d}$ for all sufficiently large $N$.

The binary expansion has $1$ digits at factorial positions and arbitrarily long blocks of zeros, but it is neither eventually zero nor eventually periodic. Since a [rational number](../../../number-theory.md#rational-number) has an [eventually periodic binary expansion](../../../number-theory.md#eventually-periodic-positional-expansion-of-a-rational-number), $\alpha$ is [irrational](../../../algebra.md#irrational-number). If it were an [algebraic number](../../../algebra.md#algebraic-number) of degree $d$, part (b), or equivalently the [Liouville approximation theorem](../../../number-theory.md#liouville-approximation-theorem), would give a fixed positive multiple of $q^{-d}$ as a lower bound for all rational approximations. The fractions $p_N/q_N$ violate that bound. Thus $\alpha$ is a [transcendental number](../../../algebra.md#transcendental-number).

<h3 id="7e/d">d</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/d/i">i</h4>

↑ **Parent:** [D](#7e/d)

<h5 id="7e/d/i/solution">Solution</h5>

↑ **Parent:** [I](#7e/d/i)

This can be false. For any nonzero [transcendental number](../../../algebra.md#transcendental-number) $\beta$, the number $\gamma=1/\beta$ is also transcendental, since otherwise its reciprocal would be [algebraic](../../../algebra.md#algebraic-number). Yet $\beta\gamma=1$ is algebraic.

<h4 id="7e/d/ii">ii</h4>

↑ **Parent:** [D](#7e/d)

<h5 id="7e/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7e/d/ii)

This is always true for every positive integer $n$. If $\beta^n$ were algebraic, then $\beta$ would be a root of the polynomial $X^n-\beta^n$ over the field of [algebraic numbers](../../../algebra.md#algebraic-number). By [transitivity of algebraic extensions](../../../algebra.md#transitivity-of-algebraic-extensions), $\beta$ would then be algebraic over $\mathbb Q$, contradicting its transcendence.

## 8E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8e/a">a</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/a/solution">Solution</h4>

↑ **Parent:** [A](#8e/a)

Write the sets as $A_1,A_2,\ldots$, and list each nonempty countable set as $A_i=\{a_{i1},a_{i2},\ldots\}$. Enumerate the pairs $(i,j)\in\mathbb N^2$ along successive diagonals, as in the [Cantor pairing function](../../../set-theory.md#cantor-pairing-function), and output $a_{ij}$ when it has not appeared before. Every member of $\bigcup_iA_i$ eventually appears, proving that a [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets) is countable.

<h3 id="8e/b">b</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/b/i">i</h4>

↑ **Parent:** [B](#8e/b)

<h5 id="8e/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8e/b/i)

Suppose all functions $\mathbb N\to\mathbb N$ could be listed as $f_1,f_2,\ldots$. Define

$$
g(n)=f_n(n)+1.
$$

Then $g$ differs from $f_n$ at $n$ for every $n$, so it is absent from the list. This [Cantor's diagonal argument](../../../set-theory.md#cantor-s-diagonal-argument) proves that $\mathbb N^{\mathbb N}$ is an [uncountable set](../../../set-theory.md#uncountable-set).

<h4 id="8e/b/ii">ii</h4>

↑ **Parent:** [B](#8e/b)

<h5 id="8e/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8e/b/ii)

$A$ is uncountable. For each [binary sequence](../../../real-analysis.md#bitstream) $(\varepsilon_j)$, define

$$
f(n)=1+\sum_{j=1}^n\varepsilon_j.
$$

This is a nondecreasing function, and different binary sequences give different functions, so the uncountable set of binary sequences injects into $A$.

$B$ is countable. Every nonincreasing sequence of positive integers can decrease only finitely many times and is therefore eventually constant. Such a sequence is specified by a finite sequence of positive integers, and the set of all finite integer sequences is a [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets). Hence $B$ is countable.

<h3 id="8e/c">c</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/c/i">i</h4>

↑ **Parent:** [C](#8e/c)

<h5 id="8e/c/i/solution">Solution</h5>

↑ **Parent:** [I](#8e/c/i)

For each $N$, only finitely many [permutations](../../../combinatorics.md#permutation) fix every $j>N$: they are precisely the permutations of $\{1,\ldots,N\}$. Thus

$$
C=\bigcup_{N\geq1}S_N
$$

is a countable union of finite sets and is countable.

<h4 id="8e/c/ii">ii</h4>

↑ **Parent:** [C](#8e/c)

<h5 id="8e/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8e/c/ii)

For every binary sequence $(\varepsilon_n)$, independently fix the pair $(2n-1,2n)$ when $\varepsilon_n=0$ and swap its two entries when $\varepsilon_n=1$. The resulting map is a [permutation](../../../combinatorics.md#permutation) with $|\sigma(j)-j|\leq1$, and different binary sequences produce different permutations. Therefore $D$ is uncountable.

In fact these are all the possibilities: if $\sigma(j)=j+1$, bijectivity and the displacement bound force $\sigma(j+1)=j$, while a point not in such an adjacent transposition is fixed.

## 9C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9c/solution">Solution</h3>

↑ **Parent:** [9C](#9c)

The [work](../../../classical-mechanics.md#work) done along the trajectory is

$$
W=\int_{t_a}^{t_b}F(x(t),t)\dot x(t)\,dt
=\int_a^bF(x,t(x))\,dx.
$$

By [Newton's second law](../../../classical-mechanics.md#newton-s-second-law), $F=m\ddot x$, so

$$
W=m\int_{t_a}^{t_b}\ddot x\dot x\,dt
=\left[\frac12m\dot x^2\right]_{t_a}^{t_b}.
$$

This is the [work-energy theorem](../../../classical-mechanics.md#work-energy-theorem): the work equals the change in [kinetic energy](../../../classical-mechanics.md#kinetic-energy).

A force is [conservative](../../../classical-mechanics.md#conservative-force) when its work between two points is independent of the path, equivalently when it is the negative gradient of a [potential energy](../../../classical-mechanics.md#potential-energy). Here a potential with $V(0)=0$ is

$$
V(x)=F_0\lambda(1-e^{-|x|/\lambda}).
$$

Conservation of [energy](../../../classical-mechanics.md#energy) for $x>0$ gives

$$
\frac12mv^2+F_0\lambda(1-e^{-x/\lambda})=\frac12mv_0^2.
$$

Thus

$$
v(x)=\sqrt{v_0^2+v_e^2(e^{-|x|/\lambda}-1)},
\qquad
\boxed{v_e=\sqrt{\frac{2F_0\lambda}{m}}}.
$$

If $v_0>v_e$, the particle escapes with asymptotic speed $\sqrt{v_0^2-v_e^2}$; the graph decreases from $v_0$ to this horizontal asymptote. At the [escape velocity](../../../classical-mechanics.md#escape-velocity) $v_0=v_e$, it decreases as $v_e e^{-x/(2\lambda)}$ and approaches zero only at infinity. If $v_0<v_e$, it reaches the [turning point](../../../classical-mechanics.md#turning-point)

$$
x_{\max}=-\lambda\log\left(1-\frac{v_0^2}{v_e^2}\right),
$$

where $v=0$, then returns on the negative branch of the same curve and oscillates symmetrically about the origin.

For oscillation put $w=1-v_0^2/v_e^2$. One quarter of the [period](../../../classical-mechanics.md#period-of-an-oscillation) is

$$
\int_0^{x_{\max}}\frac{dx}{v(x)}
=\frac{\lambda}{v_e}\int_w^1\frac{du}{u\sqrt{u-w}}
=\frac{2\lambda}{v_e\sqrt w}\cos^{-1}\sqrt w,
$$

where $u=e^{-x/\lambda}$. Therefore

$$
\boxed{T=\frac{8\lambda}{v_e\sqrt{1-v_0^2/v_e^2}}
\cos^{-1}\sqrt{1-v_0^2/v_e^2}}.
$$

## 10C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10c/a">a</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/a/solution">Solution</h4>

↑ **Parent:** [A](#10c/a)

The [torque](../../../classical-mechanics.md#torque) about the origin is

$$
\tau=r\times F=-\frac{km}{r^3}r\times r=0.
$$

Since $\dot L=\tau$, the [angular momentum](../../../classical-mechanics.md#angular-momentum) $L=mr\times\dot r$ is conserved. The force is the negative gradient of the [inverse-square potential](../../../classical-mechanics.md#inverse-square-potential)

$$
V(r)=-\frac{km}{r},
$$

so the conserved [energy](../../../classical-mechanics.md#energy) is

$$
E=\frac12m|\dot r|^2-\frac{km}{r}.
$$

Directly, $\dot E=\dot r\mathbin{\cdot}(m\ddot r+km r/r^3)=0$.

<h3 id="10c/b">b</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/b/solution">Solution</h4>

↑ **Parent:** [B](#10c/b)

Motion under a [central force](../../../physics.md#central-force) is planar. In [plane polar coordinates](../../../classical-mechanics.md#plane-polar-coordinates), the radial component of the [acceleration](../../../classical-mechanics.md#acceleration) is $\ddot r-r\dot\theta^2$, so

$$
\ddot r-r\dot\theta^2=-\frac{k}{r^2}.
$$

The conserved specific [angular momentum](../../../classical-mechanics.md#angular-momentum) is $h=r^2\dot\theta$. Substitution of $\dot\theta=h/r^2$ yields

$$
\boxed{\ddot r=-\frac{k}{r^2}+\frac{h^2}{r^3}}.
$$

The last term is the centrifugal part of the radial [effective potential](../../../physics.md#effective-potential).

<h3 id="10c/c">c</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/c/i">i</h4>

↑ **Parent:** [C](#10c/c)

<h5 id="10c/c/i/solution">Solution</h5>

↑ **Parent:** [I](#10c/c/i)

At the [periapsis](../../../classical-mechanics.md#periapsis) $r_1$ and [apoapsis](../../../classical-mechanics.md#apoapsis) $r_2$, the given [Kepler orbit](../../../classical-mechanics.md#kepler-orbit) satisfies

$$
r_1=\frac{h^2}{k(1+e)},
\qquad
r_2=\frac{h^2}{k(1-e)}.
$$

Hence

$$
e=\frac{r_2-r_1}{r_1+r_2},
\qquad
h^2=\frac{2kr_1r_2}{r_1+r_2}.
$$

Therefore

$$
\boxed{h=\sqrt{\frac{2kr_1r_2}{r_1+r_2}}},
\qquad \boxed{C=2}.
$$

<h4 id="10c/c/ii">ii</h4>

↑ **Parent:** [C](#10c/c)

<h5 id="10c/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10c/c/ii)

A circular orbit of radius $r$ has speed $v_c(r)=\sqrt{k/r}$. On the transfer [ellipse](../../../geometry-and-topology.md#ellipse), the velocity is tangential at both apsides and has magnitude $h/r$. The first prograde burst therefore changes the speed by

$$
\boxed{\Delta v_1
=\sqrt{\frac{k}{r_1}}
\left(\sqrt{\frac{2r_2}{r_1+r_2}}-1\right)}.
$$

At $r_2$ the satellite must again accelerate in the direction of motion to circularize, by

$$
\boxed{\Delta v_2
=\sqrt{\frac{k}{r_2}}
\left(1-\sqrt{\frac{2r_1}{r_1+r_2}}\right)}.
$$

These are the two impulses of a [Hohmann transfer](../../../classical-mechanics.md#hohmann-transfer-orbit).

<h4 id="10c/c/iii">iii</h4>

↑ **Parent:** [C](#10c/c)

<h5 id="10c/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#10c/c/iii)

The transfer ellipse has [semi-major axis](../../../classical-mechanics.md#semi-major-axis) and [semi-minor axis](../../../classical-mechanics.md#semi-minor-axis)

$$
a=\frac{r_1+r_2}{2},
\qquad
b=a\sqrt{1-e^2}=\sqrt{r_1r_2}.
$$

Conservation of angular momentum gives constant [areal velocity](../../../classical-mechanics.md#areal-velocity) $h/2$. The satellite sweeps half the ellipse, whose area is $\pi ab/2$, so

$$
t_2-t_1=\frac{\pi ab/2}{h/2}=\frac{\pi ab}{h}.
$$

Using part (i),

$$
\boxed{t_2-t_1
=\frac{\pi(r_1+r_2)^{3/2}}{2\sqrt{2k}}}
=\pi\sqrt{\frac{a^3}{k}}.
$$

This is half the orbital period from [Kepler's third law](../../../physics.md#kepler-s-third-law).

## 11C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11c/i">i</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/i/solution">Solution</h4>

↑ **Parent:** [I](#11c/i)

Let $e_i'(t)$ be a [Cartesian basis](../../../linear-algebra.md#cartesian-basis) fixed in the rotating frame. A vector $A=A_i'e_i'$ then satisfies

$$
\left(\frac{dA}{dt}\right)_S
=\dot A_i'e_i'+A_i'\dot e_i'
=\left(\frac{dA}{dt}\right)_{S'}+\omega\times A,
$$

because a [derivative of a body-fixed basis vector](../../../classical-mechanics.md#derivative-of-a-body-fixed-basis-vector) is $\dot e_i'=\omega\times e_i'$. Applying this transport formula twice to $r$ gives, for constant $\omega$,

$$
a_S=a_{S'}+2\omega\times v_{S'}+\omega\times(\omega\times r).
$$

The second and third terms correspond to [Coriolis acceleration](../../../physics.md#coriolis-acceleration) and [centrifugal acceleration](../../../physics.md#centrifugal-acceleration) in the rotating description.

For the bead, use cylindrical unit vectors $(e_r,e_\phi,e_z)$ with $e_z$ upward and

$$
r=R(\sin\theta\,e_r-\cos\theta\,e_z),
\qquad \dot e_r=\omega e_\phi.
$$

Projection of $m\ddot r=-mg e_z+N$ along the wire tangent $\cos\theta\,e_r+\sin\theta\,e_z$ eliminates the smooth-wire [normal force](../../../classical-mechanics.md#normal-force) $N$ and gives

$$
\boxed{\ddot\theta=(\omega^2\cos\theta-g/R)\sin\theta}.
$$

<h3 id="11c/ii">ii</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11c/ii)

The downward and upward positions $\theta=0,\pi$ are equilibria. Linearization about $\theta=0$ gives

$$
\ddot\eta=(\omega^2-g/R)\eta,
$$

so the downward equilibrium is stable for $\omega^2<g/R$ and unstable for $\omega^2>g/R$; at equality it is marginal at linear order. At $\theta=\pi$, the linear coefficient is $\omega^2+g/R>0$, so the upward equilibrium is unstable.

When $\omega^2\geq g/R$, there are also the two equilibria

$$
\theta=\pm\cos^{-1}\left(\frac{g}{R\omega^2}\right)
\pmod{2\pi}.
$$

At either nonvertical equilibrium, differentiation of the right-hand side gives $-\omega^2\sin^2\theta<0$, so both are stable when distinct. This is a [pitchfork bifurcation of a rotating hoop bead](../../../physics.md#pitchfork-bifurcation-of-a-rotating-hoop-bead) at $\omega^2=g/R$.

<h3 id="11c/iii">iii</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#11c/iii)

The inertial [acceleration](../../../classical-mechanics.md#acceleration) obtained by differentiating the position used in part (i) is

$$
\ddot r
=R(\ddot\theta\cos\theta-\dot\theta^2\sin\theta-\omega^2\sin\theta)e_r
+2R\omega\dot\theta\cos\theta e_\phi
+R(\ddot\theta\sin\theta+\dot\theta^2\cos\theta)e_z.
$$

Since $N=m\ddot r+mg e_z$, substitution of the equation of motion gives the wire's force on the bead as

$$
\boxed{
N=m\bigl(R\dot\theta^2+R\omega^2\sin^2\theta+g\cos\theta\bigr)
(-\sin\theta\,e_r+\cos\theta\,e_z)
+2mR\omega\dot\theta\cos\theta\,e_\phi }.
$$

The first component is normal to the circle within its plane; the second is perpendicular to the rotating plane.

## 12C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12c/solution">Solution</h3>

↑ **Parent:** [12C](#12c)

With [Lorentz factor](../../../special-relativity.md#lorentz-factor) $\gamma=(1-v^2/c^2)^{-1/2}$, the relativistic [momentum](../../../classical-mechanics.md#momentum) and [four-momentum](../../../special-relativity.md#four-momentum) are

$$
p=\gamma mv,
\qquad
P^\mu=(\gamma mc,\gamma mv).
$$

The Newtonian formula $a=F/m$ fails because $p$ is not $mv$: both the magnitude and direction of $v$ affect $dp/dt$. Since

$$
\dot\gamma=\frac{\gamma^3}{c^2}v\mathbin{\cdot}a,
$$

the [relativistic force](../../../special-relativity.md#relativistic-force) is

$$
F=\frac{dp}{dt}
=m\gamma\left(a+\frac{\gamma^2}{c^2}(v\mathbin{\cdot}a)v\right).
$$

Taking the dot product with $v$ gives $F\mathbin{\cdot}v=m\gamma^3v\mathbin{\cdot}a$, and substitution yields the inverse relation

$$
\boxed{a=\frac{F}{m\gamma}-\frac{(F\mathbin{\cdot}v)v}{m\gamma c^2}}.
$$

This is the requested sum of a vector parallel to $F$ and one parallel to $v$.

In the constant [electric field](../../../electromagnetism.md#electric-field), $dp/dt=qE$ and the particle starts with $p(0)=0$, so $p=qEt$. The [relativistic energy-momentum relation](../../../special-relativity.md#energy-momentum-relation) implies

$$
v=\frac{c^2p}{\sqrt{m^2c^4+c^2|p|^2}}
=\boxed{\frac{qEt/m}{\sqrt{1+q^2|E|^2t^2/(m^2c^2)}}}.
$$

**Thus the speed increases monotonically but remains [subluminal](../../../special-relativity.md#subluminal-speed), and $v$ tends to $c$ in the direction of $qE$ as $t\to\infty$.**

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
