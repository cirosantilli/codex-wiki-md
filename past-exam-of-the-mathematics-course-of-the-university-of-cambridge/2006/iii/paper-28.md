# Paper 28

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper28.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper28.pdf)

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

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $\vartheta(x)=\sum_{p\le x}\log p$ and $\psi(x)=\sum_{n\le x}\Lambda(n)$ for the two [Chebyshev functions](../../../number-theory.md#chebyshev-function), and $\pi(x)$ for the [prime-counting function](../../../number-theory.md#prime-counting-function). If $m<p\le2m$, the [prime](../../../number-theory.md#prime-number) $p$ divides the central [binomial coefficient](../../../combinatorics.md#binomial-coefficient) $\binom{2m}{m}$. Consequently

$$
\vartheta(2m)-\vartheta(m)\le\log\binom{2m}{m}\le2m\log2.
$$

Sum this inequality over dyadic integers $m=1,2,4,\ldots,2^{k-1}$. It gives $\vartheta(2^k)\le2^{k+1}\log2$. [Monotonicity](../../../calculus.md#monotonic-function), with $2^{k-1}<x\le2^k$, gives $\vartheta(x)=O(x)$ for real $x\ge2$. This is the [Chebyshev estimate from central binomial coefficients](../../../number-theory.md#chebyshev-estimate-from-central-binomial-coefficients); no information about the distribution of [primes](../../../number-theory.md#prime-number) beyond [unique factorization](../../../algebra.md#unique-factorization-in-an-integral-domain) has been used.

Split the [primes](../../../number-theory.md#prime-number) at $\sqrt x$. For $p>\sqrt x$, $\log p>\tfrac12\log x$, so

$$
\pi(x)\le\sqrt x+\frac{2\vartheta(x)}{\log x}.
$$

Since $\sqrt x=O(x/\log x)$,

$$
\boxed{\pi(x)=O\left(\frac{x}{\log x}\right).}
$$

We also need $\psi(x)=O(x)$. The contributions of higher [prime powers](../../../number-theory.md#prime-power) satisfy

$$
\psi(x)=\sum_{k\ge1}\vartheta(x^{1/k})=\vartheta(x)+O(\sqrt x\log x)=O(x),
$$

because only $k\le\log x/\log2$ contribute, and $\vartheta(x^{1/k})\ll\sqrt x$ for $k\ge2$.

The [Von Mangoldt divisor identity](../../../number-theory.md#von-mangoldt-divisor-identity) is $\log n=\sum_{d\mid n}\Lambda(d)$, which follows by factoring $n$ into [prime powers](../../../number-theory.md#prime-power). Summing it for $n\le M$, with $M$ a positive integer, gives

$$
\log(M!)=\sum_{d\le M}\Lambda(d)\left\lfloor\frac Md\right\rfloor
=M\sum_{d\le M}\frac{\Lambda(d)}d+O(\psi(M)).
$$

The bound already proved makes the last error $O(M)$. Integral comparison for $\sum_{n\le M}\log n$, or the [Stirling formula](../../../real-analysis.md#stirling-formula), gives $\log(M!)=M\log M-M+O(\log M)$. Therefore

$$
\sum_{d\le M}\frac{\Lambda(d)}d=\log M+O(1).
$$

The contribution from higher [prime powers](../../../number-theory.md#prime-power) is uniformly bounded:

$$
\sum_p\sum_{k\ge2}\frac{\log p}{p^k}=\sum_p\frac{\log p}{p(p-1)}\le\sum_{n\ge2}\frac{\log n}{n(n-1)}<\infty.
$$

Subtract it, and replace $M$ by $\lfloor x\rfloor$, to obtain the [Mertens first theorem](../../../analytic-number-theory.md#mertens-first-theorem)

$$
\boxed{A(x):=\sum_{p\le x}\frac{\log p}{p}=\log x+O(1).}
$$

Now fix $\delta>0$. Apply [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) to $A(t)$ and $f(t)=(\log t)^{-1-\delta}$. With the lower endpoint interpreted as $2^-$, so that the [prime](../../../number-theory.md#prime-number) $2$ is included, this gives

$$
\sum_{p\le x}\frac1{p(\log p)^\delta}
=\frac{A(x)}{(\log x)^{1+\delta}}+(1+\delta)\int_2^x\frac{A(t)}{t(\log t)^{2+\delta}}\,dt.
$$

The boundary term tends to zero, and the integral converges, since $A(t)\ll\log t$ and $\int_2^\infty dt/(t(\log t)^{1+\delta})<\infty$. Thus **the series converges for every positive $\delta$**. Keeping the main term of $A(t)$ also gives the useful [logarithmically weighted reciprocal-prime tail](../../../analytic-number-theory.md#logarithmically-weighted-reciprocal-prime-tail)

$$
\boxed{\sum_{p>x}\frac1{p(\log p)^\delta}=\frac1{\delta(\log x)^\delta}+O_\delta\left(\frac1{(\log x)^{1+\delta}}\right).}
$$

Indeed, subtract the finite partial sum from the limiting integral: the boundary contributes $-(\log x)^{-\delta}$ and the main integral contributes $(1+\delta)(\log x)^{-\delta}/\delta$.

## 2

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For $\sigma>1$, the absolutely convergent logarithm of the [Euler product](../../../analytic-number-theory.md#euler-product) for the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) is

$$
\log\zeta(s)=\sum_p\sum_{k\ge1}\frac{p^{-ks}}k.
$$

The elementary identity $3+4\cos v+\cos2v=2(1+\cos v)^2\ge0$ therefore gives

$$
\log\left(\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\right)
=\sum_p\sum_{k\ge1}\frac{3+4\cos(kt\log p)+\cos(2kt\log p)}{kp^{k\sigma}}\ge0.
$$

Thus the expression inside the logarithm is at least one. The [Meromorphic continuation of the Riemann zeta function to the right half-plane](../../../analytic-number-theory.md#meromorphic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane) has only a simple [pole](../../../isolated-singularity.md#pole) at one, of [residue](../../../analysis.md#residue) one. It follows, for example, from

$$
\zeta(s)=\frac{s}{s-1}-s\int_1^\infty\frac{\{u\}}{u^{s+1}}\,du\qquad(\operatorname{Re}s>0),
$$

whose integral is holomorphic there.

Suppose $t\ne0$ and $\zeta$ has a zero of order $m\ge1$ at $1+it$. As $\sigma\downarrow1$, the real factor is $O((\sigma-1)^{-3})$, the middle factor is $O((\sigma-1)^{4m})$, and the factor at $1+2it$ is bounded. Their product would tend to zero, contradicting its lower bound one. Hence

$$
\boxed{\zeta(1+it)\ne0\quad(t\ne0).}
$$

At $t=0$ there is a [pole](../../../isolated-singularity.md#pole), not a zero; the statement about the line does not assert a finite value for $\zeta(1)$. This proves the [three-four-one product proof of zeta boundary nonvanishing](../../../analytic-number-theory.md#three-four-one-product-proof-of-zeta-boundary-nonvanishing).

To relate the [Second Chebyshev function](../../../number-theory.md#second-chebyshev-function) to the [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative), differentiate the [Euler product](../../../analytic-number-theory.md#euler-product) in its half-plane of [absolute convergence](../../../real-analysis.md#absolute-convergence):

$$
-\frac{\zeta'(s)}{\zeta(s)}=\sum_{n\ge1}\frac{\Lambda(n)}{n^s}.
$$

Since $\psi(u)=\sum_{n\le u}\Lambda(n)$, its [first integral of the Chebyshev function](../../../number-theory.md#first-integral-of-the-chebyshev-function) is

$$
\Psi_1(x)=\int_0^x\psi(u)\,du=\sum_{n\le x}(x-n)\Lambda(n).
$$

For any fixed $c>1$, its [Mellin inversion formula](../../../analysis.md#mellin-inversion-theorem) is

$$
\boxed{\Psi_1(x)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}-\frac{\zeta'(s)}{\zeta(s)}\frac{x^{s+1}}{s(s+1)}\,ds.}
$$

For justification, the elementary contour kernel is $\frac1{2\pi i}\int_{(c)}y^s/(s(s+1))\,ds=1-y^{-1}$ for $y>1$ and zero for $0<y\le1$. Close left or right and take the [residues](../../../analysis.md#residue) at zero and minus one; at $y=1$ the continuous value is zero. [Absolute convergence](../../../real-analysis.md#absolute-convergence) on $\operatorname{Re}s=c$ allows termwise integration of the [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series), and multiplying this kernel by $x$ gives $(x-n)_+$.

Here is how the relation yields the asymptotic. Move the contour to the left, using the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) to control the left-hand side. The [residue](../../../analysis.md#residue) at $s=1$ is $x^2/2$, and a [Nontrivial zero of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) $\rho$ contributes $-x^{\rho+1}/(\rho(\rho+1))$, multiplied by its [multiplicity](../../../polynomial.md#multiplicity-mathematics). The kernel [poles](../../../isolated-singularity.md#pole) at zero and minus one contribute $-x\log(2\pi)$ and $\zeta'(-1)/\zeta(-1)$; a [trivial zero of the Riemann zeta function](../../../analytic-number-theory.md#trivial-zero-of-the-riemann-zeta-function) $-2k$ contributes $-x^{1-2k}/(2k(2k-1))$. Thus the [smoothed explicit formula for the Chebyshev function](../../../number-theory.md#smoothed-explicit-formula-for-the-chebyshev-function) is

$$
\Psi_1(x)=\frac{x^2}{2}-\sum_\rho\frac{x^{\rho+1}}{\rho(\rho+1)}-x\log(2\pi)+\frac{\zeta'(-1)}{\zeta(-1)}-\sum_{k\ge1}\frac{x^{1-2k}}{2k(2k-1)}.
$$

For the contour argument, use heights avoiding the zero ordinates and then let those heights increase. The local zero bound from the [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula), together with the [Local partial-fraction expansion of the Riemann zeta logarithmic derivative](../../../analytic-number-theory.md#local-partial-fraction-expansion-of-the-riemann-zeta-logarithmic-derivative), permits heights with logarithmic-derivative bound $O(\log^2 T)$ in each fixed vertical strip. The horizontal integrals then vanish because the denominator is of size $T^2$. After that, send the left edge through negative odd integers to minus infinity; the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) bounds the [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) there by a logarithm, and $x^{s+1}$ makes the left integral vanish for fixed $x>1$. This explains why this smoothing allows a convergent contour calculation without a quantitative zero-free region.

In fact the [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula), stated in the next solution, gives $N(T)=O(T\log T)$ and hence

$$
\sum_\rho\frac1{|\rho(\rho+1)|}<\infty.
$$

The [Nontrivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) satisfy $0<\operatorname{Re}\rho<1$, using the [Euler product](../../../analytic-number-theory.md#euler-product), the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function), and the nonvanishing just proved. For each such zero, $x^{\rho-1}\to0$ as $x\to\infty$, whereas $|x^{\rho-1}|\le1$ for $x\ge1$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) therefore makes the absolutely convergent zero sum, divided by $x^2$, tend to zero. All the other displayed terms are $o(x^2)$. We obtain

$$
\boxed{\int_0^x\psi(u)\,du\sim\frac{x^2}{2}.}
$$

It remains to unsmooth; differentiating an asymptotic without justification would not suffice. [Monotonicity](../../../calculus.md#monotonic-function) of $\psi$ gives, for fixed $0<h<1$,

$$
\frac{\Psi_1(x)-\Psi_1((1-h)x)}{hx}\le\psi(x)\le\frac{\Psi_1((1+h)x)-\Psi_1(x)}{hx}.
$$

Divide by $x$ and use the integral asymptotic. The lower and upper limits lie between $1-h/2$ and $1+h/2$. Letting $h\downarrow0$ proves $\psi(x)\sim x$. Higher [prime powers](../../../number-theory.md#prime-power) contribute $O(\sqrt x\log x)$, as in the first solution, so $\vartheta(x)\sim x$. Finally [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
\pi(x)=\frac{\vartheta(x)}{\log x}+\int_2^x\frac{\vartheta(t)}{t(\log t)^2}\,dt.
$$

The integral is $O(x/(\log x)^2)$, by $\vartheta(t)=O(t)$ and splitting at $\sqrt x$. Hence

$$
\boxed{\pi(x)\sim\frac{x}{\log x},}
$$

which is the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem).

## 3

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the meromorphic completion

$$
Z(s)=\pi^{-s/2}\Gamma(s/2)\zeta(s).
$$

The [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) is

$$
\boxed{Z(s)=Z(1-s).}
$$

Its entire version is $\xi(s)=\tfrac12s(s-1)Z(s)$ with $\xi(s)=\xi(1-s)$. The completion $Z$ itself has [poles](../../../isolated-singularity.md#pole) at zero and one; it should not be confused with the entire [Riemann xi function](../../../analytic-number-theory.md#riemann-xi-function).

We prove the equation by a theta integral. Set

$$
\Theta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t}\qquad(t>0).
$$

The Gaussian [Fourier transform](../../../analysis.md#fourier-transform), with kernel $e^{-2\pi i x y}$, is

$$
\int_{\mathbb R}e^{-\pi t x^2}e^{-2\pi i xy}\,dx=t^{-1/2}e^{-\pi y^2/t}.
$$

For example, differentiation in $y$ and [integration by parts](../../../calculus.md#integration-by-parts) give the differential equation $I'(y)=-(2\pi y/t)I(y)$; the [Gaussian integral](../../../calculus.md#gaussian-integral) gives $I(0)=t^{-1/2}$. Periodize the Gaussian by summing $e^{-\pi t(x+n)^2}$ over integers $n$. Its $k$th Fourier coefficient is the displayed transform at $k$. Both the periodized function and its [Fourier series](../../../fourier-series.md) converge absolutely, so evaluation at $x=0$ gives the [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula) in this case:

$$
\Theta(t)=t^{-1/2}\Theta(1/t).
$$

For $\operatorname{Re}s>1$, integration term by term in the [Gamma function](../../../complex-analysis.md#gamma-function) integral gives

$$
Z(s)=\frac12\int_0^\infty(\Theta(t)-1)t^{s/2}\frac{dt}{t}.
$$

Indeed, the two terms for $n$ and $-n$ cancel the factor $1/2$, and substitution $v=\pi n^2t$ gives $\pi^{-s/2}\Gamma(s/2)n^{-s}$. Split at one, and use the transformation above in the integral from zero to one. The elementary contribution is

$$
\frac12\int_0^1(t^{-1/2}-1)t^{s/2}\frac{dt}{t}=\frac1{s-1}-\frac1s.
$$

Substitution $t=1/u$ in the remaining term therefore gives

$$
\boxed{Z(s)=\frac1{s-1}-\frac1s+\frac12\int_1^\infty(\Theta(t)-1)\left(t^{s/2}+t^{(1-s)/2}\right)\frac{dt}{t}.}
$$

The theta tail decays exponentially. The integral is consequently an [entire function](../../../complex-analysis.md#entire-function) of $s$, with [uniform convergence](../../../real-analysis.md#uniform-convergence) and termwise differentiation on compact subsets. The formula continues $Z$ meromorphically to the whole plane. Both its rational part and its integral are unchanged by $s\mapsto1-s$, proving the equation and the entire xi formulation. Using the reflection and duplication identities of the [Gamma function](../../../complex-analysis.md#gamma-function), one may equivalently write

$$
\boxed{\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s),}
$$

understood as an identity of meromorphic functions, including points where individual factors need continuation.

Now let $N(T)$ count the [Nontrivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) $\rho=\beta+i\gamma$ with $0<\gamma\le T$, including [multiplicity](../../../polynomial.md#multiplicity-mathematics). The [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula) is

$$
\boxed{N(T)=\frac{T}{2\pi}\log\frac{T}{2\pi}-\frac{T}{2\pi}+O(\log(T+2)).}
$$

For $T$ not a zero ordinate, the more precise usual form is

$$
N(T)=\frac{T}{2\pi}\log\frac{T}{2\pi}-\frac{T}{2\pi}+\frac78+S(T)+O(T^{-1}),\qquad S(T)=\frac1\pi\arg\zeta(\tfrac12+iT)=O(\log T).
$$

Here the argument is continued from $\zeta(2)>0$ along the path $2\to2+iT\to\tfrac12+iT$. The first formula remains valid at zero ordinates with the stated endpoint convention. Only its leading asymptotic is needed below.

List the positive ordinates as $\gamma_1\le\gamma_2\le\cdots$, with [multiplicity](../../../polynomial.md#multiplicity-mathematics), consistent with this counting function. Put $b_n=2\pi n/\log n$. For every fixed $\varepsilon\in(0,1)$,

$$
\log((1\pm\varepsilon)b_n)=\log n-\log\log n+O_\varepsilon(1),\qquad
N((1\pm\varepsilon)b_n)\sim(1\pm\varepsilon)n.
$$

For all sufficiently large $n$, the lower count is less than $n$ and the upper count is greater than $n$. Consequently $(1-\varepsilon)b_n<\gamma_n\le(1+\varepsilon)b_n$. Letting $\varepsilon\downarrow0$ proves the [asymptotic inversion of the zeta zero count](../../../analytic-number-theory.md#asymptotic-inversion-of-the-zeta-zero-count)

$$
\boxed{\gamma_n\sim\frac{2\pi n}{\log n}.}
$$

This argument works even when several zeros have the same ordinate; “increasing” is interpreted in the standard nondecreasing, multiplicity-counted sense. A count listing only distinct ordinates is a different object and is not determined by this formula alone.

In this notation the [Riemann hypothesis](../../../analytic-number-theory.md#riemann-hypothesis) says that every [Nontrivial zero of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) has real part one-half:

$$
\boxed{\rho=\tfrac12+i\gamma\quad\text{for every nontrivial zero}.}
$$

It concerns their horizontal location, not merely the growth of the ordinates, and does not assert that the zeros are simple. The functional equation and [complex conjugation](../../../complex-analysis.md#complex-conjugation) make the zero set symmetric about both the real axis and the [critical line](../../../analytic-number-theory.md#critical-line); the hypothesis puts all the [Nontrivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) on that line.

## 4

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Selberg upper-bound sieve](../../../analytic-number-theory.md#selberg-upper-bound-sieve) replaces a difficult coprimality indicator by a nonnegative square whose coefficients can be optimized. Let $P(z)=\prod_{p\le z}p$, and suppose a finite sequence has divisibility counts

$$
A_d=Xg(d)+r_d\qquad(d\mid P(z)),
$$

where $g$ is multiplicative on [squarefree integers](../../../number-theory.md#squarefree-integer) and $0<g(p)<1$. Choose real [Selberg sieve weights](../../../analytic-number-theory.md#selberg-sieve-weights) $\lambda_1=1$ supported on $d\mid P(z)$ with $d\le R$. If an entry has no [prime](../../../number-theory.md#prime-number) factor in $P(z)$, its only weighted divisor is $1$, so its indicator is bounded above by the square of the divisor sum. Summing gives

$$
S\le\sum_{d,e\le R}\lambda_d\lambda_e A_{[d,e]}
=XQ(\lambda)+O\left(\sum_{d,e\le R}|\lambda_d\lambda_e r_{[d,e]}|\right),
$$

where $Q(\lambda)=\sum_{d,e}\lambda_d\lambda_e g([d,e])$. This is an upper bound regardless of the signs of the weights.

Here is the optimization. On the permitted [squarefree integers](../../../number-theory.md#squarefree-integer) put

$$
h(r)=\prod_{p\mid r}\frac{1-g(p)}{g(p)},\qquad k(r)=h(r)^{-1},\qquad
Y_r=\sum_{r\mid d}\lambda_dg(d).
$$

The identity

$$
g([d,e])=g(d)g(e)\sum_{r\mid(d,e)}h(r)
$$

can be checked one [prime](../../../number-theory.md#prime-number) at a time: a [prime](../../../number-theory.md#prime-number) in both $d$ and $e$ gives the factor $1+h(p)=1/g(p)$. Thus

$$
Q(\lambda)=\sum_rh(r)Y_r^2.
$$

Finite [Möbius inversion](../../../number-theory.md#mobius-inversion-formula) gives $\lambda_dg(d)=\sum_{d\mid r}\mu(r/d)Y_r$, and in particular the condition $\lambda_1=1$ becomes $\sum_r\mu(r)Y_r=1$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) now yields

$$
Q(\lambda)\ge\frac1{J(R,z)},\qquad
J(R,z)=\sum_{\substack{r\le R\\r\mid P(z)}}k(r).
$$

Equality is attained by $Y_r=\mu(r)k(r)/J$. Inverting again gives the explicit optimizing weights

$$
\lambda_d=\mu(d)\prod_{p\mid d}(1-g(p))^{-1}\,
\frac{\displaystyle\sum_{\substack{v\le R/d\\v\mid P(z)\\(v,d)=1}}k(v)}{J(R,z)}.
$$

They satisfy $|\lambda_d|\le1$. To see this, multiply out $\prod_{p\mid d}(1-g(p))^{-1}=\sum_{e\mid d}k(e)$. The numerator becomes the sum of $k(ev)$ over distinct permitted integers $ev\le R$ with $e\mid d$ and $(v,d)=1$, a subset of the terms in $J$. We therefore have a main term $X/J$ and a controllable remainder. This proves the basic [Selberg sieve diagonalization](../../../analytic-number-theory.md#selberg-sieve-diagonalization) and the useful bound on the weights, rather than merely asserting an optimized density.

Apply it to the polynomial $F(n)=n(n+2)$ for $1\le n\le N$. If $\omega(d)$ is the number of roots of $F$ modulo squarefree $d$, the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) gives

$$
\omega(2)=1,\qquad \omega(p)=2\ (p>2),\qquad
A_d=\frac{\omega(d)}dN+O(\omega(d)).
$$

Use $g(d)=\omega(d)/d$, $R=z=N^{1/8}$, and sieve the indices for which $F(n)$ has no [prime](../../../number-theory.md#prime-number) factor at most $z$. The local weights are

$$
k(2)=1,\qquad k(p)=\frac2{p-2}\quad(p>2).
$$

We claim $J(z,z)\gg(\log z)^2$. The following truncated-product argument supplies the necessary lower bound. Put $w=z^{1/8}$, and consider all [squarefree integers](../../../number-theory.md#squarefree-integer) on the [primes](../../../number-theory.md#prime-number) at most $w$, with total weight

$$
W=\prod_{p\le w}(1+k(p))=\prod_{p\le w}(1-g(p))^{-1}.
$$

Give such an integer $d$ [probability](../../../probability-theory.md#probability) $k(d)/W$. [Prime](../../../number-theory.md#prime-number) inclusion is independent with [probability](../../../probability-theory.md#probability) $g(p)$, so

$$
\mathbb E[\log d]=\sum_{p\le w}g(p)\log p=2\log w+O(1)=\tfrac14\log z+O(1),
$$

by the [Mertens first theorem](../../../analytic-number-theory.md#mertens-first-theorem), absorbing the [prime](../../../number-theory.md#prime-number) $2$ separately. For sufficiently large $z$, this is at most $\tfrac12\log z$. The [Markov inequality](../../../probability-inequality.md#markov-inequality) shows that at least half of $W$ lies on $d\le z$, all of which are terms in $J(z,z)$.

Moreover, [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) applied to the [Mertens first theorem](../../../analytic-number-theory.md#mertens-first-theorem) gives

$$
\sum_{p\le w}\frac1p=\log\log w+B+O(1/\log w).
$$

Indeed it is $A(w)/\log w+\int_2^w A(t)/(t(\log t)^2)\,dt$, and the contribution of $A(t)-\log t=O(1)$ has a finite limiting constant with tail $O(1/\log w)$. Expanding the logarithm of $W$ now gives

$$
\log W=2\sum_{3\le p\le w}\frac1p+O(1)=2\log\log w+O(1).
$$

The error is bounded since $\sum_p p^{-2}<\infty$. Consequently $W\asymp(\log w)^2\asymp(\log z)^2$, proving the claim. The exponent two reflects the two forbidden classes at almost every [prime](../../../number-theory.md#prime-number).

For the remainder use $|\lambda_d|\le1$ and the simple bound $\omega([d,e])\le[d,e]\le de$. Hence

$$
\sum_{d,e\le z}|\lambda_d\lambda_e r_{[d,e]}|\ll\sum_{d,e\le z}de\ll z^4.
$$

The number of surviving indices is therefore

$$
S\ll\frac{N}{(\log z)^2}+z^4.
$$

Every pair of [primes](../../../number-theory.md#prime-number) $p,p+2$ with $p>z$ survives, since both its [prime](../../../number-theory.md#prime-number) factors exceed $z$. The exceptional pairs with $p\le z$ number at most $z$. With $z=N^{1/8}$ we obtain

$$
\boxed{\#\{p\le N:p\text{ and }p+2\text{ prime}\}\ll\frac{N}{(\log N)^2}+N^{1/2}+N^{1/8}\ll\frac{N}{(\log N)^2}.}
$$

This is the [twin-prime upper bound from a quadratic sieve](../../../analytic-number-theory.md#twin-prime-upper-bound-from-a-quadratic-sieve). The method constructs a majorant and bounds the sifted set; it does not give a positive lower bound for twin [primes](../../../number-theory.md#prime-number).

## 5

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Fix integers $q\ge1$ and $a$ with $(a,q)=1$. We prove the [Dirichlet theorem on primes in arithmetic progressions](../../../analytic-number-theory.md#dirichlet-s-theorem-on-arithmetic-progressions) by showing that the [prime](../../../number-theory.md#prime-number) Dirichlet sum in this [residue class](../../../number-theory.md#residue-class) diverges as its real exponent decreases to one.

First justify the required [Dirichlet L-function](../../../algebraic-number-theory.md#dirichlet-l-function) facts. If $\chi$ is a [nonprincipal Dirichlet character](../../../algebraic-number-theory.md#nonprincipal-dirichlet-character) modulo $q$, its sum over a full period is zero: choose a unit $b$ with $\chi(b)\ne1$, and multiplication by $b$ permutes the [residue classes](../../../number-theory.md#residue-class), forcing the sum to equal $\chi(b)$ times itself. Therefore the partial sums $C_\chi(u)=\sum_{n\le u}\chi(n)$ are bounded by $q$. [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
L(s,\chi)=s\int_1^\infty C_\chi(u)u^{-s-1}\,du\qquad(\operatorname{Re}s>0),
$$

which supplies holomorphic continuation near one, with locally [uniform convergence](../../../real-analysis.md#uniform-convergence). For the [principal Dirichlet character](../../../algebraic-number-theory.md#principal-dirichlet-character) $\chi_0$,

$$
L(s,\chi_0)=\zeta(s)\prod_{p\mid q}(1-p^{-s})
$$

has a simple [pole](../../../isolated-singularity.md#pole) at one, with [residue](../../../analysis.md#residue) $\varphi(q)/q$.

The assumption in the question gives nonvanishing at one for real nonprincipal characters. We must also prove it for nonreal characters. For a nonreal $\chi$, its square $\chi^2$ is nonprincipal. For real $\sigma>1$, logarithms of the [Euler products](../../../analytic-number-theory.md#euler-product) give

$$
\zeta(\sigma)^3|L(\sigma,\chi)|^4|L(\sigma,\chi^2)|\ge1.
$$

For a [prime](../../../number-theory.md#prime-number) not dividing $q$, its logarithmic coefficient is $3+4\operatorname{Re}\chi(p)^k+\operatorname{Re}\chi(p)^{2k}=2(1+\cos\theta)^2\ge0$, where $\chi(p)^k=e^{i\theta}$. [Primes](../../../number-theory.md#prime-number) dividing $q$ contribute only the positive zeta term. If $L(1,\chi)$ vanished to order $m\ge1$, the product would be $O((\sigma-1)^{4m-3})$ and tend to zero: the squared-character factor is bounded because $\chi^2$ is nonprincipal. This is a contradiction. Hence

$$
L(1,\chi)\ne0\qquad\text{for every nonprincipal }\chi.
$$

This step uses the given real-character hypothesis and the [Euler product positivity for L-function nonvanishing](../../../analytic-number-theory.md#euler-product-positivity-for-l-function-nonvanishing) for all remaining characters.

In $\sigma>1$ choose the logarithm furnished by the absolutely convergent [Euler product](../../../analytic-number-theory.md#euler-product). Its prime-power expansion gives

$$
\log L(\sigma,\chi)=\sum_p\frac{\chi(p)}{p^\sigma}+O(1).
$$

The error from powers $k\ge2$ is uniformly bounded as $\sigma\downarrow1$, by $\sum_p\sum_{k\ge2}1/(kp^{k\sigma})<\infty$. For nonprincipal $\chi$, nonvanishing and holomorphic continuation at one provide a bounded logarithm in a neighborhood of one. The Euler-product branch differs from that branch by a constant integral multiple of $2\pi i$ on the final real interval, so it too is bounded. Thus

$$
\sum_p\frac{\chi(p)}{p^\sigma}=O_q(1)\qquad(\chi\ne\chi_0).
$$

For the principal character, its simple [pole](../../../isolated-singularity.md#pole) instead gives

$$
\sum_{p\nmid q}\frac1{p^\sigma}=\log\frac1{\sigma-1}+O_q(1).
$$

The [Orthogonality of Dirichlet characters](../../../algebraic-number-theory.md#orthogonality-of-dirichlet-characters) gives, for [primes](../../../number-theory.md#prime-number) not dividing $q$,

$$
1_{p\equiv a\pmod q}=\frac1{\varphi(q)}\sum_{\chi\bmod q}\overline{\chi(a)}\chi(p).
$$

Multiply by $p^{-\sigma}$ and sum. [Absolute convergence](../../../real-analysis.md#absolute-convergence) allows the interchange for $\sigma>1$, so

$$
\boxed{\sum_{p\equiv a\pmod q}\frac1{p^\sigma}=\frac1{\varphi(q)}\log\frac1{\sigma-1}+O_q(1).}
$$

The right side tends to infinity. If there were only finitely many [primes](../../../number-theory.md#prime-number) in the progression, the left side would have a finite limit at one. This contradiction proves **infinitely many [primes](../../../number-theory.md#prime-number) occur in every reduced [residue class](../../../number-theory.md#residue-class)**. For $q=1$ or $2$ the character argument simply has no nonprincipal terms and gives the same conclusion.

For the final deduction the modulus $q$ is fixed. Let $A(t)=\pi(t;q,a)$. The given consequence of the [Siegel–Walfisz theorem](../../../analytic-number-theory.md#siegel-walfisz-theorem) is $A(t)\sim t/(\varphi(q)\log t)$. [Partial summation](../../../analytic-number-theory.md#abel-s-summation-formula), including the [prime](../../../number-theory.md#prime-number) $2$ through the lower endpoint $2^-$ when appropriate, gives

$$
\sum_{\substack{p\le x\\p\equiv a\pmod q}}\frac1p=\frac{A(x)}x+\int_2^x\frac{A(t)}{t^2}\,dt.
$$

The boundary is $O_q(1/\log x)$. Write $A(t)=t(1+\varepsilon(t))/(\varphi(q)\log t)$ with $\varepsilon(t)\to0$. The main integral is $(\log\log x-\log\log2)/\varphi(q)$. The error is $o(\log\log x)$: given $\eta>0$, choose $T$ such that $|\varepsilon(t)|\le\eta$ for $t\ge T$. Its integral from $2$ to $T$ is a fixed constant, and its absolute value from $T$ to $x$ is at most $\eta\log\log x/\varphi(q)$ plus a fixed constant. Divide by $\log\log x$ and then let $\eta\downarrow0$. We obtain the [reciprocal primes in a fixed arithmetic progression](../../../analytic-number-theory.md#reciprocal-primes-in-a-fixed-arithmetic-progression) asymptotic

$$
\boxed{\sum_{\substack{p\le x\\p\equiv a\pmod q}}\frac1p\sim\frac1{\varphi(q)}\log\log x.}
$$

The argument uses the supplied prime-counting asymptotic in this last part; the preceding infinitude proof did not assume the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem) in [arithmetic progressions](../../../arithmetic.md#arithmetic-progression).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
