# Paper 150

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_150.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_150.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write

$$
P(z)=\prod_{\substack{p\in\mathbb P\\p\leq z}}p.
$$

The [sifting function](../../../analytic-number-theory.md#sifting-function) is

$$
S(A,\mathbb P,z)=|\{a\in A:\gcd(a,P(z))=1\}|.
$$

For each integer $a$, [Möbius inversion](../../../number-theory.md#mobius-inversion-formula) in its divisor-indicator form gives

$$
\mathbf1_{\gcd(a,P(z))=1}
=\sum_{d\mid\gcd(a,P(z))}\mu(d)
=\sum_{\substack{d\mid P(z)\\d\mid a}}\mu(d).
$$

Summing over the finite set $A$ and interchanging the finite sums yields

$$
S(A,\mathbb P,z)
=\sum_{d\mid P(z)}\mu(d)|\{a\in A:a\equiv0\pmod d\}|.
$$

This is the inclusion-exclusion formula encoded by the [Möbius function](../../../number-theory.md#mobius-function).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Apply part a to $A=\{1,\ldots,\lfloor x\rfloor\}$ and all primes. Since

$$
|\{n\leq x:d\mid n\}|=\left\lfloor\frac xd\right\rfloor,
$$

we obtain

$$
S(A,\mathbb P,z)
=x\sum_{d\mid P(z)}\frac{\mu(d)}d+O\left(\sum_{d\mid P(z)}1\right)
=x\prod_{p\leq z}\left(1-\frac1p\right)+O(2^{\pi(z)}).
$$

For $z\leq\log x$, the error is at most $2^z\leq x^{\log2}=o(x/\log z)$. By [Mertens theorem](../../../analytic-number-theory.md#mertens-theorems), as $z\to\infty$,

$$
\prod_{p\leq z}\left(1-\frac1p\right)
=\frac{e^{-\gamma}+o(1)}{\log z}.
$$

Thus

$$
|\{n\in[1,x]:n\text{ has no prime factor at most }z\}|
=\left(e^{-\gamma}+o(1)\right)\frac{x}{\log z},
$$

so one may take $C=e^{-\gamma}>0$. For bounded $z$, the preceding exact product formula gives the corresponding fixed density.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let

$$
F(n)=(2n+1)(3n+1)(5n+1).
$$

For every prime $p>5$, the congruence $F(n)\equiv0\pmod p$ excludes the three distinct residue classes

$$
n\equiv-2^{-1},-3^{-1},-5^{-1}\pmod p.
$$

The finitely many smaller primes only alter the implied constant. The [dimension-three upper-bound sieve](../../../analytic-number-theory.md#dimension-three-upper-bound-sieve), used with $z=x^{1/2}$, therefore gives

$$
|\{n\leq x:\gcd(F(n),P(z))=1\}|
\ll x\prod_{5<p\leq z}\left(1-\frac3p\right)
\ll\frac{x}{(\log z)^3}
\ll\frac{x}{(\log x)^3},
$$

where the middle estimate follows from [Mertens theorem](../../../analytic-number-theory.md#mertens-theorems).

If all three linear forms are prime, then either $F(n)$ has no prime divisor at most $z$, or one of the three forms itself equals such a prime. The latter possibility contributes only $O(\pi(z))=O(x^{1/2})$, which is absorbed by $x/(\log x)^3$. Hence the required number of $n$ is $\ll x/(\log x)^3$.

## 2

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [truncated Perron formula](../../../analytic-number-theory.md#truncated-perron-formula) says that if $F(s)=\sum_{n\geq1}a_nn^{-s}$ converges absolutely for $\Re s>\sigma_a$, then for $c>\sigma_a$, $T\geq2$, and $x$ not an integer,

$$
\sum_{n\leq x}a_n
=\frac1{2\pi i}\int_{c-iT}^{c+iT}F(s)\frac{x^s}{s}\,ds
+O\left(\sum_{n\geq1}|a_n|\left(\frac xn\right)^c
\min\left\{1,\frac1{T|\log(x/n)|}\right\}\right).
$$

Take $a_n=\Lambda(n)$ and $c=1+1/\log x$. The [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) identity gives $F(s)=-\zeta'(s)/\zeta(s)$. Since $x-1/2$ is an integer, $|x-n|\geq1/2$ for every integer $n$. In the range $x/2<n<2x$,

$$
|\log(x/n)|\asymp\frac{|x-n|}{x},
$$

and hence the contribution there is

$$
\ll\frac{x\log x}{T}\sum_{x/2<n<2x}\frac1{|x-n|}
\ll\frac{x(\log x)^2}{T}.
$$

The ranges $n\leq x/2$ and $n\geq2x$ are bounded by the same quantity using absolute convergence and $-\zeta'(c)/\zeta(c)\ll\log x$. Therefore

$$
\boxed{\sum_{n\leq x}\Lambda(n)
=-\frac1{2\pi i}\int_{1+1/\log x-iT}^{1+1/\log x+iT}
\frac{\zeta'(s)}{\zeta(s)}\frac{x^s}{s}\,ds
+O\left(\frac{x(\log x)^2}{T}\right).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $L=\log x$ and choose

$$
T=\exp(a\sqrt L),
\qquad
\sigma_0=1-\frac b{\sqrt L},
$$

with fixed positive $a,b$ chosen so that the rectangle up to height $T$ lies inside the [zero-free region of the Riemann zeta function](../../../analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function). Move the Perron contour from $1+1/L$ to $\sigma_0$. The only singularity crossed is the simple pole at $s=1$ of $-\zeta'(s)/\zeta(s)$, whose residue contributes $x$.

The standard bound $\zeta'(s)/\zeta(s)\ll(\log T)^2$ in this zero-free rectangle gives

$$
\int_{\sigma_0-iT}^{\sigma_0+iT}
\frac{\zeta'(s)}{\zeta(s)}\frac{x^s}{s}\,ds
\ll x^{\sigma_0}(\log T)^3
\ll x\exp(-b\sqrt L)L^{3/2}.
$$

The two horizontal sides are $\ll x(\log T)^2/T$, and the truncation error from part a is $\ll xL^2/T$. Polynomial factors in $L$ can be absorbed by slightly reducing the exponential constant. Thus some $c>0$ satisfies

$$
\sum_{n\leq x}\Lambda(n)
=x+O\left(x\exp(-c\sqrt{\log x})\right).
$$

This is the [Prime number theorem with classical zero-free-region error](../../../analytic-number-theory.md#prime-number-theorem-with-classical-zero-free-region-error).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $\Re s>1$, absolute convergence permits a shift of the complex variable:

$$
\sum_{n=1}^{\infty}\frac{\Lambda(n)n^{iu}}{n^s}
=\sum_{n=1}^{\infty}\frac{\Lambda(n)}{n^{s-iu}}
=-\frac{\zeta'(s-iu)}{\zeta(s-iu)}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Put

$$
A(x)=\sum_{n\leq x}\Lambda(n)n^{iu}
=\frac{x^{1+iu}}{1+iu}+O\left(x^{1/2}(\log x)^2\right).
$$

For $\Re s>1$, [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
-\frac{\zeta'(s-iu)}{\zeta(s-iu)}
=s\int_1^\infty A(x)x^{-s-1}\,dx
=\frac{s}{(1+iu)(s-1-iu)}
+s\int_1^\infty O\left(x^{1/2}(\log x)^2\right)x^{-s-1}\,dx.
$$

The last integral is holomorphic for $\Re s>1/2$. Thus the logarithmic derivative on the left continues meromorphically to that half-plane with no pole except $s=1+iu$.

A zero $\rho$ of $\zeta$ with $\Re\rho>1/2$ would make $-\zeta'(s-iu)/\zeta(s-iu)$ singular at $s=\rho+iu$, a contradiction unless $\rho=1$, which is a pole rather than a zero. Therefore no nontrivial zero lies to the right of the [critical line](../../../analytic-number-theory.md#critical-line). The [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) reflects zeros across that line, so none lies to its left either. Every nontrivial zero lies on the critical line, proving the [Riemann hypothesis](../../../analytic-number-theory.md#riemann-hypothesis). This is the [Twisted Von Mangoldt estimate implying the Riemann hypothesis](../../../analytic-number-theory.md#twisted-von-mangoldt-estimate-implying-the-riemann-hypothesis).

## 3

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $\sigma=\Re s>1$,

$$
\sum_{n=1}^\infty\left|\frac{f(n)}{n^s}\right|
\leq\sum_{n=1}^\infty\frac1{n^\sigma}
=\zeta(\sigma)<\infty.
$$

On every compact subset of $\Re s>1$, the terms are bounded by a convergent series $\sum n^{-1-\delta}$. The [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test) gives locally uniform convergence, and the theorem on [locally uniform convergence of holomorphic functions](../../../complex-analysis.md#locally-uniform-convergence-of-holomorphic-functions) shows that the limit is an [analytic function](../../../complex-analysis.md#space-of-holomorphic-functions). Hence $D_f$ is analytic throughout $\Re s>1$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For arithmetic functions $f,g$ bounded in modulus by one, their [pretentious distance](../../../number-theory.md#pretentious-distance) up to $x$ is defined by

$$
\boxed{\mathbb D(f,g;x)^2
=\sum_{p\leq x}\frac{1-\Re(f(p)\overline{g(p)})}{p}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Complete multiplicativity and absolute convergence give the [Euler product](../../../analytic-number-theory.md#euler-product)

$$
D_f(s)=\prod_p\left(1-\frac{f(p)}{p^s}\right)^{-1}
\qquad(\Re s>1).
$$

Set $\sigma=1+1/\log x$. Taking logarithms of absolute values and expanding the local factors gives, uniformly in real $t$,

$$
\log|D_f(\sigma+it)|
=\sum_p\frac{\Re(f(p)p^{-it})}{p^\sigma}+O(1)
=\sum_{p\leq x}\frac{\Re(f(p)p^{-it})}{p}+O(1).
$$

The prime powers with exponent at least two contribute $O(1)$; changing $p^{-\sigma}$ to $p^{-1}$ below $x$ and estimating the tail above $x$ also cost $O(1)$. By [Mertens theorem](../../../analytic-number-theory.md#mertens-theorems),

$$
\sum_{p\leq x}\frac{\Re(f(p)p^{-it})}{p}
=\log\log x-\mathbb D(f,n^{it};x)^2+O(1).
$$

Exponentiating yields

$$
\boxed{\left|D_f\left(1+\frac1{\log x}+it\right)\right|
\asymp(\log x)\exp\left(-\mathbb D(f,n^{it};x)^2\right).}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For $\sigma>1$, take logarithms of Euler products. With $z=f(p)p^{-it}$, the inequality

$$
3+4\Re(z^k)+\Re(z^{2k})\geq0
\qquad(|z|\leq1)
$$

at every prime power gives the [three-four-one inequality for Euler products](../../../analytic-number-theory.md#three-four-one-inequality-for-euler-products)

$$
\zeta(\sigma)^3|D_f(\sigma+it)|^4|D_{f^2}(\sigma+2it)|\geq1.
$$

Suppose $D_f(1+it)=0$ with multiplicity $m\geq1$. The assumed analytic continuation gives

$$
|D_f(\sigma+it)|\ll(\sigma-1)^m,
$$

while $D_{f^2}(\sigma+2it)$ remains bounded and $\zeta(\sigma)^3\asymp(\sigma-1)^{-3}$ as $\sigma\downarrow1$. The left side of the inequality would then be

$$
O((\sigma-1)^{4m-3})\longrightarrow0,
$$

contradicting its lower bound one. Hence $D_f$ has no zero on $\Re s=1$. Absolute convergence of its Euler product already excludes zeros for $\Re s>1$, so $D_f(s)\ne0$ throughout $\Re s\geq1$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
