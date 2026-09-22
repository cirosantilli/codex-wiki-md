# Paper 150

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_150.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_150.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Begin with the [Von Mangoldt divisor identity](../../../number-theory.md#von-mangoldt-divisor-identity)

$$
\log n=\sum_{d\mid n}\Lambda(d).
$$

Summing it for $n\leq x$ and reversing the order gives

$$
\log\lfloor x\rfloor!
=\sum_{d\leq x}\Lambda(d)\left\lfloor\frac xd\right\rfloor
=x\sum_{d\leq x}\frac{\Lambda(d)}d+O(\psi(x)).
$$

The given bound $\psi(x)\ll x$ and the [Stirling formula](../../../real-analysis.md#stirling-formula) therefore imply

$$
A(x):=\sum_{d\leq x}\frac{\Lambda(d)}d=\log x+O(1).
$$

Apply [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) with the weight $1/\log n$. Writing $A(t)=\log t+E(t)$, where $E(t)=O(1)$, gives

$$
\sum_{2\leq n\leq x}\frac{\Lambda(n)}{n\log n}
=\frac{A(x)}{\log x}
+\int_2^x\frac{A(t)}{t(\log t)^2}\,dt
=\log\log x+C+O\left(\frac1{\log x}\right).
$$

Indeed, the integral of $E(t)/(t(\log t)^2)$ converges, and its tail from $x$ to infinity is $O(1/\log x)$.

Grouping the left side by [prime powers](../../../number-theory.md#prime-power) yields

$$
\sum_{2\leq n\leq x}\frac{\Lambda(n)}{n\log n}
=\sum_{p^k\leq x}\frac1{kp^k}
=\sum_{p\leq x}\frac1p
+\sum_{\substack{k\geq2\\p^k\leq x}}\frac1{kp^k}.
$$

The full double series over $k\geq2$ converges. Its tail beyond $x$ is $O(x^{-1/2})$: split at $p=\sqrt x$, use a geometric series for $p\leq\sqrt x$, and compare $\sum_{p>\sqrt x}p^{-2}$ with the corresponding sum over integers. Absorbing its limit into the constant proves the [Mertens theorem for reciprocal primes](../../../analytic-number-theory.md#mertens-second-theorem)

$$
\boxed{\sum_{p\leq x}\frac1p
=\log\log x+c+O\left(\frac1{\log x}\right)}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put

$$
L=\log\log x,
\qquad
S=\sum_{p\leq x}\frac1p=L+O(1)
$$

by part a. Double-counting divisibility gives the first moment of the [prime omega function](../../../number-theory.md#prime-omega-function):

$$
\sum_{n\leq x}\omega(n)
=\sum_{p\leq x}\left\lfloor\frac xp\right\rfloor
=xS+O(\pi(x)).
$$

Moreover,

$$
\omega(n)^2=\omega(n)+2\sum_{\substack{p<q\\pq\mid n}}1,
$$

so

$$
\sum_{n\leq x}\omega(n)^2
\leq xS+2x\sum_{p<q\leq x}\frac1{pq}
\leq xS+xS^2.
$$

Expanding the square and using the given bound $\pi(x)\ll x/\log x$ now gives the [Turán normal-order theorem for distinct prime divisors](../../../analytic-number-theory.md#turan-normal-order-theorem-for-distinct-prime-divisors) estimate

$$
\sum_{n\leq x}(\omega(n)-L)^2
\ll x(S-L)^2+xS+L\pi(x)
\ll xL.
$$

By the [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality), the number of $n\leq x$ for which

$$
|\omega(n)-L|>\tfrac12L^{3/4}
$$

is $O(x/L^{1/2})=o(x)$. Discard the $O(\sqrt x)$ integers below $\sqrt x$. For $\sqrt x<n\leq x$,

$$
|\log\log n-L|\leq\log2
$$

and $(\log\log n)^{3/4}\sim L^{3/4}$. Hence, for all sufficiently large $x$, every remaining integer counted in the question also satisfies the preceding inequality. Therefore

$$
\boxed{\#\{n\leq x:|\omega(n)-\log\log n|>(\log\log n)^{3/4}\}=o(x)}.
$$

## 2

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For $\Re s>1$, the absolutely convergent [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series)

$$
\zeta(s)=\sum_{n=1}^\infty n^{-s}
$$

defines the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function). To continue it, use [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) in Stieltjes form:

$$
\zeta(s)
=s\int_1^\infty\lfloor x\rfloor x^{-s-1}\,dx
=\frac{s}{s-1}-s\int_1^\infty\{x\}x^{-s-1}\,dx.
$$

Since $0\leq\{x\}<1$, the final integral converges locally uniformly for $\Re s>0$ and is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) there. The displayed expression is consequently a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) on that half-plane, with its only pole at $s=1$. Since $s/(s-1)$ has residue one there, so does $\zeta$. Agreement in $\Re s>1$ makes this continuation unique by the [identity theorem](../../../complex-analysis.md#identity-theorem).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The functional equation is

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s)}.
$$

Equivalently,

$$
\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s).
$$

For a proof, let

$$
\Theta(u)=\sum_{n\in\mathbb Z}e^{-\pi n^2u}.
$$

The [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula) applied to a [Gaussian function](../../../calculus.md#gaussian-function) gives the theta transformation

$$
\Theta(u)=u^{-1/2}\Theta(1/u).
$$

The standard [Gamma function](../../../complex-analysis.md#gamma-function) integral and termwise integration initially give, for $\Re s>1$,

$$
\Lambda(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\frac12\int_0^\infty(\Theta(u)-1)u^{s/2}\frac{du}{u}.
$$

Split the integral at one, substitute $u\mapsto1/u$ in the lower half, and use the theta transformation. The result is

$$
\Lambda(s)=\frac1{s(s-1)}
+\frac12\int_1^\infty(\Theta(u)-1)
\left(u^{s/2}+u^{(1-s)/2}\right)\frac{du}{u}.
$$

The integral is an [entire function](../../../complex-analysis.md#entire-function) of $s$ because $\Theta(u)-1$ decays exponentially. The right side is visibly invariant under $s\mapsto1-s$, proving both the [analytic continuation](../../../complex-analysis.md#analytic-continuation) and the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function). This is the [Mellin representation of the completed Riemann zeta function](../../../analytic-number-theory.md#mellin-representation-of-the-completed-riemann-zeta-function).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Write the second form of the functional equation as

$$
\zeta(s)=\chi(s)\zeta(1-s),
\qquad
\chi(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s).
$$

For $-2\leq\sigma\leq2$, the elementary exponential formula for the [sine](../../../geometry-and-topology.md#sine) gives, uniformly for $t\geq4$,

$$
|\sin(\pi s/2)|\asymp e^{\pi t/2}.
$$

The stated [Stirling formula](../../../real-analysis.md#stirling-formula) gives

$$
|\Gamma(1-s)|\asymp t^{1/2-\sigma}e^{-\pi t/2}
$$

uniformly on the same strip. The bounded factors $2^\sigma\pi^{\sigma-1}$ and the cancelling exponentials therefore show that

$$
|\chi(s)|\asymp t^{1/2-\sigma}.
$$

Taking absolute values in the functional equation proves the [Vertical-strip factor in the Riemann zeta functional equation](../../../analytic-number-theory.md#vertical-strip-factor-in-the-riemann-zeta-functional-equation):

$$
\boxed{|\zeta(s)|\asymp t^{1/2-\sigma}|\zeta(1-s)|}.
$$

## 3

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $\sigma>1$, unique prime factorization and absolute convergence give the [Euler product](../../../analytic-number-theory.md#euler-product)

$$
\zeta(s)=\prod_p(1-p^{-s})^{-1}.
$$

Every factor is nonzero and the product converges to a nonzero limit. Equivalently, the absolutely convergent identity

$$
\frac1{\zeta(s)}=\sum_{n=1}^\infty\frac{\mu(n)}{n^s}
$$

provides a reciprocal. This proves the [Euler-product nonvanishing of the Riemann zeta function](../../../analytic-number-theory.md#euler-product-nonvanishing-of-the-riemann-zeta-function).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For $\sigma>1$, put $F(s)=-\zeta'(s)/\zeta(s)$. Its absolutely convergent [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) and

$$
3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2\geq0
$$

give the [three-four-one zero-free-region argument](../../../analytic-number-theory.md#three-four-one-zero-free-region-argument)

$$
3F(\sigma)+4\Re F(\sigma+it)+\Re F(\sigma+2it)\geq0.
$$

The pole of $\zeta$ at one gives

$$
F(\sigma)=\frac1{\sigma-1}+O(1).
$$

Suppose $\rho=\beta+i\gamma$ is a zero with $\gamma\geq4$ and $\beta$ close to one. Apply the supplied [Local partial-fraction expansion of the Riemann zeta logarithmic derivative](../../../analytic-number-theory.md#local-partial-fraction-expansion-of-the-riemann-zeta-logarithmic-derivative) at $\sigma+i\gamma$. Every term has positive real part, so retaining the term belonging to $\rho$ gives

$$
\Re F(\sigma+i\gamma)
\leq-\frac1{\sigma-\beta}+O(\log\gamma).
$$

At $\sigma+2i\gamma$ the same expansion gives merely $\Re F(\sigma+2i\gamma)\leq O(\log\gamma)$. The zero is included in the supplied disk whenever $1-\beta$ and $\sigma-1$ are sufficiently small. Hence

$$
0\leq\frac3{\sigma-1}-\frac4{\sigma-\beta}+O(\log\gamma).
$$

Set $L=\log\gamma$ and $\sigma=1+a/L$, where $a>0$ is a sufficiently small fixed constant. If $(1-\beta)L$ were smaller than a sufficiently small constant $c>0$, division by $L$ would give

$$
0\leq\frac3a-\frac4{a+(1-\beta)L}+O(1)<0,
$$

a contradiction. Conjugation handles negative $\gamma$. Reducing $c$ to absorb the bounded range proves the classical [zero-free region of the Riemann zeta function](../../../analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function)

$$
\boxed{\zeta(s)\ne0\quad\text{for}\quad
\sigma\geq1-\frac c{\log|t|},\quad |t|\geq4}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Shrink the constant $c$ from part b if necessary. Put $L=\log|t|$. Zeros in the disk appearing in the supplied partial-fraction formula have $\log|\gamma|=L+O(1/|t|)$, so part b ensures

$$
\beta\leq1-\frac cL
$$

for every such zero.

If $\sigma\geq1+c/(2L)$, absolute convergence of the [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) gives

$$
\left|\frac{\zeta'(s)}{\zeta(s)}\right|
\leq\sum_{n\geq1}\frac{\Lambda(n)}{n^\sigma}
=-\frac{\zeta'(\sigma)}{\zeta(\sigma)}
\ll\frac1{\sigma-1}\ll L,
$$

with the region $\sigma\geq2$ even easier.

It remains to take $1-c/(2L)<\sigma<1+c/(2L)$. Set

$$
s_0=1+\frac c{2L}+it.
$$

For every local zero, both $\Re(s-\rho)$ and $\Re(s_0-\rho)$ are positive and comparable, while $|s-s_0|\ll1/L$. The partial-fraction formula at $s_0$, together with the preceding Euler-product bound, gives

$$
\sum_\rho\Re\frac1{s_0-\rho}\ll L.
$$

Since $\Re(s_0-\rho)\gg1/L$, it follows that

$$
\sum_\rho\frac1{|s_0-\rho|^2}\ll L^2.
$$

Subtracting the partial-fraction formulas at $s$ and $s_0$ now yields

$$
\left|\frac{\zeta'(s)}{\zeta(s)}-\frac{\zeta'(s_0)}{\zeta(s_0)}\right|
\ll |s-s_0|\sum_\rho\frac1{|s-\rho||s_0-\rho|}+L
\ll L.
$$

Therefore the [logarithmic derivative inside the zeta zero-free region](../../../analytic-number-theory.md#logarithmic-derivative-inside-the-zeta-zero-free-region) satisfies

$$
\boxed{\frac{\zeta'(s)}{\zeta(s)}\ll\log|t|}
$$

throughout the required half-width region.

## 4

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $\langle x\rangle$ denote the distance from $x$ to the nearest [prime power](../../../number-theory.md#prime-power). For $x\geq2$ not an integer and $T\geq2$, the truncated [Riemann–von Mangoldt explicit formula](../../../number-theory.md#riemann-von-mangoldt-explicit-formula) is

$$
\boxed{
\begin{aligned}
\psi(x)={}&x-
\sum_{\substack{\rho=\beta+i\gamma\\0\leq\beta\leq1,
\ |\gamma|\leq T}}
\frac{x^\rho}{\rho}
-\log(2\pi)-\frac12\log(1-x^{-2})\\
&+O\left(
\frac{x}{T}(\log(xT))^2
+(\log x)\min\left\{1,\frac{x}{T\langle x\rangle}\right\}
\right).
\end{aligned}}
$$

Zeros are counted with multiplicity. The constant term comes from $s=0$, the logarithm collects the trivial zeros $-2,-4,\ldots$, and the finite sum contains the nontrivial zeros. Enlarging the implied constant covers $1\leq T<2$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Assume first the [Riemann hypothesis](../../../analytic-number-theory.md#riemann-hypothesis). Replace any $x\geq2$ by $y=\lfloor x\rfloor+1/2$; then $\psi(x)=\psi(y)$ and $\langle y\rangle\geq1/2$. Take $T=y$ in part a. Every nontrivial zero has real part $1/2$, and the [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula) implies

$$
\sum_{|\gamma|\leq y}\frac1{|\rho|}\ll(\log y)^2.
$$

Consequently

$$
\sum_{|\gamma|\leq y}\left|\frac{y^\rho}{\rho}\right|
\ll y^{1/2}(\log y)^2,
$$

while both truncation errors in part a are $O((\log y)^2)$. Thus

$$
\psi(x)=x+O\left(x^{1/2}(\log x)^2\right),
$$

which implies the stated $O_\epsilon(x^{1/2+\epsilon})$ estimate.

Conversely, suppose that estimate holds for every $\epsilon>0$. For $\Re s>1$, [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
-\frac{\zeta'(s)}{\zeta(s)}
=s\int_1^\infty\psi(x)x^{-s-1}\,dx
=\frac{s}{s-1}
+s\int_1^\infty(\psi(x)-x)x^{-s-1}\,dx.
$$

Given any $s$ with $\Re s>1/2$, choose $\epsilon<\Re s-1/2$. The error hypothesis makes the last integral locally uniformly convergent there, so it supplies a holomorphic continuation of

$$
-\frac{\zeta'(s)}{\zeta(s)}-\frac{s}{s-1}
$$

to the half-plane $\Re s>1/2$. A zero of $\zeta$ in that half-plane would create a pole of its [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative), so none exists. The [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) reflects every nontrivial zero with real part below $1/2$ to one above $1/2$. All nontrivial zeros must therefore lie on the [critical line](../../../analytic-number-theory.md#critical-line), proving the [Riemann hypothesis equivalence for the second Chebyshev function](../../../analytic-number-theory.md#riemann-hypothesis-equivalence-for-the-second-chebyshev-function).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
