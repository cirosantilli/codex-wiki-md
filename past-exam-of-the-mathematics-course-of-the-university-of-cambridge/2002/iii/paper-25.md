# Paper 25

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper25.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper25.pdf)

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

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $\theta(x)=\sum_{p\le x}\log p$ for the [Chebyshev theta function](../../../number-theory.md#chebyshev-theta-function) and $\psi(x)=\sum_{n\le x}\Lambda(n)$ for the [Second Chebyshev function](../../../number-theory.md#second-chebyshev-function), where $\Lambda$ is the [Von Mangoldt function](../../../number-theory.md#von-mangoldt-function). We first establish the [Chebyshev estimate](../../../number-theory.md#chebyshev-estimate). Every [prime](../../../number-theory.md#prime-number) $n<p\le2n$ divides the [central binomial coefficient](../../../combinatorics.md#central-binomial-coefficient) $\binom{2n}{n}$, so

$$
\theta(2n)-\theta(n)\le\log\binom{2n}{n}\le2n\log2.
$$

Apply this at successive powers of two and use [monotonicity](../../../calculus.md#monotonic-function) to obtain $\theta(x)=O(x)$. Since

$$
\psi(x)=\sum_{r\ge1}\theta(x^{1/r}),
$$

the terms $r\ge2$ contribute $O(\sqrt x\log x)$ and therefore $\psi(x)=O(x)$. This [Chebyshev estimate from central binomial coefficients](../../../number-theory.md#chebyshev-estimate-from-central-binomial-coefficients) is all the information about the distribution of [primes](../../../number-theory.md#prime-number) needed here.

The [Von Mangoldt divisor identity](../../../number-theory.md#von-mangoldt-divisor-identity) $\log n=\sum_{d\mid n}\Lambda(d)$ gives the [factorial proof of Mertens first theorem](../../../analytic-number-theory.md#factorial-proof-of-mertens-first-theorem). With $N=\lfloor x\rfloor$, interchange the finite sums to obtain

$$
\log N!=\sum_{d\le x}\Lambda(d)\left\lfloor\frac xd\right\rfloor
=x\sum_{d\le x}\frac{\Lambda(d)}d+O(\psi(x)).
$$

Comparison of $\sum_{n\le N}\log n$ with $\int_1^N\log t\,dt$ gives $\log N!=N\log N-N+O(\log N)$. Dividing the preceding identity by $x$, using $N=x+O(1)$ and the [Chebyshev estimate](../../../number-theory.md#chebyshev-estimate), gives

$$
\sum_{d\le x}\frac{\Lambda(d)}d=\log x+O(1).
$$

The contribution of higher [prime powers](../../../number-theory.md#prime-power) is bounded independently of $x$, because

$$
\sum_p\sum_{r\ge2}\frac{\log p}{p^r}
=\sum_p\frac{\log p}{p(p-1)}
\le\sum_{n\ge2}\frac{\log n}{n(n-1)}<\infty.
$$

Thus the [Mertens first theorem](../../../analytic-number-theory.md#mertens-first-theorem) is

$$
\boxed{A(x):=\sum_{p\le x}\frac{\log p}{p}=\log x+O(1).}
$$

For the [square-root logarithmic sum over primes](../../../analytic-number-theory.md#square-root-logarithmic-sum-over-primes), apply [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) to $A(t)$ with weight $(\log t)^{-1/2}$. The lower endpoint is understood as $A(2^-)=0$, so

$$
\sum_{p\le x}\frac{\sqrt{\log p}}p
=\frac{A(x)}{\sqrt{\log x}}
+\frac12\int_2^x\frac{A(t)}{t(\log t)^{3/2}}\,dt.
$$

The main terms are $\sqrt{\log x}$ and $\sqrt{\log x}-\sqrt{\log2}$. The bounded error in $A(t)$ produces a bounded integral, since $\int_2^\infty dt/(t(\log t)^{3/2})<\infty$. Therefore

$$
\boxed{\sum_{p\le x}\frac{\sqrt{\log p}}p=2\sqrt{\log x}+O(1).}
$$

Neither argument uses the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem).

## 2

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

**First alternative.** The [Euler product](../../../analytic-number-theory.md#euler-product) of the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) is absolutely convergent for $\sigma>1$. Its [logarithm](../../../calculus.md#logarithm) and the nonnegative [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial)

$$
3+4\cos u+\cos2u=2(1+\cos u)^2
$$

give

$$
3\log\zeta(\sigma)+4\log|\zeta(\sigma+it)|+\log|\zeta(\sigma+2it)|
=\sum_p\sum_{m\ge1}\frac{3+4\cos(mt\log p)+\cos(2mt\log p)}{mp^{m\sigma}}\ge0.
$$

Consequently $\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\ge1$. Suppose $t\ne0$ and the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) had a [zero](../../../polynomial.md#zero-of-a-function) of order $m\ge1$ at $1+it$. As $\sigma\downarrow1$, its simple [pole](../../../isolated-singularity.md#pole) at one gives $\zeta(\sigma)=O((\sigma-1)^{-1})$, the alleged [zero](../../../polynomial.md#zero-of-a-function) gives $\zeta(\sigma+it)=O((\sigma-1)^m)$, and $\zeta(\sigma+2it)$ remains bounded. The product would be $O((\sigma-1)^{4m-3})\to0$, contradicting its lower bound. Thus **there are no zeta [zeros](../../../polynomial.md#zero-of-a-function) on $\Re s=1$**; the point $s=1$ itself is a [pole](../../../isolated-singularity.md#pole), not a [zero](../../../polynomial.md#zero-of-a-function).

For the [first integral of the Chebyshev function](../../../number-theory.md#first-integral-of-the-chebyshev-function), define

$$
\Psi_1(x)=\int_0^x\psi(u)\,du=\sum_{n\le x}(x-n)\Lambda(n).
$$

The [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) identity $-\zeta'/\zeta(s)=\sum_n\Lambda(n)n^{-s}$, valid for $\Re s>1$, leads to

$$
\boxed{\Psi_1(x)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}
-\frac{\zeta'(s)}{\zeta(s)}\frac{x^{s+1}}{s(s+1)}\,ds,\qquad c>1.}
$$

To verify the kernel rather than assume an inversion formula, integrate $y^s/(s(s+1))$ on the vertical line $\Re s=c$. Closing to the left when $y>1$ gives the [residues](../../../analysis.md#residue) at [zero](../../../polynomial.md#zero-of-a-function) and minus one, namely $1-y^{-1}$; closing to the right when $0<y<1$ gives [zero](../../../polynomial.md#zero-of-a-function). At $y=1$ the integral is [zero](../../../polynomial.md#zero-of-a-function) as well. The horizontal integrals tend to [zero](../../../polynomial.md#zero-of-a-function) because of the quadratic denominator, and the distant vertical integrals vanish in the indicated direction. Multiplying this kernel by $x$ with $y=x/n$ gives $(x-n)^+$. The [absolute convergence](../../../real-analysis.md#absolute-convergence) of the [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) on $\Re s=c$, together with the integrable denominator, permits interchange with the integral and proves the formula.

Here is a quantitative contour route from this relation to the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem). Question 3 establishes a [zero-free region of the Riemann zeta function](../../../analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function) and the accompanying bounds for its [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative), independently of the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem). In a sufficiently narrow half-width region they imply

$$
\left|\frac{\zeta'(s)}{\zeta(s)}\right|\ll\log^2(T+3)
$$

on the left and horizontal sides of the rectangle with heights $\pm T$ and left edge $\sigma_L=1-b/(2\log(T+3))$, after making $b>0$ small enough also for bounded heights. The explanation of this bound is included at the end of Question 3. Take $c=1+1/\log x$ and $T=\exp(\sqrt{\log x})$. On the original line, the omitted tails are

$$
O\left(\frac{x^2\log x}{T}\right),
$$

since the [Euler product](../../../analytic-number-theory.md#euler-product) bounds $|\zeta'/\zeta(c+it)|$ by $-\zeta'/\zeta(c)=O(\log x)$. Shift the truncated integral to the left edge. The only enclosed [pole](../../../isolated-singularity.md#pole) is at $s=1$, with [residue](../../../analysis.md#residue) $x^2/2$; the kernel [poles](../../../isolated-singularity.md#pole) at [zero](../../../polynomial.md#zero-of-a-function) and minus one lie outside the rectangle. The left edge contributes $O(x^{2-b/(2\log(T+3))}\log^2(T+3))$, since $|s(s+1)|^{-1}\ll(1+t^2)^{-1}$ there. The two horizontal edges contribute $O(x^2\log^2(T+3)/T^2)$. In particular, for some $a>0$,

$$
\Psi_1(x)=\frac{x^2}{2}+O\left(x^2e^{-a\sqrt{\log x}}\right),
\qquad\text{so}\qquad\Psi_1(x)\sim\frac{x^2}{2}.
$$

It remains to remove the smoothing; differentiating an asymptotic formula would not justify this step. The [monotonicity](../../../calculus.md#monotonic-function) of the [Second Chebyshev function](../../../number-theory.md#second-chebyshev-function) gives, for $h=\varepsilon x$ with $0<\varepsilon<1$,

$$
\frac{\Psi_1(x)-\Psi_1(x-h)}h\le\psi(x)
\le\frac{\Psi_1(x+h)-\Psi_1(x)}h.
$$

First let $x\to\infty$ with $\varepsilon$ fixed. After division by $x$, the lower and upper bounds tend to $1-\varepsilon/2$ and $1+\varepsilon/2$. Let $\varepsilon\downarrow0$ to obtain $\psi(x)\sim x$. Higher [prime powers](../../../number-theory.md#prime-power) contribute $O(\sqrt x\log x)$ by the [Chebyshev estimate](../../../number-theory.md#chebyshev-estimate), so $\theta(x)\sim x$. Finally [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
\pi(x)=\frac{\theta(x)}{\log x}+\int_2^x\frac{\theta(t)}{t(\log t)^2}\,dt
\sim\frac{x}{\log x}.
$$

The integral is $O(x/\log^2x)$, by splitting at $\sqrt x$ and using $\theta(t)=O(t)$. This proves the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem) with **$\pi(x)\sim x/\log x$**.

**Second alternative.** We prove the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) from a [theta function](../../../modular-function.md#theta-function). Set $\Theta(u)=\sum_{n\in\mathbb Z}e^{-\pi n^2u}$ for $u>0$. With [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat f(\xi)=\int_{\mathbb R}f(v)e^{-2\pi iv\xi}\,dv$, the [Gaussian function](../../../calculus.md#gaussian-function) $f(v)=e^{-\pi uv^2}$ has

$$
\widehat f(\xi)=u^{-1/2}e^{-\pi\xi^2/u}.
$$

Indeed, differentiation under the integral and [integration by parts](../../../calculus.md#integration-by-parts) give $\widehat f'(\xi)=-2\pi\xi\widehat f(\xi)/u$, while the [Gaussian integral](../../../calculus.md#gaussian-integral) gives $\widehat f(0)=u^{-1/2}$. Periodize $f$: the smooth period-one function $\sum_n f(v+n)$ has [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) $\widehat f(k)$, by integrating on $[0,1]$ and interchanging its absolutely convergent sum with the integral. Its absolutely convergent [Fourier series](../../../fourier-series.md), evaluated at [zero](../../../polynomial.md#zero-of-a-function), proves the [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula) in this case. Hence

$$
\Theta(u)=u^{-1/2}\Theta(1/u).
$$

For $\Re s>1$, termwise integration and the defining integral of the [Gamma function](../../../complex-analysis.md#gamma-function) give the [Mellin representation of the completed Riemann zeta function](../../../analytic-number-theory.md#mellin-representation-of-the-completed-riemann-zeta-function):

$$
Z(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\frac12\int_0^\infty(\Theta(u)-1)u^{s/2-1}\,du.
$$

Split at one and substitute $u=1/v$ in the lower integral. The elementary part is

$$
\frac12\int_0^1(u^{-1/2}-1)u^{s/2-1}\,du
=\frac1{s-1}-\frac1s=\frac1{s(s-1)},
$$

and the remaining part becomes an integral over $[1,\infty)$. Thus

$$
Z(s)=\frac1{s(s-1)}+\frac12\int_1^\infty(\Theta(u)-1)
\left(u^{s/2-1}+u^{(1-s)/2-1}\right)\,du.
$$

The integral is an [entire function](../../../complex-analysis.md#entire-function) of $s$, because $\Theta(u)-1$ decays exponentially and [uniform convergence](../../../real-analysis.md#uniform-convergence) holds on every compact subset of the [complex plane](../../../complex-analysis.md#complex-plane). This proves [meromorphic continuation](../../../complex-analysis.md#meromorphic-continuation) of the [completed Riemann zeta function](../../../analytic-number-theory.md#completed-riemann-zeta-function), with only the displayed simple [poles](../../../isolated-singularity.md#pole), and the right side is invariant under $s\mapsto1-s$. Therefore

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s).}
$$

The [Gamma reflection formula](../../../complex-analysis.md#gamma-reflection-formula) and [Gamma duplication formula](../../../complex-analysis.md#gamma-duplication-formula) give the equivalent form $\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s)$, understood by [meromorphic continuation](../../../complex-analysis.md#meromorphic-continuation). Multiplication by $s(s-1)/2$ gives the [entire](../../../complex-analysis.md#entire-function) [Riemann xi function](../../../analytic-number-theory.md#riemann-xi-function) $\xi(s)=\xi(1-s)$.

Let $N(T)$ count positive ordinates of [Nontrivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) up to height $T$, including [multiplicity](../../../polynomial.md#multiplicity-mathematics). The [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula) is

$$
N(T)=\frac{T}{2\pi}\log\frac{T}{2\pi}-\frac{T}{2\pi}+O(\log T).
$$

More precisely, away from ordinates of [zeros](../../../polynomial.md#zero-of-a-function), the constant term is $7/8$, the additional term is $S(T)=\pi^{-1}\arg\zeta(1/2+iT)$, and the remaining error is $O(T^{-1})$. Here the argument is continued along $2\to2+iT\to1/2+iT$, and $S(T)=O(\log T)$. The coarse formula displayed above holds at all large heights with the usual right-continuous counting convention. Subtract it at $T+1$ and $T$: the main term changes by $O(\log T)$ and each error is $O(\log T)$. Hence

$$
\boxed{N(T+1)-N(T)\ll\log T.}
$$

For [infinitely many reciprocal-logarithmic gaps between zeta zeros](../../../analytic-number-theory.md#infinitely-many-reciprocal-logarithmic-gaps-between-zeta-zeros), fix any $0<c<2\pi$, for example $c=\pi$. Suppose all sufficiently late gaps satisfied $\gamma_{n+1}-\gamma_n\le c/\log n$. Summing and using

$$
\sum_{j=2}^{n}\frac1{\log j}\sim\frac n{\log n}
$$

gives $\gamma_n\le(c+o(1))n/\log n$. The last elementary estimate follows by integral comparison with $1/\log t$ and one [integration by parts](../../../calculus.md#integration-by-parts). The [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula) would imply

$$
n\le N(\gamma_n)\le\left(\frac c{2\pi}+o(1)\right)n,
$$

a contradiction. This reasoning is valid whether repeated ordinates are listed according to [multiplicity](../../../polynomial.md#multiplicity-mathematics) or only distinct ordinates are listed, since in either case $n\le N(\gamma_n)$. Consequently **$\gamma_{n+1}-\gamma_n>c/\log n$ infinitely often**, for any fixed $0<c<2\pi$.

## 3

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write $s=\sigma+it$ and let $\rho=\beta+i\gamma$ run over [Nontrivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function), including [multiplicity](../../../polynomial.md#multiplicity-mathematics). The bounds involving $\log|t|$ below are for $|t|\ge3$. At bounded heights their uniform versions use $\log(|t|+3)$; $\log|t|$ itself cannot be the right bound near [zero](../../../polynomial.md#zero-of-a-function) or $|t|=1$.

Start with the [Hadamard factorization](../../../complex-analysis.md#hadamard-factorization-theorem) of the [Riemann xi function](../../../analytic-number-theory.md#riemann-xi-function), an [entire function](../../../complex-analysis.md#entire-function) of order one. Its [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) has the convergent expansion

$$
\frac{\xi'}{\xi}(s)=B+\sum_\rho\left(\frac1{s-\rho}+\frac1\rho\right).
$$

Differentiating $\xi(s)=\tfrac12s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s)$ gives

$$
\frac{\zeta'}{\zeta}(s)
=B+\sum_\rho\left(\frac1{s-\rho}+\frac1\rho\right)
-\frac1s-\frac1{s-1}+\frac12\log\pi-\frac12\frac{\Gamma'}{\Gamma}(s/2).
$$

The real sum of $1/\rho$ converges absolutely: $0\le\beta\le1$ makes its terms $O(\gamma^{-2})$ at large height, and the order-one [Hadamard factorization](../../../complex-analysis.md#hadamard-factorization-theorem) ensures the required summability. Thus these terms and $\Re B$ form a fixed constant. The [Stirling formula](../../../real-analysis.md#stirling-formula) for the [digamma function](../../../complex-analysis.md#digamma-function) gives, uniformly for $1<\sigma\le2$ and $|t|\ge3$,

$$
F(\sigma+it):=-\Re\frac{\zeta'}{\zeta}(\sigma+it)
=\frac12\log|t|-\sum_\rho\frac{\sigma-\beta}{(\sigma-\beta)^2+(t-\gamma)^2}+O(1).
$$

This is the useful real form of the [global partial-fraction expansion of the zeta logarithmic derivative](../../../analytic-number-theory.md#global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative). Every term subtracted is nonnegative because the [Euler product](../../../analytic-number-theory.md#euler-product) excludes [zeros](../../../polynomial.md#zero-of-a-function) with $\beta>1$. At the simple [pole](../../../isolated-singularity.md#pole) $s=1$, one also has $F(\sigma)=1/(\sigma-1)+O(1)$ as $\sigma\downarrow1$.

The [three-four-one zero-free-region argument](../../../analytic-number-theory.md#three-four-one-zero-free-region-argument) now detects a [zero](../../../polynomial.md#zero-of-a-function) too close to one. The [Von Mangoldt function](../../../number-theory.md#von-mangoldt-function) is nonnegative and the absolutely convergent [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) gives

$$
0\le3F(\sigma)+4F(\sigma+it)+F(\sigma+2it),
$$

because the corresponding coefficient at $n$ is $\Lambda(n)n^{-\sigma}[3+4\cos(t\log n)+\cos(2t\log n)]$. If $\beta+it$ is a [zero](../../../polynomial.md#zero-of-a-function), retain its term in the expansion at height $t$ and discard the other nonpositive terms. The expansion at height $2t$ gives an upper bound even without retaining a particular [zero](../../../polynomial.md#zero-of-a-function). We obtain, for an absolute constant $C_0>0$,

$$
\frac4{\sigma-\beta}\le\frac3{\sigma-1}+C_0\log|t|.
$$

Choose $0<a<1$ so small that $5/(9a)>C_0$, put $b=a/8$, and take $\sigma=1+a/\log|t|$. If $1-\beta\le b/\log|t|$, the last inequality would require

$$
\frac{32}{9a}\le\frac3a+C_0,
\qquad\text{or}\qquad\frac5{9a}\le C_0,
$$

a contradiction. Therefore

$$
\boxed{\zeta(\sigma+it)\ne0\quad\text{for}\quad
\sigma>1-\frac b{\log|t|},\quad |t|\ge3,}
$$

for some fixed $b>0$. This proves the required [zero-free region of the Riemann zeta function](../../../analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function). Nonvanishing on $\Re s=1$ at bounded nonzero heights, proved in Question 2, and the isolation of [zeros](../../../polynomial.md#zero-of-a-function) allow a decrease of $b$ giving the uniform formulation with $\log(|t|+3)$ as well. Near $s=1$, apply this observation to the nonzero [holomorphic function](../../../complex-analysis.md#holomorphic-function) $(s-1)\zeta(s)$.

Next evaluate the real expansion at $\sigma=2$. The absolutely convergent [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) bounds $|\zeta'/\zeta(2+it)|\le\sum_n\Lambda(n)n^{-2}$ uniformly in $t$, so

$$
\sum_\rho\frac{2-\beta}{(2-\beta)^2+(t-\gamma)^2}
=\frac12\log|t|+O(1).
$$

Since $1\le2-\beta\le2$, each term on the left is at least $1/[4+(t-\gamma)^2]$. The [smoothed zeta zero-count bound](../../../analytic-number-theory.md#smoothed-zeta-zero-count-bound) follows:

$$
\boxed{\sum_\rho\frac1{4+(t-\gamma)^2}\ll\log|t|.}
$$

Each [zero](../../../polynomial.md#zero-of-a-function) satisfying $|t-\gamma|<1$ contributes more than $1/5$, so this also gives the [local zero count for the Riemann zeta function](../../../analytic-number-theory.md#local-zero-count-for-the-riemann-zeta-function):

$$
\boxed{\#\{\rho:|t-\Im\rho|<1\}\ll\log|t|.}
$$

The same kernel sum is bounded at compact heights, since its tail converges uniformly there; the bounds with $\log(|t|+3)$ are consequently valid for all real $t$.

For completeness, the contour estimate used in Question 2 follows from these very formulas. Subtract the complex [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) expansion at $2+it$ from that at $\sigma+it$, with $1-b/(2\log(T+3))\le\sigma\le2$ and $|t|\le T$. Terms with $|t-\gamma|>1$ have differences $O((t-\gamma)^{-2})$, whose sum is $O(\log(|t|+3))$ by the kernel bound. There are $O(\log(|t|+3))$ remaining terms. After reducing $b$, the [zero-free region of the Riemann zeta function](../../../analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function) separates every such [zero](../../../polynomial.md#zero-of-a-function) horizontally from the half-width boundary by $\gg1/\log(T+3)$: their heights satisfy $|\gamma|\le T+1$. Thus on the left edge, and on the horizontal edges at $t=\pm T$, each reciprocal is $O(\log(T+3))$. The [Gamma function](../../../complex-analysis.md#gamma-function) and [pole](../../../isolated-singularity.md#pole) terms satisfy the same required bound; at small heights on the left edge the [pole](../../../isolated-singularity.md#pole) distance is $\gg1/\log(T+3)$. This proves $|\zeta'/\zeta|\ll\log^2(T+3)$ on those edges and justifies the contour shift without choosing heights that dodge unknown [zeros](../../../polynomial.md#zero-of-a-function).

## 4

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Selberg upper-bound sieve](../../../analytic-number-theory.md#selberg-upper-bound-sieve) replaces the [indicator function](../../../measure-theory.md#indicator-function) of a sifted set by the square of a divisor sum. If the real [Selberg sieve weights](../../../analytic-number-theory.md#selberg-sieve-weights) satisfy $\lambda_1=1$, then

$$
\boldsymbol1_{(F(n),P(z))=1}
\le\left(\sum_{\substack{d\mid F(n)\\d\mid P(z)}}\lambda_d\right)^2,
\qquad P(z)=\prod_{p\le z}p.
$$

When $F(n)$ has no forbidden [prime factors](../../../number-theory.md#prime-factor), the divisor sum is exactly one; otherwise its square is still nonnegative. Taking the weights to vanish for $d>z$ controls the error in summing this majorant. The main term is a positive [quadratic form](../../../linear-algebra.md#quadratic-form) that can be diagonalized and minimized explicitly. This optimization, together with a bound for the remainder, is the central idea of the [Selberg sieve](../../../analytic-number-theory.md#selberg-sieve).

For [twin primes](../../../number-theory.md#twin-prime), take $F(n)=n(n+2)$ and let $\rho(d)$ be the number of its [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) modulo a [squarefree integer](../../../number-theory.md#squarefree-integer) $d$. The [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) makes $\rho$ a [multiplicative arithmetic function](../../../number-theory.md#multiplicative-function), with $\rho(2)=1$ and $\rho(p)=2$ for odd [primes](../../../number-theory.md#prime-number). Thus the [polynomial root density in a sieve](../../../analytic-number-theory.md#polynomial-root-density-in-a-sieve) is $g(d)=\rho(d)/d$, and

$$
\#\{n\le x:d\mid F(n)\}=xg(d)+r_d,\qquad |r_d|\le\rho(d).
$$

Summing the majorant gives

$$
S(x,z):=\#\{n\le x:(F(n),P(z))=1\}
\le xQ(\lambda)+O\left(\left(\sum_{d\le z}|\lambda_d|\rho(d)\right)^2\right),
$$

where $Q(\lambda)=\sum_{d,e\le z}\lambda_d\lambda_e g([d,e])$, with all indices [squarefree](../../../number-theory.md#squarefree-integer). Here $\rho([d,e])\le\rho(d)\rho(e)$ controls the error.

We carry out the [Selberg sieve diagonalization](../../../analytic-number-theory.md#selberg-sieve-diagonalization). Put

$$
h(r)=\prod_{p\mid r}\left(\frac1{g(p)}-1\right),\qquad
h(1)=1,\qquad
y_r=\sum_{\substack{d\le z\\r\mid d}}\lambda_dg(d).
$$

For [squarefree integers](../../../number-theory.md#squarefree-integer) $d,e$, [multiplicativity](../../../number-theory.md#multiplicativity-of-an-arithmetic-function) gives

$$
g([d,e])=g(d)g(e)\sum_{r\mid(d,e)}h(r),
\qquad Q(\lambda)=\sum_{r\le z}h(r)y_r^2.
$$

The identity behind the first equality is $\prod_{p\mid(d,e)}[1+h(p)]=1/g((d,e))$. [Möbius inversion](../../../number-theory.md#mobius-inversion-formula) gives $\lambda_1=\sum_r\mu(r)y_r=1$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) therefore implies

$$
1\le\left(\sum_{r\le z}h(r)y_r^2\right)
\left(\sum_{r\le z}\frac{\mu(r)^2}{h(r)}\right).
$$

Define $G(z)=\sum_{r\le z,\ r\text{ squarefree}}1/h(r)$. Equality is attained at $y_r=\mu(r)/(h(r)G(z))$, giving **$\min Q=1/G(z)$**. Inverting again, the optimizing [Selberg sieve weights](../../../analytic-number-theory.md#selberg-sieve-weights) are

$$
\lambda_d=\frac{\mu(d)}{g(d)h(d)G(z)}G_d(z/d),\qquad
G_d(v)=\sum_{\substack{m\le v\\(m,d)=1\\m\text{ squarefree}}}\frac1{h(m)}.
$$

In particular $\lambda_1=1$. Since $G_d(z/d)\le G(z)$,

$$
|\lambda_d|\le\frac1{g(d)h(d)}
=\prod_{p\mid d}\frac1{1-g(p)}\le d.
$$

The last inequality holds separately at $p=2$, $p=3$, and $p\ge5$. Together with $\rho(d)\le d$, this crude bound already makes the remainder $O(z^6)$, because $\sum_{d\le z}d^2=O(z^3)$.

We also need a lower bound for $G(z)$; we prove it rather than presuppose a sieve asymptotic. For odd [squarefree integers](../../../number-theory.md#squarefree-integer) $r$,

$$
\frac1{h(r)}=\prod_{p\mid r}\frac2{p-2}\ge\frac{2^{\omega(r)}}r,
$$

where $\omega(r)$ counts distinct [prime factors](../../../number-theory.md#prime-factor). Put $y=\sqrt z$ and $L(y)=\sum_{a\le y,\ a\text{ odd}}1/a=\tfrac12\log y+O(1)$. The total weight $1/(ab)$ of odd pairs $a,b\le y$ is $L(y)^2$. Exclude pairs for which $a$ has a square [prime factor](../../../number-theory.md#prime-factor), $b$ has a square [prime factor](../../../number-theory.md#prime-factor), or $a,b$ have a common [prime factor](../../../number-theory.md#prime-factor). For each of these three categories the total weight is at most $L(y)^2\sum_{p\text{ odd}}p^{-2}$: for example, the weighted count of odd multiples of $p^2$ is $p^{-2}L(y/p^2)\le p^{-2}L(y)$, and the common-factor category uses $p^{-1}L(y/p)$ for each variable. Moreover,

$$
\sum_{p\text{ odd}}p^{-2}
\le\sum_{m\ge1}(2m+1)^{-2}
\le\frac19+\int_1^\infty\frac{dt}{(2t+1)^2}
=\frac5{18}.
$$

Hence the remaining odd [coprime](../../../number-theory.md#coprime-integers) [squarefree](../../../number-theory.md#squarefree-integer) pairs have weight at least $L(y)^2/6$. Their products $r=ab\le z$ are [squarefree](../../../number-theory.md#squarefree-integer), and $2^{\omega(r)}$ counts all ordered [coprime](../../../number-theory.md#coprime-integers) factorizations of $r$. This proves the [elementary lower bound for the twin-prime sieve denominator](../../../analytic-number-theory.md#elementary-lower-bound-for-the-twin-prime-sieve-denominator):

$$
G(z)\ge\sum_{\substack{r\le z\\r\text{ odd and squarefree}}}\frac{2^{\omega(r)}}r
\ge\frac{L(\sqrt z)^2}{6}\gg(\log z)^2.
$$

If $p>z$ and both $p,p+2$ are [primes](../../../number-theory.md#prime-number), $F(p)$ survives the sieve. The at most $z$ smaller values are the only exceptions. Thus, with $T(x)=\#\{p\le x:p,p+2\text{ prime}\}$ and $z=x^{1/10}$, the [twin-prime upper bound from a quadratic sieve](../../../analytic-number-theory.md#twin-prime-upper-bound-from-a-quadratic-sieve) becomes

$$
T(x)\le S(x,z)+z\ll\frac{x}{(\log z)^2}+z^6+z,
\qquad\boxed{T(x)\ll\frac{x}{(\log x)^2}.}
$$

Finally [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
\sum_{\substack{p\le X\\p,p+2\text{ prime}}}\frac1p
=\frac{T(X)}X+\int_2^X\frac{T(t)}{t^2}\,dt.
$$

The integral over $[3,\infty)$ is bounded by a constant times $\int_3^\infty dt/(t(\log t)^2)<\infty$. The nonnegative partial sums are therefore bounded and increasing. Thus **the reciprocal [series](../../../real-analysis.md#series-mathematics) over the smaller members of twin-prime pairs converges**, a form of [Brun's theorem](../../../number-theory.md#brun-s-theorem). The upper bound does not assert that infinitely many [twin primes](../../../number-theory.md#twin-prime) exist.

## 5

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Fix a positive integer $q$ and an integer $a$ [coprime](../../../number-theory.md#coprime-integers) to $q$. We use [Dirichlet characters](../../../algebraic-number-theory.md#dirichlet-character) modulo $q$, extended by [zero](../../../polynomial.md#zero-of-a-function) on integers not [coprime](../../../number-theory.md#coprime-integers) to $q$, and write $\chi_0$ for the [principal Dirichlet character](../../../algebraic-number-theory.md#principal-dirichlet-character). For a [nonprincipal Dirichlet character](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character), the sum over one complete period is [zero](../../../polynomial.md#zero-of-a-function). Its partial sums $A_\chi(u)=\sum_{n\le u}\chi(n)$ are therefore $O(q)$. [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
L(s,\chi)=s\int_1^\infty A_\chi(u)u^{-s-1}\,du,\qquad\Re s>0.
$$

The integral converges locally uniformly there, so these [Dirichlet L-functions](../../../algebraic-number-theory.md#dirichlet-l-function) are [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) at one. On the other hand,

$$
L(s,\chi_0)=\zeta(s)\prod_{p\mid q}(1-p^{-s})
$$

has a simple [pole](../../../isolated-singularity.md#pole) at one, with [residue](../../../analysis.md#residue) $\varphi(q)/q$.

The assumed [nonvanishing of a nonprincipal Dirichlet L-function at one](../../../analytic-number-theory.md#nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one) for real [Dirichlet characters](../../../algebraic-number-theory.md#dirichlet-character) also excludes vanishing for nonreal ones. To prove this, form the [product over all Dirichlet characters](../../../algebraic-number-theory.md#product-over-all-dirichlet-characters)

$$
\mathcal F(\sigma)=\prod_{\chi\bmod q}L(\sigma,\chi),\qquad\sigma>1.
$$

Use the [logarithm](../../../calculus.md#logarithm) supplied by the absolutely convergent [Euler product](../../../analytic-number-theory.md#euler-product). The [Orthogonality of Dirichlet characters](../../../algebraic-number-theory.md#orthogonality-of-dirichlet-characters) yields

$$
\log\mathcal F(\sigma)
=\sum_{p\nmid q}\sum_{m\ge1}\frac{\sum_\chi\chi(p)^m}{mp^{m\sigma}}
=\varphi(q)\sum_{\substack{p\nmid q,\ m\ge1\\p^m\equiv1\pmod q}}\frac1{mp^{m\sigma}}\ge0.
$$

Thus $\mathcal F(\sigma)\ge1$. If a nonreal [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character) $\chi$ had $L(1,\chi)=0$, its distinct conjugate $\overline\chi$ would also have a [zero](../../../polynomial.md#zero-of-a-function) there, since $L(1,\overline\chi)=\overline{L(1,\chi)}$. These two [zeros](../../../polynomial.md#zero-of-a-function) would outweigh the single [pole](../../../isolated-singularity.md#pole) of the principal factor; all other factors are bounded near one. It would follow that $\mathcal F(\sigma)\to0$ as $\sigma\downarrow1$, contradicting the lower bound. Together with the assumption for real [Dirichlet characters](../../../algebraic-number-theory.md#dirichlet-character), this proves $L(1,\chi)\ne0$ for every [nonprincipal Dirichlet character](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character).

The first-degree part of the [Euler product](../../../analytic-number-theory.md#euler-product) [logarithm](../../../calculus.md#logarithm) gives

$$
\log L(\sigma,\chi)=\sum_p\frac{\chi(p)}{p^\sigma}+O(1),\qquad\sigma\downarrow1.
$$

The omitted terms are bounded uniformly, since $\sum_p\sum_{m\ge2}(mp^{m\sigma})^{-1}\ll\sum_p p^{-2}<\infty$. For each nonprincipal factor, its [logarithm](../../../calculus.md#logarithm) remains bounded: choose a [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm) near the now established nonzero value $L(1,\chi)$; the Euler-product branch differs from it by a fixed integral multiple of $2\pi i$ on a sufficiently small real interval. For the principal factor,

$$
\log L(\sigma,\chi_0)=\log\frac1{\sigma-1}+O_q(1).
$$

Applying [Orthogonality of Dirichlet characters](../../../algebraic-number-theory.md#orthogonality-of-dirichlet-characters) again gives

$$
\varphi(q)\sum_{p\equiv a\,\mathrm{mod}\,q}\frac1{p^\sigma}
=\sum_{\chi\bmod q}\overline{\chi(a)}\log L(\sigma,\chi)+O_q(1)
=\log\frac1{\sigma-1}+O_q(1).
$$

The right side diverges as $\sigma\downarrow1$, so the [arithmetic progression](../../../arithmetic.md#arithmetic-progression) contains infinitely many [primes](../../../number-theory.md#prime-number). This proves [Dirichlet's theorem on arithmetic progressions](../../../analytic-number-theory.md#dirichlet-s-theorem-on-arithmetic-progressions): **every reduced [residue class](../../../number-theory.md#residue-class) modulo $q$ contains infinitely many [primes](../../../number-theory.md#prime-number)**. The argument also covers $q=1$ and $q=2$, when there need not be a nonreal character.

For the sharper statement about [reciprocal primes in a fixed arithmetic progression](../../../analytic-number-theory.md#reciprocal-primes-in-a-fixed-arithmetic-progression), use the given [prime-counting function](../../../number-theory.md#prime-counting-function) asymptotic with $q$ fixed:

$$
\pi(x;q,a)\sim\frac{\operatorname{li}(x)}{\varphi(q)}
\sim\frac{x}{\varphi(q)\log x}.
$$

The second equivalence follows by [integration by parts](../../../calculus.md#integration-by-parts) in the [logarithmic integral function](../../../calculus.md#logarithmic-integral-function). [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) yields

$$
H(x):=\sum_{\substack{p\le x\\p\equiv a\pmod q}}\frac1p
=\frac{\pi(x;q,a)}x+\int_2^x\frac{\pi(t;q,a)}{t^2}\,dt.
$$

For any $\varepsilon>0$, choose a fixed $T$ so large that the relative error in $\pi(t;q,a)$ is at most $\varepsilon$ for $t\ge T$. The initial integral is a constant, while the remaining integral lies between

$$
\frac{1-\varepsilon}{\varphi(q)}\bigl(\log\log x-\log\log T\bigr)
\quad\text{and}\quad
\frac{1+\varepsilon}{\varphi(q)}\bigl(\log\log x-\log\log T\bigr).
$$

The boundary term is $O_q(1/\log x)$. Divide by $\log\log x$, let $x\to\infty$, and then let $\varepsilon\downarrow0$. We obtain

$$
\boxed{\sum_{\substack{p\le x\\p\equiv a\pmod q}}\frac1p
\sim\frac{\log\log x}{\varphi(q)}.}
$$

Only a relative asymptotic is deduced from the given information; an additive $O(1)$ error, or uniformity for a growing modulus $q$, would require additional estimates.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
