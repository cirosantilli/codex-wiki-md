# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperia_4_2018.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2018/paperia_4_2018.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3A](#3a)
  - [a](#3a/a)
    - [Solution](#3a/a/solution)
  - [b](#3a/b)
    - [Solution](#3a/b/solution)
  - [c](#3a/c)
    - [Solution](#3a/c/solution)
  - [d](#3a/d)
    - [Solution](#3a/d/solution)
  - [e](#3a/e)
    - [i](#3a/e/i)
      - [Solution](#3a/e/i/solution)
    - [ii](#3a/e/ii)
      - [Solution](#3a/e/ii/solution)
- [4A](#4a)
  - [Solution](#4a/solution)
- [5E](#5e)
  - [Solution](#5e/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7E](#7e)
  - [Solution](#7e/solution)
- [8E](#8e)
  - [Solution](#8e/solution)
- [9A](#9a)
  - [a](#9a/a)
    - [Solution](#9a/a/solution)
  - [b](#9a/b)
    - [Solution](#9a/b/solution)
- [10A](#10a)
  - [a](#10a/a)
    - [Solution](#10a/a/solution)
  - [b](#10a/b)
    - [Solution](#10a/b/solution)
  - [c](#10a/c)
    - [Solution](#10a/c/solution)
- [11A](#11a)
  - [Solution](#11a/solution)
- [12A](#12a)
  - [Solution](#12a/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

[Fermat's little theorem](../../../number-theory.md#fermat-little-theorem) states that if $p$ is prime, then $a^p\equiv a\pmod p$ for every integer $a$; equivalently, $a^{p-1}\equiv1\pmod p$ when $p\nmid a$.

If $p\equiv3\pmod4$ and $x^2\equiv-1\pmod p$, then

$$
x^{p-1}=(x^2)^{(p-1)/2}\equiv(-1)^{(p-1)/2}=-1\pmod p,
$$

because $(p-1)/2$ is odd. This contradicts Fermat's theorem, so **$x^2\equiv-1\pmod p$ has no solution**.

If the primes congruent to $1\pmod4$ were $p_1,\ldots,p_k$, set $N=(2p_1\cdots p_k)^2+1$. Any prime divisor $q$ of $N$ is odd and has $-1$ as a [quadratic residue](../../../number-theory.md#quadratic-residue). The preceding result forces $q\equiv1\pmod4$, but $q$ divides none of the $p_i$ because $N\equiv1\pmod{p_i}$. This contradiction proves that **infinitely many primes are congruent to $1\pmod4$**.

## 2E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

Suppose $\sqrt n=a/b$ in lowest terms. Then $a^2=nb^2$. Comparing prime exponents shows that every prime dividing $b$ also divides $a$, unless $b=1$. Hence $\sqrt n=a$ is an integer. Therefore **$\sqrt n$ is either an integer or irrational**.

Only $\alpha+q$ must be irrational: if it were rational, subtracting rational $q$ would make $\alpha$ rational. None of the others must be irrational:

$$
\sqrt2+(-\sqrt2)=0,\qquad
\sqrt2\,\sqrt2=2,\qquad
(\sqrt2)^2=2.
$$

For $\alpha^\beta$, let $r=(\sqrt2)^{\sqrt2}$. If $r$ is rational, $\alpha=\beta=\sqrt2$ is a counterexample. If $r$ is irrational, take $\alpha=r$ and $\beta=\sqrt2$; then $\alpha^\beta=2$. Thus **$\alpha+q$ is the sole expression forced to be irrational**.

## 3A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3a/a">a</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/a/solution">Solution</h4>

↑ **Parent:** [A](#3a/a)

An [inertial frame](../../../physics.md#inertial-frame) is a reference frame in which a force-free particle moves with constant velocity, so [Newton's first law](../../../classical-mechanics.md#newton-s-first-law) holds.

<h3 id="3a/b">b</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/b/solution">Solution</h4>

↑ **Parent:** [B](#3a/b)

The basic [Galilean transformations](../../../special-relativity.md#galilean-transformation) include spacetime translations $\mathbf x'=\mathbf x-\mathbf a$, $t'=t-b$; spatial rotations $\mathbf x'=R\mathbf x$, $t'=t$; and boosts $\mathbf x'=\mathbf x-\mathbf vt$, $t'=t$, where $R$ is a [rotation matrix](../../../linear-algebra.md#rotation-matrix) and $\mathbf v$ is constant.

<h3 id="3a/c">c</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/c/solution">Solution</h4>

↑ **Parent:** [C](#3a/c)

The [Principle of Galilean relativity](../../../special-relativity.md#principle-of-galilean-relativity) states that the laws of mechanics have the same form in every inertial frame.

<h3 id="3a/d">d</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/d/solution">Solution</h4>

↑ **Parent:** [D](#3a/d)

The equation of motion is

$$
m\ddot x=-V'(x).
$$

Multiplication by $\dot x$ gives

$$
\frac d{dt}\left(\frac12m\dot x^2+V(x)\right)=\dot x(m\ddot x+V'(x))=0,
$$

so the [mechanical energy](../../../classical-mechanics.md#mechanical-energy) $E=\frac12m\dot x^2+V(x)$ is conserved. On a segment where the direction of motion is fixed,

$$
\boxed{t-t_0=\pm\sqrt{\frac m2}\int_{x_0}^{x}\frac{du}{\sqrt{E-V(u)}}.}
$$

<h3 id="3a/e">e</h3>

↑ **Parent:** [3A](#3a)

<h4 id="3a/e/i">i</h4>

↑ **Parent:** [E](#3a/e)

<h5 id="3a/e/i/solution">Solution</h5>

↑ **Parent:** [I](#3a/e/i)

For $V=(x^2-4)^2$, $V'=4x(x^2-4)$. Thus **$x=\pm2$ are stable equilibria** at the two potential minima, while **$x=0$ is unstable** at the local maximum.

<h4 id="3a/e/ii">ii</h4>

↑ **Parent:** [E](#3a/e)

<h5 id="3a/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3a/e/ii)

For $x\ne0$, $V'(x)=2x^{-3}e^{-1/x^2}$ never vanishes. At $x=0$, the smooth flat extension has $V'(0)=0$, and $V(x)>V(0)=0$ for every $x\ne0$. Hence **$x=0$ is the unique equilibrium and is stable**.

## 4A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4a/solution">Solution</h3>

↑ **Parent:** [4A](#4a)

A [central force](../../../physics.md#central-force) has the form $\mathbf F=f(r)\widehat{\mathbf r}$, so it always points along the line from a fixed centre to the particle. Its torque about the centre vanishes:

$$
\frac{d\mathbf L}{dt}=\mathbf r\times\mathbf F=0,
\qquad
\mathbf L=m\mathbf r\times\dot{\mathbf r}.
$$

Thus [angular momentum](../../../classical-mechanics.md#angular-momentum) is conserved. Since $\mathbf r\cdot\mathbf L=0$, the trajectory lies in the fixed plane through the origin perpendicular to $\mathbf L$.

The area swept in time $dt$ is $dA=\frac12|\mathbf r\times d\mathbf r|$, so

$$
\boxed{\frac{dA}{dt}=\frac12|\mathbf r\times\dot{\mathbf r}|=\frac{|\mathbf L|}{2m},}
$$

which is constant. This proves [Kepler's second law](../../../physics.md#kepler-s-second-law).

## 5E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5e/solution">Solution</h3>

↑ **Parent:** [5E](#5e)

[Bezout identity](../../../algebra.md#bezout-identity) gives integers $b,c$ with $ab+nc=1$ whenever $\gcd(a,n)=1$, so $ab\equiv1\pmod n$. If $b,b'$ are inverses, multiplying $a(b-b')\equiv0$ by an inverse gives $b\equiv b'\pmod n$. Multiplying Bezout identities for $a$ and $b$ shows that $\gcd(ab,n)=1$.

[Wilson theorem](../../../number-theory.md#wilson-s-theorem) states that $(p-1)!\equiv-1\pmod p$ for prime $p$. Pair the nonzero residues with their unique multiplicative inverses. The only self-inverse residues are $1,-1$, whose product is $-1$, proving the theorem.

Counting one factor of $p$ for every multiple of $p$, another for every multiple of $p^2$, and so on proves [Legendre formula](../../../number-theory.md#legendre-s-formula)

$$
\boxed{v_p(n!)=\sum_{i\geq1}\left\lfloor\frac n{p^i}\right\rfloor.}
$$

Now $22!\equiv20!\cdot21\cdot22\equiv2(20!)\equiv-1\pmod{23}$, so **$20!\equiv11\pmod{23}$**. Also $v_5(1000!)=200+40+8+1=249$, while $v_2(1000!)>249$, so **$1000!\equiv0\pmod{10^{249}}$**.

Finally,

$$
\binom{p^m}{k}=\frac{p^m}{k}\binom{p^m-1}{k-1}.
$$

For $1\leq j<p^m$, $v_p(p^m-j)=v_p(j)$, so the second factor is a $p$-adic unit. If $v_p(k)=\ell$, then

$$
\boxed{v_p\binom{p^m}{k}=m-\ell.}
$$

## 6E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

The [Hamming distance](../../../coding-theory.md#hamming-distance) satisfies the triangle inequality coordinate by coordinate: if $x_i\ne z_i$, then $x_i\ne y_i$ or $y_i\ne z_i$. Summing these indicator inequalities proves the claim. A word at distance exactly $i$ from $x$ is obtained by choosing the $i$ coordinates to flip, so

$$
\boxed{|B(x,j)|=\sum_{i=0}^j\binom ni.}
$$

For a $k$-code, radius-$k$ balls about codewords are disjoint, giving $|C|\sum_{i=0}^k\binom ni\leq2^n$. Conversely, take a maximal code of minimum distance $2k+1$. Its radius-$2k$ balls cover $Q_n$, since an uncovered word could otherwise be added, so $2^n\leq|C|\sum_{i=0}^{2k}\binom ni$. Maximizing gives the requested coding bounds.

For $(n,k)=(4,1)$, translate a codeword to $0000$. Every other word has weight at least three, but any two distinct length-four words of weight at least three have distance at most two. Thus at most one can accompany $0000$, while $\{0000,1111\}$ works. Hence **$M(4,1)=2$**.

## 7E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7e/solution">Solution</h3>

↑ **Parent:** [7E](#7e)

Let $M=\{i:x\in A_i\}$, with $|M|=m$. Then $\mathbf1_{A_S}(x)=1$ exactly when $S\subseteq M$, and the sum becomes

$$
\sum_{s=t}^{m}\binom ms\binom st(-1)^{s-t}
=\binom mt\sum_{r=0}^{m-t}\binom{m-t}{r}(-1)^r
=\binom mt(1-1)^{m-t}.
$$

This is $1$ when $m=t$ and $0$ otherwise. Summing over $x\in X$ yields

$$
\boxed{\#\{x:x\text{ belongs to exactly }t\text{ sets}\}
=\sum_S\binom{|S|}{t}(-1)^{|S|-t}|A_S|.}
$$

Taking the complement of the $t=0$ case gives the [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle)

$$
\left|\bigcup_iA_i\right|=\sum_{\varnothing\ne S}(-1)^{|S|+1}|A_S|.
$$

If $p_1,\ldots,p_r$ are the distinct prime divisors of $N$, inclusion-exclusion removes their multiples from $\{1,\ldots,N\}$ and gives

$$
\boxed{\varphi(N)=N\prod_{p\mid N}\left(1-\frac1p\right).}
$$

For the stated squarefree $n=q_1\cdots q_k$ and $\gcd(x,n)=1$, Fermat's theorem gives $x^{q_j-1}\equiv1\pmod{q_j}$. Since $q_j-1\mid n-1$, every $q_j$ divides $x^{n-1}-1$; their product does too. Thus **$n$ is a Carmichael number**.

## 8E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8e/solution">Solution</h3>

↑ **Parent:** [8E](#8e)

A set is [countable](../../../set-theory.md#countable-set) if it is finite or bijects with a subset of $\mathbb N$. For any $f:X\to\mathcal P(X)$, the [Cantor diagonal argument](../../../set-theory.md#cantor-diagonal-argument) set $D=\{x:x\notin f(x)\}$ differs from every $f(y)$ at $y$. Hence no such map is surjective. Binary sequences are indicator functions of subsets of $\mathbb N$, so $\{0,1\}^{\mathbb N}\cong\mathcal P(\mathbb N)$ is uncountable.

Every member of $L$ corresponds to a unique permutation $(a_0,a_1,\ldots)$ of $\mathbb N$, with $F_n=\{a_0,\ldots,a_{n-1}\}$. Let $p(j)$ be the position of $j$.

For $L_0$, $p(n)<n$ eventually. Choose $N$ after which this holds and then $m$ larger than all $p(0),\ldots,p(N-1)$. The $m$ positions $0,\ldots,m-1$ would contain all $m+1$ values $0,\ldots,m$, a contradiction. Thus **$L_0$ is empty**, hence countable.

For $L_1$, $p(n)\leq n$ eventually. For every sufficiently large $m$, all values $0,\ldots,m$ occur in positions $0,\ldots,m$, so this initial segment is invariant. Comparing consecutive invariant initial segments gives $p(m)=m$ eventually. These are the finite-support permutations, of which there are countably many. Hence **$L_1$ is countable**.

## 9A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9a/a">a</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/a/solution">Solution</h4>

↑ **Parent:** [A](#9a/a)

For rolling without slipping, $\dot s=a\Omega$. [Conservation of energy](../../../physics.md#conservation-of-energy) gives

$$
Mg\,s\sin\alpha=\frac12M\dot s^2+\frac12I\frac{\dot s^2}{a^2},
$$

and differentiation yields

$$
\boxed{\ddot s=\frac{g\sin\alpha}{1+I/(Ma^2)}.}
$$

For a sphere with density proportional to $r^c$,

$$
M=4\pi\rho_0\frac{a^{c+3}}{c+3},\qquad
I=\frac{8\pi\rho_0}{3}\frac{a^{c+5}}{c+5},
$$

so $I/(Ma^2)=2(c+3)/(3(c+5))$. A uniform disc has $I/(Ma^2)=1/2$. Equal launch speeds give equal return times exactly when the accelerations, and hence these ratios, agree. Solving gives **$c=3$**.

<h3 id="9a/b">b</h3>

↑ **Parent:** [9A](#9a)

<h4 id="9a/b/solution">Solution</h4>

↑ **Parent:** [B](#9a/b)

Let $M$ be the mass of a complete uniform sphere of radius $a$. The intact marble has $I_1=2Ma^2/5$. Each removed bubble has mass $M/8$, radius $a/2$, and centre a distance $a/2$ from the rolling axis. By the [parallel axis theorem](../../../classical-mechanics.md#parallel-axis-theorem), each removes

$$
\frac25\frac M8\left(\frac a2\right)^2+\frac M8\left(\frac a2\right)^2
=\frac{7}{160}Ma^2.
$$

Thus $M_2=3M/4$, $I_2=2Ma^2/5-7Ma^2/80=5Ma^2/16$, and $I_2/(M_2a^2)=5/12$. The two accelerations are therefore $(5/7)g\sin\alpha$ and $(12/17)g\sin\alpha$. From rest, distance is proportional to acceleration, so

$$
\boxed{\frac{s_1(t)}{s_2(t)}=\frac{85}{84}.}
$$

## 10A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10a/a">a</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/a/solution">Solution</h4>

↑ **Parent:** [A](#10a/a)

The [four-momentum](../../../special-relativity.md#four-momentum) is

$$
P=(P^0,\mathbf P)=(\gamma mc,\gamma m\mathbf u),
\qquad
\gamma=(1-|\mathbf u|^2/c^2)^{-1/2}.
$$

Thus

$$
P^0=mc+\frac{m|\mathbf u|^2}{2c}+\frac{3m|\mathbf u|^4}{8c^3}+O(|\mathbf u|^6/c^5).
$$

Multiplication by $c$ identifies the first two terms as the [rest energy](../../../special-relativity.md#rest-energy) $mc^2$ and the Newtonian [kinetic energy](../../../classical-mechanics.md#kinetic-energy) $m|\mathbf u|^2/2$.

For the fixed-target reaction, the initial invariant is

$$
(P_1+P_2)^2=2m^2c^2(1+\gamma).
$$

At threshold the four final particles are at rest in their centre-of-momentum frame, giving invariant $(4mc)^2$. Hence $\gamma=7$ and the least laboratory speed is

$$
\boxed{u=c\sqrt{1-\frac1{49}}=\frac{4\sqrt3}{7}c.}
$$

<h3 id="10a/b">b</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/b/solution">Solution</h4>

↑ **Parent:** [B](#10a/b)

[Four-momentum conservation](../../../special-relativity.md#four-momentum-conservation) gives $P=\sum_iQ_i$, while the [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) gives $P\cdot P=M^2c^2$. Therefore

$$
\boxed{M=\frac1c\sqrt{\left(\sum_iQ_i\right)\cdot\left(\sum_jQ_j\right)}.}
$$

In the parent rest frame, $Mc^2=\sum_iE_i$, and each relativistic energy obeys $E_i\geq m_ic^2$. Thus

$$
\boxed{M\geq\sum_{i=1}^Nm_i.}
$$

<h3 id="10a/c">c</h3>

↑ **Parent:** [10A](#10a)

<h4 id="10a/c/solution">Solution</h4>

↑ **Parent:** [C](#10a/c)

Work in the rest frame of $B$. Two-body decay kinematics gives the massless-particle energies

$$
E_1=\frac{(m_A^2-m_B^2)c^2}{2m_B},
\qquad
E_2=\frac{(m_B^2-m_C^2)c^2}{2m_B}.
$$

If $\theta$ is the angle between their momenta, then

$$
(Q_1+Q_2)^2=2Q_1\cdot Q_2
=\frac{2E_1E_2}{c^2}(1-\cos\theta).
$$

Since $0\leq1-\cos\theta\leq2$,

$$
\boxed{0\leq(Q_1+Q_2)^2\leq
\frac{(m_A^2-m_B^2)(m_B^2-m_C^2)c^2}{m_B^2}.}
$$

## 11A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11a/solution">Solution</h3>

↑ **Parent:** [11A](#11a)

The [Lorentz force law](../../../electromagnetism.md#lorentz-force) is $\mathbf F=q(\mathbf E+\mathbf v\times\mathbf B)$. Before impact the acceleration toward the wall is $a=qE/m$, so the first-impact speed is **$v_0=\sqrt{2qEh/m}$**.

After the $n$th bounce, the outward speed is $\gamma^nv_0$, so the outward height is $\gamma^{2n}h$ and that excursion contributes twice this distance. Hence

$$
L=h+2h\sum_{n\geq1}\gamma^{2n}
=\boxed{h\frac{1+\gamma^2}{1-\gamma^2}},
$$

so $q_1(\gamma)=1+\gamma^2$ and $q_2(\gamma)=1-\gamma^2$.

With quadratic drag, put $w=-\dot z\geq0$. Then

$$
m\dot w=qE-\alpha w^2,\qquad w(0)=0,
$$

whose solution is $w=\sqrt{qE/\alpha}\tanh(\sqrt{\alpha qE}\,t/m)$. Integration gives

$$
\boxed{z(t)=h-\frac m\alpha\log\cosh\left(\frac{\sqrt{\alpha qE}}m\,t\right).}
$$

Thus $A=m/\alpha$, $B=\sqrt{\alpha qE}/m$, and $f(s)=\log\cosh s$.

## 12A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12a/solution">Solution</h3>

↑ **Parent:** [12A](#12a)

For constant angular velocity, the [equation of motion in a rotating frame](../../../classical-mechanics.md#equation-of-motion-in-a-rotating-frame) is

$$
m\left(\ddot{\mathbf x}+2\boldsymbol\omega\times\dot{\mathbf x}
+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x)\right)
=-9m|\boldsymbol\omega|^2\mathbf x.
$$

For $\boldsymbol\omega=(0,0,\omega)$ and $\xi=x+iy$, the planar equations combine to

$$
\ddot\xi+2i\omega\dot\xi+8\omega^2\xi=0.
$$

The initial conditions give

$$
\boxed{\xi(t)=\frac23e^{2i\omega t}+\frac13e^{-4i\omega t},\qquad z(t)=0.}
$$

Therefore

$$
|\dot{\mathbf x}|=|\dot\xi|
=\frac{8|\omega|}{3}|\sin(3\omega t)|.
$$

The maximum speed and, for $\omega>0$, its times are

$$
\boxed{v_{\max}=\frac{8\omega}{3},\qquad
t=\frac{(2k+1)\pi}{6\omega}\quad(k=0,1,2,\ldots).}
$$

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
