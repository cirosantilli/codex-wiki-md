# Paper 22

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper22.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper22.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $\vartheta(x)=\sum_{p\le x}\log p$ for the [Chebyshev theta function](../../../number-theory.md#chebyshev-theta-function) and $\psi(x)=\sum_{p^j\le x}\log p$ for the [Second Chebyshev function](../../../number-theory.md#second-chebyshev-function). Throughout, $p$ denotes a [prime](../../../number-theory.md#prime-number) and all [logarithms](../../../calculus.md#logarithm) are natural. Each [prime](../../../number-theory.md#prime-number) $n<p\le2n$ divides the central [binomial coefficient](../../../combinatorics.md#binomial-coefficient), so

$$
\vartheta(2n)-\vartheta(n)\le\log\binom{2n}{n}\le2n\log2.
$$

Apply this at $n=1,2,4,\ldots,2^{r-1}$ and telescope: $\vartheta(2^r)\le(2^{r+1}-2)\log2$. Bounding a general $x$ by the next power of two proves $\vartheta(x)=O(x)$. Splitting the [prime-counting function](../../../number-theory.md#prime-counting-function) at $\sqrt x$ now gives

$$
\pi(x)\le\sqrt x+\frac2{\log x}\vartheta(x),
\qquad\boxed{\pi(x)=O(x/\log x).}
$$

This is the required [Chebyshev estimate from central binomial coefficients](../../../number-theory.md#chebyshev-estimate-from-central-binomial-coefficients), with no use of a [prime](../../../number-theory.md#prime-number) asymptotic.

The higher [prime powers](../../../number-theory.md#prime-power) also satisfy

$$
\psi(x)=\sum_{1\le j\le\log x/\log2}\vartheta(x^{1/j})
=\vartheta(x)+O(\sqrt x\log x)=O(x).
$$

For an [integer](../../../number-theory.md#integer) $N$, the [prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) of a [factorial](../../../combinatorics.md#factorial) gives

$$
\log N!=\sum_{p^j\le N}\left\lfloor\frac N{p^j}\right\rfloor\log p
=N\sum_{p^j\le N}\frac{\log p}{p^j}+O(\psi(N)).
$$

The [Stirling formula](../../../real-analysis.md#stirling-formula), or integral comparison for $\log t$, says $\log N!=N\log N-N+O(\log N)$. After division by $N$ we obtain $\sum_{p^j\le N}(\log p)/p^j=\log N+O(1)$. Moreover

$$
0\le\sum_{p}\sum_{j\ge2}\frac{\log p}{p^j}
=\sum_p\frac{\log p}{p(p-1)}
\le\sum_{n\ge2}\frac{\log n}{n(n-1)}<\infty.
$$

Subtract this bounded contribution and replace $N$ by $\lfloor x\rfloor$. The [factorial proof of Mertens first theorem](../../../analytic-number-theory.md#factorial-proof-of-mertens-first-theorem) therefore yields

$$
\boxed{A(x):=\sum_{p\le x}\frac{\log p}{p}=\log x+O(1).}
$$

For fixed $\lambda>1$, apply [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) to $A(t)$ and $f(t)=(\log t)^{\lambda-1}$:

$$
\sum_{p\le x}\frac{(\log p)^\lambda}{p}
=A(x)(\log x)^{\lambda-1}
-(\lambda-1)\int_2^x A(t)\frac{(\log t)^{\lambda-2}}t\,dt.
$$

The main contribution is

$$
(\log x)^\lambda-\frac{\lambda-1}{\lambda}(\log x)^\lambda+O(1)
=\frac1\lambda(\log x)^\lambda+O(1).
$$

The bounded error in $A(t)$ contributes $O((\log x)^{\lambda-1})$ at the endpoint and in the integral, since $\int_2^x(\log t)^{\lambda-2}dt/t=O_\lambda((\log x)^{\lambda-1})$. Thus the [positive logarithmic moments of reciprocal primes](../../../analytic-number-theory.md#positive-logarithmic-moments-of-reciprocal-primes) satisfy

$$
\boxed{\sum_{p\le x}\frac{(\log p)^\lambda}{p}
=\frac1\lambda(\log x)^\lambda+O_\lambda((\log x)^{\lambda-1}).}
$$

## 2

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

First continue the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) into $\Re s>0$. Summing the integral of the integer-part function gives, initially for $\Re s>1$,

$$
\zeta(s)=s\int_1^\infty\lfloor u\rfloor u^{-s-1}\,du
=\frac{s}{s-1}-s\int_1^\infty\{u\}u^{-s-1}\,du.
$$

The last integral defines a [holomorphic function](../../../complex-analysis.md#holomorphic-function) for $\Re s>0$, so this continuation has only a simple [pole](../../../isolated-singularity.md#pole) at one, of [residue](../../../analysis.md#residue) one.

For $\sigma>1$, logarithmic expansion of the [Euler product](../../../analytic-number-theory.md#euler-product) and $3+4\cos v+\cos2v=2(1+\cos v)^2\ge0$ give

$$
3\log\zeta(\sigma)+4\log|\zeta(\sigma+it)|+\log|\zeta(\sigma+2it)|
=\sum_p\sum_{j\ge1}\frac{3+4\cos(jt\log p)+\cos(2jt\log p)}{jp^{j\sigma}}\ge0.
$$

This proves the [three-four-one product proof of zeta boundary nonvanishing](../../../analytic-number-theory.md#three-four-one-product-proof-of-zeta-boundary-nonvanishing) inequality

$$
\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\ge1.
$$

If $t\ne0$ and $\zeta(1+it)=0$ to order $r\ge1$, the middle factor is $O((\sigma-1)^{4r})$, the first is $O((\sigma-1)^{-3})$, and the last remains bounded. Their product tends to zero, a contradiction. At $t=0$ there is a [pole](../../../isolated-singularity.md#pole), not a zero. **The zeta function has no zero on $\Re s=1$.**

Put $I(x)=\int_0^x\psi(u)\,du=\sum_{n\le x}(x-n)\Lambda(n)$, where $\Lambda$ is the [Von Mangoldt function](../../../number-theory.md#von-mangoldt-function). Logarithmic differentiation of the [Euler product](../../../analytic-number-theory.md#euler-product) gives $-\zeta'(s)/\zeta(s)=\sum_n\Lambda(n)n^{-s}$ for $\Re s>1$. The [first integral of the Chebyshev function](../../../number-theory.md#first-integral-of-the-chebyshev-function) is consequently

$$
\boxed{I(x)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}
-\frac{\zeta'(s)}{\zeta(s)}\frac{x^{s+1}}{s(s+1)}\,ds,\qquad c>1.}
$$

To check its kernel, evaluate the [contour integral](../../../complex-analysis.md#contour-integral) of $y^s/(s(s+1))$ by closing to the left for $y>1$ and to the right for $0<y<1$. The [residues](../../../analysis.md#residue) at zero and minus one give $1-y^{-1}$ in the first case and zero in the second. Multiplication by $x$ and substitution $y=x/n$ therefore produce $(x-n)_+$. On the line $c>1$, the [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) and vertical integral have [absolute convergence](../../../real-analysis.md#absolute-convergence), justifying their interchange; at $x=n$ the kernel is zero on either side.

Here is the smoothing step that establishes the requested asymptotic. Shift the line of this [contour integral](../../../complex-analysis.md#contour-integral) to the left. The [pole](../../../isolated-singularity.md#pole) of $-\zeta'/\zeta$ at one has [residue](../../../analysis.md#residue) $+1$; at each [Nontrivial zero of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) $\rho$ of [zero multiplicity](../../../complex-analysis.md#multiplicity-of-a-zero) $m_\rho$ its [residue](../../../analysis.md#residue) is $-m_\rho$. The denominators also contribute at zero and minus one, and the [trivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#trivial-zero-of-the-riemann-zeta-function) occur at $-2,-4,\ldots$. Summing these [residues](../../../analysis.md#residue) yields the [smoothed explicit formula for the Chebyshev function](../../../number-theory.md#smoothed-explicit-formula-for-the-chebyshev-function)

$$
I(x)=\frac{x^2}2-\sum_\rho\frac{x^{\rho+1}}{\rho(\rho+1)}
-x\log(2\pi)+\frac{\zeta'(-1)}{\zeta(-1)}
-\sum_{k\ge1}\frac{x^{1-2k}}{2k(2k-1)}.
$$

Zeros are repeated with [zero multiplicity](../../../complex-analysis.md#multiplicity-of-a-zero). For the limits of the [contour integral](../../../complex-analysis.md#contour-integral), choose horizontal heights avoiding zero ordinates, where the logarithmic derivative on each fixed strip is $O((\log T)^2)$. The factor $s(s+1)$ makes their integrals tend to zero. On left edges chosen a fixed distance from the trivial zeros, the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) controls the logarithmic derivative by $O(\log(|s|+2))$; for fixed $x>1$ the remaining vertical integral vanishes as that edge moves left. This is why the extra integration of $\psi$ is useful.

The [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula), stated in Question 3, gives $N(T)=O(T\log T)$, hence

$$
\sum_\rho\frac1{|\rho(\rho+1)|}<\infty.
$$

Indeed each dyadic height block contributes $O((\log T)/T)$. The zero-free line just proved, the nonvanishing [Euler product](../../../analytic-number-theory.md#euler-product) on its right, and the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) put every [Nontrivial zero of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) in $0<\Re\rho<1$. Therefore each $x^{\rho-1}$ tends to zero, with absolute value at most one for $x\ge1$. Divide the explicit formula by $x^2$ and use [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) on the zero terms with [absolute convergence](../../../real-analysis.md#absolute-convergence). The remaining displayed terms are $o(x^2)$, and we obtain

$$
\boxed{I(x)\sim x^2/2.}
$$

Monotonicity of $\psi$ removes the smoothing. For $0<h<1$,

$$
\frac{I(x)-I((1-h)x)}{hx}\le\psi(x)
\le\frac{I((1+h)x)-I(x)}{hx}.
$$

After division by $x$, the limits of the two bounds are $1-h/2$ and $1+h/2$. Let $h\downarrow0$ to get $\psi(x)\sim x$. Question 1 gives $\psi(x)-\vartheta(x)=O(\sqrt x\log x)=o(x)$, so $\vartheta(x)\sim x$. [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) now gives

$$
\pi(x)=\frac{\vartheta(x)}{\log x}+\int_2^x\frac{\vartheta(t)}{t(\log t)^2}\,dt
\sim\frac{x}{\log x}.
$$

The integral is $O(x/(\log x)^2)$, by splitting at $\sqrt x$ and using $\vartheta(t)=O(t)$. Inverting this at $x=p_n$, we have $n\sim p_n/\log p_n$ and hence $\log n\sim\log p_n$. Thus **the $n$th [prime](../../../number-theory.md#prime-number) satisfies**

$$
\boxed{p_n\sim n\log n.}
$$

## 3

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the [Jacobi theta function](../../../modular-function.md#jacobi-theta-function) $\Theta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t}$, $t>0$. Its transformation law follows directly from the [Gaussian Fourier transform](../../../fourier-analysis.md#fourier-transform-of-a-gaussian). With the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat f(\xi)=\int_{\mathbb R}f(u)e^{-2\pi i\xi u}\,du$,

$$
\widehat{e^{-\pi t u^2}}(\xi)=t^{-1/2}e^{-\pi\xi^2/t}.
$$

For example, differentiating the transform and using [integration by parts](../../../calculus.md#integration-by-parts) gives $\widehat f'(\xi)=-(2\pi\xi/t)\widehat f(\xi)$; its value at zero is the [Gaussian integral](../../../calculus.md#gaussian-integral) $t^{-1/2}$. Periodize the Gaussian. Its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) are these transforms at [integer](../../../number-theory.md#integer) frequencies, and both series converge absolutely, so evaluating its [Fourier series](../../../fourier-series.md) at zero proves the [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula) here:

$$
\Theta(t)=t^{-1/2}\Theta(1/t).
$$

For $\Re s>1$, integrating the exponentially convergent series termwise gives the [Mellin representation of the completed Riemann zeta function](../../../analytic-number-theory.md#mellin-representation-of-the-completed-riemann-zeta-function)

$$
\Lambda(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\frac12\int_0^\infty(\Theta(t)-1)t^{s/2-1}\,dt.
$$

Split at one and substitute $u=1/t$ in the lower part, using the transformation just proved. The contribution of $t^{-1/2}-1$ is $1/(s-1)-1/s$. We obtain the [pole-subtracted theta integral for the completed zeta function](../../../analytic-number-theory.md#pole-subtracted-theta-integral-for-the-completed-zeta-function)

$$
\Lambda(s)=\frac1{s-1}-\frac1s
+\frac12\int_1^\infty(\Theta(t)-1)
\left(t^{s/2-1}+t^{(1-s)/2-1}\right)\,dt.
$$

The integral is [entire](../../../complex-analysis.md#entire-function): $\Theta(t)-1$ decays exponentially, uniformly dominating the integrand and all its $s$ derivatives on [compact sets](../../../topology.md#compact-space). Both the rational term and the integral are invariant under $s\mapsto1-s$. This proves the meromorphic identity

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s).}
$$

Equivalently the [Riemann xi function](../../../analytic-number-theory.md#riemann-xi-function)

$$
\xi(s)=\tfrac12s(s-1)\Lambda(s)
$$

is [entire](../../../complex-analysis.md#entire-function) and satisfies $\xi(s)=\xi(1-s)$. The reflection and duplication formulas for the [Gamma function](../../../complex-analysis.md#gamma-function) turn the same identity into

$$
\boxed{\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s),}
$$

understood by [meromorphic continuation](../../../complex-analysis.md#meromorphic-continuation) at removable exceptional points. This establishes the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function), rather than assuming it.

If $N(T)$ counts zeros $\rho=\beta+i\gamma$ in the [critical strip](../../../analytic-number-theory.md#critical-strip) with $0<\gamma\le T$, **including [zero multiplicity](../../../complex-analysis.md#multiplicity-of-a-zero)**, the [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula) is

$$
\boxed{N(T)=\frac{T}{2\pi}\log\frac{T}{2\pi}-\frac{T}{2\pi}+O(\log T).}
$$

At a zero ordinate one may instead use the conventional half-weight boundary count; that only alters the stated error. In particular $N(T)\sim T\log T/(2\pi)$.

To invert without assuming simple zeros, fix $0<\varepsilon<1$ and set $T_n^\pm=(1\pm\varepsilon)2\pi n/\log n$. Then $\log T_n^\pm/\log n\to1$, so

$$
\frac{N(T_n^\pm)}n\longrightarrow1\pm\varepsilon.
$$

For large $n$, $N(T_n^-)<n<N(T_n^+)$, and hence $T_n^-<\gamma_n\le T_n^+$. Let $\varepsilon\downarrow0$. The [asymptotic inversion of the zeta zero count](../../../analytic-number-theory.md#asymptotic-inversion-of-the-zeta-zero-count) gives

$$
\boxed{\gamma_n\sim\frac{2\pi n}{\log n}.}
$$

As in the zero-counting formula, the sequence lists ordinates with [zero multiplicity](../../../complex-analysis.md#multiplicity-of-a-zero); “increasing” means nondecreasing here. The argument does not require the [Riemann hypothesis](../../../analytic-number-theory.md#riemann-hypothesis) or simplicity of zeros.

## 4

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Selberg upper-bound sieve](../../../analytic-number-theory.md#selberg-upper-bound-sieve) replaces an exact but long inclusion-exclusion expansion by a short nonnegative square, and then minimizes its main term. For an interval $\mathcal A=(a,a+x]\cap\mathbb Z$, the count of multiples of every [integer](../../../number-theory.md#integer) $d$ is

$$
|\mathcal A_d|=\left\lfloor\frac{a+x}d\right\rfloor-\left\lfloor\frac ad\right\rfloor
=\frac xd+r_d,\qquad |r_d|\le1.
$$

Crucially the remainder bound is independent of $a$.

Let $P(z)=\prod_{p\le z}p$ and take real weights $\lambda_d$, supported on [squarefree](../../../number-theory.md#squarefree-integer) $d\le z$, with $\lambda_1=1$. If $(n,P(z))=1$, the sum of these weights over [divisors](../../../number-theory.md#divisor) of $n$ is just one; for all other $n$ its square is nonnegative. Thus

$$
\mathbf1_{(n,P(z))=1}\le\left(\sum_{d\mid n}\lambda_d\right)^2.
$$

Expanding and counting common multiples gives

$$
S(\mathcal A,z)\le xQ(\lambda)+\left(\sum_{d\le z}|\lambda_d|\right)^2,
\qquad Q(\lambda)=\sum_{d,e\le z}\frac{\lambda_d\lambda_e}{[d,e]}.
$$

This separates the local density $1/[d,e]$ from a uniform interval error. The weights will be chosen to minimize $Q$.

The [Euler totient function](../../../number-theory.md#euler-totient-function) identity $(d,e)=\sum_{r\mid d,\ r\mid e}\varphi(r)$ yields the [Selberg sieve diagonalization](../../../analytic-number-theory.md#selberg-sieve-diagonalization)

$$
Q(\lambda)=\sum_{r\le z}\varphi(r)y_r^2,
\qquad y_r=\sum_{\substack{d\le z\\r\mid d}}\frac{\lambda_d}{d}.
$$

Only [squarefree](../../../number-theory.md#squarefree-integer) $r$ occur. Inverting this finite triangular sum by [Möbius inversion](../../../number-theory.md#mobius-inversion-formula) gives

$$
\frac{\lambda_d}d=\sum_{\substack{r\le z\\d\mid r}}\mu(r/d)y_r,
\qquad1=\lambda_1=\sum_{r\le z}\mu(r)y_r.
$$

Write $G(z)=\sum_{r\le z}\mu(r)^2/\varphi(r)$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $1\le G(z)Q(\lambda)$, with equality at $y_r=\mu(r)/(\varphi(r)G(z))$. The inverse formula then produces the optimal [Selberg sieve weights](../../../analytic-number-theory.md#selberg-sieve-weights)

$$
\lambda_d=\mu(d)\frac{d}{\varphi(d)}\frac{G_d(z/d)}{G(z)},
\qquad G_d(v)=\sum_{\substack{\ell\le v\\(\ell,d)=1}}\frac{\mu(\ell)^2}{\varphi(\ell)},
\qquad Q(\lambda)=\frac1{G(z)}.
$$

The constraints are satisfied, since the diagonal transformation is invertible and $\sum_r\mu(r)y_r=1$.

We need the leading constant, not just $G(z)\gg\log z$. Here is an elementary proof of the [Selberg sieve denominator asymptotic](../../../analytic-number-theory.md#selberg-sieve-denominator-asymptotic). For $g(n)=\mu(n)^2/\varphi(n)$ define the [multiplicative arithmetic function](../../../number-theory.md#multiplicative-function) $h$ by

$$
h(p)=\frac1{p(p-1)},\qquad h(p^2)=-\frac1{p(p-1)},\qquad h(p^j)=0\quad(j\ge3).
$$

Checking the prime-local factors shows $g=h*(n\mapsto1/n)$. Also $\sum_n|h(n)|\log(2n)<\infty$: the local factors for absolute values differ from one by $O(p^{-2})$, and their logarithmic first moments sum $O((\log p)/p^2)$. The signed local sums are all one, so [absolute convergence](../../../real-analysis.md#absolute-convergence) gives $\sum_nh(n)=1$. Using the [harmonic number](../../../analytic-number-theory.md#harmonic-number) estimate,

$$
G(z)=\sum_{d\le z}h(d)H_{\lfloor z/d\rfloor}
=\sum_{d\le z}h(d)\log(z/d)+O(1)=\log z+O(1).
$$

For the last equality, $\sum|h(d)|\log d$ is bounded and $\log z\sum_{d>z}|h(d)|\le\sum_{d>z}|h(d)|\log d$ is bounded too.

The [optimal Selberg weights have modulus at most one](../../../analytic-number-theory.md#optimal-selberg-weights-have-modulus-at-most-one). To prove this here, for [squarefree](../../../number-theory.md#squarefree-integer) $d$ use $d/\varphi(d)=\sum_{e\mid d}1/\varphi(e)$. The product $(d/\varphi(d))G_d(z/d)$ is the sum of $1/\varphi(e\ell)$ over $e\mid d$, $\ell\le z/d$, $(\ell,d)=1$, with $\ell$ [squarefree](../../../number-theory.md#squarefree-integer). All $e\ell$ are distinct [squarefree integers](../../../number-theory.md#squarefree-integer) at most $z$, and so these are a subset of the terms of $G(z)$. The displayed weight formula now gives $|\lambda_d|\le1$. Consequently

$$
S(\mathcal A,z)\le\frac{x}{G(z)}+z^2.
$$

Every [prime](../../../number-theory.md#prime-number) in the interval exceeding $z$ survives the sieve; at most $z$ smaller [primes](../../../number-theory.md#prime-number) must be restored. Choose $z=\lfloor\sqrt x/(\log x)^2\rfloor$. Then

$$
\log z=\tfrac12\log x-2\log\log x+o(1),\qquad
z+z^2=o(x/\log x),
$$

and the [uniform interval bound from optimal Selberg weights](../../../analytic-number-theory.md#uniform-interval-bound-from-optimal-selberg-weights) follows:

$$
\pi(a+x)-\pi(a)\le\frac{x}{G(z)}+z^2+z
=\left(2+O\left(\frac{\log\log x}{\log x}\right)\right)\frac{x}{\log x}.
$$

All constants are independent of $a$. Given $\varepsilon>0$, make the absolute error in the coefficient smaller than $\varepsilon/2$ by choosing $x_0(\varepsilon)$ large enough. **Uniformly for every $a>0$ and $x>x_0(\varepsilon)$,**

$$
\boxed{\pi(a+x)-\pi(a)<(2+\varepsilon)\frac{x}{\log x}.}
$$

## 5

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Fix a modulus $q$ and a [residue class](../../../number-theory.md#residue-class) $a$ with $(a,q)=1$. The [Dirichlet characters](../../../algebraic-number-theory.md#dirichlet-character) modulo $q$ are the one-dimensional [characters of a representation](../../../representation-theory.md#character-of-a-representation) of $(\mathbb Z/q\mathbb Z)^\times$, extended by zero on nonunits. Let $\chi_0$ be the [principal Dirichlet character](../../../algebraic-number-theory.md#principal-dirichlet-character).

For every [nonprincipal Dirichlet character](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character) the [partial sums](../../../real-analysis.md#partial-sum) $\sum_{n\le u}\chi(n)$ are bounded: the sum over a full period is zero, and a remaining incomplete period has bounded length. [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) therefore continues its [Dirichlet L-function](../../../algebraic-number-theory.md#dirichlet-l-function) holomorphically to $\Re s>0$ by

$$
L(s,\chi)=s\int_1^\infty\left(\sum_{n\le u}\chi(n)\right)u^{-s-1}\,du.
$$

This shows in particular that it has no [pole](../../../isolated-singularity.md#pole) at one. By contrast

$$
L(s,\chi_0)=\zeta(s)\prod_{p\mid q}(1-p^{-s})
$$

has a simple [pole](../../../isolated-singularity.md#pole) there. We use the stipulated nonvanishing $L(1,\chi)\ne0$ for every real [nonprincipal Dirichlet character](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character), and establish the remaining nonvanishing as follows.

For real $\sigma>1$, take the [product over all Dirichlet characters](../../../algebraic-number-theory.md#product-over-all-dirichlet-characters). The [Euler product](../../../analytic-number-theory.md#euler-product) [logarithms](../../../calculus.md#logarithm) and [Orthogonality of Dirichlet characters](../../../algebraic-number-theory.md#orthogonality-of-dirichlet-characters) give

$$
\log\prod_{\chi\bmod q}L(\sigma,\chi)
=\sum_{p\nmid q}\sum_{j\ge1}\frac{\sum_\chi\chi(p)^j}{jp^{j\sigma}}
=\varphi(q)\sum_{p\nmid q}\sum_{\substack{j\ge1\\p^j\equiv1\pmod q}}\frac1{jp^{j\sigma}}\ge0.
$$

Thus this product is real and at least one. If a nonreal [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character) had $L(1,\chi)=0$, [complex conjugation](../../../complex-analysis.md#complex-conjugation) would also give $L(1,\overline\chi)=0$. These are distinct factors. Two zeros and only one possible simple [pole](../../../isolated-singularity.md#pole) force the whole product to tend to zero as $\sigma\downarrow1$, contradicting the lower bound. Hence **all [nonprincipal Dirichlet characters](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character) have $L(1,\chi)\ne0$**, under the given real-character assumption.

For $\sigma>1$, [absolute convergence](../../../real-analysis.md#absolute-convergence) of each [Euler product](../../../analytic-number-theory.md#euler-product) gives

$$
\log L(\sigma,\chi)
=\sum_{p\nmid q}\frac{\chi(p)}{p^\sigma}+O(1),
$$

with bounded remainder as $\sigma\downarrow1$: the terms of prime-power exponent at least two have total modulus at most $\sum_{n\ge2}1/(n(n-1))$. Since a nonprincipal $L$ defines a [holomorphic function](../../../complex-analysis.md#holomorphic-function) that is nonzero near one, its Euler-product [logarithm](../../../calculus.md#logarithm) differs from a local [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm) by a fixed [integer](../../../number-theory.md#integer) multiple of $2\pi i$ on a short real interval. It is therefore bounded there. For the [principal Dirichlet character](../../../algebraic-number-theory.md#principal-dirichlet-character) the [pole](../../../isolated-singularity.md#pole) instead gives

$$
\log L(\sigma,\chi_0)=\log\frac1{\sigma-1}+O_q(1).
$$

Apply the [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character) orthogonality relation at each [prime](../../../number-theory.md#prime-number). The [prime-character sum near one](../../../analytic-number-theory.md#prime-character-sum-near-one) yields

$$
\sum_{p\equiv a\pmod q}p^{-\sigma}
=\frac1{\varphi(q)}\sum_{\chi\bmod q}\overline{\chi(a)}\log L(\sigma,\chi)+O_q(1)
=\frac1{\varphi(q)}\log\frac1{\sigma-1}+O_q(1).
$$

This tends to infinity. A finite set of [primes](../../../number-theory.md#prime-number) would have a bounded sum as $\sigma\downarrow1$, so **every [coprime](../../../number-theory.md#coprime-integers) [residue class](../../../number-theory.md#residue-class) contains infinitely many [primes](../../../number-theory.md#prime-number)**. This proves the [Dirichlet theorem on primes in arithmetic progressions](../../../analytic-number-theory.md#dirichlet-s-theorem-on-arithmetic-progressions) from the specified assumption. In fact it proves divergence of the corresponding reciprocal-prime series and gives [Dirichlet density](../../../algebraic-number-theory.md#dirichlet-density) $1/\varphi(q)$.

Finally, for real $s>1$ each [prime](../../../number-theory.md#prime-number) satisfies

$$
p^{-s}=s\int_p^\infty t^{-s-1}\,dt.
$$

The integrands are nonnegative, so [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) permits summation inside the integral. At a fixed $t$, exactly $\pi(t,q,a)$ [primes](../../../number-theory.md#prime-number) from the [residue class](../../../number-theory.md#residue-class) have entered. Therefore

$$
\boxed{\sum_{p\equiv a\pmod q}\frac1{p^s}
=s\int_1^\infty\frac{\pi(t,q,a)}{t^{s+1}}\,dt.}
$$

Both sides are finite, since they are bounded respectively by $\sum_{n\ge2}n^{-s}$ and $s\int_1^\infty t^{-s}\,dt$. The values of a counting function at its isolated jump endpoints do not change this integral.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
