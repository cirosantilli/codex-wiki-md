# Paper 29

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_29.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_29.pdf)

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

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $\mu$ be the [Möbius function](../../../number-theory.md#mobius-function). Its [Möbius divisor-sum identity](../../../number-theory.md#mobius-divisor-sum-identity) is

$$
\sum_{d\mid n}\mu(d)=\begin{cases}1,&n=1,\\0,&n>1.\end{cases}
$$

Indeed, for $n>1$ the sum is the expansion of $\prod_{p\mid n}(1-1)$; nonsquarefree [divisors](../../../number-theory.md#divisor) contribute zero. Thus, for [arithmetic functions](../../../number-theory.md#arithmetic-function) $a,b$,

$$
\boxed{b(n)=\sum_{d\mid n}a(d)\iff a(n)=\sum_{d\mid n}\mu(d)b(n/d).}
$$

To prove [Möbius inversion](../../../number-theory.md#mobius-inversion-formula), substitute the first formula into the second and collect the coefficient of $a(e)$. It is $\sum_{d\mid n/e}\mu(d)$, which is one for $e=n$ and zero otherwise. Conversely the same [divisor](../../../number-theory.md#divisor) interchange recovers $b$ from the displayed formula for $a$. In [Dirichlet convolution](../../../number-theory.md#dirichlet-convolution) notation this is simply $\mu*\mathbf1=\varepsilon$, where $\varepsilon$ is supported at one.

The [Prime number theorem with classical zero-free-region error](../../../analytic-number-theory.md#prime-number-theorem-with-classical-zero-free-region-error) states that some absolute $c>0$ satisfies

$$
\boxed{\Psi(x):=\sum_{n\leq x}\Lambda(n)=x+O\bigl(xe^{-c\sqrt{\log x}}\bigr).}
$$

Here $\Lambda$ is the [Von Mangoldt function](../../../number-theory.md#von-mangoldt-function). An equivalent prime-counting form, after decreasing $c$ if needed, is $\pi(x)=\operatorname{Li}(x)+O(xe^{-c\sqrt{\log x}})$. The contributions of proper [prime powers](../../../number-theory.md#prime-power) are $O(\sqrt x\log^2x)$ and can be absorbed into this error. We use $\Psi$ to keep it distinct from the [Fourier transform](../../../analysis.md#fourier-transform) appearing in Question 5.

Here is a direct deduction of the requested [Mertens bound from a log-integrable Chebyshev error](../../../number-theory.md#mertens-bound-from-a-log-integrable-chebyshev-error) from the stated [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem). First, the [divisor](../../../number-theory.md#divisor) identity gives

$$
1=\sum_{d\leq x}\mu(d)\left\lfloor\frac xd\right\rfloor,
\qquad \left|\sum_{d\leq x}\frac{\mu(d)}d\right|\leq\frac1x+\frac{\lfloor x\rfloor}{x}\leq2.
$$

Second, the exact [Dirichlet convolution](../../../number-theory.md#dirichlet-convolution) identity

$$
\mu(n)\log n=-(\mu*\Lambda)(n)
$$

follows from $\log=\mathbf1*\Lambda$: multiplication of a [Dirichlet convolution](../../../number-theory.md#dirichlet-convolution) by $\log n$ differentiates its two factors, so applying it to $\mu*\mathbf1=\varepsilon$ and convolving again with $\mu$ gives this formula. Summing it yields

$$
\sum_{n\leq x}\mu(n)\log n=-\sum_{d\leq x}\mu(d)\Psi(x/d)
=-x\sum_{d\leq x}\frac{\mu(d)}d+O\left(x\sum_{d\leq x}\frac{e^{-c\sqrt{\log(x/d)}}}{d}\right).
$$

The last harmonic sum is $O(1)$. To see this without an endpoint approximation, split $x/d$ into dyadic ranges $[2^j,2^{j+1})$. In each range $\sum1/d=O(1)$, and its exponential factor is at most $e^{-c\sqrt{j\log2}}$. Their sum over $j\geq0$ converges. The finitely many terms with $1\leq x/d<2$ obey the same estimate after adjusting the constant in the prime-number-theorem error. Therefore

$$
\sum_{n\leq x}\mu(n)\log n=O(x).
$$

For the [Mertens function](../../../number-theory.md#mertens-function) $M(x)=\sum_{n\leq x}\mu(n)$,

$$
M(x)\log x=\sum_{n\leq x}\mu(n)\log n+\sum_{n\leq x}\mu(n)\log(x/n).
$$

The second sum has absolute value at most $\sum_{n\leq x}\log(x/n)=O(x)$, by an integral comparison or the [Stirling formula](../../../real-analysis.md#stirling-formula). Consequently

$$
\boxed{\frac{|M(x)|}{x}\ll\frac1{\log x}\qquad(x\geq2).}
$$

The absolute value in this conclusion is present in the original PDF.

## 2

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For the unit-modulus [prime](../../../number-theory.md#prime-number) values in this question, the [Granville-Soundararajan distance](../../../number-theory.md#pretentious-distance) is

$$
\boxed{D(f,g;X)^2=\sum_{p\leq X}\frac{1-\operatorname{Re}(f(p)\overline{g(p)})}{p}
=\frac12\sum_{p\leq X}\frac{|f(p)-g(p)|^2}{p}.}
$$

The second identity uses $|f(p)|=|g(p)|=1$. Thus it is the [Euclidean distance](../../../topological-analysis.md#euclidean-distance) between the finite weighted vectors $(f(p)/\sqrt{2p})_{p\leq X}$ and $(g(p)/\sqrt{2p})_{p\leq X}$. Nonnegativity, symmetry and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) follow from that [norm](../../../functional-analysis.md#norm) representation, and it vanishes exactly when the two prime-value vectors agree. This proves the [prime-restriction metric for pretentious distance](../../../number-theory.md#prime-restriction-metric-for-pretentious-distance).

**On whole [arithmetic functions](../../../number-theory.md#arithmetic-function) at fixed $X$ it is a [pseudometric](../../../topological-analysis.md#pseudometric).** For example $f=\mathbf1$ and $g=\mu^2$ have identical values at every [prime](../../../number-theory.md#prime-number) and zero distance for every $X$, but different values at four. Thus the literal identity-of-indiscernibles assertion needs the prime-restriction quotient.

Since $\mu(p)=-1$,

$$
D(1,\mu;X)^2=2\sum_{p\leq X}\frac1p.
$$

For completeness, [partial summation](../../../analytic-number-theory.md#abel-s-summation-formula) and the prime-counting form of the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem) give

$$
\sum_{p\leq X}\frac1p=\frac{\pi(X)}X+\int_2^X\frac{\pi(u)}{u^2}\,du
=\log\log X+B_1+o(1).
$$

To verify the constant and the error, replace $\pi$ by $\operatorname{Li}+E$ in the first expression. Differentiating $\operatorname{Li}(u)/u$ shows its two contributions combine to $\log\log X$ plus a constant. The error integral converges absolutely because $|E(u)|/u^2\ll e^{-c\sqrt{\log u}}/u$, and $E(X)/X\to0$. This proves the [Mertens second theorem](../../../analytic-number-theory.md#mertens-second-theorem) in the form needed here. In particular the [pretentious distance between one and the Möbius function](../../../number-theory.md#pretentious-distance-between-one-and-the-mobius-function) satisfies

$$
\boxed{D(1,\mu;X)^2=2\log\log X+2B_1+o(1),\qquad D(1,\mu;X)\sim\sqrt{2\log\log X}.}
$$

For the last request, retain the earlier [prime](../../../number-theory.md#prime-number) normalization $|f(p)|=1$; the proof also works with the weaker assumption $|f(p)|\leq1$. Without a bound on [prime](../../../number-theory.md#prime-number) values, the original definition and the [absolute convergence](../../../real-analysis.md#absolute-convergence) of the displayed measure need not apply to an unrestricted [multiplicative arithmetic function](../../../number-theory.md#multiplicative-function). For example $f(n)=\mu(n)^2n$ is multiplicative and squarefree-supported, but for $X>e$ the displayed measure has infinite positive mass: its [prime](../../../number-theory.md#prime-number) terms alone are $\sum_p p^{-1/\log X}$, which diverges by the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem).

Put $L=\log X$, $\sigma=1+1/L$, and use the [Fourier transform](../../../analysis.md#fourier-transform) convention $\widehat\nu(t)=\int e^{-itu}\,d\nu(u)$. Since $f$ is supported on [squarefree integers](../../../number-theory.md#squarefree-integer), the defining property of a [multiplicative arithmetic function](../../../number-theory.md#multiplicative-function) gives the absolutely convergent [Euler product](../../../analytic-number-theory.md#euler-product)

$$
\widehat\nu(t)=\sum_{n\geq1}\frac{f(n)}{n^{\sigma+it}}
=\prod_p\left(1+\frac{f(p)p^{-it}}{p^\sigma}\right).
$$

The bound on [prime](../../../number-theory.md#prime-number) values gives $|f(n)|\leq1$ for squarefree $n$, so the [total variation norm of a measure](../../../measure-theory.md#total-variation-norm-of-a-measure) is bounded by $\zeta(\sigma)$; thus $\nu$ is a [finite measure](../../../measure-theory.md#finite-measure). Expanding the logarithm of the modulus, with an absolute $O(1)$ remainder since $\sum_pp^{-2\sigma}\ll1$, gives

$$
\log|\widehat\nu(t)|=\sum_p\frac{\operatorname{Re}(f(p)p^{-it})}{p^\sigma}+O(1).
$$

All constants here are uniform in $t$. Moreover

$$
\sum_pp^{-\sigma}=\log\zeta(\sigma)+O(1)=\log L+O(1),
$$

using the pole of the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function). The nonnegative deficits $1-\operatorname{Re}(f(p)p^{-it})$ give

$$
\sum_p\frac{1-\operatorname{Re}(f(p)p^{-it})}{p^\sigma}
\geq D(f,n^{it};X)^2-O(1).
$$

Indeed, the replacement of $p^{-\sigma}$ by $1/p$ for $p\leq X$ costs at most

$$
2\sum_{p\leq X}\frac{1-p^{-1/L}}p
\leq\frac2L\sum_{p\leq X}\frac{\log p}p=O(1),
$$

by the [Mertens first theorem](../../../analytic-number-theory.md#mertens-first-theorem), while discarding the $p>X$ terms costs nothing in this lower bound. Thus the [large Fourier coefficient criterion for pretentiousness](../../../number-theory.md#large-fourier-coefficient-criterion-for-pretentiousness) is

$$
|\widehat\nu(t)|\leq C\log X\,e^{-D(f,n^{it};X)^2}.
$$

In particular,

$$
|\widehat\nu(t)|\geq\delta\log X\ \Longrightarrow\
\boxed{D(f,n^{it};X)^2\leq\log(C/\delta)=O_\delta(1).}
$$

The comparison function is the [Archimedean character](../../../number-theory.md#archimedean-character) $n^{it}$ with this sign because our [Fourier transform](../../../analysis.md#fourier-transform) uses $e^{-itu}$.

## 3

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For $\operatorname{Re}s>1$, define the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) by the absolutely convergent [Dirichlet series](../../../analytic-number-theory.md#dirichlet-series)

$$
\zeta(s)=\sum_{n\geq1}n^{-s}=\prod_p(1-p^{-s})^{-1}.
$$

The [Euler product](../../../analytic-number-theory.md#euler-product) follows from [unique prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic) and [absolute convergence](../../../real-analysis.md#absolute-convergence). The counting-function integral gives

$$
\zeta(s)=s\int_1^\infty\lfloor u\rfloor u^{-s-1}\,du
=\frac{s}{s-1}-s\int_1^\infty\{u\}u^{-s-1}\,du.
$$

Because the [fractional part](../../../calculus.md#fractional-part) is bounded, the last integral, and its derivatives with respect to $s$ on compact subsets, converge uniformly for $\operatorname{Re}s>0$. It is a [holomorphic function](../../../complex-analysis.md#holomorphic-function) there. This proves the [Meromorphic continuation of the Riemann zeta function to the right half-plane](../../../analytic-number-theory.md#meromorphic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane), with a [simple pole](../../../isolated-singularity.md#simple-pole) at one of [residue](../../../analysis.md#residue) one and no other singularity in that half-plane.

The [Gamma function](../../../complex-analysis.md#gamma-function) is

$$
\Gamma(z)=\int_0^\infty e^{-u}u^{z-1}\,du\qquad(\operatorname{Re}z>0).
$$

The [Gamma function recurrence](../../../complex-analysis.md#gamma-function-recurrence) extends it meromorphically; its poles are at the nonpositive integers and it has no zeros. The [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) can be stated as

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s),}
$$

or, equivalently,

$$
\boxed{\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s).}
$$

These are identities of [meromorphic functions](../../../isolated-singularity.md#meromorphic-function); the second also extends the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) to the remaining half-plane. The [critical strip](../../../analytic-number-theory.md#critical-strip) is $0<\operatorname{Re}s<1$; its boundary lines will also be treated below, rather than included among possible exceptional zeros.

For $\operatorname{Re}s>1$, the absolutely convergent reciprocal [Euler product](../../../analytic-number-theory.md#euler-product) gives $\zeta(s)\neq0$. For $\operatorname{Re}s<0$, the factors $2^s$, $\pi^{s-1}$, $\Gamma(1-s)$ and $\zeta(1-s)$ in the second [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) are finite and nonzero. Hence the only zeros there are the zeros of the sine factor:

$$
\boxed{s=-2,-4,-6,\ldots.}
$$

Each is simple. At zero, the sine zero cancels the pole of $\zeta(1-s)$; using its [residue](../../../analysis.md#residue) one gives $\zeta(0)=-1/2$, not zero. Nonvanishing on the rest of $\operatorname{Re}s=0$ follows from the boundary-line proof below and the [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function). Together these facts prove that the [trivial zeros of the Riemann zeta function](../../../analytic-number-theory.md#trivial-zero-of-the-riemann-zeta-function) are the only zeros outside the open [critical strip](../../../analytic-number-theory.md#critical-strip).

Here is a [Jensen disk proof of the zeta zero-count bound](../../../analytic-number-theory.md#jensen-disk-proof-of-the-zeta-zero-count-bound) which avoids any unproved left-half-plane growth estimate. Set $F(s)=(s-1)\zeta(s)$, a [holomorphic function](../../../complex-analysis.md#holomorphic-function) throughout $\operatorname{Re}s>0$, including at one. The integral continuation formula gives

$$
|F(s)|\ll(|s|+1)^2\qquad(\operatorname{Re}s\geq1/4).
$$

For each integer $j$, apply [Jensen's formula](../../../complex-analysis.md#jensen-s-formula) in the disk with centre $2+ij$, outer radius $R=7/4$ and inner radius $r=8/5$. The outer disk stays in $\operatorname{Re}s\geq1/4$, so its maximum modulus is $O((|j|+2)^2)$. At its centre,

$$
|\zeta(2+ij)|\geq\zeta(2)^{-1},
\qquad |F(2+ij)|\geq|1+ij|/\zeta(2),
$$

since $|1/\zeta(2+ij)|\leq\sum_n|\mu(n)|n^{-2}\leq\zeta(2)$. Therefore the number of zeros in its inner disk, counted with multiplicity, is at most

$$
\frac{\log\bigl(\max_{|s-(2+ij)|\leq R}|F(s)|/|F(2+ij)|\bigr)}{\log(R/r)}
\ll\log(|j|+2).
$$

The rectangle $1/2\leq\operatorname{Re}s\leq1$, $|\operatorname{Im}s-j|\leq1/2$ fits in the inner disk because its farthest point has distance $\sqrt{(3/2)^2+(1/2)^2}=\sqrt{5/2}<8/5$. Summing over $O(T)$ such disks counts $O(T\log T)$ zeros in the right half of the [critical strip](../../../analytic-number-theory.md#critical-strip) up to height $T$. The first [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) bijects zeros, with multiplicities, in the left half with their reflections $s\mapsto1-s$ in the right half; its [Gamma function](../../../complex-analysis.md#gamma-function) factors are finite and nonzero in the strip. Thus

$$
\boxed{\#\{\rho:\zeta(\rho)=0,\ 0<\operatorname{Re}\rho<1,\ |\operatorname{Im}\rho|\leq T\}\ll T\log T.}
$$

The pole of [zeta function](../../../analytic-number-theory.md#riemann-zeta-function) at one does not count as a zero: $F(1)=1$.

Finally, for real $\sigma>1$ and $t\neq0$, the Euler-product logarithms and the nonnegative [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial)

$$
3+4\cos\theta+\cos(2\theta)=2(1+\cos\theta)^2\geq0
$$

give the [three-four-one product proof of zeta boundary nonvanishing](../../../analytic-number-theory.md#three-four-one-product-proof-of-zeta-boundary-nonvanishing):

$$
\log\bigl(\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\bigr)
=\sum_{p,k\geq1}\frac{3+4\cos(kt\log p)+\cos(2kt\log p)}{kp^{k\sigma}}\geq0.
$$

If $\zeta(1+it)$ had a zero of order $a\geq1$, its factor would be $O((\sigma-1)^{4a})$ as $\sigma\downarrow1$. The real [zeta function](../../../analytic-number-theory.md#riemann-zeta-function) factor has pole order three, and the factor at $1+2it$ stays bounded because $t\neq0$. The product would tend to zero as $O((\sigma-1)^{4a-3})$, contradicting that it is at least one. Therefore

$$
\boxed{\zeta(1+it)\neq0\qquad(t\neq0).}
$$

At $t=0$ there is a pole, not a zero. Applying the sine-form [functional equation of the Riemann zeta function](../../../analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function) at $s=it\neq0$ now proves nonvanishing on the remaining imaginary axis, completing the earlier assertion about all zeros outside the [critical strip](../../../analytic-number-theory.md#critical-strip).

## 4

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A precise useful form of the principle is the [type I–type II inverse principle for Möbius correlation](../../../number-theory.md#type-i-type-ii-inverse-principle-for-mobius-correlation). Normalize $|f(n)|\leq1$, and suppose

$$
\left|\sum_{n\leq X}\mu(n)f(n)\right|\geq\delta X.
$$

For any positive integer cutoffs $U,V$ with $U+V\leq\delta X/2$, define

$$
c_d=\sum_{\substack{bc=d\\b\leq U,\ c\leq V}}\mu(b)\mu(c),
\qquad a_d=\sum_{\substack{c\mid d\\c>V}}\mu(c).
$$

Then $|c_d|,|a_d|\leq\tau(d)$, where $\tau$ is the [divisor function](../../../number-theory.md#divisor-function), and at least one of the following two sums has modulus at least $\delta X/4$:

$$
T_{\mathrm I}=\sum_{d\leq UV}c_d\sum_{k\leq X/d}f(dk),
\qquad
T_{\mathrm {II}}=\sum_{\substack{d>V,\ w>U\\dw\leq X}}a_d\mu(w)f(dw).
$$

The first is correlation against a controlled linear combination of indicators of multiples of small moduli, each a [periodic function](../../../function.md#periodic-function): this is the “somewhat periodic” branch. The second is a [bilinear sum](../../../analytic-number-theory.md#bilinear-sum) with independently weighted factors, both larger than the cutoffs: this is the “somewhat multiplicative” branch. The statement concerns these precise correlations, not an assertion that $f$ must itself be periodic or multiplicative.

For clarity, the [Vaughan identity for the Möbius function](../../../number-theory.md#vaughan-identity-for-the-mobius-function) proves this version immediately. Split $\mu=\mu_{\leq U}+\mu_{>U}$ and likewise at $V$. Since $\mu*\mu*\mathbf1=\mu$,

$$
\boxed{\mu=\mu_{\leq U}+\mu_{\leq V}
-\mu_{\leq U}*\mu_{\leq V}*\mathbf1
+\mu_{>U}*\mu_{>V}*\mathbf1.}
$$

Multiply by $f(n)$ and sum. The first two terms contribute at most $U+V$ in modulus, and the remaining terms are $-T_{\mathrm I}+T_{\mathrm {II}}$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives the stated dichotomy. It is valid at finite $X$ and for any chosen cutoffs in the indicated range.

We now prove the required orthogonality without appealing to a stronger uniform exponential-sum theorem. Write $\alpha=\sqrt2$ and $e(u)=e^{2\pi iu}$. The [Diophantine bound for the square root of two](../../../number-theory.md#diophantine-bound-for-the-square-root-of-two) is

$$
\|h\alpha\|\geq\frac1{4h}\qquad(h\geq1),
$$

where $\|u\|$ is distance to the nearest integer. If $a$ is that nearest integer, then $|2h^2-a^2|\geq1$, while $h\sqrt2+a\leq4h$; dividing proves the bound.

Use the preceding [Dirichlet convolution](../../../number-theory.md#dirichlet-convolution) identity with $U=V=P=\lfloor X^{1/10}\rfloor$. The two short terms are $O(P)$. For the [type I sum](../../../analytic-number-theory.md#type-i-sum), the [exponential geometric sum bound](../../../real-analysis.md#exponential-geometric-sum-bound) gives

$$
\left|\sum_{k\leq X/d}e(\alpha dk)\right|
\ll\min\{X/d,\|d\alpha\|^{-1}\}\ll d.
$$

Consequently

$$
|T_{\mathrm I}|\ll\sum_{d\leq P^2}\tau(d)d
\ll P^4\log(2P)=O(X^{2/5}\log X),
$$

using $\sum_{d\leq Y}\tau(d)\ll Y\log(2Y)$ from counting factor pairs.

For the [type II sum](../../../analytic-number-theory.md#type-ii-sum), perform a [dyadic decomposition](../../../analytic-number-theory.md#dyadic-decomposition) into $d\in(D,2D]$, $w\in(W,2W]$, keeping $dw\leq X$. Nonempty blocks have $DW<X$, while $D,W\gg P$. A block $B$ satisfies, by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the [divisor-square summatory bound](../../../number-theory.md#divisor-square-summatory-bound),

$$
|B|^2\ll D\log^3X\left(DW+W\sum_{1\leq h\leq W}\min\{D,\|h\alpha\|^{-1}\}\right).
$$

To justify the cutoff, after expanding the square the permissible $d$ for a pair $w,w'$ still form an interval, with upper endpoint $\min(2D,X/\max(w,w'))$. Its exponential sum has the same geometric bound. Diagonal pairs supply $DW$; for each nonzero difference $h=w-w'$ there are $O(W)$ pairs.

The points $0,\alpha,2\alpha,\ldots,\lfloor W\rfloor\alpha$ modulo one are separated by at least $1/(4W)$. Counting points in consecutive distance bands around zero therefore gives

$$
\sum_{1\leq h\leq W}\|h\alpha\|^{-1}\ll W\log(2W).
$$

Substitution yields the [bilinear cancellation for badly approximable phases](../../../analytic-number-theory.md#bilinear-cancellation-for-badly-approximable-phases) estimate

$$
|B|\ll DW\log^2X\left(D^{-1/2}+W^{-1/2}\right)
\ll X\log^2X\,P^{-1/2}.
$$

There are $O(\log^2X)$ blocks, so $T_{\mathrm {II}}\ll X^{19/20}\log^4X$. The divisor-square bound itself can be obtained elementarily from $\tau(n)^2\leq\tau_4(n)$ prime-power by prime-power and $\sum_{n\leq Y}\tau_4(n)\leq Y(1+\log Y)^3$; no uncontrolled coefficient bound is being suppressed.

Combining the short, type I and type II terms,

$$
\left|\sum_{n\leq X}\mu(n)e(n\sqrt2)\right|
\ll X^{2/5}\log X+X^{19/20}\log^4X+X^{1/10}=o(X).
$$

Hence

$$
\boxed{\lim_{X\to\infty}\frac1X\left|\sum_{n\leq X}\mu(n)e(n\sqrt2)\right|=0.}
$$

## 5

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For a [prime](../../../number-theory.md#prime-number) $p$, the [divisor sum](../../../number-theory.md#divisor-sum) defining the real weight is $\phi(0)-\phi(\log p/\log X)$. If $p>X^{1/3}$, the second term vanishes and the first is one. Thus **$F(p)=1$**, while $F(n)\geq0$ for every integer because $\phi$ is real and the sum is squared.

Put $h(x)=e^x\phi(x)$. With the [Fourier transform](../../../analysis.md#fourier-transform) convention in the question, [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
\psi(t)=\frac1{2\pi}\int_{\mathbb R}h(x)e^{ixt}\,dx.
$$

The function $h$ is [smooth](../../../analysis.md#smooth-function) and has [compact support](../../../function.md#compact-support). Using [integration by parts](../../../calculus.md#integration-by-parts) $k$ times, with zero endpoint terms, proves

$$
|\psi(t)|\leq\frac{\|h^{(k)}\|_1}{2\pi|t|^k}.
$$

Choose an integer $k\geq A$ to obtain **$|\psi(t)|\ll_A|t|^{-A}$ for $|t|\geq1$**. In particular every polynomially weighted absolute integral of $\psi$ is finite.

For the double integral, use

$$
\frac1{2+i(t+t')}=\int_0^\infty e^{-(2+i(t+t'))u}\,du,
\qquad
\phi(u)=\int_{\mathbb R}\psi(t)e^{-(1+it)u}\,dt.
$$

Differentiating the second formula gives $\int\psi(t)(1+it)e^{-(1+it)u}\,dt=-\phi'(u)$. [absolute convergence](../../../real-analysis.md#absolute-convergence) from the rapid decay permits [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem). The [derivative energy constant for a smooth sieve cutoff](../../../analytic-number-theory.md#derivative-energy-constant-for-a-smooth-sieve-cutoff) is therefore

$$
\boxed{\iint\psi(t)\psi(t')\frac{(1+it)(1+it')}{2+i(t+t')}\,dt\,dt'
=c_\phi:=\int_0^\infty\phi'(u)^2\,du
=\int_0^{1/3}\phi'(u)^2\,du.}
$$

There is no [complex conjugate](../../../complex-analysis.md#complex-conjugate) in this integral: the two factors both become $-\phi'(u)$, which is real. The constant is positive; in fact the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) applied to $\phi(1/3)-\phi(0)=-1$ gives $c_\phi\geq3$.

Here is the basic structure of the [smooth divisor-square sieve asymptotic](../../../analytic-number-theory.md#smooth-divisor-square-sieve-asymptotic), with enough uniform estimates to specify the error. Write $L=\log X$ and $R=X^{1/3}$. Expand the square and count multiples of the [least common multiple](../../../number-theory.md#least-common-multiple) $[d,e]$ in an arbitrary interval $I$ of length $X$:

$$
\sum_{n\in I}F(n)=X S_X+O_\phi(R^2),
\qquad
S_X=\sum_{d,e\geq1}\frac{\mu(d)\mu(e)}{[d,e]}\phi\left(\frac{\log d}L\right)\phi\left(\frac{\log e}L\right).
$$

The sum is effectively restricted to $d,e<R$. Each count is $X/[d,e]+O(1)$, independent of the interval's position, so the total error is $O_\phi(X^{2/3})$.

The [Fourier representation of a smooth Selberg weight](../../../analytic-number-theory.md#fourier-representation-of-a-smooth-selberg-weight) reads

$$
\phi\left(\frac{\log d}L\right)=\int_{\mathbb R}\psi(t)d^{-z}\,dt,
\qquad z=\frac{1+it}L.
$$

Hence, with $z'=(1+it')/L$,

$$
S_X=\iint\psi(t)\psi(t')E(z,z')\,dt\,dt',
\qquad
E(z,z')=\prod_p(1-p^{-1-z}-p^{-1-z'}+p^{-1-z-z'}).
$$

The four local terms correspond to the [prime](../../../number-theory.md#prime-number) dividing neither [divisor](../../../number-theory.md#divisor), only the first, only the second, or both. This is the [Euler product for a smoothed divisor-square correlation](../../../analytic-number-theory.md#euler-product-for-a-smoothed-divisor-square-correlation). Factor it as

$$
E(z,z')=\frac{\zeta(1+z+z')}{\zeta(1+z)\zeta(1+z')}H(z,z'),
$$

where

$$
H(z,z')=\prod_p\frac{(1-a_p-b_p+c_p)(1-c_p)}{(1-a_p)(1-b_p)},
\quad a_p=p^{-1-z},\ b_p=p^{-1-z'},\ c_p=p^{-1-z-z'}.
$$

The local factors of $H$ are $1+O(p^{-2+4\eta})$ when $|\operatorname{Re}z|,|\operatorname{Re}z'|\leq\eta$ for small fixed $\eta<1/4$. Thus $H$ is a [holomorphic function](../../../complex-analysis.md#holomorphic-function) near $(0,0)$, and evaluating each local factor at zero gives exactly one. Consequently $H(0,0)=1$ and $H(z,z')=1+O(|z|+|z'|)$ there.

The pole expansion $\zeta(1+w)=w^{-1}+O(1)$ now yields

$$
E(z,z')=\frac1L\frac{(1+it)(1+it')}{2+i(t+t')}
\left(1+O\left(\frac{2+|t|+|t'|}L\right)\right)
$$

when $|t|,|t'|\leq L^{1/4}$. Integrating the error against the rapidly decreasing transforms gives $O_\phi(L^{-2})$. The complementary tails are harmless uniformly: absolute values in the original [divisor](../../../number-theory.md#divisor) series give

$$
|E((1+it)/L,(1+it')/L)|
\leq\prod_p(1+2p^{-1-1/L}+p^{-1-2/L})
\leq\zeta(1+1/L)^3\ll L^3.
$$

Any prescribed power decay of $\int_{|t|>L^{1/4}}|\psi(t)|\,dt$ is available, so these tails and the tails of the limiting kernel are $O_\phi(L^{-2})$ after choosing sufficiently many applications of [integration by parts](../../../calculus.md#integration-by-parts). The same absolute bound justifies the original exchanges of infinite sums and integrals. Using the evaluated double integral,

$$
S_X=\frac{c_\phi}L+O_\phi(L^{-2}).
$$

We conclude, uniformly over all interval locations,

$$
\boxed{\sum_{n\in I}F(n)=c_\phi\frac X{\log X}
+O_\phi\left(\frac X{\log^2X}+X^{2/3}\right)
\sim c_\phi\frac X{\log X}.}
$$

This proof does not assume that the interval starts near the origin.

Finally choose this one fixed [smooth](../../../analysis.md#smooth-function) cutoff. [primes](../../../number-theory.md#prime-number) above $R$ in $(X_0,X_0+X]$ contribute one each to the nonnegative weight, and at most $R$ [primes](../../../number-theory.md#prime-number) lie below $R$. Therefore

$$
\pi(X_0+X)-\pi(X_0)\leq\sum_{X_0<n\leq X_0+X}F(n)+R
\ll\frac X{\log X}
$$

for all sufficiently large $X$, uniformly in $X_0$. The bounded range $2\leq X\leq X_1$ follows by increasing the fixed constant and using the trivial interval bound $X+1$. Thus the [short-interval prime upper bound from a smooth divisor weight](../../../analytic-number-theory.md#short-interval-prime-upper-bound-from-a-smooth-divisor-weight) is

$$
\boxed{\pi(X_0+X)-\pi(X_0)\ll\frac X{\log X}\qquad(X_0,X\geq2).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
