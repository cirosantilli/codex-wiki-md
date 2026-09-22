# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperia_4_2019.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2019/paperia_4_2019.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3A](#3a)
  - [Solution](#3a/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
- [5E](#5e)
  - [a](#5e/a)
    - [Solution](#5e/a/solution)
  - [b](#5e/b)
    - [Solution](#5e/b/solution)
  - [c](#5e/c)
    - [i](#5e/c/i)
      - [Solution](#5e/c/i/solution)
    - [ii](#5e/c/ii)
      - [Solution](#5e/c/ii/solution)
- [6E](#6e)
  - [a](#6e/a)
    - [Solution](#6e/a/solution)
  - [b](#6e/b)
    - [Solution](#6e/b/solution)
  - [c](#6e/c)
    - [Solution](#6e/c/solution)
  - [d](#6e/d)
    - [Solution](#6e/d/solution)
- [7E](#7e)
  - [a](#7e/a)
    - [i](#7e/a/i)
      - [Solution](#7e/a/i/solution)
    - [ii](#7e/a/ii)
      - [Solution](#7e/a/ii/solution)
    - [iii](#7e/a/iii)
      - [Solution](#7e/a/iii/solution)
  - [b](#7e/b)
    - [Solution](#7e/b/solution)
- [8E](#8e)
  - [a](#8e/a)
    - [Solution](#8e/a/solution)
  - [b](#8e/b)
    - [Solution](#8e/b/solution)
  - [c](#8e/c)
    - [Solution](#8e/c/solution)
- [9A](#9a)
  - [a](#9a/a)
    - [Solution](#9a/a/solution)
  - [b](#9a/b)
    - [Solution](#9a/b/solution)
  - [c](#9a/c)
    - [Solution](#9a/c/solution)
- [10A](#10a)
  - [a](#10a/a)
    - [Solution](#10a/a/solution)
  - [b](#10a/b)
    - [i](#10a/b/i)
      - [Solution](#10a/b/i/solution)
    - [ii](#10a/b/ii)
      - [Solution](#10a/b/ii/solution)
    - [iii](#10a/b/iii)
      - [Solution](#10a/b/iii/solution)
- [11A](#11a)
  - [a](#11a/a)
    - [i](#11a/a/i)
      - [Solution](#11a/a/i/solution)
    - [ii](#11a/a/ii)
      - [Solution](#11a/a/ii/solution)
  - [b](#11a/b)
    - [Solution](#11a/b/solution)
  - [c](#11a/c)
    - [Solution](#11a/c/solution)
- [12A](#12a)
  - [a](#12a/a)
    - [Solution](#12a/a/solution)
  - [b](#12a/b)
    - [Solution](#12a/b/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

Since $4^{-1}\equiv16\pmod{21}$ and $2^{-1}\equiv23\pmod{45}$, the two [linear congruences](../../../number-theory.md#linear-congruence) reduce to

$$
x\equiv16\pmod{21},
\qquad
x\equiv25\pmod{45}.
$$

Write $x=16+21k$. The second congruence becomes

$$
21k\equiv9\pmod{45},
$$

or $7k\equiv3\pmod{15}$ after division by three. Since $7^{-1}\equiv13\pmod{15}$, $k\equiv9\pmod{15}$. The [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) therefore gives the complete family

$$
\boxed{x\equiv205\pmod{315}}.
$$

The modulus is $\operatorname{lcm}(21,45)=315$ because the compatibility condition modulo their greatest common divisor is satisfied.

## 2E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

The first series is [telescoping](../../../real-analysis.md#telescoping-series), since

$$
\frac1{n^2+n}=\frac1n-\frac1{n+1}.
$$

Its $N$th partial sum is $1-1/(N+1)$, so

$$
\boxed{\sum_{n=1}^{\infty}\frac1{n^2+n}=1},
$$

a [rational number](../../../number-theory.md#rational-number).

The second series converges absolutely, for example by the [ratio test](../../../real-analysis.md#ratio-test), and is the odd part of the [exponential series](../../../calculus.md#exponential-series):

$$
\sum_{n=1}^{\infty}\frac1{(2n-1)!}
=\sum_{k=0}^{\infty}\frac1{(2k+1)!}
=\sinh1=\frac{e-e^{-1}}2.
$$

This value is irrational. Indeed, if $a=\sinh1$ were algebraic, then $e$ would satisfy

$$
e^2-2ae-1=0,
$$

making $e$ algebraic over the algebraic numbers and hence algebraic, contrary to the [Hermite theorem on the transcendence of e](../../../algebra.md#hermite-theorem-on-the-transcendence-of-e). Thus the second sum is in fact [transcendental](../../../algebra.md#transcendental-number).

## 3A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3a/solution">Solution</h3>

↑ **Parent:** [3A](#3a)

During a short interval $dt$, let the rocket's mass change by $dm<0$ and its speed by $dv$. The expelled mass $-dm$ has inertial-frame speed $v-u$ to first order. Conservation of [linear momentum](../../../classical-mechanics.md#momentum), including the [impulse](../../../classical-mechanics.md#impulse) $Fdt$, gives

$$
(m+dm)(v+dv)+(-dm)(v-u)-mv=Fdt.
$$

Discarding the second-order product $dm\,dv$ leaves

$$
m\,dv+u\,dm=Fdt,
$$

and hence the [Tsiolkovsky rocket equation](../../../classical-mechanics.md#rocket-equation)

$$
\boxed{m\frac{dv}{dt}+u\frac{dm}{dt}=F}.
$$

In deep space $F=0$, so $dv=-u\,dm/m$. Burning from initial mass $m_0$ to $m_0/2$ increases the speed by

$$
\boxed{\Delta v=-u\int_{m_0}^{m_0/2}\frac{dm}{m}=u\log2}.
$$

## 4A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

Measure displacement downward from the release point and take downward speed $v\geq0$. [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) with [quadratic drag](../../../fluid-mechanics.md#quadratic-drag) gives

$$
m\frac{dv}{dt}=mg-\gamma v^2,
\qquad v(0)=0.
$$

Writing

$$
V=\sqrt{\frac{mg}{\gamma}},
\qquad k=\sqrt{\frac{g\gamma}{m}},
$$

separation of variables gives the [terminal velocity](../../../classical-mechanics.md#terminal-velocity) solution

$$
v(t)=V\tanh(kt).
$$

The distance fallen by time $t$ is therefore

$$
y(t)=\int_0^tv(s)ds
=\frac{m}{\gamma}\log\cosh(kt).
$$

Setting $y(t)=h$ and solving for $t$ yields

$$
\boxed{t=\sqrt{\frac{m}{g\gamma}}\,
\operatorname{arcosh}\!\left(e^{\gamma h/m}\right)}.
$$

## 5E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5e/a">a</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/a/solution">Solution</h4>

↑ **Parent:** [A](#5e/a)

[Fermat's little theorem](../../../number-theory.md#fermat-little-theorem) states that for a prime $p$ and integer $a$,

$$
a^p\equiv a\pmod p;
$$

if $p\nmid a$, equivalently $a^{p-1}\equiv1\pmod p$. For the latter form, multiplication by $a$ permutes the nonzero [residue classes](../../../number-theory.md#residue-class) modulo $p$. Multiplying the congruences $a,2a,\ldots,(p-1)a$ and cancelling $(p-1)!$ gives $a^{p-1}\equiv1$. The first form also covers $p\mid a$.

Since $803=50\cdot16+3$, the theorem gives

$$
3^{803}\equiv3^3=27\equiv\boxed{10}\pmod{17}.
$$

<h3 id="5e/b">b</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/b/solution">Solution</h4>

↑ **Parent:** [B](#5e/b)

We prove both identities by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction). They hold at $n=1$. Assume they hold at $n$. Using $F_{n-1}=F_{n+1}-F_n$,

$$
\begin{aligned}
F_{2n+2}&=F_{2n+1}+F_{2n}\\
&=F_n^2+F_{n+1}^2+F_n(F_{n-1}+F_{n+1})\\
&=F_{n+1}(F_n+F_{n+2}).
\end{aligned}
$$

Adding this to $F_{2n+1}=F_n^2+F_{n+1}^2$ and using $F_{n+2}=F_n+F_{n+1}$ gives

$$
F_{2n+3}=F_{n+1}^2+F_{n+2}^2.
$$

These are precisely the two assertions with $n$ replaced by $n+1$, completing the induction.

<h3 id="5e/c">c</h3>

↑ **Parent:** [5E](#5e)

<h4 id="5e/c/i">i</h4>

↑ **Parent:** [C](#5e/c)

<h5 id="5e/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5e/c/i)

**True.** Write the odd integer as $m=2n+1$. The identity from part (b) and $p\mid F_m$ give

$$
F_n^2+F_{n+1}^2\equiv0\pmod p.
$$

Consecutive [Fibonacci numbers](../../../real-analysis.md#fibonacci-number) are coprime, so $F_{n+1}$ is invertible modulo $p$. Hence

$$
(F_nF_{n+1}^{-1})^2\equiv-1\pmod p.
$$

Thus $-1$ is a [quadratic residue](../../../number-theory.md#quadratic-residue) modulo the odd prime $p$, which occurs exactly when $\boxed{p\equiv1\pmod4}$.

<h4 id="5e/c/ii">ii</h4>

↑ **Parent:** [C](#5e/c)

<h5 id="5e/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5e/c/ii)

This statement can be false. For example, $m=10$ is even and

$$
F_{10}=55,
$$

but the odd prime divisor $p=5$ satisfies $p\equiv1\pmod4$, rather than $3\pmod4$.

## 6E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6e/a">a</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/a/solution">Solution</h4>

↑ **Parent:** [A](#6e/a)

The [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) states that for finite sets $A_1,\ldots,A_k$,

$$
\left|\bigcup_iA_i\right|
=\sum_i|A_i|-\sum_{i<j}|A_i\cap A_j|+\cdots+(-1)^{k+1}|A_1\cap\cdots\cap A_k|.
$$

For each prime $p\mid n$, exclude pairs whose two coordinates are divisible by $p$. For a set of distinct prime divisors $p_1,\ldots,p_j$, exactly $n^2/(p_1\cdots p_j)^2$ pairs have both coordinates divisible by their product. Inclusion-exclusion therefore gives

$$
\boxed{|Y|=n^2\prod_{p\mid n}\left(1-\frac1{p^2}\right)}.
$$

<h3 id="6e/b">b</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/b/solution">Solution</h4>

↑ **Parent:** [B](#6e/b)

The condition $\gcd(a,b,n)=1$ says that the ideal of $\mathbb Z$ generated by $a,b,n$ is all of $\mathbb Z$. The multi-integer [Bezout identity](../../../algebra.md#bezout-identity) therefore supplies integers $r,s,t$ such that

$$
\boxed{ra+sb+tn=1}.
$$

Equivalently, first apply Bézout's identity to $a,b$ and then to $\gcd(a,b),n$.

<h3 id="6e/c">c</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/c/solution">Solution</h4>

↑ **Parent:** [C](#6e/c)

Assume $ad\equiv bc\pmod n$ and choose $r,s$ as in part (b). Put $\lambda=rc+sd$. Multiplying $ra+sb\equiv1$ by $c$ and using $ad\equiv bc$ gives

$$
\lambda a=rac+sad\equiv rac+sbc\equiv c\pmod n.
$$

Similarly, multiplication by $d$ gives $\lambda b\equiv d\pmod n$.

Moreover, $\lambda$ is a [unit modulo n](../../../number-theory.md#unit-modulo-n): if a prime divided both $\lambda$ and $n$, the two congruences would make it divide $c,d,n$, contrary to $(c,d)\in Y$. Thus $R$ means precisely that two pairs differ by multiplication by a unit modulo $n$. Reflexivity, symmetry using $\lambda^{-1}$, and transitivity using products of units now show that $R$ is an [equivalence relation](../../../set-theory.md#equivalence-relation).

<h3 id="6e/d">d</h3>

↑ **Parent:** [6E](#6e)

<h4 id="6e/d/solution">Solution</h4>

↑ **Parent:** [D](#6e/d)

The class of $(1,1)$ is

$$
\{(\lambda,\lambda):\lambda\in(\mathbb Z/n\mathbb Z)^\times\},
$$

so its size is [Euler's totient function](../../../number-theory.md#euler-totient-function)

$$
\varphi(n)=n\prod_{p\mid n}\left(1-\frac1p\right).
$$

The unit group acts freely on every pair in $Y$: if $\lambda a\equiv a$ and $\lambda b\equiv b$, multiplying the [Bezout identity](../../../algebra.md#bezout-identity) by $\lambda-1$ gives $\lambda\equiv1\pmod n$. Hence every equivalence class has size $\varphi(n)$. Dividing the answer from part (a) by this size gives

$$
\boxed{\frac{|Y|}{\varphi(n)}
=n\prod_{p\mid n}\frac{1-p^{-2}}{1-p^{-1}}
=n\prod_{p\mid n}\left(1+\frac1p\right)}.
$$

## 7E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7e/a">a</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/a/i">i</h4>

↑ **Parent:** [A](#7e/a)

<h5 id="7e/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7e/a/i)

If $f$ is [injective](../../../algebra.md#injective-function) and $x\in f^{-1}(f(A))$, then $f(x)=f(a)$ for some $a\in A$, so injectivity gives $x=a\in A$. The reverse inclusion always holds; hence $f^{-1}(f(A))=A$.

Conversely, if (ii) holds and $f(x)=f(y)$, then $y\in f^{-1}(f(\{x\}))=\{x\}$, so $x=y$. Thus (i) and (ii) are equivalent.

<h4 id="7e/a/ii">ii</h4>

↑ **Parent:** [A](#7e/a)

<h5 id="7e/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7e/a/ii)

Assume $f$ is injective. The inclusion $f(A\cap B)\subseteq f(A)\cap f(B)$ holds for every function. If $y$ belongs to the right-hand side, write $y=f(a)=f(b)$ with $a\in A$ and $b\in B$. Injectivity gives $a=b\in A\cap B$, proving equality.

Conversely, suppose (iii) holds and $f(x)=f(y)$. If $x\ne y$, take $A=\{x\}$ and $B=\{y\}$. Then $f(A)\cap f(B)$ is nonempty whereas $f(A\cap B)=f(\varnothing)=\varnothing$, a contradiction. Hence $f$ is injective.

<h4 id="7e/a/iii">iii</h4>

↑ **Parent:** [A](#7e/a)

<h5 id="7e/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7e/a/iii)

Parts (i) and (ii) prove (i)$\Leftrightarrow$(ii), while the two directions in part (ii) prove (i)$\Leftrightarrow$(iii). Therefore all three statements are equivalent.

<h3 id="7e/b">b</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/b/solution">Solution</h4>

↑ **Parent:** [B](#7e/b)

Define

$$
B=\bigcap_{n=0}^{\infty}f^n(X),
\qquad A=X\setminus B.
$$

Certainly $f(B)\subseteq B$. If $y\in B$, then $y\in f(X)$ and has a unique predecessor $x$ because $f$ is injective. For every $n$, writing $y=f^{n+1}(z)$ and using uniqueness gives $x=f^n(z)$; hence $x\in B$ and $y\in f(B)$. Thus $f(B)=B$.

If $f(a)\in B$, its unique predecessor must lie in $B$, so $a\in B$; consequently $f(A)\subseteq A$. If a point belonged to every $f^n(A)$ for $n\geq1$, it would belong to $B$ and also to $f(A)\subseteq A$, which is impossible. Therefore

$$
\boxed{X=A\cup B,\qquad \bigcap_{n=1}^{\infty}f^n(A)=\varnothing,\qquad f(B)=B}.
$$

## 8E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8e/a">a</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/a/solution">Solution</h4>

↑ **Parent:** [A](#8e/a)

A set is [countable](../../../set-theory.md#countable-set) if it is finite or admits an injection into the [natural numbers](../../../arithmetic.md#natural-number); equivalently, its elements can be listed by a finite list or a sequence.

The product of two countable sets is countable: after choosing enumerations, its elements are indexed by pairs $(m,n)\in\mathbb N^2$, and these pairs can be listed diagonally. Thus an injection $X\to A\times B$ followed by an injection $A\times B\to\mathbb N$ proves that $X$ is countable.

The integers are listed as $0,1,-1,2,-2,\ldots$, so $\mathbb Z$ is countable. Every [rational number](../../../number-theory.md#rational-number) is represented by a pair $(p,q)\in\mathbb Z\times\mathbb N_{>0}$, so $\mathbb Q$ is countable as the image of a countable set.

Finally, if $A_0,A_1,\ldots$ are countable, choose listings $A_n=\{a_{n,0},a_{n,1},\ldots\}$, allowing repetitions for finite sets. The diagonal listing of the pairs $(n,m)$ lists every $a_{n,m}$, proving that a [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets) is countable.

<h3 id="8e/b">b</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/b/solution">Solution</h4>

↑ **Parent:** [B](#8e/b)

Fix a positive rational radius $r$. Distinct disjoint circles of radius $r$ have centers more than $2r$ apart, so their open interior disks are pairwise disjoint. Each such disk contains a point of the countable dense set $\mathbb Q^2$. Fix an enumeration of $\mathbb Q^2$ and assign to each disk the first rational point it contains. Disjointness makes this assignment injective, so there are only countably many circles of radius $r$.

The positive rational numbers are countable. Taking the [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets) over all rational radii proves that the whole collection is countable.

<h3 id="8e/c">c</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/c/solution">Solution</h4>

↑ **Parent:** [C](#8e/c)

The conclusion remains true, even though the scaling factor and hence the radius may now be arbitrary. At the point where its handle meets its circle, every lollipop contains a simple triod: take a short arc of the circle in each direction together with a short segment of the handle. Pairwise disjoint lollipops therefore contain pairwise disjoint simple triods. The [Moore triod theorem](../../../topology.md#moore-triod-theorem) says that every such family in the plane is countable, so

$$
\boxed{\text{every pairwise disjoint collection of lollipops in the plane is countable}}.
$$

## 9A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9a/a">a</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/a/solution">Solution</h4>

↑ **Parent:** [A](#9a/a)

The rod imposes a [mechanical constraint](../../../classical-mechanics.md#constraint-mechanics), and its force is perpendicular to the wrecking ball's instantaneous [velocity](../../../classical-mechanics.md#velocity), so it does no [work](../../../classical-mechanics.md#work). In the constant parallel [Newtonian gravitational field](../../../classical-mechanics.md#newtonian-gravitational-field), the ball falls through the vertical distance $l-l\cos\theta_0$. [Conservation of energy](../../../physics.md#conservation-of-energy) between $B$ and $W$ therefore gives

$$
\frac12mv_1^2=mgl(1-\cos\theta_0),
$$

and hence

$$
\boxed{v_1=\sqrt{2gl(1-\cos\theta_0)}}.
$$

<h3 id="9a/b">b</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/b/solution">Solution</h4>

↑ **Parent:** [B](#9a/b)

Let $C$ be the centre of the Earth and let $M$ be its mass. Since $CW=R$ and $CS=R+l$, the [law of cosines](../../../geometry-and-topology.md#law-of-cosines) in triangle $CSB$ gives the ball's initial distance from $C$ as

$$
r_B=CB=\sqrt{(R+l)^2+l^2-2l(R+l)\cos\theta_0}.
$$

The surface value of the [Newtonian gravitational field](../../../classical-mechanics.md#newtonian-gravitational-field) satisfies $g=GM/R^2$. Using the [Newtonian gravitational potential energy](../../../classical-mechanics.md#newtonian-gravitational-potential-energy) $-GMm/r$, [conservation of energy](../../../physics.md#conservation-of-energy) now gives

$$
\frac12mv_2^2=GMm\left(\frac1R-\frac1{r_B}\right).
$$

Therefore

$$
\boxed{v_2=\left[2gR^2\left(\frac1R-\frac1{\sqrt{(R+l)^2+l^2-2l(R+l)\cos\theta_0}}\right)\right]^{1/2}}.
$$

<h3 id="9a/c">c</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/c/solution">Solution</h4>

↑ **Parent:** [C](#9a/c)

Put $\epsilon=l/R$ and $a=1-\cos\theta_0$. Then

$$
\frac{r_B}{R}=\left(1+2a\epsilon+2a\epsilon^2\right)^{1/2}.
$$

The [binomial series](../../../real-analysis.md#binomial-series) gives

$$
\frac{R}{r_B}=1-a\epsilon+\left(\frac32a^2-a\right)\epsilon^2+O(\epsilon^3),
$$

so

$$
v_2^2=2gR\left[a\epsilon+\left(a-\frac32a^2\right)\epsilon^2+O(\epsilon^3)\right].
$$

Since $v_1^2=2gRa\epsilon$, a second [binomial series](../../../real-analysis.md#binomial-series) expansion yields

$$
\frac{v_2}{v_1}=1+\frac12\left(1-\frac32a\right)\epsilon+O(\epsilon^2)
=1+\left(-\frac14+\frac34\cos\theta_0\right)\frac lR+O\!\left(\frac{l^2}{R^2}\right).
$$

Thus the constants in the stated [Big O notation](../../../real-analysis.md#big-o-notation) expansion are

$$
\boxed{A=-\frac14,\qquad B=\frac34}.
$$

## 10A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10a/a">a</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/a/solution">Solution</h4>

↑ **Parent:** [A](#10a/a)

The [Lorentz force](../../../electromagnetism.md#lorentz-force) and [Newton's second law](../../../classical-mechanics.md#newton-s-second-law) give

$$
m\ddot{\mathbf x}=q\dot{\mathbf x}\times\mathbf B.
$$

Writing $\Omega=qB/m$, the component equations are

$$
\ddot x=\Omega\dot y,\qquad \ddot y=-\Omega\dot x,\qquad \ddot z=0.
$$

The initial [velocity](../../../classical-mechanics.md#velocity) therefore gives

$$
\dot x=v\sin(\Omega t),\qquad \dot y=v\cos(\Omega t),\qquad \dot z=v,
$$

and integration with the initial [position](../../../classical-mechanics.md#position) gives

$$
\boxed{\mathbf x(t)=\left(1+\frac v\Omega[1-\cos(\Omega t)],\ \frac v\Omega\sin(\Omega t),\ vt\right)}.
$$

This is [helical motion in a uniform magnetic field](../../../electromagnetism.md#helical-motion-in-a-uniform-magnetic-field): a [helix](../../../topology.md#helix) of radius $v/\Omega$ around the line $x=1+v/\Omega$, $y=0$, with its axis parallel to the [magnetic field](../../../electromagnetism.md#magnetic-field).

<a id="10a/a/image-the-helical-trajectory-of-a-charged-particle-in-a-magnetic-field"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4-magnetic-helix.png)

**[Figure 1](#10a/a/image-the-helical-trajectory-of-a-charged-particle-in-a-magnetic-field). The helical trajectory of a charged particle in a magnetic field**.

<h3 id="10a/b">b</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/b/i">i</h4>

↑ **Parent:** [B](#10a/b)

<h5 id="10a/b/i/solution">Solution</h5>

↑ **Parent:** [I](#10a/b/i)

The three fixed charges are related by rotations through $2\pi/3$ about the origin. Their three [Coulomb's law](../../../electromagnetism.md#coulomb-s-law) forces on a charge placed at the origin have equal magnitudes and directions separated by $2\pi/3$, so their vector sum vanishes. Thus

$$
\boxed{\mathbf r=\mathbf0}
$$

is an equilibrium point.

<h4 id="10a/b/ii">ii</h4>

↑ **Parent:** [B](#10a/b)

<h5 id="10a/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10a/b/ii)

Let $\rho=a/\sqrt3$ be the distance from the origin to each fixed charge, and denote their position vectors by $\mathbf R_j$. For a small planar displacement $\mathbf r$, the [Taylor expansion](../../../calculus.md#taylor-expansion)

$$
\frac1{|\mathbf R_j-\mathbf r|}=\frac1\rho+\frac{\mathbf R_j\cdot\mathbf r}{\rho^3}+\frac{3(\mathbf R_j\cdot\mathbf r)^2-\rho^2|\mathbf r|^2}{2\rho^5}+O(|\mathbf r|^3)
$$

can be summed using the threefold [symmetry](../../../physics.md#symmetry-physics) relations

$$
\sum_j\mathbf R_j=0,
\qquad
\sum_j\mathbf R_j\mathbf R_j^{\mathsf T}=\frac{3\rho^2}{2}I.
$$

The [electric potential](../../../electromagnetism.md#electric-potential) due to the fixed charges is consequently

$$
\Phi(\mathbf r)=\frac{q}{4\pi\epsilon_0}\left(\frac3\rho+\frac{3|\mathbf r|^2}{4\rho^3}+O(|\mathbf r|^3)\right).
$$

The moving charge has [electrostatic potential energy of point charges](../../../electromagnetism.md#electrostatic-potential-energy-of-point-charges) $U=q\Phi$. Because the quadratic coefficient is positive, the origin is a strict [local minimum](../../../analysis.md#local-minimum) of $U$, and the equilibrium is stable.

<h4 id="10a/b/iii">iii</h4>

↑ **Parent:** [B](#10a/b)

<h5 id="10a/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#10a/b/iii)

Taking the [gradient](../../../calculus.md#gradient) of the quadratic [potential energy](../../../classical-mechanics.md#potential-energy) found in part (ii) resolves the linearized force into identical $x$ and $y$ components:

$$
F_x=-\frac{3q^2}{8\pi\epsilon_0\rho^3}x,
\qquad
F_y=-\frac{3q^2}{8\pi\epsilon_0\rho^3}y.
$$

Each component therefore performs [simple harmonic motion](../../../classical-mechanics.md#simple-harmonic-motion) with

$$
\omega^2=\frac{3q^2}{8\pi\epsilon_0m\rho^3}
=\frac{9\sqrt3}{8\pi}\frac{q^2}{m\epsilon_0a^3}.
$$

Thus the [angular frequency](../../../classical-mechanics.md#angular-frequency) is

$$
\boxed{\omega=\frac{3^{5/4}}{\sqrt{8\pi}}\frac{|q|}{\sqrt{m\epsilon_0a^3}},
\qquad A=\frac{3^{5/4}}{\sqrt{8\pi}}}.
$$

## 11A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11a/a">a</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/a/i">i</h4>

↑ **Parent:** [A](#11a/a)

<h5 id="11a/a/i/solution">Solution</h5>

↑ **Parent:** [I](#11a/a/i)

By [Newton's second law](../../../classical-mechanics.md#newton-s-second-law), [force](../../../classical-mechanics.md#force) is mass times [acceleration](../../../classical-mechanics.md#acceleration). Hence its dimensions are

$$
\boxed{[F]=MLT^{-2}}.
$$

<h4 id="11a/a/ii">ii</h4>

↑ **Parent:** [A](#11a/a)

<h5 id="11a/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#11a/a/ii)

The [electric field](../../../electromagnetism.md#electric-field) is force per unit [electric charge](../../../electromagnetism.md#electric-charge), so

$$
\boxed{[E]=MLT^{-2}Q^{-1}}.
$$

<h3 id="11a/b">b</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/b/solution">Solution</h4>

↑ **Parent:** [B](#11a/b)

Write $E=|\mathbf E|$ and $\widehat{\mathbf E}=\mathbf E/E$. The constant electric [force](../../../classical-mechanics.md#force) gives [momentum](../../../classical-mechanics.md#momentum)

$$
\mathbf p(t)=q\mathbf E t.
$$

Combining $\mathbf p=\gamma m\dot{\mathbf x}$ with the [relativistic energy-momentum relation](../../../special-relativity.md#energy-momentum-relation) gives

$$
\boxed{\dot{\mathbf x}(t)=\frac{q\mathbf E t/m}{\sqrt{1+(qEt/mc)^2}}}.
$$

The [dimensional analysis](../../../physics.md#dimensional-analysis) from part (a) confirms that $qEt$ has the dimensions of [momentum](../../../classical-mechanics.md#momentum), so $qEt/(mc)$ is dimensionless and the expression has the dimensions of [velocity](../../../classical-mechanics.md#velocity).

The [speed](../../../classical-mechanics.md#speed) increases monotonically from zero and approaches the [speed of light](../../../special-relativity.md#speed-of-light) asymptotically:

$$
\lim_{t\to\infty}|\dot{\mathbf x}(t)|=c.
$$

Integrating in the direction of the field gives

$$
\boxed{\mathbf x(t)=\frac{mc^2}{qE}\left[\sqrt{1+\left(\frac{qEt}{mc}\right)^2}-1\right]\widehat{\mathbf E}}.
$$

At small times, the [Taylor expansion](../../../calculus.md#taylor-expansion) of the square root gives the [nonrelativistic limit](../../../special-relativity.md#nonrelativistic-limit)

$$
\mathbf x(t)=\frac{q\mathbf E}{2m}t^2+O(t^4),
$$

which is motion from rest with the constant [acceleration](../../../classical-mechanics.md#acceleration) $q\mathbf E/m$.

<h3 id="11a/c">c</h3>

↑ **Parent:** [11A](#11a)

<h4 id="11a/c/solution">Solution</h4>

↑ **Parent:** [C](#11a/c)

At time $t_0$, the accelerated [proton](../../../physics.md#proton) has [momentum](../../../classical-mechanics.md#momentum) $p=qEt_0$ and, by the [relativistic energy-momentum relation](../../../special-relativity.md#energy-momentum-relation), energy

$$
\mathcal E_p=\sqrt{m^2c^4+q^2E^2t_0^2c^2}.
$$

The incident [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) [photon](../../../quantum-mechanics.md#photon) adds energy $E_\gamma$. Since the final state contains only the [Delta-plus baryon](../../../physics.md#delta-plus-baryon), [conservation of relativistic energy](../../../special-relativity.md#conservation-of-relativistic-energy) gives its laboratory-frame [Lorentz factor](../../../special-relativity.md#lorentz-factor)

$$
\gamma_\Delta=\frac{\mathcal E_p+E_\gamma}{m_\Delta c^2}.
$$

Its rest-frame decay time $t_\Delta$ is a [proper time](../../../special-relativity.md#proper-time), so [time dilation](../../../special-relativity.md#time-dilation) gives the laboratory decay time

$$
\boxed{t_{\rm lab}=\frac{t_\Delta}{m_\Delta c^2}\left(\sqrt{m^2c^4+q^2E^2t_0^2c^2}+E_\gamma\right)}.
$$

## 12A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12a/a">a</h3>

↑ **Parent:** [12A](#12a)

<h4 id="12a/a/solution">Solution</h4>

↑ **Parent:** [A](#12a/a)

Let $\{\mathbf e_i(t)\}$ be an orthonormal [basis](../../../vector-space.md#basis) fixed in $S'$ and write $\mathbf a=a_i\mathbf e_i$. A basis vector rotating with [angular velocity](../../../classical-mechanics.md#angular-velocity) $\boldsymbol\omega$ satisfies

$$
\left(\dot{\mathbf e}_i\right)_S=\boldsymbol\omega\times\mathbf e_i.
$$

Differentiating the components and the basis vectors in $S$ therefore gives the [rotating-frame derivative formula](../../../physics.md#rotating-frame-derivative-formula)

$$
\boxed{(\dot{\mathbf a})_S
=\dot a_i\mathbf e_i+a_i\boldsymbol\omega\times\mathbf e_i
=(\dot{\mathbf a})_{S'}+\boldsymbol\omega\times\mathbf a.}
$$

<h3 id="12a/b">b</h3>

↑ **Parent:** [12A](#12a)

<h4 id="12a/b/solution">Solution</h4>

↑ **Parent:** [B](#12a/b)

Apply part (a) first to the [position](../../../classical-mechanics.md#position) $\mathbf r$:

$$
(\dot{\mathbf r})_S=(\dot{\mathbf r})_{S'}+\boldsymbol\omega\times\mathbf r.
$$

Applying it again to both terms on the right gives

$$
(\ddot{\mathbf r})_S=(\ddot{\mathbf r})_{S'}+\boldsymbol\omega\times(\dot{\mathbf r})_{S'}+(\dot{\boldsymbol\omega})_{S'}\times\mathbf r+\boldsymbol\omega\times(\dot{\mathbf r})_S,
$$

where $(\dot{\boldsymbol\omega})_S=(\dot{\boldsymbol\omega})_{S'}$ because $\boldsymbol\omega\times\boldsymbol\omega=0$. Substituting the first formula into the last term produces

$$
\boxed{(\ddot{\mathbf r})_S=(\ddot{\mathbf r})_{S'}+2\boldsymbol\omega\times(\dot{\mathbf r})_{S'}+(\dot{\boldsymbol\omega})_{S'}\times\mathbf r+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf r)}.
$$

In the Earth-fixed [rotating reference frame](../../../physics.md#rotating-reference-frame), the sideways apparent force is the [Coriolis acceleration](../../../physics.md#coriolis-acceleration) multiplied by the ski-doo's [mass](../../../classical-mechanics.md#mass):

$$
\mathbf F_{\rm side}=-2m\boldsymbol\omega\times\mathbf v.
$$

At the South Pole, $\boldsymbol\omega$ is vertical and antiparallel to the local outward normal, while $\mathbf v$ is horizontal, so

$$
\boxed{|\mathbf F_{\rm side}|=2m\omega v}.
$$

The force points to the left of the direction of travel, which is westward when the ski-doo is moving north after crossing the pole.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
