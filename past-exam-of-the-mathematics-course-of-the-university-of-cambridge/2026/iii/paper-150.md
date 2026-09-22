# Paper 150

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20150.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20150.pdf)

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
  - [e](#2/e)
    - [Solution](#2/e/solution)
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

Let $\mathbf1(n)=1$. The basic [Von Mangoldt divisor identity](../../../number-theory.md#von-mangoldt-divisor-identity) is

$$
\log n=\sum_{d\mid n}\Lambda(d),
$$

because if $n=\prod_pp^{v_p(n)}$, the right-hand side is $\sum_pv_p(n)\log p=\log n$. In terms of [Dirichlet convolution](../../../number-theory.md#dirichlet-convolution), this says $\log=\mathbf1*\Lambda$. Since the [Möbius function](../../../number-theory.md#mobius-function) is the convolution inverse of $\mathbf1$, convolving with $\mu$ gives $\Lambda=\mu*\log$. Consequently

$$
\boxed{\Lambda(n)=\sum_{d\mid n}\mu(d)\log\frac nd.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Dirichlet hyperbola method](../../../number-theory.md#dirichlet-hyperbola-method) counts each factorization $n=ab$ once and gives, with $y=\lfloor\sqrt x\rfloor$,

$$
\sum_{n\leq x}\tau(n)
=\sum_{ab\leq x}1
=2\sum_{a\leq y}\left\lfloor\frac xa\right\rfloor-y^2.
$$

Using $\lfloor x/a\rfloor=x/a+O(1)$ and the [harmonic number](../../../analytic-number-theory.md#harmonic-number) estimate $H_y=\log y+\gamma+O(1/y)$, where $\gamma$ is the [Euler--Mascheroni constant](../../../complex-analysis.md#euler-s-constant), we obtain

$$
\sum_{n\leq x}\tau(n)
=2x(\log y+\gamma)-y^2+O(y)
=x\log x+(2\gamma-1)x+O(\sqrt x).
$$

**Thus one may take $C=2\gamma-1$.**

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For each [prime number](../../../number-theory.md#prime-number) $p\nmid a$, the congruence $an+1\equiv0\pmod p$ removes exactly one [residue class](../../../number-theory.md#residue-class) of $n$ modulo $p$; for $p\mid a$, it removes none. The dimension-one [upper-bound sieve](../../../analytic-number-theory.md#upper-bound-sieve) therefore gives

$$
\bigl|\{n\leq x:(an+1,\prod_{w\leq p\leq z}p)=1\}\bigr|
\ll x\prod_{\substack{w\leq p\leq z\\p\nmid a}}
\left(1-\frac1p\right).
$$

Separating the primes that divide $a$ bounds the product by

$$
\prod_{w\leq p\leq z}\left(1-\frac1p\right)
\prod_{p\mid a}\left(1-\frac1p\right)^{-1}.
$$

The ratio form of [Mertens theorem](../../../analytic-number-theory.md#mertens-theorems) says that the first product is $\ll\log w/\log z$. Hence

$$
\boxed{\bigl|\{n\in[1,x]:an+1\text{ has no prime factor in }[w,z]\}\bigr|
\ll x\frac{\log w}{\log z}
\prod_{p\mid a}\left(1-\frac1p\right)^{-1}.}
$$

## 2

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

If $f$ is a [multiplicative function](../../../number-theory.md#multiplicative-function) with $|f(n)|\leq1$, then for $\Re s>1$ its [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) has the [Euler product](../../../analytic-number-theory.md#euler-product)

$$
\sum_{n=1}^{\infty}\frac{f(n)}{n^s}
=\prod_p\left(1+\frac{f(p)}{p^s}+\frac{f(p^2)}{p^{2s}}+\cdots\right).
$$

Indeed, expanding the product over a finite set of primes and using [unique prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) gives the sum over integers having no other prime factors. Moreover,

$$
\sum_{n\geq1}\left|\frac{f(n)}{n^s}\right|
\leq\sum_{n\geq1}n^{-\Re s}<\infty,
$$

so [absolute convergence](../../../real-analysis.md#absolute-convergence) permits rearrangement and passage to the limit over all primes. This proves the formula.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The symmetric form of the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) is

$$
\xi(s)=\xi(1-s),
\qquad
\xi(s)=\frac12s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s).
$$

The [complex conjugation](../../../complex-analysis.md#complex-conjugate) identity $\zeta(\overline s)=\overline{\zeta(s)}$ and the functional equation show that every [Nontrivial zero of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) $\rho$ is accompanied by $\overline\rho$, $1-\rho$, and $1-\overline\rho$.

Let $\rho=\beta+i\gamma$ be the given nonreal zero. If $\beta>1/2$, use $\rho$ itself; if $\beta<1/2$, use $1-\rho$, whose real part is $1-\beta>1/2$. The resulting zero cannot have real part greater than one, by the stated zero-free half-plane. It therefore has real part in $(1/2,1]$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Write $M(x)=\sum_{n\leq x}\mu(n)$ for the [Mertens function](../../../number-theory.md#mertens-function). Suppose, to the contrary, that for some $\varepsilon>0$ the quotient $|M(x)|/x^{1/2-\varepsilon}$ were bounded. [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) would then make

$$
\sum_{n=1}^{\infty}\frac{\mu(n)}{n^s}
=s\int_1^\infty M(x)x^{-s-1}\,dx
$$

converge and define a [holomorphic function](../../../complex-analysis.md#holomorphic-function) throughout $\Re s>1/2-\varepsilon$. In $\Re s>1$ the [Euler product](../../../analytic-number-theory.md#euler-product) identifies this function with $1/\zeta(s)$, so [analytic continuation](../../../complex-analysis.md#analytic-continuation) would make $1/\zeta(s)$ holomorphic in that larger half-plane.

By assumption, $\zeta$ has a [nontrivial zero](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function). The [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) reflects one of that zero and its partner into $\Re s\geq1/2$, where $1/\zeta$ must have a pole, a contradiction. Thus $|M(x)|/x^{1/2-\varepsilon}$ is unbounded, which gives an $x\geq1$ exceeding any prescribed constant $C$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

One quantitative form of [Halász theorem](../../../number-theory.md#halasz-theorem) is the following. If $f$ is [multiplicative](../../../number-theory.md#multiplicative-function) and $|f(n)|\leq1$, put

$$
M(f;x,T)=\min_{|t|\leq T}\mathbb D(f,n^{it};x)^2,
\qquad
\mathbb D(f,g;x)^2
=\sum_{p\leq x}\frac{1-\Re(f(p)\overline{g(p)})}{p}.
$$

Then, uniformly for $2\leq T\leq x$,

$$
\frac1x\left|\sum_{n\leq x}f(n)\right|
\ll (1+M(f;x,T))e^{-M(f;x,T)}+\frac1{\sqrt T}.
$$

**Thus a bounded [multiplicative arithmetic function](../../../number-theory.md#multiplicative-function) can have a large mean only when it has small [pretentious distance](../../../number-theory.md#pretentious-distance) from some Archimedean character $n^{it}$.**

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Put $g=f\mu$. At every prime, $f(p)^2=1$, so the [triangle inequality for pretentious distance](../../../number-theory.md#triangle-inequality-for-pretentious-distance) gives

$$
\mathbb D(f,n^{it};x)+\mathbb D(g,n^{iu};x)
\geq\mathbb D(\mu,n^{i(t+u)};x).
$$

The standard [strong aperiodicity of the Möbius function](../../../number-theory.md#strong-aperiodicity-of-the-mobius-function) states, for example with $T=(\log x)^{1/10}$, that

$$
\inf_{|v|\leq2T}\mathbb D(\mu,n^{iv};x)^2\longrightarrow\infty.
$$

Indeed, its left side is controlled by the prime sum $\sum_{p\leq x}(1+\cos(v\log p))/p$, uniformly in this range.

Choose $t$ and $u$ minimizing the two distances in [Halász theorem](../../../number-theory.md#halasz-theorem). The displayed triangle inequality implies that at least one of $M(f;x,T)$ and $M(g;x,T)$ tends to infinity. Halász's bound, and $T\to\infty$, then show that at least one of

$$
\frac1x\left|\sum_{n\leq x}f(n)\right|,
\qquad
\frac1x\left|\sum_{n\leq x}f(n)\mu(n)\right|
$$

tends to zero. Their minimum is consequently $o(1)$, which is the claimed $o(x)$ estimate before normalization.

## 3

↑ **Parent:** [Paper 150](paper-150.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $F(s)=\sum_{n\geq1}a_nn^{-s}$ converge absolutely for $\Re s>\sigma_a$. [Perron formula](../../../analytic-number-theory.md#perron-s-formula) states that for $c>\sigma_a$ and nonintegral $x>0$,

$$
\sum_{n\leq x}a_n
=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}
F(s)\frac{x^s}{s}\,ds,
$$

where the integral is understood as the limit of symmetric truncations under the usual convergence hypotheses. If $x$ is an integer, the endpoint term is counted with weight $1/2$. Effective versions truncate at height $T$ and include an explicit error depending on the coefficients and the distance of $x$ from nearby integers.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $t=s-1$. The [Laurent series](../../../analysis.md#laurent-series) of the [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) at the simple pole of $\zeta$ has the form

$$
\frac{\zeta'(s)}{\zeta(s)}=-\frac1t+c_0+O(t),
$$

where in fact $c_0=\gamma$. Hence

$$
\left(\frac{\zeta'}\zeta(s)\right)^2
=\frac1{t^2}-\frac{2c_0}{t}+O(1),
\qquad
\frac{x^s}{s}
=x\bigl(1+t(\log x-1)+O(t^2)\bigr).
$$

The coefficient of $t^{-1}$ in their product, and therefore the [residue](../../../analysis.md#residue), is

$$
x(\log x-1-2c_0)=x\log x+Ax,
$$

with the constant $A=-1-2c_0$; equivalently, $A=-1-2\gamma$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Von Mangoldt function](../../../number-theory.md#von-mangoldt-function) is nonnegative and satisfies $\Lambda(m)\leq\log m$. Using the [Von Mangoldt divisor identity](../../../number-theory.md#von-mangoldt-divisor-identity),

$$
(\Lambda*\Lambda)(n)
=\sum_{d\mid n}\Lambda(d)\Lambda(n/d)
\leq\sum_{d\mid n}\Lambda(d)\log(n/d)
\leq\log n\sum_{d\mid n}\Lambda(d)
=(\log n)^2.
$$

For $0<u\leq1$, a comparison with an [improper integral](../../../real-analysis.md#improper-integral) gives

$$
\boxed{\sum_{n=1}^{\infty}\frac{(\log n)^2}{n^{1+u}}
\ll1+\int_1^\infty\frac{(\log t)^2}{t^{1+u}}\,dt
=1+\frac2{u^3}
\ll u^{-3}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For $\Re s>1$, the [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) multiplication rule and $-\zeta'/\zeta(s)=\sum_{n\geq1}\Lambda(n)n^{-s}$ give

$$
\left(\frac{\zeta'(s)}{\zeta(s)}\right)^2
=\sum_{n=1}^{\infty}\frac{(\Lambda*\Lambda)(n)}{n^s}.
$$

Apply an effective [Perron formula](../../../analytic-number-theory.md#perron-s-formula) on the line $\kappa=1+1/\log x$ and truncate at

$$
T=\exp(\sqrt{\log x}).
$$

The bound from part (c) controls the truncation error.

Use the classical [zero-free region of the Riemann zeta function](../../../analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function)

$$
\zeta(s)\ne0
\quad\text{when}\quad
\Re s\geq1-\frac{c_0}{\log(|\Im s|+3)},
$$

together with $\zeta'/\zeta(s)\ll\log^2(|\Im s|+3)$ there. [Contour shifting](../../../complex-analysis.md#contour-shifting) moves the Perron contour to $\Re s=1-c_1/\log T$. The only crossed singularity is the double pole at $s=1$, whose [residue](../../../analysis.md#residue) is $x\log x+Ax$ by part (b). On the new contour,

$$
|x^s|
\leq x\exp\left(-\frac{c_1\log x}{\log T}\right)
=x\exp(-c_1\sqrt{\log x}),
$$

and the logarithmic-derivative bounds contribute only powers of $\log x$, which can be absorbed by reducing the positive constant in the exponential. The horizontal integrals and Perron truncation error are $O(x\exp(-c_2\sqrt{\log x}))$ as well. Therefore, for some $c>0$,

$$
\boxed{\sum_{n\leq x}(\Lambda*\Lambda)(n)
=x\log x+Ax+O\bigl(x\exp(-c\sqrt{\log x})\bigr).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
