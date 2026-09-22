# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperia_4_2022.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2022/paperia_4_2022.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
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
  - [b](#4c/b)
    - [Solution](#4c/b/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
- [6D](#6d)
  - [a](#6d/a)
    - [Solution](#6d/a/solution)
  - [b](#6d/b)
    - [Solution](#6d/b/solution)
  - [c](#6d/c)
    - [Solution](#6d/c/solution)
- [7F](#7f)
  - [a](#7f/a)
    - [Solution](#7f/a/solution)
  - [b](#7f/b)
    - [Solution](#7f/b/solution)
  - [c](#7f/c)
    - [Solution](#7f/c/solution)
  - [d](#7f/d)
    - [Solution](#7f/d/solution)
- [8F](#8f)
  - [a](#8f/a)
    - [Solution](#8f/a/solution)
  - [b](#8f/b)
    - [i](#8f/b/i)
      - [Solution](#8f/b/i/solution)
    - [ii](#8f/b/ii)
      - [Solution](#8f/b/ii/solution)
    - [iii](#8f/b/iii)
      - [Solution](#8f/b/iii/solution)
  - [c](#8f/c)
    - [Solution](#8f/c/solution)
- [9C](#9c)
  - [a](#9c/a)
    - [Solution](#9c/a/solution)
  - [b](#9c/b)
    - [Solution](#9c/b/solution)
  - [c](#9c/c)
    - [i](#9c/c/i)
      - [Solution](#9c/c/i/solution)
    - [ii](#9c/c/ii)
      - [Solution](#9c/c/ii/solution)
    - [iii](#9c/c/iii)
      - [Solution](#9c/c/iii/solution)
    - [iv](#9c/c/iv)
      - [Solution](#9c/c/iv/solution)
- [10C](#10c)
  - [a](#10c/a)
    - [Solution](#10c/a/solution)
  - [b](#10c/b)
    - [Solution](#10c/b/solution)
  - [c](#10c/c)
    - [Solution](#10c/c/solution)
- [11C](#11c)
  - [a](#11c/a)
    - [i](#11c/a/i)
      - [Solution](#11c/a/i/solution)
    - [ii](#11c/a/ii)
      - [Solution](#11c/a/ii/solution)
  - [b](#11c/b)
    - [i](#11c/b/i)
      - [Solution](#11c/b/i/solution)
    - [ii](#11c/b/ii)
      - [Solution](#11c/b/ii/solution)
    - [iii](#11c/b/iii)
      - [Solution](#11c/b/iii/solution)
- [12C](#12c)
  - [a](#12c/a)
    - [Solution](#12c/a/solution)
  - [b](#12c/b)
    - [i](#12c/b/i)
      - [Solution](#12c/b/i/solution)
    - [ii](#12c/b/ii)
      - [Solution](#12c/b/ii/solution)
    - [iii](#12c/b/iii)
      - [Solution](#12c/b/iii/solution)
  - [c](#12c/c)
    - [Solution](#12c/c/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

Suppose there were only finitely many [prime numbers](../../../number-theory.md#prime-number) congruent to $2$ modulo $3$, and list them as $p_1,\ldots,p_k$. Consider

$$
N=3p_1\cdots p_k-1.
$$

No $p_i$ divides $N$, and $3$ does not divide $N$. In the [prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) of $N$, not every prime factor can be congruent to $1$ modulo $3$, since their product would then also be congruent to $1$, whereas

$$
N\equiv2\pmod3.
$$

Thus some prime factor is congruent to $2$ modulo $3$, contradicting the completeness of the list. Hence

$$
\boxed{\text{there are infinitely many primes of the form }3n+2}.
$$

Now let $p$ be prime. If $p\ne3$, then either $p=2$, giving

$$
2p^2+1=9,
$$

or $p$ is not divisible by $3$, so $p^2\equiv1\pmod3$. In the latter case

$$
2p^2+1\equiv0\pmod3
$$

and is greater than $3$, hence is composite. For $p=3$ the number is $19$, which is prime. Therefore

$$
\boxed{p=3\text{ is the only possibility}}.
$$

## 2D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

Let

$$
x=\sqrt[3]2+\sqrt[3]3.
$$

If $x$ were [rational](../../../number-theory.md#rational-number), then

$$
x^3=5+3x\sqrt[3]6
$$

would make $\sqrt[3]6=(x^3-5)/(3x)$ rational. But if $\sqrt[3]6=a/b$ in lowest terms, then $a^3=6b^3$, which is impossible by [unique prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic): the exponent of $2$ on the two sides is respectively a multiple of three and one more than a multiple of three. Therefore

$$
\boxed{\sqrt[3]2+\sqrt[3]3\text{ is irrational}}.
$$

Use the given [convergent series](../../../real-analysis.md#convergent-series)

$$
e-e^{-1}=2\sum_{n=0}^{\infty}\frac1{(2n+1)!}.
$$

Suppose this number were $a/b\in\mathbb Q$. Choose $N$ large enough that $b\mid(2N+1)!$. Multiplication by $(2N+1)!$ makes both the rational number and the partial sum through $n=N$ integers. Their difference

$$
R_N
=2(2N+1)!\sum_{n=N+1}^{\infty}\frac1{(2n+1)!}
$$

would therefore be an integer. It is positive, while

$$
0<R_N
\leq2\sum_{j=1}^{\infty}\frac1{(2N+2)^{2j}}
<1
$$

for sufficiently large $N$, a contradiction. Hence

$$
\boxed{e-e^{-1}\text{ is irrational}}.
$$

A [transcendental number](../../../algebra.md#transcendental-number) is a complex number that is not a root of any nonzero polynomial with rational, equivalently integer, coefficients. Let

$$
y=ae+be^{-1},
\qquad (a,b)\ne(0,0).
$$

If $a\ne0$ and $y$ were an [algebraic number](../../../algebra.md#algebraic-number), then $e$ would satisfy

$$
aX^2-yX+b=0
$$

over the algebraic extension $\mathbb Q(y)$. By [transitivity of algebraic extensions](../../../algebra.md#transitivity-of-algebraic-extensions), $e$ would be algebraic over $\mathbb Q$, contradicting its transcendence. If $a=0$, then $b\ne0$ and $e=b/y$ would again be algebraic. Thus

$$
\boxed{ae+be^{-1}\text{ is transcendental}}.
$$

## 3C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3c/a">a</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/a/solution">Solution</h4>

↑ **Parent:** [A](#3c/a)

Take the scalar product of the [Lorentz force](../../../electromagnetism.md#lorentz-force) equation with the constant [magnetic field](../../../electromagnetism.md#magnetic-field) $\mathbf B$. Since $\mathbf E\cdot\mathbf B=0$ and $(\dot{\mathbf x}\times\mathbf B)\cdot\mathbf B=0$,

$$
m\frac{d^2}{dt^2}(\mathbf x\cdot\mathbf B)=0.
$$

The initial velocity also obeys $\mathbf v\cdot\mathbf B=0$, so $\mathbf x\cdot\mathbf B$ remains equal to $\mathbf x_0\cdot\mathbf B$. The trajectory therefore lies in the plane

$$
\boxed{(\mathbf x-\mathbf x_0)\cdot\mathbf B=0},
$$

the plane through $\mathbf x_0$ perpendicular to $\mathbf B$.

<h3 id="3c/b">b</h3>

↑ **Parent:** [3C](#3c)

<h4 id="3c/b/solution">Solution</h4>

↑ **Parent:** [B](#3c/b)

Let $\mathbf E=E\widehat{\mathbf x}$ and $\mathbf B=B\widehat{\mathbf y}$, and choose $\widehat{\mathbf z}=\widehat{\mathbf x}\times\widehat{\mathbf y}$. Part (a) gives $y=0$. With the origin at $\mathbf x_0$, the remaining Cartesian components are

$$
\ddot x=\frac{qE}{m}-\omega\dot z,
\qquad
\ddot z=\omega\dot x,
\qquad
\omega=\frac{qB}{m}.
$$

The initial conditions are $x=z=\dot x=\dot z=0$. Integrating the second equation gives $\dot z=\omega x$, so

$$
\ddot x+\omega^2x=\frac{qE}{m}.
$$

Solving this [forced harmonic oscillator](../../../analysis.md#forced-harmonic-oscillator) and then integrating $\dot z=\omega x$ yields

$$
\boxed{
\begin{aligned}
x(t)&=\frac{mE}{qB^2}\bigl(1-\cos\omega t\bigr),\\
y(t)&=0,\\
z(t)&=\frac EB\left(t-\frac{\sin\omega t}{\omega}\right).
\end{aligned}}
$$

**Thus the position vector is $\mathbf x_0+x(t)\widehat{\mathbf x}+z(t)\widehat{\mathbf z}$. The oscillation occurs at the signed [cyclotron frequency](../../../quantum-theory.md#cyclotron-frequency), superposed on the usual [E-cross-B drift](../../../electromagnetism.md#e-cross-b-drift).**

## 4C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4c/a">a</h3>

↑ **Parent:** [4C](#4c)

<h4 id="4c/a/i">i</h4>

↑ **Parent:** [A](#4c/a)

<h5 id="4c/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4c/a/i)

The [Galilean transformation](../../../special-relativity.md#galilean-transformation) is

$$
ct'=ct,\qquad x'=x-ut=x-\beta ct.
$$

Therefore

$$
\boxed{
A_{\mathrm N}
=\begin{pmatrix}
1&0\\
-\beta&1
\end{pmatrix}}.
$$

<h4 id="4c/a/ii">ii</h4>

↑ **Parent:** [A](#4c/a)

<h5 id="4c/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4c/a/ii)

The one-dimensional [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) gives

$$
ct'=\gamma(ct-\beta x),
\qquad
x'=\gamma(x-\beta ct),
\qquad
\gamma=\frac1{\sqrt{1-\beta^2}}.
$$

Hence

$$
\boxed{
A_{\mathrm{SR}}
=\gamma
\begin{pmatrix}
1&-\beta\\
-\beta&1
\end{pmatrix}}.
$$

As $|\beta|\to0$, $\gamma=1+O(\beta^2)$. The spatial transformation is therefore $x'=x-ut+O(\beta^2)$, while

$$
t'=t-\frac{ux}{c^2}+O(\beta^2t).
$$

Under the stated condition $|x|<c|t|$, the fractional correction $|ux|/(c^2|t|)$ is smaller than $|\beta|$ and tends to zero. Thus the Lorentz transformation has the [nonrelativistic limit](../../../special-relativity.md#nonrelativistic-limit) given by the Galilean transformation.

<h3 id="4c/b">b</h3>

↑ **Parent:** [4C](#4c)

<h4 id="4c/b/solution">Solution</h4>

↑ **Parent:** [B](#4c/b)

For the special-relativistic matrix,

$$
A\binom11=\gamma(1-\beta)\binom11,
\qquad
A\binom1{-1}=\gamma(1+\beta)\binom1{-1}.
$$

Thus the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) and corresponding [eigenvectors](../../../linear-operator-theory.md#eigenvector) are

$$
\boxed{
\lambda_+=\sqrt{\frac{1-\beta}{1+\beta}},
\quad v_+=\binom11},
\qquad
\boxed{
\lambda_-=\sqrt{\frac{1+\beta}{1-\beta}},
\quad v_-=\binom1{-1}}.
$$

The eigenvector equations are $x=ct$ and $x=-ct$. They are the two [null directions](../../../special-relativity.md#null-directions) of the [light cone](../../../special-relativity.md#light-cone), representing right-moving and left-moving light rays. A Lorentz boost preserves each light-ray direction while rescaling its null coordinate.

## 5E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

The [Bezout identity](../../../algebra.md#bezout-identity) states that for integers $a,b$, not both zero, there are integers $r,s$ such that

$$
ra+sb=\gcd(a,b).
$$

If the [prime number](../../../number-theory.md#prime-number) $p$ divides $ab$ but does not divide $a$, then $\gcd(p,a)=1$. Thus $rp+sa=1$ for some integers $r,s$, and multiplication by $b$ gives

$$
b=rpb+sab.
$$

Both terms on the right are divisible by $p$, so $p\mid b$. Hence

$$
\boxed{p\mid ab\Longrightarrow p\mid a\text{ or }p\mid b}.
$$

If $\gcd(m,n)=1$, choose $r,s$ with $rm+sn=1$. Then

$$
x=a(sn)+b(rm)
$$

satisfies $x\equiv a\pmod m$ and $x\equiv b\pmod n$. If $x,x'$ are two simultaneous solutions, both $m$ and $n$ divide $x-x'$. Coprimality implies $mn\mid x-x'$, so the solution is unique modulo $mn$. This proves the two-modulus [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem).

Let $p$ be odd and suppose

$$
x^2\equiv1\pmod{p^d}.
$$

Then $p^d\mid(x-1)(x+1)$. Since $\gcd(x-1,x+1)$ divides $2$, the odd prime $p$ cannot divide both factors. The full power $p^d$ must therefore divide one of them, giving

$$
x\equiv1\pmod{p^d}
\quad\hbox{or}\quad
x\equiv-1\pmod{p^d}.
$$

These are distinct, so there are exactly two solutions.

For an odd integer

$$
n=\prod_{j=1}^kp_j^{d_j},
$$

the Chinese remainder theorem identifies a solution modulo $n$ with independent solutions modulo the $k$ [prime powers](../../../number-theory.md#prime-power). Each component has two choices, hence

$$
\boxed{\#\{x\bmod n:x^2\equiv1\}=2^k}.
$$

For $n=2^d$, there is one solution when $d=1$ and two when $d=2$. If $d\geq3$, a solution $x$ is odd, and of the consecutive even integers $x-1,x+1$, exactly one is divisible by $4$. The [2-adic valuations](../../../number-theory.md#p-adic-valuation) therefore have minimum one; for their sum to be at least $d$, the other must be at least $d-1$. Thus $x\equiv\pm1\pmod{2^{d-1}}$, giving the four distinct classes

$$
1,\quad -1,\quad1+2^{d-1},\quad-1+2^{d-1}\pmod{2^d}.
$$

Consequently the answer is

$$
\boxed{
\begin{cases}
1,&d=1,\\
2,&d=2,\\
4,&d\geq3.
\end{cases}}
$$

## 6D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6d/a">a</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/a/solution">Solution</h4>

↑ **Parent:** [A](#6d/a)

For $0\leq k\leq n$, the [binomial coefficient](../../../combinatorics.md#binomial-coefficient) is

$$
\binom nk=\frac{n!}{k!(n-k)!}.
$$

When $1\leq k\leq n-1$,

$$
\begin{aligned}
\binom{n-1}k+\binom{n-1}{k-1}
&=\frac{(n-1)!}{k!(n-1-k)!}
+\frac{(n-1)!}{(k-1)!(n-k)!}\\
&=\frac{(n-1)![(n-k)+k]}{k!(n-k)!}\\
&=\boxed{\binom nk}.
\end{aligned}
$$

This is [Pascal's identity](../../../combinatorics.md#pascal-s-rule).

<h3 id="6d/b">b</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/b/solution">Solution</h4>

↑ **Parent:** [B](#6d/b)

The special [binomial theorem](../../../combinatorics.md#binomial-theorem)

$$
(1+t)^n=\sum_{k=0}^n\binom nk t^k
$$

follows by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction). Multiplication of the formula for $n$ by $1+t$ and collection of the coefficient of $t^k$ uses Pascal's identity from part (a).

Termwise integration from $0$ to $1$ gives

$$
\boxed{
\sum_{k=0}^n\frac1{k+1}\binom nk
=\int_0^1(1+t)^n\,dt
=\frac{2^{n+1}-1}{n+1}}.
$$

Replacing $t$ by $-t$ gives

$$
\boxed{
\sum_{k=0}^n\frac{(-1)^k}{k+1}\binom nk
=\int_0^1(1-t)^n\,dt
=\frac1{n+1}}.
$$

Finally,

$$
\sum_{k=1}^n\frac{(-1)^{k+1}}k\binom nk
=\int_0^1\frac{1-(1-x)^n}{x}\,dx.
$$

Writing $y=1-x$ and using the finite [geometric series](../../../real-analysis.md#geometric-series),

$$
\frac{1-y^n}{1-y}=1+y+\cdots+y^{n-1},
$$

turns this into

$$
\boxed{\sum_{j=0}^{n-1}\int_0^1y^j\,dy
=1+\frac12+\cdots+\frac1n}.
$$

<h3 id="6d/c">c</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/c/solution">Solution</h4>

↑ **Parent:** [C](#6d/c)

Put

$$
S_n=\sum_{k=0}^{\lfloor(n-1)/2\rfloor}
\binom{n-k-1}{k}.
$$

The initial values are $S_1=S_2=1$. Using Pascal's identity and the convention that an out-of-range binomial coefficient is zero,

$$
\begin{aligned}
S_{n+2}
&=\sum_{k\geq0}\binom{n+1-k}{k}\\
&=\sum_{k\geq0}\binom{n-k}{k}
+\sum_{k\geq1}\binom{n-k}{k-1}\\
&=S_{n+1}+S_n.
\end{aligned}
$$

Thus $(S_n)$ has the same initial values and [linear recurrence relation](../../../algebra.md#linear-recurrence-relation) as the [Fibonacci numbers](../../../real-analysis.md#fibonacci-number). [Mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) gives

$$
\boxed{
F_n=\sum_{k=0}^{\lfloor(n-1)/2\rfloor}
\binom{n-k-1}{k}}.
$$

## 7F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7f/a">a</h3>

↑ **Parent:** [7F](#7f)

<h4 id="7f/a/solution">Solution</h4>

↑ **Parent:** [A](#7f/a)

Because $P(\mathbf x)\subseteq P(\mathbf x)$, the relation is [reflexive](../../../set-theory.md#reflexive-relation). If $\mathbf x\preceq\mathbf y$ and $\mathbf y\preceq\mathbf z$, then

$$
P(\mathbf x)\subseteq P(\mathbf y)\subseteq P(\mathbf z),
$$

so it is [transitive](../../../set-theory.md#transitive-relation). It is not [symmetric](../../../set-theory.md#symmetric-relation): for

$$
\mathbf x=(1,0,\ldots,0),
\qquad
\mathbf y=(1,1,0,\ldots,0),
$$

one has $\mathbf x\preceq\mathbf y$ but not $\mathbf y\preceq\mathbf x$.

<h3 id="7f/b">b</h3>

↑ **Parent:** [7F](#7f)

<h4 id="7f/b/solution">Solution</h4>

↑ **Parent:** [B](#7f/b)

Suppose $\mathbf x\preceq\mathbf y$. Define the nonnegative tuple $\mathbf z$ coordinatewise by

$$
z_i=
\begin{cases}
x_i/y_i,&y_i>0,\\
0,&y_i=0.
\end{cases}
$$

When $y_i=0$, support inclusion forces $x_i=0$, so $x_i=y_iz_i$ in every coordinate.

Conversely, if $x_i=y_iz_i$ with $y_i,z_i\geq0$, then $x_i>0$ implies $y_i>0$. Hence $P(\mathbf x)\subseteq P(\mathbf y)$ and $\mathbf x\preceq\mathbf y$. This proves the equivalence.

<h3 id="7f/c">c</h3>

↑ **Parent:** [7F](#7f)

<h4 id="7f/c/solution">Solution</h4>

↑ **Parent:** [C](#7f/c)

The definition says

$$
\mathbf x\sim\mathbf y
\quad\Longleftrightarrow\quad
P(\mathbf x)=P(\mathbf y).
$$

Equality of sets is reflexive, symmetric, and transitive, so $\sim$ is an [equivalence relation](../../../set-theory.md#equivalence-relation). Its classes are indexed by all subsets of $\{1,\ldots,n\}$, and every subset occurs as the support of its zero-one [indicator vector](../../../measure-theory.md#indicator-vector). The number of classes is therefore

$$
\boxed{2^n}.
$$

<h3 id="7f/d">d</h3>

↑ **Parent:** [7F](#7f)

<h4 id="7f/d/solution">Solution</h4>

↑ **Parent:** [D](#7f/d)

Define

$$
y_i=
\begin{cases}
x_i,&s_i>0,\\
0,&s_i=0,
\end{cases}
\qquad
z_i=x_i-y_i.
$$

Then $\mathbf x=\mathbf y+\mathbf z$, the support of $\mathbf y$ lies in $P(\mathbf s)$, and the support of $\mathbf z$ is disjoint from $P(\mathbf s)$. Thus $\mathbf y\preceq\mathbf s$ and $\mathbf z\perp\mathbf s$.

For uniqueness, if $s_i>0$, orthogonality forces $z_i=0$, hence $y_i=x_i$. If $s_i=0$, the condition $\mathbf y\preceq\mathbf s$ forces $y_i=0$, hence $z_i=x_i$. Every coordinate is therefore forced, proving uniqueness.

## 8F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8f/a">a</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/a/solution">Solution</h4>

↑ **Parent:** [A](#8f/a)

A set is [countable](../../../set-theory.md#countable-set) when it is finite or its elements can be put in one-to-one correspondence with a subset of $\mathbb N$. Equivalently, there is an injection from the set into $\mathbb N$.

<h3 id="8f/b">b</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/b/i">i</h4>

↑ **Parent:** [B](#8f/b)

<h5 id="8f/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8f/b/i)

List pairs $(m,n)\in\mathbb N^2$ by increasing value of $m+n$, and within each diagonal by increasing $m$:

$$
(1,1),\ (1,2),(2,1),\ (1,3),(2,2),(3,1),\ldots.
$$

Every pair occurs after finitely many earlier diagonals. More explicitly, the [Cantor pairing function](../../../set-theory.md#cantor-pairing-function)

$$
\pi(m,n)=\frac{(m+n-2)(m+n-1)}2+m
$$

is an injection $\mathbb N^2\to\mathbb N$. Hence $\mathbb N\times\mathbb N$ is countable.

<h4 id="8f/b/ii">ii</h4>

↑ **Parent:** [B](#8f/b)

<h5 id="8f/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8f/b/ii)

The integers are countable under the enumeration

$$
0,1,-1,2,-2,\ldots.
$$

Part (i) then shows that $\mathbb Z\times\mathbb N$ is countable. The map

$$
(a,b)\longmapsto\frac ab
$$

is a surjection from $\mathbb Z\times\mathbb N$ onto the [rational numbers](../../../number-theory.md#rational-number). Selecting, for example, the representation in lowest terms with positive denominator gives an injection in the other direction. Thus $\mathbb Q$ is countable.

<h4 id="8f/b/iii">iii</h4>

↑ **Parent:** [B](#8f/b)

<h5 id="8f/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8f/b/iii)

For a [increasing function](../../../calculus.md#monotonic-function) $F$, define its one-sided limits by

$$
F(x-)=\sup_{t<x}F(t),
\qquad
F(x+)=\inf_{t>x}F(t).
$$

They exist because of [monotonicity](../../../calculus.md#monotonic-function). The function is discontinuous at $x$ only if the jump interval

$$
J_x=(F(x-),F(x+))
$$

is nonempty. By the [density of the rational numbers](../../../number-theory.md#density-of-the-rational-numbers), choose $q_x\in J_x\cap\mathbb Q$.

If $x<y$, monotonicity gives $F(x+)\leq F(y-)$, so $J_x$ and $J_y$ are disjoint. Consequently $q_x\ne q_y$, and $x\mapsto q_x$ injects the set of discontinuities into $\mathbb Q$. Since the rationals are countable by part (ii), the set of discontinuities is countable.

<h3 id="8f/c">c</h3>

↑ **Parent:** [8F](#8f)

<h4 id="8f/c/solution">Solution</h4>

↑ **Parent:** [C](#8f/c)

Suppose first that $|A_n|=1$ for every $n>N$. Then an element of $B$ is determined by its first $N$ coordinates, so $B$ is in bijection with

$$
A_1\times\cdots\times A_N.
$$

A finite [Cartesian product](../../../set-theory.md#cartesian-product) of countable sets is countable by repeated application of the diagonal enumeration in part (b)(i). Hence $B$ is countable.

Conversely, suppose infinitely many factors contain at least two elements. Choose increasing indices $n_1<n_2<\cdots$ and distinct elements

$$
a_j^0,a_j^1\in A_{n_j}.
$$

Fix one element in every remaining factor. Each [binary sequence](../../../real-analysis.md#bitstream) $\varepsilon=(\varepsilon_1,\varepsilon_2,\ldots)$ then defines an element of $B$ by placing $a_j^{\varepsilon_j}$ in coordinate $n_j$ and the fixed element elsewhere. This map is injective.

The set $\{0,1\}^{\mathbb N}$ is uncountable by [Cantor's diagonal argument](../../../set-theory.md#cantor-s-diagonal-argument): from any proposed list of binary sequences, form a new sequence whose $j$th digit differs from the $j$th digit of the $j$th listed sequence. It is absent from the list. Thus $B$ contains an uncountable subset and cannot be countable.

Therefore

$$
\boxed{
B\text{ is countable }\Longleftrightarrow
\exists N\ \forall n>N,\ |A_n|=1}.
$$

## 9C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9c/a">a</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/a/solution">Solution</h4>

↑ **Parent:** [A](#9c/a)

The [center of mass](../../../classical-mechanics.md#center-of-mass) is

$$
\mathbf R=\frac{m_1\mathbf x_1+m_2\mathbf x_2}{m_1+m_2}.
$$

By [Newton's third law](../../../classical-mechanics.md#newton-s-third-law), $\mathbf F_{21}=-\mathbf F_{12}$, so

$$
(m_1+m_2)\ddot{\mathbf R}
=m_1\ddot{\mathbf x}_1+m_2\ddot{\mathbf x}_2
=\mathbf F_{12}+\mathbf F_{21}=0.
$$

Thus $\dot{\mathbf R}$ is constant. For $\mathbf r=\mathbf x_1-\mathbf x_2$,

$$
\ddot{\mathbf r}
=\left(\frac1{m_1}+\frac1{m_2}\right)\mathbf F_{12}.
$$

Therefore

$$
\boxed{\mu\ddot{\mathbf r}=\mathbf F_{12}},
\qquad
\boxed{\mu=\frac{m_1m_2}{m_1+m_2}},
$$

where $\mu$ is the [reduced mass](../../../classical-mechanics.md#reduced-mass).

<h3 id="9c/b">b</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/b/solution">Solution</h4>

↑ **Parent:** [B](#9c/b)

For the proposed [circular motion](../../../classical-mechanics.md#circular-motion),

$$
\ddot{\mathbf x}_1=-a\omega^2(\cos\omega t,\sin\omega t,0).
$$

The separation is $\mathbf x_1-\mathbf x_2=2a(\cos\omega t,\sin\omega t,0)$, so the [inverse-square force](../../../classical-mechanics.md#inverse-square-force) on particle 1 is

$$
\mathbf F_{12}
=-\frac{km^2}{4a^2}(\cos\omega t,\sin\omega t,0).
$$

The equation $m\ddot{\mathbf x}_1=\mathbf F_{12}$ holds exactly when

$$
\boxed{\omega^2=\frac{km}{4a^3}}.
$$

The equation for particle 2 follows by symmetry.

<h3 id="9c/c">c</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/c/i">i</h4>

↑ **Parent:** [C](#9c/c)

<h5 id="9c/c/i/solution">Solution</h5>

↑ **Parent:** [I](#9c/c/i)

At a point $(0,0,z)$, the two particles are at equal distance $\sqrt{a^2+z^2}$. Their force components in the rotating $xy$-plane cancel, while their $z$-components add. Hence a particle initially moving along the $z$-axis remains on it, and

$$
m_3\ddot z
=-\frac{km_3mz}{(a^2+z^2)^{3/2}}
-\frac{km_3mz}{(a^2+z^2)^{3/2}}.
$$

Cancelling $m_3$ gives

$$
\boxed{\ddot z=-\frac{2mkz}{(z^2+a^2)^{3/2}}}.
$$

<h4 id="9c/c/ii">ii</h4>

↑ **Parent:** [C](#9c/c)

<h5 id="9c/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9c/c/ii)

The equation has the one-dimensional [effective potential](../../../physics.md#effective-potential) per unit mass

$$
\boxed{\Phi(z)=-\frac{2mk}{\sqrt{z^2+a^2}}},
\qquad
\ddot z=-\Phi'(z).
$$

Thus the conserved specific energy is

$$
\mathcal E=\frac12\dot z^2+\Phi(z).
$$

The potential has its minimum $-2mk/a$ at $z=0$ and tends to $0$ from below as $|z|\to\infty$. Therefore $-2mk/a<\mathcal E<0$ gives bounded oscillation between two [turning points](../../../analysis.md#classical-turning-point); $\mathcal E=0$ gives marginal escape with asymptotic speed zero; and $\mathcal E>0$ gives escape with nonzero asymptotic speed. The minimum itself is the equilibrium $z=0$.

<h4 id="9c/c/iii">iii</h4>

↑ **Parent:** [C](#9c/c)

<h5 id="9c/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#9c/c/iii)

For $|z|\ll a$, [linearization](../../../algebra.md#linearization) gives

$$
\ddot z=-\frac{2mk}{a^3}z+O(z^3).
$$

The leading motion is [simple harmonic motion](../../../classical-mechanics.md#simple-harmonic-motion) with angular frequency

$$
\omega_z=\sqrt{\frac{2mk}{a^3}}.
$$

With $z(0)=z_0$ and $\dot z(0)=0$,

$$
z(t)\simeq z_0\cos(\omega_zt),
$$

and its period is

$$
\boxed{T=2\pi\sqrt{\frac{a^3}{2mk}}}.
$$

<h4 id="9c/c/iv">iv</h4>

↑ **Parent:** [C](#9c/c)

<h5 id="9c/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#9c/c/iv)

The initial specific energy is

$$
\mathcal E=\frac12u^2-\frac{2mk}{a}.
$$

Escape to infinity is possible exactly when $\mathcal E\geq0$. Thus the [escape velocity](../../../classical-mechanics.md#escape-velocity) criterion is

$$
\boxed{|u|\geq2\sqrt{\frac{mk}{a}}}.
$$

Equality corresponds to marginal escape.

## 10C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10c/a">a</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/a/solution">Solution</h4>

↑ **Parent:** [A](#10c/a)

The term $-2\boldsymbol\Omega\times\dot{\mathbf x}$ is the [Coriolis acceleration](../../../physics.md#coriolis-acceleration), and $-\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf x)$ is the [centrifugal acceleration](../../../physics.md#centrifugal-acceleration). With $\boldsymbol\Omega=-\Omega\widehat{\mathbf z}$, the Cartesian components are

$$
\boxed{
\begin{aligned}
\ddot x&=-2\Omega\dot y+\Omega^2x+\frac{N_x}{m},\\
\ddot y&= 2\Omega\dot x+\Omega^2y+\frac{N_y}{m},\\
\ddot z&=g+\frac{N_z}{m}.
\end{aligned}}
$$

<h3 id="10c/b">b</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/b/solution">Solution</h4>

↑ **Parent:** [B](#10c/b)

The circular constraint is

$$
x=R\sin\theta,\qquad z=R\cos\theta.
$$

Its tangent in the $xz$-plane is $(\cos\theta,0,-\sin\theta)$, while the [normal force](../../../classical-mechanics.md#normal-force) is radial. Projecting the equations from part (a) onto this tangent eliminates the normal force and gives

$$
\boxed{
R\ddot\theta
=-g\sin\theta+\Omega^2R\cos\theta\sin\theta
-2\Omega\dot y\cos\theta}.
$$

Because the ramp is translation-invariant along $y$, $N_y=0$; using $\dot x=R\dot\theta\cos\theta$ gives

$$
\boxed{\ddot y=\Omega^2y+2\Omega R\dot\theta\cos\theta}.
$$

For rest in the rotating frame, $\dot\theta=\dot y=\ddot\theta=\ddot y=0$. Assuming $\Omega\ne0$, the second equation gives $y=0$, and the first gives

$$
\sin\theta(\Omega^2R\cos\theta-g)=0.
$$

On the semicircular ramp the rest points are therefore

$$
\boxed{\theta=0,\ y=0}
$$

and, when $\Omega^2R\geq g$,

$$
\boxed{\theta=\pm\arccos\frac{g}{\Omega^2R},\ y=0}.
$$

<h3 id="10c/c">c</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/c/solution">Solution</h4>

↑ **Parent:** [C](#10c/c)

Neglecting terms of order $\Omega^2$ and linearizing in $\theta$ gives

$$
R\ddot\theta=-g\theta-2\Omega\dot y,
\qquad
\ddot y=2\Omega R\dot\theta.
$$

The second equation and the initial data imply

$$
\dot y=2\Omega R(\theta-\theta_0).
$$

Its contribution to the first equation is of order $\Omega^2$, so the retained equation is

$$
\ddot\theta+\frac gR\theta=0.
$$

Thus

$$
\boxed{\theta(t)=\theta_0\cos(\omega_0t)},
\qquad
\boxed{\omega_0=\sqrt{\frac gR}}.
$$

Integrating the associated $y$ velocity and using $y(0)=0$ gives

$$
\boxed{
y(t)=2\Omega R\theta_0
\left(\frac{\sin(\omega_0t)}{\omega_0}-t\right)}.
$$

## 11C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11c/a">a</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/a/i">i</h4>

↑ **Parent:** [A](#11c/a)

<h5 id="11c/a/i/solution">Solution</h5>

↑ **Parent:** [I](#11c/a/i)

The [moment of inertia](../../../classical-mechanics.md#moment-of-inertia) about an axis is

$$
I=\int_V\rho\,r_\perp^2\,dV,
$$

where $r_\perp$ is the perpendicular distance to the axis. The disc mass is

$$
M=\rho\pi r^2\delta.
$$

To leading order in $\delta/r$, the distance from the $x$-axis is $|y|$. Using polar coordinates in the disc,

$$
\begin{aligned}
I_x
&=\rho\delta\int_0^r\int_0^{2\pi}
(s\sin\phi)^2s\,d\phi\,ds\\
&=\rho\delta\frac{r^4}{4}\pi
=\boxed{\frac14Mr^2}.
\end{aligned}
$$

<h4 id="11c/a/ii">ii</h4>

↑ **Parent:** [A](#11c/a)

<h5 id="11c/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11c/a/ii)

The axis $y=0,z=h$ is parallel to the $x$-axis and lies a distance $|h|$ from it. The [parallel axis theorem](../../../classical-mechanics.md#parallel-axis-theorem) therefore gives

$$
\boxed{I=\frac14Mr^2+Mh^2
=M\left(\frac{r^2}{4}+h^2\right)}
$$

to leading order in the thickness.

<h3 id="11c/b">b</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/b/i">i</h4>

↑ **Parent:** [B](#11c/b)

<h5 id="11c/b/i/solution">Solution</h5>

↑ **Parent:** [I](#11c/b/i)

Measure $z$ from the apex along the cone's symmetry axis. A thin disc at height $z$ has radius

$$
s(z)=\frac RH z
$$

and mass $dM=\rho\pi s^2\,dz$. Its moment about a parallel diameter through its centre is $s^2dM/4$, while its centre is distance $z$ from the required axis. Part (a)(ii) gives

$$
dI=\left(z^2+\frac{s^2}{4}\right)dM.
$$

Hence

$$
\begin{aligned}
I
&=\rho\pi\int_0^H
\frac{R^2z^2}{H^2}
\left(z^2+\frac{R^2z^2}{4H^2}\right)dz\\
&=\rho\pi\left(\frac{R^2H^3}{5}
+\frac{R^4H}{20}\right).
\end{aligned}
$$

Since $M=\rho\pi R^2H/3$,

$$
\boxed{
I=M\left(\frac3{20}R^2+\frac35H^2\right)},
\qquad
\boxed{\alpha=\frac3{20},\quad\beta=\frac35}.
$$

<h4 id="11c/b/ii">ii</h4>

↑ **Parent:** [B](#11c/b)

<h5 id="11c/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11c/b/ii)

Without friction, [rotational kinetic energy](../../../classical-mechanics.md#rotational-kinetic-energy) is conserved:

$$
K_0=\frac12I\omega^2.
$$

The constant angular speed is $\omega=\sqrt{2K_0/I}$, so one full rotation takes

$$
\boxed{T=\frac{2\pi}{\omega}
=2\pi\sqrt{\frac{I}{2K_0}}}.
$$

<h4 id="11c/b/iii">iii</h4>

↑ **Parent:** [B](#11c/b)

<h5 id="11c/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#11c/b/iii)

The work law means that friction exerts a constant opposing [torque](../../../classical-mechanics.md#torque) of magnitude $W$. Until the cone stops,

$$
I\dot\omega=-W.
$$

Its initial angular speed is $\omega_0=\sqrt{2K_0/I}$, and uniform angular deceleration gives

$$
0=\omega_0-\frac WI t.
$$

Therefore

$$
\boxed{t=\frac{I\omega_0}{W}
=\sqrt{\frac{2K_0I}{W^2}}}.
$$

## 12C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12c/a">a</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/a/solution">Solution</h4>

↑ **Parent:** [A](#12c/a)

A [four-vector](../../../special-relativity.md#four-vector) is an object whose components transform between inertial frames by a [Lorentz transformation](../../../special-relativity.md#lorentz-transformation),

$$
U'^\mu=\Lambda^\mu{}_\nu U^\nu.
$$

Lorentz transformations are defined by

$$
\Lambda^T\eta\Lambda=\eta,
$$

where $\eta$ is the [Minkowski metric](../../../special-relativity.md#minkowski-metric). Consequently

$$
U'\cdot U'
=(\Lambda U)^T\eta(\Lambda U)
=U^T\Lambda^T\eta\Lambda U
=U^T\eta U
=U\cdot U.
$$

**Thus the [Minkowski norm](../../../special-relativity.md#minkowski-norm) of a four-vector is the same in every inertial frame.**

<h3 id="12c/b">b</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/b/i">i</h4>

↑ **Parent:** [B](#12c/b)

<h5 id="12c/b/i/solution">Solution</h5>

↑ **Parent:** [I](#12c/b/i)

Along the particle's worldline,

$$
x=u_xt,\qquad y=u_yt.
$$

The boost from $S$ to $S'$ gives

$$
x'=\gamma(x-Vt),\qquad
y'=y,\qquad
t'=\gamma\left(t-\frac{Vx}{c^2}\right).
$$

Therefore

$$
\frac{dt'}{dt}
=\gamma\left(1-\frac{Vu_x}{c^2}\right),
$$

and division of the transformed coordinate velocities by this factor gives the [relativistic velocity-addition formula](../../../special-relativity.md#velocity-addition-formula)

$$
\boxed{
u'_x=\frac{u_x-V}{1-Vu_x/c^2},
\qquad
u'_y=\frac{u_y}{\gamma(1-Vu_x/c^2)},
\qquad
u'_z=0}.
$$

<h4 id="12c/b/ii">ii</h4>

↑ **Parent:** [B](#12c/b)

<h5 id="12c/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#12c/b/ii)

To first order in $V/c$, $\gamma=1+O(V^2/c^2)$ and

$$
\frac1{1-Vu_x/c^2}
=1+\frac{Vu_x}{c^2}+O(V^2/c^2).
$$

Thus

$$
u'_x=u_x-V+\frac{Vu_x^2}{c^2}+O(V^2/c^2),
\qquad
u'_y=u_y+\frac{Vu_xu_y}{c^2}+O(V^2/c^2).
$$

Since $\mathbf V=(V,0,0)$ and $\mathbf V\cdot\mathbf u=Vu_x$, these components combine into

$$
\boxed{
\mathbf u'=\mathbf u-\mathbf V
+\frac{\mathbf V\cdot\mathbf u}{c^2}\mathbf u
+O(V^2/c^2)}.
$$

<h4 id="12c/b/iii">iii</h4>

↑ **Parent:** [B](#12c/b)

<h5 id="12c/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#12c/b/iii)

For a photon,

$$
\mathbf u=c(\cos\theta,\sin\theta,0).
$$

Part (ii) gives the first-order changes

$$
\delta u_x=-V\sin^2\theta,
\qquad
\delta u_y=V\sin\theta\cos\theta.
$$

For a vector of fixed leading-order magnitude $c$, its small change of angle is

$$
\delta\theta
=\frac{u_x\delta u_y-u_y\delta u_x}{c^2}.
$$

Substitution yields the [relativistic aberration](../../../physics.md#relativistic-aberration) formula

$$
\boxed{\theta'-\theta=\frac Vc\sin\theta}
$$

to leading order.

<h3 id="12c/c">c</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/c/solution">Solution</h4>

↑ **Parent:** [C](#12c/c)

Let the incident and final photon momentum magnitudes be

$$
p=\frac h\lambda,
\qquad
p'=\frac h{\lambda'}.
$$

In a nontrivial collinear collision, the photon is backscattered and the electron moves in the original photon direction, so momentum conservation gives electron momentum $P=p+p'$. [Conservation of relativistic energy](../../../special-relativity.md#conservation-of-relativistic-energy) gives

$$
pc+mc^2=p'c+\sqrt{m^2c^4+P^2c^2}.
$$

Substitute $P=p+p'$, isolate the square root, and square. Cancellation leaves

$$
mc(p-p')=2pp'.
$$

Dividing by $pp'$ and using the wavelength definitions gives the [Compton scattering](../../../physics.md#compton-scattering) shift

$$
\boxed{\lambda'=\lambda+\frac{2h}{mc}}.
$$

The other collinear possibility is the trivial forward solution $\lambda'=\lambda$, in which the electron remains at rest.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
