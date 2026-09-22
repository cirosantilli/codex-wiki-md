# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperia_4_2023.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperia_4_2023.pdf)

**Table of contents**

- [1F](#1f)
  - [a](#1f/a)
    - [Solution](#1f/a/solution)
  - [b](#1f/b)
    - [Solution](#1f/b/solution)
- [2E](#2e)
  - [Solution](#2e/solution)
- [3C](#3c)
  - [Solution](#3c/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5F](#5f)
  - [a](#5f/a)
    - [Solution](#5f/a/solution)
  - [b](#5f/b)
    - [Solution](#5f/b/solution)
  - [c](#5f/c)
    - [Solution](#5f/c/solution)
  - [d](#5f/d)
    - [i](#5f/d/i)
      - [Solution](#5f/d/i/solution)
    - [ii](#5f/d/ii)
      - [Solution](#5f/d/ii/solution)
- [6E](#6e)
  - [Solution](#6e/solution)
- [7D](#7d)
  - [a](#7d/a)
    - [Solution](#7d/a/solution)
  - [b](#7d/b)
    - [Solution](#7d/b/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
  - [i](#8d/i)
    - [Solution](#8d/i/solution)
  - [ii](#8d/ii)
    - [Solution](#8d/ii/solution)
  - [iii](#8d/iii)
    - [Solution](#8d/iii/solution)
- [9C](#9c)
  - [Solution](#9c/solution)
- [10C](#10c)
  - [a](#10c/a)
    - [Solution](#10c/a/solution)
  - [b](#10c/b)
    - [Solution](#10c/b/solution)
- [11C](#11c)
  - [Solution](#11c/solution)
- [12C](#12c)
  - [a](#12c/a)
    - [Solution](#12c/a/solution)
  - [b](#12c/b)
    - [Solution](#12c/b/solution)

## 1F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1f/a">a</h3>

↑ **Parent:** [1F](#1f)

<h4 id="1f/a/solution">Solution</h4>

↑ **Parent:** [A](#1f/a)

Define

$$
\tau(\sigma)(j)=n+1-\sigma(j).
$$

This is an involution on permutations. Every inequality is reversed, so it maps up-down permutations bijectively to down-up permutations.

<h3 id="1f/b">b</h3>

↑ **Parent:** [1F](#1f)

<h4 id="1f/b/solution">Solution</h4>

↑ **Parent:** [B](#1f/b)

By part (a), there are $A_{n+1}$ permutations of each alternating type. In an up-down permutation the maximum $n+1$ can occur only at a peak, while in a down-up permutation it can occur only at the complementary positions. Thus, after combining the two types, each possible number $k$ of entries to the left of the maximum occurs once.

Choose those $k$ labels in $\binom nk$ ways. The entries on the two sides must independently alternate, and after order-preserving relabelling can be chosen in $A_k$ and $A_{n-k}$ ways. This [alternating-permutation convolution](../../../combinatorics.md#alternating-permutation-convolution) is

$$
\boxed{2A_{n+1}=\sum_{k=0}^n\binom nkA_kA_{n-k}.}
$$

## 2E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2e/solution">Solution</h3>

↑ **Parent:** [2E](#2e)

The [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) says that for pairwise coprime positive integers $m_i$, the map

$$
\mathbb Z/(m_1\cdots m_r)\mathbb Z
\longrightarrow\prod_i\mathbb Z/m_i\mathbb Z
$$

is a bijection. For two [moduli](../../../complex-analysis.md#modulus), choose $u,v$ with $um+vn=1$; then

$$
x=b,um+a,vn
$$

has residues $a$ modulo $m$ and $b$ modulo $n$. Uniqueness follows because the difference of two solutions is divisible by both coprime [moduli](../../../complex-analysis.md#modulus), hence by their product. Induction proves the general case.

The two given congruences are compatible modulo $\gcd(6,8)=2$, and checking modulo $\operatorname{lcm}(6,8)=24$ gives

$$
x\equiv10\pmod{24}.
$$

Write $d=2^r3^sm$ with $(m,6)=1$. Use the Chinese remainder theorem to choose

$$
a\equiv0\pmod{2^r},\qquad 2a\equiv1\pmod{3^sm},
$$



$$
3b\equiv1\pmod{2^r},\qquad b\equiv0\pmod{3^sm}.
$$

Then $4a^2+9b^2\equiv1$ modulo each of the pairwise coprime factors $2^r$, $3^s$, and $m$, hence modulo $d$.

## 3C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3c/solution">Solution</h3>

↑ **Parent:** [3C](#3c)

During a short time $dt$, the rocket loses mass $-dm>0$. Conservation of upward [momentum](../../../classical-mechanics.md#momentum), including gravity's impulse and exhaust [velocity](../../../classical-mechanics.md#velocity) $v-U$, gives to first order

$$
m\,dv+U\,dm=-mg\,dt,
$$

which is the stated rocket equation.

Here $dm/dt=-\alpha$ and $U=U_0m_0/m$, so

$$
\frac{dv}{dt}=\frac{\alpha U_0m_0}{(m_0-\alpha t)^2}-g.
$$

Lift-off from rest requires positive initial [acceleration](../../../classical-mechanics.md#acceleration),

$$
\frac{\alpha U_0}{m_0}>g.
$$

With $v(0)=0$, integration gives

$$
v(t)=U_0\left(\frac{m_0}{m_0-\alpha t}-1\right)-gt.
$$

The dimensions are $[m_0]=[m]=M$, $[\alpha]=M/T$, $[U_0]=[U]=[v]=L/T$, $[g]=L/T^2$, and $[t]=T$. Both displayed terms in $v$ therefore have dimension $L/T$.

## 4C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

With $\gamma(v)=(1-v^2/c^2)^{-1/2}$,

$$
x'=\gamma(x-vt),
\qquad
t'=\gamma\left(t-\frac{vx}{c^2}\right).
$$

Adding and subtracting $ct'$ gives

$$
x'_+=\gamma(1-v/c)x_+
=\sqrt{\frac{c-v}{c+v}},x_+,
$$



$$
x'_- =\gamma(1+v/c)x_-
=\sqrt{\frac{c+v}{c-v}},x_-.
$$

The product of the two multipliers is one, so $x'_+x'_-=x_+x_-$, which is $x'^2-c^2t'^2=x^2-c^2t^2$.

Successive transformations multiply the $x_+$ factors. Equating

$$
\lambda(v_3)=\lambda(v_2)\lambda(v_1)
$$

and solving gives the relativistic velocity-addition law

$$
\boxed{v_3=\frac{v_1+v_2}{1+v_1v_2/c^2}.}
$$

## 5F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5f/a">a</h3>

↑ **Parent:** [5F](#5f)

<h4 id="5f/a/solution">Solution</h4>

↑ **Parent:** [A](#5f/a)

The recurrence and the addition formula give the result by induction. It is true for $n=0,1$, and if true for $n,n-1$, then

$$
\boxed{T_{n+1}(\cos y)=2\cos y\cos(ny)-\cos((n-1)y)=\cos((n+1)y).}
$$

<h3 id="5f/b">b</h3>

↑ **Parent:** [5F](#5f)

<h4 id="5f/b/solution">Solution</h4>

↑ **Parent:** [B](#5f/b)

The recurrence shows that $T_n$ is a [polynomial](../../../polynomial.md) with integer coefficients. Part (a) gives

$$
T_n(\cos(\pi/n))+1=\cos\pi+1=0.
$$

**Thus $\cos(\pi/n)$ is a root of a nonzero integer [polynomial](../../../polynomial.md) and is algebraic.**

<h3 id="5f/c">c</h3>

↑ **Parent:** [5F](#5f)

<h4 id="5f/c/solution">Solution</h4>

↑ **Parent:** [C](#5f/c)

Put $z=2\cos(\pi/n)$. The recurrence

$$
S_0(z)=2,\quad S_1(z)=z,\quad S_{k+1}(z)=zS_k(z)-S_{k-1}(z)
$$

defines monic integer [polynomials](../../../polynomial.md) and gives $S_k(z)=2\cos(k\pi/n)$. Hence $z$ is an algebraic integer. If $\cos(\pi/n)$ is rational, then the rational algebraic integer $z$ is an integer. Since $-2\leq z<2$, this leaves the values corresponding to

$$
n=1:\cos\pi=-1,\qquad n=2:\cos(\pi/2)=0,\qquad n=3:\cos(\pi/3)=\frac12.
$$

This is the [rational cosine of an integral submultiple of pi](../../../numerical-analysis.md#rational-cosine-of-an-integral-submultiple-of-pi) result. For every $n\geq4$, the value lies strictly between $1/2$ and $1$, so it is irrational.

<h3 id="5f/d">d</h3>

↑ **Parent:** [5F](#5f)

<h4 id="5f/d/i">i</h4>

↑ **Parent:** [D](#5f/d)

<h5 id="5f/d/i/solution">Solution</h5>

↑ **Parent:** [I](#5f/d/i)

Every term is nonnegative. Since $1-\cos x\leq x^2/2$,

$$
0\leq1-\cos(\pi/k)\leq\frac{\pi^2}{2k^2}.
$$

Comparison with $\sum k^{-2}$ shows that the partial sums are bounded. Being increasing, they converge to the finite [limit](../../../calculus.md#limit-of-a-function)

$$
\boxed{\sum_{k=1}^{\infty}(1-\cos(\pi/k)).}
$$

<h4 id="5f/d/ii">ii</h4>

↑ **Parent:** [D](#5f/d)

<h5 id="5f/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5f/d/ii)

Taking real parts of the geometric sum gives

$$
a_n=\Re\frac{1-e^{i(n+1)y}}{1-e^{iy}},
$$

so $(a_n)$ is bounded when $\cos y\ne1$. It cannot converge: convergence would imply $\cos(ny)=a_n-a_{n-1}\to0$, but then

$$
\cos(2ny)=2\cos^2(ny)-1\to-1,
$$

whereas the same necessary condition applied to the subsequence $2n$ would give a [limit](../../../calculus.md#limit-of-a-function) of zero.

## 6E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6e/solution">Solution</h3>

↑ **Parent:** [6E](#6e)

For prime $p$, the nonzero residues pair with their distinct inverses except for $1$ and $-1$, so [Wilson theorem](../../../number-theory.md#wilson-s-theorem) gives

$$
(p-1)!\equiv-1\pmod p.
$$

If composite $n>4$ has a factorization $n=ab$ with $1<a<b<n$, both factors occur in $(n-1)!$. If $n=m^2$, the distinct factors $m$ and $2m$ occur and their product is divisible by $n$; the excluded case $m=2$ is exactly $n=4$. Thus $(n-1)!\equiv0\pmod n$.

The [Fermat-Euler theorem](../../../number-theory.md#euler-s-theorem) states $a^{\phi(n)}\equiv1\pmod n$ when $(a,n)=1$. For prime $p$, $\phi(p)=p-1$, giving Fermat's little theorem for $p\nmid a$; the form $a^p\equiv a\pmod p$ also covers $p\mid a$.

If $a\equiv b\pmod p$, induction and the binomial theorem show

$$
a^{p^n}\equiv b^{p^n}\pmod{p^{n+1}}.
$$

Indeed, write $a^{p^n}=b^{p^n}+cp^{n+1}$ and raise to the $p$th power; every nonleading binomial term gains enough powers of $p$.

Fix $a>1$ and choose any odd prime $p\nmid a^2-1$. Put

$$
N_p=\frac{a^{2p}-1}{a^2-1}=1+a^2+\cdots+a^{2(p-1)}.
$$

Fermat's theorem gives $N_p\equiv1\pmod p$, and $N_p$ is odd, so $2p\mid N_p-1$. Also $a^{2p}\equiv1\pmod{N_p}$, hence $a^{N_p-1}\equiv1\pmod{N_p}$. For odd $p$,

$$
N_p=\frac{a^p-1}{a-1}\frac{a^p+1}{a+1}
$$

is composite. This [generalized repunit pseudoprime construction](../../../number-theory.md#generalized-repunit-pseudoprime-construction) gives infinitely many distinct base-$a$ pseudoprimes because the values are unbounded.

## 7D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7d/a">a</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/a/solution">Solution</h4>

↑ **Parent:** [A](#7d/a)

Induction shows that every iterate $f^n$ is injective. Applying $f$ repeatedly gives

$$
X\supseteq f(X)\supseteq f^2(X)\supseteq\cdots.
$$

If $f^k(X)=f^{k+1}(X)$, applying $f$ inductively gives equality with every later image. Set $A=f^k(X)$. Then $f(A)=A$, so the restriction $f:A\to A$ is surjective, and it remains injective; hence it is bijective.

<h3 id="7d/b">b</h3>

↑ **Parent:** [7D](#7d)

<h4 id="7d/b/solution">Solution</h4>

↑ **Parent:** [B](#7d/b)

The relation preserves the equality pattern among positions. The identity permutation gives reflexivity, inverses give symmetry, and compositions give transitivity.

For $W_3$, representatives are the restricted-growth words

$$
111;\qquad 111,112,121,122;\qquad 111,112,121,122,123
$$

when $n=1$, $n=2$, and $n\geq3$, respectively. Here digits denote distinct symbols, and each displayed word represents one class.

For $W_4$ with $n=3$, the fourteen classes have representatives

$$
1111,1112,1121,1122,1123,1211,1212,1213,
1221,1222,1223,1231,1232,1233.
$$

The cyclic [subgroup](../../../group.md#subgroup) $F$ gives finer classes than all of $P_4$. For example, $x_1x_1x_2$ and $x_1x_1x_3$ have the same equality pattern and are equivalent under $P_4$, but no power of the four-cycle fixes $x_1$ while sending $x_2$ to $x_3$. Thus the two equivalence-class decompositions of $W_3$ differ.

## 8D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

If $A_n$ are countable, choose enumerations and map each element of $\bigcup_nA_n$ to the first pair $(n,k)$ at which it occurs. Since $\mathbb N^2$ is countable, the union is countable.

A periodic [function](../../../function.md) of period $k$ is determined by its $k$ values on a complete residue system. Thus all periodic [functions](../../../function.md) form a countable union over $k$ of the countable sets $\mathbb N^k$, and are countable.

The set of bijections $\mathbb N\to\mathbb N$ is uncountable. Indeed, each binary [sequence](../../../real-analysis.md#sequence) determines a bijection that swaps $2j-1$ and $2j$ exactly when its $j$th bit is one. This is an injection from the uncountable set of binary [sequences](../../../real-analysis.md#sequence).

<h3 id="8d/i">i</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/i/solution">Solution</h4>

↑ **Parent:** [I](#8d/i)

The set is uncountable by Cantor's diagonal argument: from any proposed list, form a [sequence](../../../real-analysis.md#sequence) whose $n$th bit differs from the $n$th bit of the $n$th listed [sequence](../../../real-analysis.md#sequence).

<h3 id="8d/ii">ii</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#8d/ii)

[Sequences](../../../real-analysis.md#sequence) with finitely many ones correspond to finite subsets of $\mathbb N$, a countable union of the countable sets of $k$-element subsets. Complementation gives the same result for finitely many zeros. Their union is therefore countable.

<h3 id="8d/iii">iii</h3>

↑ **Parent:** [8D](#8d)

<h4 id="8d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#8d/iii)

All binary [sequences](../../../real-analysis.md#sequence) are uncountable, while part (ii) accounts for the [sequences](../../../real-analysis.md#sequence) which fail to have infinitely many symbols of both kinds and is countable. Removing that countable subset leaves an uncountable set.

## 9C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9c/solution">Solution</h3>

↑ **Parent:** [9C](#9c)

Using spherical shells and averaging the squared distance from the axis gives

$$
I=\frac25Ma^2.
$$

Sliding without friction has [acceleration](../../../classical-mechanics.md#acceleration) $g\sin\alpha$, so

$$
t_s=\sqrt{\frac{2l}{g\sin\alpha}}.
$$

For rolling, $Ma_{\rm cm}=Mg\sin\alpha-F$ and $I(a_{\rm cm}/a)=Fa$, whence

$$
a_{\rm cm}=\frac{g\sin\alpha}{1+I/(Ma^2)}.
$$

The [rolling acceleration with rotational inertia](../../../classical-mechanics.md#rolling-acceleration-with-rotational-inertia) gives $5g\sin\alpha/7$ for the uniform sphere, and therefore

$$
\frac{t_s}{t_r}=\sqrt{\frac57}.
$$

Mechanical energy is conserved in both idealizations: there is no friction in sliding, while static friction does no work at the instantaneous contact point in pure rolling.

For $I=\gamma Ma^2$, the same calculation gives

$$
\boxed{\frac{t_s}{t_r}=\frac1{\sqrt{1+\gamma}}.}
$$

## 10C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10c/a">a</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/a/solution">Solution</h4>

↑ **Parent:** [A](#10c/a)

With signature $(+,-,-,-)$, the four-momenta are

$$
P_{\rm massive}=m\gamma(c,v),
\qquad
P_\gamma=\frac{\hbar\omega}{c}(1,e).
$$

In the rest frame of a future timelike $P_1$, one has $P_1=(Mc,0)$ and $P_2^0>0$, so $P_1\cdot P_2=McP_2^0>0$; Lorentz invariance proves the assertion in every frame.

The [impossibility of photon decay into two massive particles](../../../special-relativity.md#impossibility-of-photon-decay-into-two-massive-particles) follows because a photon has squared [four-momentum](../../../special-relativity.md#four-momentum) zero. If it decayed into an electron and positron, conservation would give

$$
0=(P_-+P_+)^2=2m^2c^2+2P_-\cdot P_+>0,
$$

a contradiction.

<h3 id="10c/b">b</h3>

↑ **Parent:** [10C](#10c)

<h4 id="10c/b/solution">Solution</h4>

↑ **Parent:** [B](#10c/b)

[Momentum](../../../classical-mechanics.md#momentum) conservation makes the sum of the two photon [momenta](../../../classical-mechanics.md#momentum) parallel to $u$, so all three [vectors](../../../vector-space.md#vector) are coplanar. Put the photons on opposite sides of the incident direction. Transverse and longitudinal [momentum](../../../classical-mechanics.md#momentum) and energy conservation give

$$
E_1\sin\theta_1=E_2\sin\theta_2,
$$



$$
E_1\cos\theta_1+E_2\cos\theta_2=\gamma muc,
\qquad E_1+E_2=mc^2(\gamma+1).
$$

Eliminating $E_1,E_2$ yields

$$
\frac{\sin(\theta_1+\theta_2)}{\sin\theta_1+\sin\theta_2}
=\frac{\gamma u/c}{\gamma+1}
=\sqrt{\frac{\gamma-1}{\gamma+1}}.
$$

Using the half-angle identities on the left gives exactly

$$
\boxed{\frac{1+\cos(\theta_1+\theta_2)}{\cos\theta_1+\cos\theta_2}
=\sqrt{\frac{\gamma-1}{\gamma+1}}.}
$$

## 11C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11c/solution">Solution</h3>

↑ **Parent:** [11C](#11c)

Assume [Newton's second law](../../../classical-mechanics.md#newton-s-second-law), $F_{ij}=-F_{ji}$, and that each internal pair force is central, so $F_{ij}$ is parallel to $r_i-r_j$. Summing

$$
m_i\ddot r_i=F_i+\sum_{j\ne i}F_{ij}
$$

cancels internal pairs and gives $dP/dt=F:=\sum_iF_i$. Taking moments about fixed $a$ cancels the internal [torques](../../../classical-mechanics.md#torque) pairwise and gives

$$
\frac{dL}{dt}=G:=\sum_i(r_i-a)\times F_i.
$$

The [angular momentum about the centre of mass](../../../classical-mechanics.md#angular-momentum-about-the-centre-of-mass) result follows similarly: differentiating $\sum_i(r_i-R)\times m_i(\dot r_i-\dot R)$ introduces no extra term because both total relative position weighted by mass and total relative [momentum](../../../classical-mechanics.md#momentum) vanish. Thus its [derivative](../../../calculus.md#derivative) is the external [torque](../../../classical-mechanics.md#torque) about $R$.

Finally, if every mass is $m$ and $F_i=-k\dot r_i$, then about a fixed point

$$
G=-k\sum_i(r_i-a)\times\dot r_i=-\frac{k}{m}L.
$$

Therefore

$$
\boxed{L(t)=L(0)e^{-kt/m}.}
$$

## 12C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12c/a">a</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/a/solution">Solution</h4>

↑ **Parent:** [A](#12c/a)

The transverse equation of motion is $r^{-1}d(r^2\dot\theta)/dt=0$, so

$$
l=r^2\dot\theta
$$

is constant. With $u=1/r$,

$$
\dot r=\frac{dr}{d\theta}\dot\theta
=-u^{-2}u'\,lu^2=-lu'.
$$

Differentiating once more and substituting into the radial equation $\ddot r-r\dot\theta^2=-f(r)$ gives the [Binet equation](../../../classical-mechanics.md#binet-equation)

$$
\boxed{l^2u^2(u''+u)=f(1/u).}
$$

<h3 id="12c/b">b</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/b/solution">Solution</h4>

↑ **Parent:** [B](#12c/b)

Take $\theta=0$ initially. The [velocity](../../../classical-mechanics.md#velocity) components are

$$
\dot r(0)=-4\cos(\pi/3)=-2,
\qquad r\dot\theta(0)=4\sin(\pi/3)=2\sqrt3,
$$

so $l=2\sqrt3$. Since $f(1/u)=3u^2+9u^3$, the orbit equation becomes

$$
u''+\frac14u=\frac14.
$$

Thus

$$
u=1+A\cos(\theta/2)+B\sin(\theta/2).
$$

The data $u(0)=1$ and $\dot r=-lu'$ give $A=0$, $B=2/\sqrt3$, hence

$$
\boxed{u(\theta)=1+\frac2{\sqrt3}\sin(\theta/2)}.
$$

At $\theta=2\pi$, $u=1$ again, so the particle returns to its initial position after one revolution; now $u'=-1/\sqrt3$, so it is moving outward. Subsequently $u$ first reaches zero at $\theta=8\pi/3$, where $r=1/u\to\infty$. It therefore flies off to infinity.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
