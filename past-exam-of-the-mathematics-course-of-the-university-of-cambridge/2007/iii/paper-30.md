# Paper 30

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper30.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper30.pdf)

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
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use $e(t)=e^{2\pi it}$ and the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat f(\xi)=\int_{\mathbb R}f(x)e(-x\xi)\,dx$, initially for an [integrable function](../../../measure-theory.md#lebesgue-integrable-function). For the interval [indicator function](../../../measure-theory.md#indicator-function), direct integration gives

$$
\widehat{1_{[0,1]}}(\xi)=\begin{cases}(1-e(-\xi))/(2\pi i\xi),&\xi\ne0,\\1,&\xi=0.\end{cases}
$$

The integral bound is one, and the displayed numerator has modulus at most two. By the [convolution theorem](../../../fourier-analysis.md#convolution-theorem), the [Fourier transform](../../../analysis.md#fourier-transform) of the $m$-fold [convolution](../../../fourier-analysis.md#convolution) is its $m$th power. Thus the [Fourier decay of repeated interval convolutions](../../../fourier-analysis.md#fourier-decay-of-repeated-interval-convolutions) gives

$$
\boxed{|\widehat f(\xi)|\le\min(1,(\pi|\xi|)^{-m})\ll\min(1,|\xi|^{-m}).}
$$

At zero, interpret the second term of the minimum as infinity.

The [Schwartz space](../../../fourier-analysis.md#schwartz-space) $\mathcal S(\mathbb R)$ consists of [smooth functions](../../../analysis.md#smooth-function) for which every [Schwartz seminorm](../../../fourier-analysis.md#schwartz-seminorm) $\sup_x|x^a f^{(b)}(x)|$ is finite, for nonnegative integers $a,b$. [Differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) and [integration by parts](../../../calculus.md#integration-by-parts) give

$$
\widehat f^{(b)}(\xi)=\widehat{(-2\pi ix)^bf}(\xi),\qquad
(2\pi i\xi)^a\widehat f^{(b)}(\xi)=\widehat{\frac{d^a}{dx^a}\bigl((-2\pi ix)^bf(x)\bigr)}(\xi).
$$

All differentiated integrands are [integrable](../../../measure-theory.md#integrability), and their boundary terms vanish because of rapid decay. The last transform is bounded by its integrand's $L^1$ [norm](../../../functional-analysis.md#norm). The same argument applies at every derivative order, so $\widehat f\in\mathcal S(\mathbb R)$.

For $f\in\mathcal S(\mathbb R)$, the [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula) is

$$
\boxed{\sum_{n\in\mathbb Z}f(n)=\sum_{k\in\mathbb Z}\widehat f(k).}
$$

To prove it, form the [periodization of a Schwartz function](../../../fourier-analysis.md#periodization-of-a-schwartz-function) $F(x)=\sum_n f(x+n)$. Rapid decay gives [uniform convergence](../../../real-analysis.md#uniform-convergence) of this series and of every differentiated series on $[0,1]$, so $F$ is a smooth [periodic function](../../../function.md#periodic-function). Its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) are

$$
\int_0^1F(x)e(-kx)\,dx=\sum_n\int_n^{n+1}f(u)e(-ku)\,du=\widehat f(k).
$$

The series $\sum_k\widehat f(k)e(kx)$ converges absolutely and uniformly. Its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) equal those of $F$. The uniqueness theorem for [Fourier series](../../../fourier-series.md) says that two [integrable functions](../../../measure-theory.md#lebesgue-integrable-function) with the same coefficients agree almost everywhere; as both functions here are continuous, they agree everywhere. Evaluating at zero proves [Poisson summation](../../../fourier-analysis.md#poisson-summation-formula).

The [Gaussian Fourier transform](../../../fourier-analysis.md#fourier-transform-of-a-gaussian) of $e^{-\pi tx^2}$, $t>0$, is $t^{-1/2}e^{-\pi\xi^2/t}$. Apply [Poisson summation](../../../fourier-analysis.md#poisson-summation-formula) to obtain the transformation of the [Jacobi theta function](../../../modular-function.md#jacobi-theta-function)

$$
\vartheta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t},\qquad \vartheta(t)=t^{-1/2}\vartheta(1/t).
$$

For $\Re s>1$, termwise integration in the [Mellin transform](../../../analysis.md#mellin-transform) gives the [Mellin representation of the completed Riemann zeta function](../../../analytic-number-theory.md#mellin-representation-of-the-completed-riemann-zeta-function)

$$
\Lambda(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)=\frac12\int_0^\infty(\vartheta(t)-1)t^{s/2-1}\,dt.
$$

Split at one and substitute $t=1/u$ in the lower integral. The theta transformation gives

$$
\Lambda(s)=\frac1{s-1}-\frac1s+\frac12\int_1^\infty(\vartheta(t)-1)\bigl(t^{s/2-1}+t^{(1-s)/2-1}\bigr)\,dt.
$$

The integral is an [entire function](../../../complex-analysis.md#entire-function) of $s$, since $\vartheta(t)-1$ decays exponentially. This [pole-subtracted theta integral for the completed zeta function](../../../analytic-number-theory.md#pole-subtracted-theta-integral-for-the-completed-zeta-function) supplies a [meromorphic continuation](../../../complex-analysis.md#meromorphic-continuation) with simple [poles](../../../isolated-singularity.md#pole) at zero and one. Both the rational term and the integral are unchanged by $s\mapsto1-s$, proving the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function)

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s).}
$$

Equivalently the [Riemann xi function](../../../analytic-number-theory.md#riemann-xi-function) $\xi(s)=\frac12s(s-1)\Lambda(s)$ is [entire](../../../complex-analysis.md#entire-function) and satisfies $\xi(s)=\xi(1-s)$. The reflection and duplication identities for the [Gamma function](../../../complex-analysis.md#gamma-function) also give $\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s)$ by [meromorphic continuation](../../../complex-analysis.md#meromorphic-continuation).

## 2

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $F(s)=-\zeta'(s)/\zeta(s)$ and $\psi_\Gamma=\Gamma'/\Gamma$. The [global partial-fraction expansion of the zeta logarithmic derivative](../../../analytic-number-theory.md#global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative) is

$$
F(s)=\frac1{s-1}-\frac12\log\pi+\frac12\psi_\Gamma(1+s/2)-B-\sum_\rho\left(\frac1{s-\rho}+\frac1\rho\right),\qquad B=\log2+\frac12\log\pi-1-\frac\gamma2.
$$

Here $\gamma$ is the [Euler--Mascheroni constant](../../../complex-analysis.md#euler-s-constant), and the sum includes multiplicities of the [Nontrivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function). The paired terms are locally absolutely convergent away from their [poles](../../../isolated-singularity.md#pole), by the [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula). This identity follows by differentiating the genus-one [Hadamard factorization](../../../complex-analysis.md#hadamard-factorization-theorem) of the [Riemann xi function](../../../analytic-number-theory.md#riemann-xi-function) and using the [Gamma function recurrence](../../../complex-analysis.md#gamma-function-recurrence).

We first prove the classical [zero-free region of the Riemann zeta function](../../../analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function). The [Euler-product nonvanishing of the Riemann zeta function](../../../analytic-number-theory.md#euler-product-nonvanishing-of-the-riemann-zeta-function) and its [functional equation](../../../analysis.md#functional-equation) place every nontrivial zero in the closed strip $0\le\beta\le1$; no assertion about zeros on its boundary is needed yet. The [real logarithmic derivative of Riemann xi](../../../analytic-number-theory.md#real-logarithmic-derivative-of-riemann-xi) and the [digamma function](../../../complex-analysis.md#digamma-function) asymptotic imply, for $1<\sigma\le2$ and $|t|\ge1$,

$$
\Re F(\sigma+it)\le C\log(|t|+2)-\sum_\rho\frac{\sigma-\beta}{(\sigma-\beta)^2+(t-\gamma_\rho)^2}.
$$

Every summand being subtracted is nonnegative. If $\beta+it$ is a zero, retaining its summand gives $\Re F(\sigma+it)\le C\log(|t|+2)-1/(\sigma-\beta)$; at height $2t$ the upper bound $C\log(|t|+2)$ suffices. At real $\sigma$ the simple [pole](../../../isolated-singularity.md#pole) of $\zeta$ gives $F(\sigma)=1/(\sigma-1)+O(1)$.

For $\sigma>1$, the [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series) $F(s)=\sum_n\Lambda(n)n^{-s}$ has nonnegative coefficients. The identity $3+4\cos u+\cos2u=2(1+\cos u)^2\ge0$ therefore gives the [three-four-one zero-free-region argument](../../../analytic-number-theory.md#three-four-one-zero-free-region-argument)

$$
0\le3F(\sigma)+4\Re F(\sigma+it)+\Re F(\sigma+2it).
$$

With $L=\log(|t|+2)$, a zero at $\beta+it$ would consequently satisfy

$$
\frac4{\sigma-\beta}\le\frac3{\sigma-1}+CL.
$$

Choose $\sigma=1+a/L$, with an absolute $a>0$ sufficiently small, and put $c=a/8$. If $\beta\ge1-c/L$, this inequality would imply $4/(a+c)\le3/a+C$. But $4/(a+a/8)-3/a=5/(9a)>C$ for small enough $a$, a contradiction.

For any fixed $t\ne0$, the same positivity inequality as $\sigma\downarrow1$ excludes a zero at $1+it$: its negative contribution has coefficient at least four, whereas the real [pole](../../../isolated-singularity.md#pole) contributes only three. Any zero at $1+2it$ only strengthens the contradiction. The [pole](../../../isolated-singularity.md#pole) at $s=1$ has a zero-free punctured neighbourhood. By compactness, the remaining bounded-height portion of the line has a zero-free neighbourhood as well. Shrink $c$ to combine these facts with the large-height bound. Hence

$$
\boxed{\zeta(\beta+i\gamma)\ne0\quad\text{if}\quad\beta\ge1-\frac c{\log(|\gamma|+2)},}
$$

with the understanding that $s=1$ is a [pole](../../../isolated-singularity.md#pole).

The [Riemann–von Mangoldt explicit formula](../../../number-theory.md#riemann-von-mangoldt-explicit-formula) for the [Second Chebyshev function](../../../number-theory.md#second-chebyshev-function), with half weight at a prime-power endpoint, is

$$
\psi_0(x)=x-\lim_{T\to\infty}\sum_{|\Im\rho|\le T}\frac{x^\rho}{\rho}-\log(2\pi)-\frac12\log(1-x^{-2}),\qquad x>1.
$$

The zero sum uses symmetric height truncation. To estimate it, take a half-integer $x$ and use the [truncated explicit formula for the second Chebyshev function](../../../number-theory.md#truncated-explicit-formula-for-the-second-chebyshev-function)

$$
\psi(x)=x-\sum_{|\Im\rho|\le T}\frac{x^\rho}{\rho}+O\left(\frac{x\log^2(xT)}T+\log x\right),\qquad 2\le T\le x.
$$

The zero-free region gives $|x^\rho|\le x\exp(-c\log x/\log(T+2))$ for these zeros. The [Riemann–von Mangoldt formula](../../../analytic-number-theory.md#riemann-von-mangoldt-formula) and [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) give $\sum_{|\Im\rho|\le T}|\rho|^{-1}\ll\log^2(T+2)$. Choose $T=\exp(\sqrt{\log x})$. Both the zero sum and the truncation error are then $O(xe^{-c'\sqrt{\log x}})$ after reducing the positive constant to absorb logarithmic factors. Replacing an arbitrary $X$ by $\lfloor X\rfloor+1/2$ preserves the [Von Mangoldt function](../../../number-theory.md#von-mangoldt-function) sum and changes the main term by at most one. This proves the requested form of the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem):

$$
\boxed{\sum_{n\le X}\Lambda(n)=X+O\left(Xe^{-c'\sqrt{\log X}}\right).}
$$

## 3

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $A(x)$ count [primes](../../../number-theory.md#prime-number) $p\le x$ for which $p+2$ is also [prime](../../../number-theory.md#prime-number). We prove $A(x)\ll x/\log^2x$ using a quadratic [Selberg sieve](../../../analytic-number-theory.md#selberg-sieve), then apply [Abel summation](../../../analytic-number-theory.md#abel-s-summation-formula).

For $F(n)=n(n+2)$, each odd [prime](../../../number-theory.md#prime-number) has exactly two roots modulo that prime. The [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) gives the [polynomial root density in a sieve](../../../analytic-number-theory.md#polynomial-root-density-in-a-sieve)

$$
\#\{n\le x:d\mid F(n)\}=xg(d)+O(\rho_F(d)),\qquad g(d)=\frac{2^{\omega(d)}}d,
$$

for odd [squarefree integers](../../../number-theory.md#squarefree-integer) $d$. Put $R=x^{1/8}$ and choose the optimizing real [Selberg sieve weights](../../../analytic-number-theory.md#selberg-sieve-weights) $\lambda_d$, supported on these $d\le R$, with $\lambda_1=1$. If $p,p+2$ are prime and $p>R$, their weight $(\sum_{d\mid F(p)}\lambda_d)^2$ is one. It is nonnegative for every other integer. Expanding the square therefore gives

$$
A(x)\le O(R)+x\sum_{d,e\le R}\lambda_d\lambda_e g([d,e])+O\left(\sum_{d,e\le R}|\lambda_d\lambda_e|\rho_F([d,e])\right).
$$

The [Selberg sieve diagonalization](../../../analytic-number-theory.md#selberg-sieve-diagonalization) makes the main quadratic form $1/J(R)$, where

$$
J(R)=\sum_{\substack{d\le R\\d\text{ odd and squarefree}}}\prod_{p\mid d}\frac2{p-2}.
$$

The [optimal Selberg weights have modulus at most one](../../../analytic-number-theory.md#optimal-selberg-weights-have-modulus-at-most-one). Since $\rho_F([d,e])\le[d,e]\le R^2$, the remainder is at most $O(R^4)$.

For completeness, the lower bound on $J$ is where the second logarithm enters. Restrict to [primes](../../../number-theory.md#prime-number) $3\le p\le y=R^{1/8}$ and put $k(p)=2/(p-2)$. The full product $W=\prod_{3\le p\le y}(1+k(p))$ is $\asymp\log^2 y$, since its [logarithm](../../../calculus.md#logarithm) is $2\sum_{3\le p\le y}1/p+O(1)$ and the [Mertens second theorem](../../../analytic-number-theory.md#mertens-second-theorem) applies. Give the associated [squarefree divisor](../../../number-theory.md#squarefree-divisor) $d$ probability $k(d)/W$. Prime inclusion probabilities are $2/p$, so the [Mertens first theorem](../../../analytic-number-theory.md#mertens-first-theorem) gives

$$
\mathbb E\log d=2\sum_{3\le p\le y}\frac{\log p}p=2\log y+O(1)<\frac12\log R
$$

for large $R$. The [Markov inequality](../../../probability-inequality.md#markov-inequality) shows that at least half the weight has $d\le R$. This proves the [truncated Euler-product lower bound](../../../analytic-number-theory.md#truncated-euler-product-lower-bound) $J(R)\gg W\gg\log^2R$. Consequently the [twin-prime upper bound from a quadratic sieve](../../../analytic-number-theory.md#twin-prime-upper-bound-from-a-quadratic-sieve) is

$$
A(x)\ll R+\frac{x}{\log^2R}+R^4\ll\frac{x}{\log^2x}.
$$

Finally, [Abel summation](../../../analytic-number-theory.md#abel-s-summation-formula) gives

$$
\sum_{\substack{p\le X\\p,p+2\text{ prime}}}\frac1p=\frac{A(X)}X+\int_2^X\frac{A(t)}{t^2}\,dt.
$$

The tail is dominated by $\int_3^\infty dt/(t\log^2t)<\infty$. Thus [reciprocal-sum convergence from a counting bound](../../../analytic-number-theory.md#reciprocal-sum-convergence-from-a-counting-bound) proves convergence of the first reciprocal sum. The second is smaller termwise. We have proved [Brun's theorem](../../../number-theory.md#brun-s-theorem):

$$
\boxed{\sum_{p,p+2\text{ prime}}\left(\frac1p+\frac1{p+2}\right)<\infty.}
$$

Counting each twin prime just once changes at most a finite repetition and gives the same conclusion.

## 4

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Put $d=\gcd(k,p-1)$ and write $S(a)=\sum_{x\in\mathbb F_p}e(ax^k/p)=pG_{a,p}$. The [multiplicative group of a finite field is cyclic](../../../algebra.md#multiplicative-group-of-a-finite-field-is-cyclic), so on its nonzero elements the $k$th-power map has kernel of size $d$. For $y\ne0$, [character orthogonality](../../../representation-theory.md#character-orthogonality) consequently gives

$$
\#\{x:x^k=y\}=\sum_{\chi^d=1}\chi(y),
$$

where the sum is over its multiplicative [characters](../../../representation-theory.md#character-of-a-representation). Thus, for $a\ne0$,

$$
S(a)=1+\sum_{\chi^d=1}\sum_{y\ne0}\chi(y)e(ay/p)=\sum_{\substack{\chi^d=1\\\chi\ne1}}\tau(\chi,a).
$$

The term from the trivial [character](../../../representation-theory.md#character-of-a-representation) is $-1$ and cancels the initial one.

For a nontrivial [character](../../../representation-theory.md#character-of-a-representation), the [prime-field character Gauss sum identity](../../../algebraic-number-theory.md#prime-field-character-gauss-sum-identity) can be proved directly. Since $|\chi(z)|=1$ on nonzero elements, substituting $y=tz$ gives

$$
|\tau(\chi,a)|^2=\sum_{t\ne0}\chi(t)\sum_{z\ne0}e(a(t-1)z/p).
$$

The inner sum is $p-1$ for $t=1$ and $-1$ otherwise. Since $\sum_{t\ne0}\chi(t)=0$, the result is $p$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) now proves the [power Gauss sum over a prime field](../../../analytic-number-theory.md#power-gauss-sum-over-a-prime-field) bound

$$
\boxed{|G_{a,p}|\le\frac{d-1}{\sqrt p}\le\frac k{\sqrt p}.}
$$

This also includes $d=1$, when the nonzero-frequency sum vanishes.

For $x\in\mathbb F_p$, additive [character orthogonality](../../../representation-theory.md#character-orthogonality) counts its representations as three powers:

$$
R(x)=\#\{(u,v,w):u^k+v^k+w^k=x\}=\frac1p\sum_{a\in\mathbb F_p}S(a)^3e(-ax/p).
$$

The zero-frequency term is $p^2$. Each other term has $|S(a)|\le k\sqrt p$, so

$$
|R(x)-p^2|\le\frac{p-1}{p}k^3p^{3/2}<k^3p^{3/2}.
$$

If $p>k^6$, this is less than $p^2$, giving $R(x)>0$ for every $x$. Hence **$p>k^6$ is a sufficient threshold** for the [three power summands over a large prime field](../../../analytic-number-theory.md#three-power-summands-over-a-large-prime-field) conclusion.

## 5

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Put $S(\theta)=\sum_{r=1}^n e(\theta r^3)$. Its modulus is the modulus of the [Fourier transform](../../../analysis.md#fourier-transform) in the question, independently of the sign convention. We use [Hua's lemma](../../../analytic-number-theory.md#hua-s-lemma) in the cubic form $\int_0^1|S|^8\ll_\delta n^{5+\delta}$; the [cubic eighth-moment proof by differencing](../../../analytic-number-theory.md#cubic-eighth-moment-proof-by-differencing) establishes this from the [subpower bound for the divisor function](../../../number-theory.md#subpower-bound-for-the-divisor-function). Therefore

$$
\frac{N^2}{2007}\le\int_m|S|^9\le\sup_{\theta\in m}|S(\theta)|\int_0^1|S|^8
$$

and $n\asymp N^{1/3}$ imply $\sup_m|S|\gg_\delta n^{1-\delta}$. Choose an actual $\theta\in m$ attaining at least half this bound; attainment of the supremum itself is unnecessary.

Fix $\varepsilon>0$ and put $\varepsilon_0=\min(\varepsilon,1/6)$. The [Dirichlet approximation theorem](../../../number-theory.md#dirichlet-s-approximation-theorem) with $Q=\lfloor N^{1-\varepsilon_0}\rfloor$ gives [coprime integers](../../../number-theory.md#coprime-integers) $a,q$ satisfying

$$
1\le q\le Q,\qquad \|q\theta\|\le Q^{-1},\qquad |\theta-a/q|\le(qQ)^{-1}\le q^{-2}.
$$

The [cubic Weyl inequality](../../../analytic-number-theory.md#cubic-weyl-inequality), which is the quantitative equidistribution estimate needed here, says

$$
|S(\theta)|\ll_\eta n^{1+\eta}\left(q^{-1}+n^{-1}+q/n^3\right)^{1/4}.
$$

Compare it with the lower bound. Choose $\delta,\eta>0$ so small that $b=4(\delta+\eta)/3<\varepsilon_0/2$. It follows that

$$
q^{-1}+n^{-1}+q/n^3\gg_{\delta,\eta}N^{-b}.
$$

But $n^{-1}=O(N^{-1/3})$ and $q/n^3=O(N^{-\varepsilon_0})$. Both are $o(N^{-b})$, so for large $N$ the first term must supply this lower bound. Consequently $q\ll_\varepsilon N^b\ll_\varepsilon N^\varepsilon$, while the approximation above gives $\|q\theta\|\ll N^{\varepsilon_0-1}\le N^{\varepsilon-1}$. Enlarging the constants covers bounded $N$. Thus

$$
\boxed{\theta\in m,\qquad q\ll_\varepsilon N^\varepsilon,\qquad \|q\theta\|\ll_\varepsilon N^{\varepsilon-1}.}
$$

Here $\|\cdot\|$ is [distance modulo one](../../../number-theory.md#distance-to-the-nearest-integer). A ninth moment of this size therefore forces at least one near-rational frequency, rather than merely a large pointwise sum somewhere outside $m$.

## 6

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Extend $f$ by zero outside $[1,N]\cap\mathbb Z$. Here is a dyadic endpoint convention for [small Type I and Type II sums](../../../analytic-number-theory.md#small-type-i-and-type-ii-sums). Write $D_M=[M,2M)\cap\mathbb Z$, with $M$ a power of two. [Type I sums](../../../analytic-number-theory.md#type-i-sum) are $\delta$-small if, for every $M\le N^{1/100}$, dyadic $K$ with $MK\le N$, and arbitrary integer intervals $I_m\subset D_K$,

$$
\frac1N\sum_{m\in D_M}\left|\sum_{n\in I_m}f(mn)\right|\le\delta.
$$

[Type II sums](../../../analytic-number-theory.md#type-ii-sum) are $\delta$-small if, for all dyadic $M,K\in[N^{1/100},N^{99/100}]$ and sequences $|a_m|,|b_n|\le1$,

$$
\frac1N\left|\sum_{m\in D_M}\sum_{n\in D_K}a_mb_nf(mn)\right|\le\delta.
$$

Zero extension handles boxes crossing the endpoint $mn=N$. Fixed choices of open or closed dyadic endpoints do not matter, but interval uniformity and uniformity in both bounded coefficient sequences do matter. These are the estimates used in the [Vinogradov Type I–II method](../../../analytic-number-theory.md#vinogradov-type-i-ii-method).

An interesting technical step is [Fourier separation of interval cutoffs](../../../analytic-number-theory.md#fourier-separation-of-interval-cutoffs). For an integer interval $I_m$, let $\widehat{1_{I_m}}(\theta)=\sum_{r\in I_m}e(-r\theta)$. Discrete [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
1_{I_m}(n)=\int_0^1\widehat{1_{I_m}}(\theta)e(n\theta)\,d\theta.
$$

The [exponential geometric sum bound](../../../real-analysis.md#exponential-geometric-sum-bound) gives a common envelope $H_N(\theta)\ll\min(N,\|\theta\|^{-1})$, with $\int_0^1H_N\ll\log(2N)$. Divide the interval transform by this envelope: at each frequency it is a bounded coefficient depending on $m$, and $e(n\theta)$ is a bounded coefficient depending on $n$. The [Type II sum](../../../analytic-number-theory.md#type-ii-sum) assumption therefore bounds the interval-cutoff sum by $O(\delta N\log N)$. Choosing the outer unit phases to turn each inner sum into its modulus extends the [Type I sum](../../../analytic-number-theory.md#type-i-sum) bound to boxes where both variables are in the Type II range.

Take $U=V=\lfloor N^{1/3}\rfloor$. With subscripts denoting truncation of arithmetic functions, the [Vaughan identity](../../../number-theory.md#vaughan-s-identity) is

$$
\Lambda=\Lambda_{\le V}+\mu_{\le U}*\log-\mu_{\le U}*\Lambda_{\le V}*1+\mu_{>U}*\Lambda_{>V}*1,
$$

where $*$ now means [Dirichlet convolution](../../../number-theory.md#dirichlet-convolution). For completeness it follows from $\mu*1=\epsilon$ and $\Lambda*1=\log$: expand $\mu_{>U}*\Lambda_{>V}*1$, cancel the short terms, and retain $\Lambda$. The short first term contributes $O(N^{1/3}\log N)$ to the sum against $f$.

The next two terms give [Type I sums](../../../analytic-number-theory.md#type-i-sum). The logarithmic term has outer coefficient $\mu(m)$, $m\le U$, and inner factor $\log n$, removed by [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) at a cost $O(\log N)$. In the other term the outer variable is $m=cd\le UV$ with coefficient

$$
\omega_m=\sum_{\substack{cd=m\\c\le U,d\le V}}\mu(c)\Lambda(d),\qquad |\omega_m|\le\sum_{d\mid m}\Lambda(d)=\log m.
$$

This [logarithmic coefficient bound in Vaughan identity](../../../number-theory.md#logarithmic-coefficient-bound-in-vaughan-identity) avoids a loss from a divisor weight. On boxes with short outer variable use the hypothesis directly; on boxes where both variables are at least $N^{1/100}$ use the extended bound proved above. Boxes with inner variable less than $N^{1/100}$ contain at most $O(N^{2/3+1/100})$ pairs in total and are treated trivially. All remaining inner scales are at most $N^{99/100}$ whenever the outer scale exceeds $N^{1/100}$.

For the final convolution, group the variables as

$$
\sum_{\substack{m>U,n>V\\mn\le N}}\mu(m)b(n)f(mn),\qquad b(n)=\sum_{\substack{d\mid n\\d>V}}\Lambda(d),\qquad 0\le b(n)\le\log n.
$$

Both variables lie between constant multiples of $N^{1/3}$ and $N^{2/3}$, well inside the Type II range. Divide $b(n)$ by $\log N$, and apply the [Type II sum](../../../analytic-number-theory.md#type-ii-sum) estimate. If the product cutoff is kept explicitly, [Fourier separation of interval cutoffs](../../../analytic-number-theory.md#fourier-separation-of-interval-cutoffs) costs only one extra logarithm; zero extension also permits its omission. There are $O(\log^2N)$ boxes in the [dyadic decomposition](../../../analytic-number-theory.md#dyadic-decomposition). The coefficient bound and, where needed, [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) cost at most one more logarithm. These estimates give the convenient bound

$$
\left|\sum_{n\le N}\Lambda(n)f(n)\right|\ll\delta N\log^4N+N^{2/3+1/100}\log N+N^{1/3}\log N.
$$

With $\delta=(\log N)^{-20}$, each term is $o(N)$, proving the assertion. The grouping of the long term uses the nonnegativity of the [Von Mangoldt function](../../../number-theory.md#von-mangoldt-function); more usual groupings instead control a divisor coefficient by a second-moment truncation. [Ben Green's notes, Sections 2.3–2.4](https://arxiv.org/pdf/0710.0823) describe that standard alternative.

Now take the sign version of the [Thue–Morse sequence](../../../real-analysis.md#thue-morse-sequence), $f(n)=(-1)^{s_2(n)}$. Concatenation of [binary digits](../../../number-theory.md#binary-digit) gives $f(a2^j+r)=f(a)f(r)$ for $0\le r<2^j$. Expanding over all choices of digits proves the [Thue–Morse Fourier product](../../../real-analysis.md#thue-morse-fourier-product)

$$
S_j(\theta):=\sum_{0\le r<2^j}f(r)e(r\theta)=\prod_{l=0}^{j-1}(1-e(2^l\theta)).
$$

Pair adjacent factors. If $u=|\cos(\pi t)|$, their modulus is

$$
|(1-e(t))(1-e(2t))|=8u(1-u^2)\le\frac{16}{3\sqrt3}=:B<4,
$$

since the maximum on $[0,1]$ occurs at $u=1/\sqrt3$. Thus $|S_j(\theta)|\ll2^{\sigma j}$ uniformly, where $\sigma=\frac12\log_2B=2-\frac34\log_23<1$.

Every integer interval $J\subset[0,N]$ is a disjoint union of aligned binary blocks with at most two blocks of each length. On such a block the digit concatenation identity and the [Thue–Morse Fourier product](../../../real-analysis.md#thue-morse-fourier-product) give the same bound, up to a unit phase. Summing the [geometric series](../../../real-analysis.md#geometric-series) proves the [uniform interval cancellation for binary digit parity](../../../real-analysis.md#uniform-interval-cancellation-for-binary-digit-parity)

$$
\sup_{\theta,J}\left|\sum_{r\in J}f(r)e(r\theta)\right|\ll N^\sigma.
$$

For a fixed $m$, the sum $\sum_{n\in I_m}f(mn)$ is a sum over multiples of $m$ in an integer interval $J\subset[1,N]$. The additive [character orthogonality](../../../representation-theory.md#character-orthogonality) filter gives

$$
\sum_{\substack{r\in J\\m\mid r}}f(r)=\frac1m\sum_{a=0}^{m-1}\sum_{r\in J}f(r)e(ar/m).
$$

Its modulus is $O(N^\sigma)$, independently of $m$ and the interval. Summing at most $O(N^{1/100})$ outer values proves the [small Type I sums for binary digit parity](../../../real-analysis.md#small-type-i-sums-for-binary-digit-parity):

$$
\boxed{\frac1N\sum_{m\in D_M}\left|\sum_{n\in I_m}f(mn)\right|\ll N^{\sigma+1/100-1},\qquad \sigma+1/100<1.}
$$

This is smaller than $(\log N)^{-20}$ for sufficiently large $N$. It proves the required Type I cancellation; the substantially harder Type II cancellation is not needed for this final clause.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
