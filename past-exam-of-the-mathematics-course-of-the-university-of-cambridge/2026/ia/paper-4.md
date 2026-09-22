# Paper 4

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2026/Paperia_4_2026.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2026/Paperia_4_2026.pdf)

**Table of contents**

- [1F](#1f)
  - [i](#1f/i)
    - [Solution](#1f/i/solution)
  - [ii](#1f/ii)
    - [Solution](#1f/ii/solution)
- [2D](#2d)
  - [a](#2d/a)
    - [Solution](#2d/a/solution)
  - [b](#2d/b)
    - [Solution](#2d/b/solution)
- [3B](#3b)
  - [i](#3b/i)
    - [Solution](#3b/i/solution)
  - [ii](#3b/ii)
    - [Solution](#3b/ii/solution)
  - [iii](#3b/iii)
    - [Solution](#3b/iii/solution)
  - [iv](#3b/iv)
    - [Solution](#3b/iv/solution)
  - [v](#3b/v)
    - [Solution](#3b/v/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5F](#5f)
  - [i](#5f/i)
    - [a](#5f/i/a)
      - [Solution](#5f/i/a/solution)
    - [b](#5f/i/b)
      - [Solution](#5f/i/b/solution)
    - [c](#5f/i/c)
      - [Solution](#5f/i/c/solution)
    - [d](#5f/i/d)
      - [Solution](#5f/i/d/solution)
  - [ii](#5f/ii)
    - [Solution](#5f/ii/solution)
- [6D](#6d)
  - [i](#6d/i)
    - [Solution](#6d/i/solution)
  - [ii](#6d/ii)
    - [Solution](#6d/ii/solution)
  - [iii](#6d/iii)
    - [Solution](#6d/iii/solution)
  - [iv](#6d/iv)
    - [Solution](#6d/iv/solution)
  - [v](#6d/v)
    - [Solution](#6d/v/solution)
- [7E](#7e)
  - [a](#7e/a)
    - [Solution](#7e/a/solution)
  - [b](#7e/b)
    - [Solution](#7e/b/solution)
  - [c](#7e/c)
    - [Solution](#7e/c/solution)
  - [d](#7e/d)
    - [Solution](#7e/d/solution)
  - [e](#7e/e)
    - [Solution](#7e/e/solution)
- [8E](#8e)
  - [a](#8e/a)
    - [Solution](#8e/a/solution)
  - [b](#8e/b)
    - [Solution](#8e/b/solution)
  - [c](#8e/c)
    - [Solution](#8e/c/solution)
- [9B](#9b)
  - [Solution](#9b/solution)
- [10B](#10b)
  - [a](#10b/a)
    - [Solution](#10b/a/solution)
  - [b](#10b/b)
    - [Solution](#10b/b/solution)
  - [c](#10b/c)
    - [Solution](#10b/c/solution)
  - [d](#10b/d)
    - [Solution](#10b/d/solution)
- [11B](#11b)
  - [a](#11b/a)
    - [Solution](#11b/a/solution)
  - [b](#11b/b)
    - [Solution](#11b/b/solution)
- [12B](#12b)
  - [a](#12b/a)
    - [Solution](#12b/a/solution)
  - [b](#12b/b)
    - [Solution](#12b/b/solution)
  - [c](#12b/c)
    - [Solution](#12b/c/solution)

## 1F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1f/i">i</h3>

↑ **Parent:** [1F](#1f)

<h4 id="1f/i/solution">Solution</h4>

↑ **Parent:** [I](#1f/i)

The two conjugate roots satisfy $r^2=6r-4$, so $u_n=6u_{n-1}-4u_{n-2}$ with $u_0=2,u_1=6$. Induction gives $u_n\in\mathbb Z$.

<h3 id="1f/ii">ii</h3>

↑ **Parent:** [1F](#1f)

<h4 id="1f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1f/ii)

The same recurrence and $2^0\mid u_0$, $2^1\mid u_1$ prove the claim: if $2^{n-1}\mid u_{n-1}$ and $2^{n-2}\mid u_{n-2}$, both terms on the right are divisible by $2^n$.

## 2D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2d/a">a</h3>

↑ **Parent:** [2D](#2d)

<h4 id="2d/a/solution">Solution</h4>

↑ **Parent:** [A](#2d/a)

The congruences reduce to $z\equiv14\pmod {17}$ and $z\equiv8\pmod {19}$. Writing $z=14+17k$ gives $k\equiv3\pmod {19}$, hence $z\equiv65\pmod {323}$.

<h3 id="2d/b">b</h3>

↑ **Parent:** [2D](#2d)

<h4 id="2d/b/solution">Solution</h4>

↑ **Parent:** [B](#2d/b)

$\varphi(33)=20$ and $7^{-1}\equiv3\pmod {20}$, so Bob computes $29^3\equiv2\pmod {33}$. RSA relies on modular exponentiation being easy while recovering the private exponent without the factorisation of a large $N$ is believed hard.

## 3B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3b/i">i</h3>

↑ **Parent:** [3B](#3b)

<h4 id="3b/i/solution">Solution</h4>

↑ **Parent:** [I](#3b/i)

From $F=Gm_1m_2/r^2$, $[G]=L^3M^{-1}T^{-2}$.

<h3 id="3b/ii">ii</h3>

↑ **Parent:** [3B](#3b)

<h4 id="3b/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3b/ii)

Using only $G,M$ and orbital scale $R$, dimensional balance gives $T^2\propto R^3/(GM)$.

<h3 id="3b/iii">iii</h3>

↑ **Parent:** [3B](#3b)

<h4 id="3b/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3b/iii)

The only length from $G,M,c$ is $R\sim GM/c^2$.

<h3 id="3b/iv">iv</h3>

↑ **Parent:** [3B](#3b)

<h4 id="3b/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3b/iv)

The only length from $\hbar,m,c$ is $\lambda\sim\hbar/(mc)$.

<h3 id="3b/v">v</h3>

↑ **Parent:** [3B](#3b)

<h4 id="3b/v/solution">Solution</h4>

↑ **Parent:** [V](#3b/v)

Equating the two lengths gives $m\sim\sqrt{\hbar c/G}$, the [Planck mass](../../../physics.md#planck-mass).

## 4B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

[Proper time](../../../special-relativity.md#proper-time) satisfies $c^2d\tau^2=c^2dt^2-dx^2$ and is invariant, so differentiating by it defines a four-vector. The path is timelike iff $R|\omega|\lt c$. Its next return occurs after coordinate time $2\pi/|\omega|$, so Bob ages

$$
\Delta\tau=\frac{2\pi}{|\omega|}\sqrt{1-R^2\omega^2/c^2}.
$$

With $\gamma=(1-R^2\omega^2/c^2)^{-1/2}$,  
$U^\mu=\gamma(c,R\omega\cos\omega t,-R\omega\sin\omega t,0)$ and $U\cdot U=c^2$ for signature $(+---)$.

## 5F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5f/i">i</h3>

↑ **Parent:** [5F](#5f)

<h4 id="5f/i/a">a</h4>

↑ **Parent:** [I](#5f/i)

<h5 id="5f/i/a/solution">Solution</h5>

↑ **Parent:** [A](#5f/i/a)

Whether $\log2$ is irrational is not presently known; the given fact about $e$ does not decide it.

<h4 id="5f/i/b">b</h4>

↑ **Parent:** [I](#5f/i)

<h5 id="5f/i/b/solution">Solution</h5>

↑ **Parent:** [B](#5f/i/b)

$\log_2 3$ is irrational: if it were $p/q$, then $2^p=3^q$, contradicting unique prime factorisation.

<h4 id="5f/i/c">c</h4>

↑ **Parent:** [I](#5f/i)

<h5 id="5f/i/c/solution">Solution</h5>

↑ **Parent:** [C](#5f/i/c)

$ae+b/e$ is transcendental, hence irrational. If it were algebraic, $e$ would solve $ax^2-(ae+b/e)x+b=0$ over the algebraic numbers, contradicting transcendence of $e$.

<h4 id="5f/i/d">d</h4>

↑ **Parent:** [I](#5f/i)

<h5 id="5f/i/d/solution">Solution</h5>

↑ **Parent:** [D](#5f/i/d)

The cubic is strictly increasing and has one real root. A rational root of the monic integer [polynomial](../../../polynomial.md) would be an integer divisor of $3$; testing $\pm1,\pm3$ gives none, so the root is irrational.

<h3 id="5f/ii">ii</h3>

↑ **Parent:** [5F](#5f)

<h4 id="5f/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5f/ii)

Let $2^k\le n\lt 2^{k+1}$. In the reduced common-denominator expression for $H_n$, the term $1/2^k$ is the unique term whose denominator contains the largest power $2^k$; after multiplication by the least common multiple it contributes an odd integer while all other terms contribute even integers. Thus the numerator is odd and the denominator remains even, so $H_n$ is not an integer.

## 6D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6d/i">i</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/i/solution">Solution</h4>

↑ **Parent:** [I](#6d/i)

For $a\ne0\pmod p$, $\gcd(a,p)=1$, so Bézout gives $au+pv=1$ and $u$ is an inverse modulo $p$.

<h3 id="6d/ii">ii</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6d/ii)

If $x^2\equiv a$ and $y^2\equiv a\pmod p$, then $(x-y)(x+y)\equiv0$, hence $y\equiv\pm x$; these differ for odd $p$. It fails for composite [moduli](../../../complex-analysis.md#modulus): $1$ has four square roots modulo $8$.

<h3 id="6d/iii">iii</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6d/iii)

For prime $n$, pair each nonzero residue with its inverse; only $\pm1$ are self-inverse, yielding [Wilson theorem](../../../number-theory.md#wilson-s-theorem). Conversely, if $(n-1)!\equiv-1\pmod n$, every $1\le a\lt n$ is a unit (otherwise a common divisor would divide the left side and $n$ but not $-1$), so $n$ is prime.

<h3 id="6d/iv">iv</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6d/iv)

Wilson gives $18!\equiv-1\pmod {19}$. Since $18\cdot17\equiv2$, $2\cdot16!\equiv-1$, hence $16!\equiv9\pmod {19}$.

<h3 id="6d/v">v</h3>

↑ **Parent:** [6D](#6d)

<h4 id="6d/v/solution">Solution</h4>

↑ **Parent:** [V](#6d/v)

By Fermat, $a^{p-1}=1$. Thus $a^{(p-1)/2}=\pm1$. The squaring map on $\mathbb F_p^*$ has kernel $\{\pm1\}$, so exactly $(p-1)/2$ inputs are squares; the [polynomial](../../../polynomial.md) $x^{(p-1)/2}-1$ has at most that many roots and already has all squares, proving the two cases.

## 7E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7e/a">a</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/a/solution">Solution</h4>

↑ **Parent:** [A](#7e/a)

**True.** Take $C=f(A)$ and define $g(f(a))=a$, which is well-defined and injective because $f$ is injective.

<h3 id="7e/b">b</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/b/solution">Solution</h4>

↑ **Parent:** [B](#7e/b)

**False.** A constant surjection from a two-element set to a singleton followed by the singleton’s inclusion is not injective.

<h3 id="7e/c">c</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/c/solution">Solution</h4>

↑ **Parent:** [C](#7e/c)

**False.** Include a singleton into a two-element set and then map both elements onto a singleton; the composite need not cover a larger target in analogous examples. Concretely $A=\{1\}$, $B=\{1,2\}$, $C=\{1,2\}$, $f(1)=1$, and let $g$ swap/surject with $g(1)=g(2)=1$ after taking $C$ singleton; then the claimed implication fails whenever an element of $C$ is reached only outside $f(A)$.

<h3 id="7e/d">d</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/d/solution">Solution</h4>

↑ **Parent:** [D](#7e/d)

**True.** If $f(a_1)=f(a_2)$ with $a_1\ne a_2$, then $(g\circ f)(a_1)=(g\circ f)(a_2)$.

<h3 id="7e/e">e</h3>

↑ **Parent:** [7E](#7e)

<h4 id="7e/e/solution">Solution</h4>

↑ **Parent:** [E](#7e/e)

Put $|B|=m$. There are $\binom{m+1}{2}m!=(m+1)!m/2$ surjections and $(m+1)!$ injections. For $m\ge3$ the domain is larger, so $\Psi$ cannot be injective, regardless of the choices. For $m=1$ there is only one surjection, so it is injective. For $m=2$ both sets have size $6$; injectivity depends on the representative choices and, if achieved, is equivalent to bijectivity.

## 8E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8e/a">a</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/a/solution">Solution</h4>

↑ **Parent:** [A](#8e/a)

Monomials are indexed by $\mathbb N^n$, a [countable set](../../../set-theory.md#countable-set). A [polynomial](../../../polynomial.md) is a finite list of monomials with rational coefficients, so $P_n$ is a countable union of countable sets.

<h3 id="8e/b">b</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/b/solution">Solution</h4>

↑ **Parent:** [B](#8e/b)

$X_1$ is the set of real algebraic numbers and is countable because each nonzero [polynomial](../../../polynomial.md) has finitely many roots. For $n\ge2$, $X_n$ is uncountable: the [polynomial](../../../polynomial.md) $x_1$ vanishes on $\{0\}\times\mathbb R^{n-1}$.

<h3 id="8e/c">c</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/c/solution">Solution</h4>

↑ **Parent:** [C](#8e/c)

Start with $S_0=\mathbb Q$. Given countable $S_n$, let $S_{n+1}$ be the field generated by $S_n\cup\{\sqrt{|x|}:x\in S_n\}$. It is countable because its elements are values of rational expressions in finitely many members of a countable set. Then $S=\bigcup_nS_n$ is countable and has (i)–(iii). Any other set with those properties contains every $S_n$ by induction, proving minimality and uniqueness.

## 9B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9b/solution">Solution</h3>

↑ **Parent:** [9B](#9b)

Let the full cube mass be $M=8\rho a^3$ and the removed cylinder mass $m_h=2\pi\rho ar^2$. About the rod, the remaining moment is

$$
I=M a^2(2/3+\gamma^2)-\tfrac12m_hr^2.
$$

The remaining centre-of-mass distance $\ell$ obeys $(M-m_h)\ell=M\gamma a$, so the small-angle equation is $I\ddot\theta+M g\gamma a\,\theta=0$. Hence

$$
\boxed{T=2\pi\sqrt{\frac a{g\gamma}\left(\frac23+\gamma^2-\frac\pi8\frac{r^4}{a^4}\right)}.}
$$

## 10B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10b/a">a</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/a/solution">Solution</h4>

↑ **Parent:** [A](#10b/a)

$m\ddot x=-\nabla V$. Dotting with $\dot x$ gives $d(\tfrac12m|\dot x|^2+V)/dt=0$.

<h3 id="10b/b">b</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/b/solution">Solution</h4>

↑ **Parent:** [B](#10b/b)

A central potential is $V(r)$. Then $\dot L=x\times(-\nabla V)=0$. Since $L\cdot x=0$, the trajectory lies in the fixed plane perpendicular to $L$.

<h3 id="10b/c">c</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/c/solution">Solution</h4>

↑ **Parent:** [C](#10b/c)

The equation is $m\ddot x=-\nabla V+q\dot x\times B$; the magnetic force does no work. For $B=\beta\hat r/r^2$, the triple-product identity gives $\dot L=q\beta\,d\hat r/dt$, so $J=L-q\beta\hat r$ is conserved. Since $J\cdot\hat r=-q\beta$, the trajectory lies on a cone with $\cos\alpha=-q\beta/|J|$.

<h3 id="10b/d">d</h3>

↑ **Parent:** [10B](#10b)

<h4 id="10b/d/solution">Solution</h4>

↑ **Parent:** [D](#10b/d)

$L^2=J^2-(q\beta)^2=J^2\sin^2\alpha$. Splitting [kinetic energy](../../../classical-mechanics.md#kinetic-energy) into radial and angular parts therefore gives $E=\tfrac12m\dot r^2+J^2\sin^2\alpha/(2mr^2)+V(r)$, proving the stated [effective potential](../../../physics.md#effective-potential).

## 11B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11b/a">a</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/a/solution">Solution</h4>

↑ **Parent:** [A](#11b/a)

Differentiating a [vector](../../../vector-space.md#vector) using $(dA/dt)_S=(dA/dt)_{S\prime}+\omega\times A$ twice yields  
$m\ddot x=F-2m\omega\times\dot x-m\dot\omega\times x-m\omega\times(\omega\times x)$.

<h3 id="11b/b">b</h3>

↑ **Parent:** [11B](#11b)

<h4 id="11b/b/solution">Solution</h4>

↑ **Parent:** [B](#11b/b)

Along $BC$, write $x=(2a,s,0)$. With $\omega=-\alpha\hat z/t$, the tangential equation is

$$
\ddot s=\frac{\alpha^2s-2a\alpha}{t^2}.
$$

A stationary point is $s_0=2a/\alpha$, lying on the side iff $\alpha\ge1$. The general perturbed motion is

$$
s=s_0+C t^{(1+\sqrt{1+4\alpha^2})/2}+D t^{(1-\sqrt{1+4\alpha^2})/2}.
$$

Except on the decaying-mode fine tuning, the growing term carries the bead to $B$ or $C$, according to its sign.

## 12B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12b/a">a</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/a/solution">Solution</h4>

↑ **Parent:** [A](#12b/a)

Two-body energy-momentum conservation in the pion rest frame gives $E_e=(m_\pi^2+m_e^2)c^2/(2m_\pi)$ and $p_e=(m_\pi^2-m_e^2)c/(2m_\pi)$. Thus $v_e=c(m_\pi^2-m_e^2)/(m_\pi^2+m_e^2)$.

<h3 id="12b/b">b</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/b/solution">Solution</h4>

↑ **Parent:** [B](#12b/b)

Let the incident positron total energy be $E$. For perpendicular photon [momenta](../../../classical-mechanics.md#momentum), real positive photon energies require  
$(E+m_ec^2)^2-4m_ec^2(E+m_ec^2)\ge0$.  
**Thus the threshold is $E=3m_ec^2$.**

<h3 id="12b/c">c</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/c/solution">Solution</h4>

↑ **Parent:** [C](#12b/c)

Squaring $p_H=p_1+p_2$ gives $m^2c^4=2E_1E_2(1-\cos\theta)=4E_1E_2\sin^2(\theta/2)$, proving the formula. If the rest-frame photons are along $\pm y$, an $x$-boost gives equal energies and $\sin(\theta/2)=1/\gamma$, hence $v=c\cos(\theta/2)$.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
