# Fourier series

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fourier_series)

**Table of contents**

- [Square wave](#square-wave)
- [Fourier series of a noninteger-frequency sine](#fourier-series-of-a-noninteger-frequency-sine)
- [Fourier orthogonality](#fourier-orthogonality)
- [Uniqueness of a trigonometric series outside a finite set](#uniqueness-of-a-trigonometric-series-outside-a-finite-set)
- [Riemann summation of a convergent trigonometric series](#riemann-summation-of-a-convergent-trigonometric-series)
- [Decay of coefficients of an almost-everywhere convergent trigonometric series](#decay-of-coefficients-of-an-almost-everywhere-convergent-trigonometric-series)
- [Periodic triangular bump](#periodic-triangular-bump)
- [Du Bois-Reymond theorem](#du-bois-reymond-theorem)
- [Smooth-window Fourier coefficients of a periodic distribution](#smooth-window-fourier-coefficients-of-a-periodic-distribution)
- [Fourier coefficients of a periodic logarithmic singularity](#fourier-coefficients-of-a-periodic-logarithmic-singularity)
- [Cohomological equation on a Diophantine torus](#cohomological-equation-on-a-diophantine-torus)
  - [Translated conjugacy of a Diophantine vector field](#translated-conjugacy-of-a-diophantine-vector-field)
  - [Analytic estimate for the torus cohomological equation](#analytic-estimate-for-the-torus-cohomological-equation)
- [Kahane-Katznelson divergence theorem](#kahane-katznelson-divergence-theorem)
- [Orthogonality of integer Fourier modes](#orthogonality-of-integer-fourier-modes)
- [Dirichlet-Jordan convergence theorem](#dirichlet-jordan-convergence-theorem)
- [Fourier series of a periodically extended quadratic arch](#fourier-series-of-a-periodically-extended-quadratic-arch)
- [Pointwise convergence of a piecewise smooth Fourier series](#pointwise-convergence-of-a-piecewise-smooth-fourier-series)
- [Complex Fourier series](#complex-fourier-series)
- [Reciprocal-square sine series positivity](#reciprocal-square-sine-series-positivity)
- [Wiener algebra](#wiener-algebra)
  - [Character space of the Wiener algebra](#character-space-of-the-wiener-algebra)
  - [Analytic Wiener algebra](#analytic-wiener-algebra)
    - [Character space of the analytic Wiener algebra](#character-space-of-the-analytic-wiener-algebra)
- [Fourier harmonic](#fourier-harmonic)
- [Cotangent partial-fraction Fourier kernel](#cotangent-partial-fraction-fourier-kernel)
  - [Cosecant partial-fraction identity](#cosecant-partial-fraction-identity)
- [Fourier basis](#fourier-basis)
- [Fourier sine series](#fourier-sine-series)
  - [Uniform bound for harmonic sine polynomials](#uniform-bound-for-harmonic-sine-polynomials)
  - [Fourier sine basis](#fourier-sine-basis)
- [Leibniz formula for π](#leibniz-formula-for-pi)
- [Trigonometric polynomial](#trigonometric-polynomial)
  - [Bernstein inequality for trigonometric polynomials](#bernstein-inequality-for-trigonometric-polynomials)
  - [Gram matrix representation of a trigonometric polynomial](#gram-matrix-representation-of-a-trigonometric-polynomial)
    - [Rank-one spectral-factor Gram matrix](#rank-one-spectral-factor-gram-matrix)
  - [Fejér–Riesz theorem](#fejer-riesz-theorem)
  - [Even multiplicity of unit-circle roots of a nonnegative trigonometric polynomial](#even-multiplicity-of-unit-circle-roots-of-a-nonnegative-trigonometric-polynomial)
  - [Conjugate symmetry of trigonometric polynomial coefficients](#conjugate-symmetry-of-trigonometric-polynomial-coefficients)
    - [Reciprocal-conjugate root pairing](#reciprocal-conjugate-root-pairing)
- [Fourier partial sum](#fourier-partial-sum)
  - [Generic unbounded Fourier sums at a fixed point](#generic-unbounded-fourier-sums-at-a-fixed-point)
  - [de la Vallée Poussin sum](#de-la-vallee-poussin-sum)
  - [Bounded nonconvergent Fourier partial sums](#bounded-nonconvergent-fourier-partial-sums)
  - [Frequency-separated Fourier block series](#frequency-separated-fourier-block-series)
  - [Compact-set Fourier amplification lemma](#compact-set-fourier-amplification-lemma)
    - [Positive-real logarithmic amplifier for short arcs](#positive-real-logarithmic-amplifier-for-short-arcs)
  - [Dirichlet kernel](#dirichlet-kernel)
    - [Dirichlet kernel harmonic lower bound](#dirichlet-kernel-harmonic-lower-bound)
- [Fejér kernel](#fejer-kernel)
  - [Fejér sum](#fejer-sum)
    - [Hölder error bound for Fejér summation](#holder-error-bound-for-fejer-summation)
    - [Fejér first-moment approximation bound](#fejer-first-moment-approximation-bound)
      - [Fractional-scale Fejér approximation bound](#fractional-scale-fejer-approximation-bound)
    - [Fejér second-modulus approximation bound](#fejer-second-modulus-approximation-bound)
      - [Fejér saturation on a Fourier mode](#fejer-saturation-on-a-fourier-mode)
    - [Fejér summation is a uniform-norm contraction](#fejer-summation-is-a-uniform-norm-contraction)
- [Fourier coefficient](#fourier-coefficient)
  - [Periodic dilation annihilates low Fourier modes](#periodic-dilation-annihilates-low-fourier-modes)
  - [Absolute Fourier convergence from a square-integrable derivative](#absolute-fourier-convergence-from-a-square-integrable-derivative)
  - [Uniqueness of Fourier coefficients in L1](#uniqueness-of-fourier-coefficients-in-l1)
  - [Fourier coefficient decay of an analytic periodic function](#fourier-coefficient-decay-of-an-analytic-periodic-function)
  - [Termwise differentiation of a Fourier series](#termwise-differentiation-of-a-fourier-series)
- [Fourier cosine series](#fourier-cosine-series)
  - [Half-range Fourier cosine series](#half-range-fourier-cosine-series)
- [Fourier series of x cubed minus pi squared x](#fourier-series-of-x-cubed-minus-pi-squared-x)

## Square wave

↑ **Parent:** [Fourier series](fourier-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square_wave)

A [square wave](#square-wave) alternates between two constant values for equal halves of a [period](mathematics.md#period-of-a-function). For the $2\pi$-periodic function equal to $1$ on $(0,\pi)$ and $-1$ on $(\pi,2\pi)$, the [Fourier coefficients](#fourier-coefficient) are $a_0=a_n=0$ and $b_n=2[1-(-1)^n]/(\pi n)$. Its [Fourier series](fourier-series.md) contains only odd [sine](geometry-and-topology.md#sine) modes. At a [jump discontinuity](calculus.md#jump-discontinuity) the [Fourier series](fourier-series.md) converges to the midpoint $0$, irrespective of the assigned point value.

## Fourier series of a noninteger-frequency sine

↑ **Parent:** [Fourier series](fourier-series.md)

For real noninteger $\lambda$, the periodic extension from $[-\pi,\pi]$ has the displayed [Fourier series](fourier-series.md), obtained by the product-to-sum identity in the sine coefficient integral. It equals the original function in the open interval and zero at the periodic endpoint jumps. At $\lambda=1/2$, [Parseval's identity](fourier-analysis.md#parseval-identity) gives $\sum_{n\geq1}n^2/(4n^2-1)^2=\pi^2/64$. Integer frequencies instead already belong to the ordinary sine basis and should not be substituted into the removable coefficient singularities without taking limits.

## Fourier orthogonality

↑ **Parent:** [Fourier series](fourier-series.md)

The complex [exponential functions](calculus.md#exponential-function) $e^{int}$, for integers $n$, are orthogonal under the normalized integral [inner product](linear-algebra.md#inner-product) on a full period. If $n=m$ the integrand is one; otherwise integrating the exponential gives zero because its endpoint values coincide. Sine and cosine orthogonality follow by taking real and imaginary parts.

## Uniqueness of a trigonometric series outside a finite set

↑ **Parent:** [Fourier series](fourier-series.md)

If the symmetric partial sums of $\sum_{r\in\mathbb Z}a_re^{irt}$ tend to zero at every point outside a finite set, then all coefficients vanish. Almost-everywhere convergence first gives $a_{\pm n}\to0$. The twice-integrated series $F(t)=a_0t^2/2-\sum_{r\ne0}a_re^{irt}/r^2$ is continuous. [Riemann summation of a convergent trigonometric series](#riemann-summation-of-a-convergent-trigonometric-series) makes its symmetric second derivative zero away from the exceptional points, so it is affine on each intervening interval. [Sinc-squared summation of a sequence tending to zero](fourier-analysis.md#sinc-squared-summation-of-a-sequence-tending-to-zero) makes its symmetric first-order quotient zero everywhere, removing all possible affine corners. The globally affine function differs from a periodic function by $a_0t^2/2$, forcing $a_0=0$; periodicity then makes it constant, and integration against each nonzero frequency gives $a_r=0$.

## Riemann summation of a convergent trigonometric series

↑ **Parent:** [Fourier series](fourier-series.md)

Suppose the symmetric partial sums converge at a fixed point. Group positive and negative frequencies together, let $S_n$ be the resulting partial sums and set $w(x)=(\sin x/x)^2$, with $w(0)=1$. [Summation by parts](analytic-number-theory.md#abel-s-summation-formula) expresses the weighted sum as $\sum_{n\ge0}S_n[w(nk)-w((n+1)k)]$, where $k=|h|/2$. The total variation of these weights is at most $\int_0^\infty|w'(x)|dx<\infty$, independently of $k$, and each fixed difference tends to zero. Subtract the limiting value of $S_n$ and split into a finite prefix and a uniformly small tail to prove convergence to that value. This is a regular summation method even though the sinc-squared weights need not decrease monotonically.

## Decay of coefficients of an almost-everywhere convergent trigonometric series

↑ **Parent:** [Fourier series](fourier-series.md)

If symmetric partial sums $\sum_{r=-n}^n a_re^{irt}$ converge almost everywhere on the circle, then $a_n,a_{-n}\to0$. Their successive differences $T_n=a_ne^{int}+a_{-n}e^{-int}$ tend to zero almost everywhere. If $M_n=|a_n|+|a_{-n}|$ failed to tend to zero, choose a subsequence with $M_n\ge\varepsilon$. The normalized $T_n/M_n$ are bounded by one and tend to zero almost everywhere, so [dominated convergence](measure-theory.md#dominated-convergence-theorem) makes their squared integrals tend to zero. [Fourier orthogonality](#fourier-orthogonality) instead makes those integrals $(|a_n|^2+|a_{-n}|^2)/M_n^2\ge1/2$, a contradiction.

## Periodic triangular bump

↑ **Parent:** [Fourier series](fourier-series.md)

For $0<\varepsilon\le1/2$, this continuous function on $\mathbb R/\mathbb Z$ has nonnegative [Fourier coefficients](#fourier-coefficient)

$$
\widehat b_\varepsilon(r)=\varepsilon\left(\frac{\sin(\pi r\varepsilon)}{\pi r\varepsilon}\right)^2,
\qquad \widehat b_\varepsilon(0)=\varepsilon.
$$

It is $\varepsilon^{-1}$ times the periodic [convolution](fourier-analysis.md#convolution) of two indicators of $[-\varepsilon/2,\varepsilon/2]$. Its [Fourier series](fourier-series.md) is absolutely convergent, $\sum_r\widehat b_\varepsilon(r)=b_\varepsilon(0)=1$, and $\sum_{|r|>R}\widehat b_\varepsilon(r)\ll1/(\varepsilon R)$. Consequently, if all $N$ points $t_n$ avoid the interval $\|t\|<\varepsilon$, some frequency $1\le r\ll\varepsilon^{-2}$ satisfies $|\sum_ne(rt_n)|\gg N\varepsilon$. This detects missing small neighborhoods by a large [exponential sum](analytic-number-theory.md#exponential-sum).

## Du Bois-Reymond theorem

↑ **Parent:** [Fourier series](fourier-series.md)

There are [continuous functions](calculus.md#continuous-function) whose [Fourier series](fourier-series.md) diverges at a prescribed point. In contrast, the [Fejér kernel](#fejer-kernel) is nonnegative and has integral one, so [Fejér summation is a uniform-norm contraction](#fejer-summation-is-a-uniform-norm-contraction). The resulting [Fejér sums](#fejer-sum) need not be positive: for the [constant function](function.md#constant-function) $f=-1$, every sum is $-1$.

## Smooth-window Fourier coefficients of a periodic distribution

↑ **Parent:** [Fourier series](fourier-series.md)

A smooth compactly supported window with $\sum_{j\in\mathbb Z}\chi(x+j)=1$ permits multiplying every periodic [distribution](distribution-theory.md#distribution-mathematical-analysis) unambiguously. Its [Fourier transform](analysis.md#fourier-transform) sampled at integer harmonics gives the periodic coefficients. The sharp window $H(x)-H(x-1)$ works for locally integrable functions but can be undefined at singular period endpoints, such as delta derivatives.

## Fourier coefficients of a periodic logarithmic singularity

↑ **Parent:** [Fourier series](fourier-series.md)

For the period-one continuation of $\log|x-1/2|$, symmetry and [integration by parts](calculus.md#integration-by-parts) give $c_m=-(-1)^m\operatorname{Si}(\pi m)/(\pi m)$ for $m\ne0$. Thus the [sine integral](calculus.md#sine-integral) asymptotic gives $c_m=-(-1)^m/(2m)+1/(\pi^2m^2)+O(m^{-4})$ as $m\to+\infty$. Translation of the logarithmic singularity causes the alternating phase; the endpoint derivative mismatch causes the next term.

## Cohomological equation on a Diophantine torus

↑ **Parent:** [Fourier series](fourier-series.md)

For a [Diophantine frequency vector](number-theory.md#diophantine-frequency-vector), the equation $\omega\cdot\partial_x f=g$ on a periodic [torus](topology.md#torus) has an analytic solution on each smaller complex strip exactly when $g$ has zero average. Its nonzero [Fourier coefficients](#fourier-coefficient) are $f_k=g_k/(i k\cdot\omega)$, and its zero coefficient is arbitrary. Thus the normalized zero-mean solution is unique.

### Translated conjugacy of a Diophantine vector field

↑ **Parent:** [Cohomological equation on a Diophantine torus](#cohomological-equation-on-a-diophantine-torus)

For a sufficiently small analytic periodic [vector field](calculus.md#vector-field) $w$, a near-identity angular [diffeomorphism](geometry-and-topology.md#diffeomorphism) $\chi$ and a constant vector $a$ solve $D\chi\,\omega=\omega+w\circ\chi+a$. They satisfy $\chi-\mathrm{id}=O(w)$, $a=O(w)$; if $\langle w\rangle=0$, then $a=O(w^2)$. For the defect $e=\mathcal D_\omega\chi-\omega-w\circ\chi-a$, set $A=D\chi$, choose $\Delta a=\langle A^{-1}\rangle^{-1}\langle A^{-1}e\rangle$, and solve $\mathcal D_\omega v=A^{-1}(\Delta a-e)$ with zero mean. Updating $\chi$ by $Av$ leaves a quadratic defect $(De)v-[w(\chi+Av)-w(\chi)-Dw(\chi)Av]$. The [torus small-divisor estimate](#analytic-estimate-for-the-torus-cohomological-equation) and geometrically decreasing strip losses yield a convergent analytic iteration.

### Analytic estimate for the torus cohomological equation

↑ **Parent:** [Cohomological equation on a Diophantine torus](#cohomological-equation-on-a-diophantine-torus)

If $g$ is analytic on a complex strip of width $\sigma$ and has zero mean, the normalized solution satisfies $\|f\|_{\sigma-\delta}\le C_{n,\tau}\gamma^{-1}\delta^{-(n+\tau)}\|g\|_\sigma$. Fourier decay supplies $e^{-\delta|k|_1}$ after the strip loss, and lattice-shell counting bounds the remaining sum $\sum_{k\ne0}|k|_1^\tau e^{-\delta|k|_1}$. This simple bound is sufficient for analytic conjugacy iterations even when sharper estimates are available.

## Kahane-Katznelson divergence theorem

↑ **Parent:** [Fourier series](fourier-series.md)

Every null subset of the circle lies in the divergence set of the [Fourier series](fourier-series.md) of some continuous complex-valued [function](function.md). One can arrange unbounded [Fourier partial sums](#fourier-partial-sum) there. The [compact-set Fourier amplification lemma](#compact-set-fourier-amplification-lemma), [compact batching of a small open set](measure-theory.md#compact-batching-of-a-small-open-set) and [frequency-separated Fourier block series](#frequency-separated-fourier-block-series) construct the function by a summable series of small blocks. The result covers nonclosed and dense null sets; it does not require the divergence set to equal the originally specified set.

## Orthogonality of integer Fourier modes

↑ **Parent:** [Fourier series](fourier-series.md)

For an integer $m$, direct integration gives zero unless $m=0$, in which case it gives one. Products of this identity on the unit cube turn [integrals](calculus.md#integral) of finite [exponential sums](analytic-number-theory.md#exponential-sum) into counts of integer solutions. This is the elementary orthogonality used in the [Vinogradov mean value](analytic-number-theory.md#vinogradov-mean-value).

## Dirichlet-Jordan convergence theorem

↑ **Parent:** [Fourier series](fourier-series.md)

The [Fourier series](fourier-series.md) of a periodic function of [bounded variation](real-analysis.md#total-variation-of-a-function) converges at each point to the mean of its two one-sided limits. In particular, it converges to the function at continuity points. Periodizing a compact interval introduces jumps at its integer endpoints; their half-values explain the half-weight convention in the [Van der Corput sum-integral lemma](analytic-number-theory.md#van-der-corput-sum-integral-lemma). The conclusion is pointwise convergence, not a claim of [absolute convergence](real-analysis.md#absolute-convergence) of every such Fourier series.

## Fourier series of a periodically extended quadratic arch

↑ **Parent:** [Fourier series](fourier-series.md)

The period-one extension of $x(1-x)$ on $[0,1]$ has [Fourier series](fourier-series.md) $1/6-\pi^{-2}\sum_{n\ge1}n^{-2}\cos(2\pi nx)$. Endpoint agreement makes the periodic function continuous. Its derivative series is $(2/\pi)\sum_{n\ge1}n^{-1}\sin(2\pi nx)$, which equals $1-2x$ in the open unit interval and converges to zero at integers, the midpoint of the derivative's jump. [Termwise differentiation of a Fourier series](#termwise-differentiation-of-a-fourier-series) applies locally away from the corners.

## Pointwise convergence of a piecewise smooth Fourier series

↑ **Parent:** [Fourier series](fourier-series.md)

For a periodic [function](function.md) that is piecewise continuously differentiable with finitely many pieces, its [Fourier series](fourier-series.md) converges at each point to the average of the two one-sided limits. At a point of continuity this is the function value. This includes the identified interval endpoints, whose two limits belong to the periodic extension. Absolute summability of the [Fourier coefficients](#fourier-coefficient) additionally gives uniform convergence.

## Complex Fourier series

↑ **Parent:** [Fourier series](fourier-series.md)

The complex form of a [Fourier series](fourier-series.md) for period $2L$ uses coefficients $c_n=(2L)^{-1}\int_{-L}^Lf(x)e^{-in\pi x/L}dx$ and complex exponentials $e^{in\pi x/L}$. For [square-integrable functions](measure-theory.md#square-integrable-function) it converges in the $L^2$ norm, and the [Parseval identity](fourier-analysis.md#parseval-identity) is $(2L)^{-1}\int|f|^2=\sum_n|c_n|^2$. Real functions satisfy $c_{-n}=\overline{c_n}$.

## Reciprocal-square sine series positivity

↑ **Parent:** [Fourier series](fourier-series.md)

The absolutely convergent sine series $S(\xi)=\sum_{l\ge1}\sin(l\xi)/l^2$ has the integral representation $S(\xi)=\sin\xi\int_0^\infty t e^{-t}/(1-2e^{-t}\cos\xi+e^{-2t})\,dt$. The integrand is positive for $0<\xi<\pi$, proving $S>0$ there without incorrectly maximizing individual Fourier terms.

## Wiener algebra

↑ **Parent:** [Fourier series](fourier-series.md)

The Wiener algebra consists of periodic [functions](function.md) with absolutely summable [Fourier coefficients](#fourier-coefficient), with [norm](functional-analysis.md#norm) $\sum_k|a_k|$. Multiplication corresponds to [discrete convolution](fourier-analysis.md#discrete-convolution) of coefficients, so the [norm](functional-analysis.md#norm) is submultiplicative. Consequently $e^f=\sum_{n\ge0}f^n/n!$ also belongs to the algebra when $f$ does. Every such [Fourier series](fourier-series.md) is uniformly convergent and defines a [continuous function](calculus.md#continuous-function).

### Character space of the Wiener algebra

↑ **Parent:** [Wiener algebra](#wiener-algebra)

Every [algebra character](banach-algebra.md#character-of-an-algebra) of the [Wiener algebra](#wiener-algebra) is evaluation at a unique point of the [unit circle](complex-analysis.md#complex-unit-circle). Writing $u(w)=w$, both $u$ and $u^{-1}$ have [norm](functional-analysis.md#norm) one. Thus $z=\phi(u)$ satisfies $|z|\leq1$ and $|z^{-1}|\leq1$, hence $|z|=1$. Continuity then gives $\phi(\sum_{n\in\mathbb Z}a_nu^n)=\sum a_nz^n$. Conversely, evaluation defines a continuous [algebra character](banach-algebra.md#character-of-an-algebra). The resulting bijection is a [homeomorphism](topology.md#homeomorphism) for the [Gelfand topology](banach-algebra.md#gelfand-topology).

### Analytic Wiener algebra

↑ **Parent:** [Wiener algebra](#wiener-algebra)

The analytic Wiener algebra consists of the [power series](real-analysis.md#power-series) $f(z)=\sum_{n\geq0}a_nz^n$ with $\sum_{n\geq0}|a_n|<\infty$, identified with their values on the [unit circle](complex-analysis.md#complex-unit-circle). The [norm](functional-analysis.md#norm) is $\|f\|=\sum|a_n|$. [Discrete convolution](fourier-analysis.md#discrete-convolution) gives multiplication and a submultiplicative [norm](functional-analysis.md#norm); completeness follows from the [absolutely summable sequence space](banach-space.md#absolutely-summable-sequence-space). Each series converges uniformly on the closed [unit disk](geometry-and-topology.md#unit-disk) and is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) in its interior.

#### Character space of the analytic Wiener algebra

↑ **Parent:** [Analytic Wiener algebra](#analytic-wiener-algebra)

Every [algebra character](banach-algebra.md#character-of-an-algebra) of the [analytic Wiener algebra](#analytic-wiener-algebra) is evaluation at a unique point $z$ of the closed [unit disk](geometry-and-topology.md#unit-disk). Indeed, for $u(w)=w$, continuity and multiplicativity give $z=\phi(u)$, $|z|\leq\|u\|=1$ and $\phi(f)=\sum_{n\geq0}a_nz^n$. Conversely, this formula defines a continuous [algebra character](banach-algebra.md#character-of-an-algebra) for every such $z$. The evaluation correspondence is a [homeomorphism](topology.md#homeomorphism) for the [Gelfand topology](banach-algebra.md#gelfand-topology), since the [power series](real-analysis.md#power-series) are uniformly convergent on the closed [unit disk](geometry-and-topology.md#unit-disk).

## Fourier harmonic

↑ **Parent:** [Fourier series](fourier-series.md)

A sinusoidal component at an integer multiple of a fundamental angular frequency. For a $2\pi$-periodic angular coordinate $\phi$, real [Fourier series](fourier-series.md) use $\cos(k\phi)$ and $\sin(k\phi)$. Summing over $q$ equally spaced phases removes every component whose integer $k$ is not a multiple of $q$, since $\sum_{j=0}^{q-1}e^{2\pi i k j/q}=0$ in that case. Indeed, the [geometric series](real-analysis.md#geometric-series) has ratio $w=e^{2\pi i k/q}\ne1$ and sum $(1-w^q)/(1-w)=0$. When $q$ divides $k$, all $q$ terms are one. This cancellation isolates higher-order feedback in [resonant conjunction geometry](classical-mechanics.md#resonant-conjunction-geometry).

## Cotangent partial-fraction Fourier kernel

↑ **Parent:** [Fourier series](fourier-series.md)

For an integer $k\geq2$ and $\operatorname{Im}z>0$, differentiating the partial-fraction expansion of $\pi\cot\pi z$ gives

$$
\sum_{n\in\mathbb Z}(z+n)^{-k}=\frac{(-2\pi i)^k}{(k-1)!}\sum_{r\geq1}r^{k-1}e^{2\pi irz}.
$$

Both differentiated series converge locally uniformly. This kernel computes the [Fourier expansion of a modular form](modular-function.md#fourier-expansion-of-a-modular-form) for holomorphic [Eisenstein series](modular-function.md#eisenstein-series).

### Cosecant partial-fraction identity

↑ **Parent:** [Cotangent partial-fraction Fourier kernel](#cotangent-partial-fraction-fourier-kernel)

For $w\notin\mathbb Z$, integrate $\pi\cot(\pi\zeta)/(\zeta-w)^2$ around large squares whose sides have half-integer coordinates. The [cotangent](geometry-and-topology.md#cotangent) is uniformly bounded on these sides and the integral tends to zero. The [residue theorem](analysis.md#residue-theorem) gives residues $(n-w)^{-2}$ at the integers and $-\pi^2\csc^2(\pi w)$ at $w$, proving the identity. For $\operatorname{Im}w>0$, the geometric-series formula for the [cotangent](geometry-and-topology.md#cotangent) also gives $\pi^2\csc^2(\pi w)=-4\pi^2\sum_{r\geq1}r e^{2\pi irw}$.

## Fourier basis

↑ **Parent:** [Fourier series](fourier-series.md)

On the circle of circumference $2\pi$, the functions $e_k(x)=e^{ikx}$ for $k\in\mathbb Z$ form an orthogonal basis of $L^2$.

## Fourier sine series

↑ **Parent:** [Fourier series](fourier-series.md)

A Fourier sine series expands a function on an interval in the eigenfunctions $\sin(n\pi x/L)$ of the Dirichlet Laplacian. It is the odd Fourier-series extension across the interval endpoints.

### Uniform bound for harmonic sine polynomials

↑ **Parent:** [Fourier sine series](#fourier-sine-series)

For $0<t\leq\pi$, split the sum at $\lfloor1/t\rfloor$. The first part is bounded using $|\sin kt|\leq kt$; [summation by parts](analytic-number-theory.md#abel-s-summation-formula) and the geometric bound on interval sine sums control the rest. The harmonic coefficient sum grows like $\log m$, but cancellations keep the whole [trigonometric polynomial](#trigonometric-polynomial) uniformly bounded. Modulating this polynomial lets a [Fourier partial sum](#fourier-partial-sum) expose the large uncancelled half.

### Fourier sine basis

↑ **Parent:** [Fourier sine series](#fourier-sine-series)

The functions $\sqrt{2/\pi}\sin(nx)$, $n\geq1$, form a complete [orthonormal basis](linear-algebra.md#orthonormal-basis) of $L^2(0,\pi)$. An odd extension to $(-\pi,\pi)$ reduces completeness to that of the [Fourier series](fourier-series.md). Equality of all sine coefficients therefore implies equality almost everywhere; if both functions are continuous, it implies equality everywhere.

<h2 id="leibniz-formula-for-pi">Leibniz formula for π</h2>

↑ **Parent:** [Fourier series](fourier-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Leibniz_formula_for_π)

The Leibniz formula is the conditionally convergent alternating series

$$
\frac\pi4=\sum_{r=0}^{\infty}\frac{(-1)^r}{2r+1}.
$$

## Trigonometric polynomial

↑ **Parent:** [Fourier series](fourier-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trigonometric_polynomial)

A trigonometric polynomial is a finite linear combination of complex exponentials $e^{inx}$, or equivalently of sines and cosines. If it vanishes on an interval, all its coefficients vanish.

### Bernstein inequality for trigonometric polynomials

↑ **Parent:** [Trigonometric polynomial](#trigonometric-polynomial)

A [trigonometric polynomial](#trigonometric-polynomial) of degree at most $n$ obeys the displayed derivative bound. Iteration gives $\|T_n^{(r)}\|_\infty\le n^r\|T_n\|_\infty$. Applied to differences of approximants at dyadic degrees, this inequality underlies the [inverse theorem for trigonometric approximation](uniform-approximation.md#inverse-theorem-for-trigonometric-approximation). It differs from the endpoint-weighted [Bernstein inequality for algebraic polynomials](uniform-approximation.md#bernstein-inequality-for-algebraic-polynomials).

### Gram matrix representation of a trigonometric polynomial

↑ **Parent:** [Trigonometric polynomial](#trigonometric-polynomial)

Under the displayed diagonal-sum convention, set $w(z)=(1,z^{-1},\ldots,z^{-d})^T$ on the [unit circle](complex-analysis.md#complex-unit-circle). A [Hermitian matrix](hilbert-space.md#hermitian-operator) $M$ then gives

$$
p(z)=w(z)^*Mw(z).
$$

Consequently $M\succeq0$ proves nonnegativity. Conversely the [Fejér–Riesz theorem](#fejer-riesz-theorem) produces the [rank-one spectral-factor Gram matrix](#rank-one-spectral-factor-gram-matrix). This gives a [semidefinite programming](convex-optimization.md#semidefinite-programming) representation of nonnegative trigonometric [polynomials](polynomial.md). The reversed convention $j-i=k$ instead uses the unconjugated monomial [vector](vector-space.md#vector).

#### Rank-one spectral-factor Gram matrix

↑ **Parent:** [Gram matrix representation of a trigonometric polynomial](#gram-matrix-representation-of-a-trigonometric-polynomial)

For [coefficient](vector-space.md#coefficient) column $q=(q_0,\ldots,q_d)^T$, $M_{ij}=q_i\overline{q_j}$ is a [Hermitian matrix](hilbert-space.md#hermitian-operator) and a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) because $x^*Mx=|q^*x|^2$. Expanding $|q(z)|^2$ on the [unit circle](complex-analysis.md#complex-unit-circle) gives [coefficient](vector-space.md#coefficient) $p_k=\sum_{i-j=k}M_{ij}$. Thus $M$ has [matrix rank](vector-space.md#matrix-rank) one when $q\ne0$ and zero otherwise. General feasible [Gram matrices](linear-algebra.md#gram-matrix) need not have [matrix rank](vector-space.md#matrix-rank) one.

<h3 id="fejer-riesz-theorem">Fejér–Riesz theorem</h3>

↑ **Parent:** [Trigonometric polynomial](#trigonometric-polynomial)

A [trigonometric polynomial](#trigonometric-polynomial) nonnegative on the [unit circle](complex-analysis.md#complex-unit-circle) has a [polynomial](polynomial.md) modulus-square factor of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most its trigonometric order. For a nonzero [trigonometric polynomial](#trigonometric-polynomial) of actual order $d$, [conjugate symmetry of trigonometric polynomial coefficients](#conjugate-symmetry-of-trigonometric-polynomial-coefficients) yields [reciprocal-conjugate root pairing](#reciprocal-conjugate-root-pairing) for $P=z^dp$. [Even multiplicity of unit-circle roots of a nonnegative trigonometric polynomial](#even-multiplicity-of-unit-circle-roots-of-a-nonnegative-trigonometric-polynomial) permits pairing all $2d$ [roots of a polynomial](polynomial.md#root-of-a-polynomial). Select representatives $\zeta_1,\ldots,\zeta_d$ and use

$$
z-\frac1{\overline{\zeta_i}}
=-\frac z{\overline{\zeta_i}}(\overline z-\overline{\zeta_i})
\quad(|z|=1).
$$

It follows that $p(z)=c\prod_i|z-\zeta_i|^2$ with $c=(-1)^dp_d/\prod_i\overline{\zeta_i}$. Evaluating away from the [roots of a polynomial](polynomial.md#root-of-a-polynomial) gives $c>0$. Thus $q(z)=\sqrt c\prod_i(z-\zeta_i)$ works. Constant and zero [trigonometric polynomials](#trigonometric-polynomial) have constant or zero factors. Different selections of [roots of a polynomial](polynomial.md#root-of-a-polynomial) and constant phases can give different factors.

### Even multiplicity of unit-circle roots of a nonnegative trigonometric polynomial

↑ **Parent:** [Trigonometric polynomial](#trigonometric-polynomial)

If $P=z^dp$ and $p$ is nonnegative on the [unit circle](complex-analysis.md#complex-unit-circle), a [root of a polynomial](polynomial.md#root-of-a-polynomial) $\zeta=e^{i\theta_0}$ there has even [multiplicity of a root](polynomial.md#multiplicity-of-a-root). Indeed $p(e^{i\theta})$ is a [real analytic](analysis.md#real-analytic-function) nonnegative function, whose first nonzero term in its [Taylor series](calculus.md#taylor-series) at a zero must have even order. The map $\theta\mapsto e^{i\theta}-\zeta$ has a simple zero, and multiplication by $e^{-id\theta}$ is nonvanishing, so the order equals the [polynomial](polynomial.md) multiplicity.

### Conjugate symmetry of trigonometric polynomial coefficients

↑ **Parent:** [Trigonometric polynomial](#trigonometric-polynomial)

A [trigonometric polynomial](#trigonometric-polynomial) is real on the [unit circle](complex-analysis.md#complex-unit-circle) precisely when its finite [coefficients](vector-space.md#coefficient) have the displayed symmetry. To prove necessity, conjugate its values on the circle, use $\overline z=z^{-1}$, and compare [coefficients](vector-space.md#coefficient). Multiplying a [coefficient](vector-space.md#coefficient) difference by $z^d$ gives an ordinary [polynomial](polynomial.md) vanishing at infinitely many points, so it is zero. Symmetry also gives $p(z^{-1})=\overline{p(\overline z)}$ for every nonzero complex $z$.

#### Reciprocal-conjugate root pairing

↑ **Parent:** [Conjugate symmetry of trigonometric polynomial coefficients](#conjugate-symmetry-of-trigonometric-polynomial-coefficients)

For a nonzero real-on-the-circle [trigonometric polynomial](#trigonometric-polynomial) of actual order $d$, the [polynomial](polynomial.md) $P(z)=z^dp(z)$ satisfies $P(z)=z^{2d}\overline{P(1/\overline z)}$. Its constant term is the nonzero conjugate of its leading [coefficient](vector-space.md#coefficient). Hence its nonzero [roots of a polynomial](polynomial.md#root-of-a-polynomial) occur in pairs $\zeta,1/\overline\zeta$ with the same [multiplicity of a root](polynomial.md#multiplicity-of-a-root). The [coefficient](vector-space.md#coefficient) reversal and [complex conjugation](complex-analysis.md#complex-conjugation) preserve the exponents of the paired factors. Fixed [roots of a polynomial](polynomial.md#root-of-a-polynomial) on the [unit circle](complex-analysis.md#complex-unit-circle) require nonnegativity, rather than this symmetry alone, to have even multiplicity.

## Fourier partial sum

↑ **Parent:** [Fourier series](fourier-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fourier_partial_sum)

A Fourier partial sum retains the modes with $|k|\leq n$.

### Generic unbounded Fourier sums at a fixed point

↑ **Parent:** [Fourier partial sum](#fourier-partial-sum)

For each integer $m\geq1$, the set of continuous functions satisfying $|S_N(f,0)|\leq m$ for every $N$ is closed in the [uniform norm](functional-analysis.md#supremum-norm). If it contained a ball of radius $r$, subtracting two members of that ball would bound every partial-sum functional norm by $4m/r$. The [Dirichlet kernel harmonic lower bound](#dirichlet-kernel-harmonic-lower-bound) excludes this, so these sets are [nowhere dense](topological-analysis.md#nowhere-dense-set). By the [Baire category theorem](topological-analysis.md#baire-category-theorem), their complement is a dense $G_\delta$ set. Every function in that complement has unbounded Fourier partial sums at zero. Translation gives the same conclusion at any prescribed point. This is a direct [Uniform boundedness principle](banach-space.md#uniform-boundedness-principle) argument on the real [Banach space](banach-space.md) of continuous functions on the circle.

<h3 id="de-la-vallee-poussin-sum">de la Vallée Poussin sum</h3>

↑ **Parent:** [Fourier partial sum](#fourier-partial-sum)

This average of [Fourier partial sums](#fourier-partial-sum) reproduces every degree-at-most-$n$ [trigonometric polynomial](#trigonometric-polynomial). With $\sigma_r=r^{-1}\sum_{j=0}^{r-1}s_j$,

$$
v_{n,m}=\frac{(n+m)\sigma_{n+m}-n\sigma_n}{m},\qquad
\|v_{n,m}\|_\infty\le1+\frac{2n}{m}.
$$

The bound follows because [Fejér summation is a uniform-norm contraction](#fejer-summation-is-a-uniform-norm-contraction). For $n=0$, the term involving $\sigma_0$ is omitted.

### Bounded nonconvergent Fourier partial sums

↑ **Parent:** [Fourier partial sum](#fourier-partial-sum)

A continuous complex-valued [function](function.md) can have uniformly bounded [Fourier partial sums](#fourier-partial-sum) which fail to converge at one point. Normalize harmonic sine polynomials by their harmonic coefficient sums, modulate them into disjoint high-frequency intervals and choose their degrees so that the complete norms are summable. At zero, complete blocks vanish while their midpoint prefixes have a common nonzero value. The [frequency-separated Fourier block series](#frequency-separated-fourier-block-series) gives a uniform bound on every partial sum as well as two distinct subsequential values.

### Frequency-separated Fourier block series

↑ **Parent:** [Fourier partial sum](#fourier-partial-sum)

If [trigonometric polynomials](#trigonometric-polynomial) have spectra in increasing disjoint positive-frequency intervals, the displayed summability gives a continuous uniform sum. At any cutoff its [Fourier partial sum](#fourier-partial-sum) contains complete earlier blocks, at most one active prefix and no later blocks. Differences across an active prefix therefore isolate that block exactly. Fixed-size excursions occurring in arbitrarily late blocks contradict the Cauchy criterion, even when the complete blocks vanish at the point under consideration.

### Compact-set Fourier amplification lemma

↑ **Parent:** [Fourier partial sum](#fourier-partial-sum)

For a compact circle set with normalized [Lebesgue measure](measure-theory.md#lebesgue-measure) at most $\exp(-8\pi M/\varepsilon)$, where $M\geq1$ and $0<\varepsilon\leq1$, the displayed bounds can be realized by a [trigonometric polynomial](#trigonometric-polynomial) with spectrum in a positive-frequency interval arbitrarily far from zero. Take the logarithm of a positive-real-part [Schwarz integral on the unit disk](partial-differential-equation.md#schwarz-integral-on-the-unit-disk) of a small-mean cutoff, truncate after radial dilation, and modulate its bounded imaginary part. A prefix isolates one analytic half and thus reveals the large real part. The separation between small function norm and large [Fourier partial sums](#fourier-partial-sum) drives the [Kahane-Katznelson divergence theorem](#kahane-katznelson-divergence-theorem).

#### Positive-real logarithmic amplifier for short arcs

↑ **Parent:** [Compact-set Fourier amplification lemma](#compact-set-fourier-amplification-lemma)

Let finitely many arcs have centers $\theta_j$, half-lengths $0<\delta_j\leq1$ and $D=\sum_j\delta_j$. Each summand has positive real part on the closed disk, and $\Phi(0)=1$. On the $j$th arc its contribution has real part at least $1/(4D)$. Thus the analytic logarithm $A=\log\Phi$ obeys $A(0)=0$, $|\operatorname{Im}A|<\pi/2$, and $\operatorname{Re}A\geq\log(1/(4D))$ throughout the arc union. Approximate $A$ by an analytic polynomial and modulate its bounded imaginary part; a partial Fourier sum isolates one half of the polynomial, producing a large value from a bounded function.

### Dirichlet kernel

↑ **Parent:** [Fourier partial sum](#fourier-partial-sum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_kernel)

#### Dirichlet kernel harmonic lower bound

↑ **Parent:** [Dirichlet kernel](#dirichlet-kernel)

For $D_N(t)=\sin((N+1/2)t)/\sin(t/2)$, define $\Lambda_N=(2\pi)^{-1}\int_{-\pi}^{\pi}|D_N|$. Evenness and $\sin(t/2)\leq t/2$ on $(0,\pi]$ give $\Lambda_N\geq(2/\pi)\int_0^{(N+1/2)\pi}|\sin v|/v\,dv$. The first $N$ complete sine periods of length $\pi$ have absolute sine integral two, and on the $j$th such interval $1/v\geq1/(j\pi)$. This proves the displayed unbounded lower bound. The real functional $f\mapsto S_N(f,0)$ on continuous functions has norm exactly $\Lambda_N$: the upper bound is its kernel integral, and the continuous functions $D_N/\sqrt{D_N^2+\delta^2}$ approach that bound as $\delta\downarrow0$ by [dominated convergence](measure-theory.md#dominated-convergence-theorem).

<h2 id="fejer-kernel">Fejér kernel</h2>

↑ **Parent:** [Fourier series](fourier-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fejér_kernel)

The Fejér kernel is the arithmetic mean of the Dirichlet kernels. It is nonnegative and has normalized integral one.

<h3 id="fejer-sum">Fejér sum</h3>

↑ **Parent:** [Fejér kernel](#fejer-kernel)

The $n$th Fejér sum is the arithmetic mean of the first $n$ [Fourier partial sums](#fourier-partial-sum). Equivalently, it is the convolution of the function with the [Fejér kernel](#fejer-kernel).

<h4 id="holder-error-bound-for-fejer-summation">Hölder error bound for Fejér summation</h4>

↑ **Parent:** [Fejér sum](#fejer-sum)

For a periodic [Hölder continuous function](sobolev-space.md#holder-condition) of [Hölder exponent](sobolev-space.md#holder-exponent) $0<\alpha<1$ and [Hölder seminorm](sobolev-space.md#holder-seminorm) at most $M$, the degree-$n-1$ [Fejér sum](#fejer-sum) has the displayed [supremum norm](functional-analysis.md#supremum-norm) error bound. In the half-kernel normalization $F_{n-1}=(2n)^{-1}\sin^2(nt/2)/\sin^2(t/2)$, use $F_{n-1}(t)\le\min\{n/2,\pi^2/(2nt^2)\}$. Splitting the convolution error integral at $1/n$ gives the valid constant $C_\alpha=1/[\pi(\alpha+1)]+\pi/(1-\alpha)$. At the endpoint $\alpha=1$ this argument instead gives $O(M\log n/n)$.

<h4 id="fejer-first-moment-approximation-bound">Fejér first-moment approximation bound</h4>

↑ **Parent:** [Fejér sum](#fejer-sum)

The normalized [Fejér kernel](#fejer-kernel) satisfies $0\le F_n(t)\le\min\{n/(2\pi),\pi/(2nt^2)\}$ on $0<|t|\le\pi$. Splitting its first absolute moment at $1/n$ gives $\int|t|F_n(t)dt\le1/(2\pi n)+(\pi/n)\log(\pi n)$. The chaining inequality for the [modulus of continuity](topological-analysis.md#modulus-of-continuity), $\omega(f,t)\le(1+t/\delta)\omega(f,\delta)$, then bounds the [Fejér sum](#fejer-sum) error by $\omega(f,\delta)[1+\delta^{-1}\int|t|F_n]$. Taking $\delta=\log n/n$ proves the stated bound for $n\ge2$ and hence [uniform convergence](real-analysis.md#uniform-convergence) for continuous periodic functions. The logarithm vanishes at $n=1$, so the displayed estimate is not intended at that index.

<h5 id="fractional-scale-fejer-approximation-bound">Fractional-scale Fejér approximation bound</h5>

↑ **Parent:** [Fejér first-moment approximation bound](#fejer-first-moment-approximation-bound)

The positive normalized [Fejér kernel](#fejer-kernel) has a $1/(nt^2)$ tail. Split the error integral at $\delta=n^{-\alpha}$ and use the chaining inequality $\omega(f,t)\leq(1+t/\delta)\omega(f,\delta)$. Its tail contributes at most a constant times $n^{\alpha-1}(1+\alpha\log n)\omega(f,\delta)$. The factor is uniformly bounded for each fixed $\alpha<1$, proving the displayed estimate. Its constant need not remain bounded as $\alpha$ tends to one.

<h4 id="fejer-second-modulus-approximation-bound">Fejér second-modulus approximation bound</h4>

↑ **Parent:** [Fejér sum](#fejer-sum)

The even positive [Fejér kernel](#fejer-kernel) of total mass one gives $\sigma_nf-f=\tfrac12\int F_n(t)[f(\cdot+t)-2f+f(\cdot-t)]dt$. The scaling property of the [second modulus of smoothness](uniform-approximation.md#second-modulus-of-smoothness) bounds this by $\omega_2(f,\delta)(1+\delta^{-2}\int t^2F_n(t)dt)$. On $[-\pi,\pi]$, $\sin(|t|/2)\ge |t|/\pi$ gives $\int t^2F_n(t)dt\le\pi^2/n$. Choose $\delta=n^{-1/2}$. For twice continuously differentiable functions, the [second-difference integral formula](uniform-approximation.md#second-difference-integral-formula) makes the error $O(n^{-1})$.

<h5 id="fejer-saturation-on-a-fourier-mode">Fejér saturation on a Fourier mode</h5>

↑ **Parent:** [Fejér second-modulus approximation bound](#fejer-second-modulus-approximation-bound)

For fixed positive integer $k$ and $n>k$, the [Fourier coefficient](#fourier-coefficient) of the [Fejér kernel](#fejer-kernel) at frequency $k$ multiplies the mode by $1-k/n$. The displayed error is exact. Consequently the order $n^{-1}$ cannot be replaced by $o(n^{-1})$ for all twice continuously differentiable periodic functions, even though each fixed Fourier mode is infinitely differentiable.

<h4 id="fejer-summation-is-a-uniform-norm-contraction">Fejér summation is a uniform-norm contraction</h4>

↑ **Parent:** [Fejér sum](#fejer-sum)

The [Fejér kernel](#fejer-kernel) is nonnegative and has unit mass in its convolution normalization. The integral triangle inequality therefore bounds the [supremum norm](functional-analysis.md#supremum-norm) of a [Fejér sum](#fejer-sum) by that of the original function. In the half-kernel convention $F_n=(2n)^{-1}|\sum_{j=0}^{n-1}e^{ijt}|^2$, its integral is $\pi$ and the convolution prefactor is $1/\pi$.

## Fourier coefficient

↑ **Parent:** [Fourier series](fourier-series.md)

For a function of period $L$, its complex Fourier coefficients are

$$
\widehat f_n=\frac1L\int_{x_0}^{x_0+L}f(x)e^{-2\pi inx/L}\,dx.
$$

### Periodic dilation annihilates low Fourier modes

↑ **Parent:** [Fourier coefficient](#fourier-coefficient)

If $f$ is integrable and $2\pi$-periodic and $n$ is a positive integer, then $\int_0^{2\pi}f(nx)e^{imx}\,dx=0$ for every integer $m$ with $0<|m|<n$. Split the integral into $n$ equal intervals and substitute $y=nx-2\pi j$ to obtain

$$
\frac1n\int_0^{2\pi}f(y)e^{imy/n}\,dy
\sum_{j=0}^{n-1}e^{2\pi imj/n}=0.
$$

The [root of unity](algebra.md#root-of-unity) sum vanishes by the finite [geometric series](real-analysis.md#geometric-series) formula. The zero mode is $\int f$, so a mean-zero dilated function is orthogonal to all [trigonometric polynomials](#trigonometric-polynomial) of degree at most $n-1$.

### Absolute Fourier convergence from a square-integrable derivative

↑ **Parent:** [Fourier coefficient](#fourier-coefficient)

For a periodic absolutely continuous [function](function.md) with derivative in $L^2$, [integration by parts](calculus.md#integration-by-parts) gives $\widehat{f'}(n)=in\widehat f(n)$. [Bessel's inequality](hilbert-space.md#bessel-s-inequality) and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) prove the displayed bound in the normalized circle norm. Adding the constant coefficient gives an absolutely and uniformly convergent [Fourier series](fourier-series.md). Merely bounding individual coefficients by $O(1/|n|)$ would not establish absolute convergence.

### Uniqueness of Fourier coefficients in L1

↑ **Parent:** [Fourier coefficient](#fourier-coefficient)

If a periodic integrable function has all [Fourier coefficients](#fourier-coefficient) zero, it vanishes almost everywhere. Its [Fejér sums](#fejer-sum) vanish, whereas the [Fejér kernel](#fejer-kernel) is an approximate identity and converges to that function in the integrable norm. Applied to a periodized squared [Fourier transform](analysis.md#fourier-transform), this detects orthogonality of integer translates.

### Fourier coefficient decay of an analytic periodic function

↑ **Parent:** [Fourier coefficient](#fourier-coefficient)

If a periodic function extends analytically and remains bounded in a nonzero complex strip around the real axis, contour shifting gives constants $C,c>0$ such that

$$
|\widehat f_n|\leq Ce^{-c|n|}.
$$

This exponential decay underlies spectral convergence of Fourier approximation and periodic trapezoidal quadrature.

### Termwise differentiation of a Fourier series

↑ **Parent:** [Fourier coefficient](#fourier-coefficient)

When regularity and convergence justify termwise differentiation, the derivative of a Fourier mode multiplies its coefficient by its frequency. For period $L$,

$$
\widehat{f'}_n=\frac{2\pi in}{L}\widehat f_n.
$$

## Fourier cosine series

↑ **Parent:** [Fourier series](fourier-series.md)

A Fourier cosine series has the form

$$
\frac{a_0}{2}+\sum_{n=1}^{\infty}a_n\cos(nx).
$$

It represents the [even function](calculus.md#even-function) obtained by reflecting its data across the origin.

### Half-range Fourier cosine series

↑ **Parent:** [Fourier cosine series](#fourier-cosine-series)

For a function prescribed on $0<x<L$, its half-range [Fourier cosine series](#fourier-cosine-series) is the [Fourier series](fourier-series.md) of the even extension, made $2L$-periodic. Its coefficients are $a_n=(2/L)\int_0^L f(x)\cos(n\pi x/L)\,dx$, including $n=0$. At a jump the usual piecewise-smooth convergence theorem gives the average of the two one-sided limits of the periodic extension.

## Fourier series of x cubed minus pi squared x

↑ **Parent:** [Fourier series](fourier-series.md)

On $(-\pi,\pi)$,

$$
x^3-\pi^2x
=12\sum_{n=1}^{\infty}\frac{(-1)^n}{n^3}\sin(nx).
$$

Parseval's identity and direct integration of the square give

$$
\sum_{n=1}^{\infty}\frac1{n^6}=\frac{\pi^6}{945}.
$$

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (156)

- [Absolute Fourier convergence from a square-integrable derivative](#absolute-fourier-convergence-from-a-square-integrable-derivative)
- [Bandwidth limitation in fixed-power filament optimization](mathematical-biology.md#bandwidth-limitation-in-fixed-power-filament-optimization)
- [Biharmonic equation](calculus.md#biharmonic-equation)
- [Characters of a real torus](fourier-analysis.md#characters-of-a-real-torus)
- [Complex Fourier series](#complex-fourier-series)
- [Cotangent Fourier expansion](geometry-and-topology.md#cotangent-fourier-expansion)
- [Cross-spectrum of two stationary time series](time-series.md#cross-spectrum-of-two-stationary-time-series)
- [Dirichlet-Jordan convergence theorem](#dirichlet-jordan-convergence-theorem)
- [Dirichlet test](real-analysis.md#dirichlet-test)
- [Du Bois-Reymond theorem](#du-bois-reymond-theorem)
- [Fay solution](partial-differential-equation.md#fay-solution)
- [Flat torus](second-fundamental-form.md#flat-torus)
- [Fourier-cutoff oscillator functional determinant](quantum-field-theory.md#fourier-cutoff-oscillator-functional-determinant)
- [Fourier–Galerkin method](numerical-analysis.md#fourier-galerkin-method)
- [Fourier harmonic](#fourier-harmonic)
- [Fourier series of a noninteger-frequency sine](#fourier-series-of-a-noninteger-frequency-sine)
- [Fourier series of a periodically extended quadratic arch](#fourier-series-of-a-periodically-extended-quadratic-arch)
- [Fourier sine basis](#fourier-sine-basis)
- [Fourth-order edges of the second Mathieu instability tongue](differential-equation.md#fourth-order-edges-of-the-second-mathieu-instability-tongue)
- [Half-range Fourier cosine series](#half-range-fourier-cosine-series)
- [Harmonic analysis](analysis.md#harmonic-analysis)
- [Harmonic balance](differential-equation.md#harmonic-balance)
- [Harmonic matching across a circle with a derivative jump](partial-differential-equation.md#harmonic-matching-across-a-circle-with-a-derivative-jump)
- [Hecke prime-power recurrence from q-shift operators](modular-function.md#hecke-prime-power-recurrence-from-q-shift-operators)
- [Impulsively struck fixed-end string](wave-equation.md#impulsively-struck-fixed-end-string)
- [Integer-current representation of the Villain model](statistical-physics.md#integer-current-representation-of-the-villain-model)
- [Kahane-Katznelson divergence theorem](#kahane-katznelson-divergence-theorem)
- [Kaluza-Klein charge quantization](physics.md#kaluza-klein-charge-quantization)
- [Kaluza-Klein tower](physics.md#kaluza-klein-tower)
- [Linear N-term approximation](hilbert-space.md#linear-n-term-approximation)
- [Low-pass filter of a multiresolution analysis](fourier-analysis.md#low-pass-filter-of-a-multiresolution-analysis)
- [Mathieu characteristic value](differential-equation.md#mathieu-characteristic-value)
- [Maxwell reduction on a circle](physics.md#maxwell-reduction-on-a-circle)
- [MRA projection Fourier identity](fourier-analysis.md#mra-projection-fourier-identity)
- [Orthogonality of complex exponentials](fourier-analysis.md#orthogonality-of-complex-exponentials)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#16e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#2h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3.md#12h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3.md#2g/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-55.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-75.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-6.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-50.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-50.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-58.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2.md#6b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-18.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-59.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-61.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1.md#14e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1.md#15g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4.md#15f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-54.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-55.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-6.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-67.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#30a/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#30a/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-18.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-19.md#6/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-28.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-54.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-7.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-82.md#4/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-2.md#5d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-29.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4.md#16a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4.md#5a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3.md#29c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2.md#5b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#19f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-58.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#25i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#30e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-12.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-20.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#6/b/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-8.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-8.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-8.md#1/vii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2.md#5d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2.md#5d/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2.md#5d/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-25.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-7.md#2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-14.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-80.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-80.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-9.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2.md#15c/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#14a/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#5a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-117.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2.md#5b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-336.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-2.md#16a/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#39c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#39c/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-307.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-338.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3.md#5a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-333.md#3/vii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#41c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-333.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-334.md#2/a/ii/solution)
- [Periodic convolution operator](fourier-analysis.md#periodic-convolution-operator)
- [Periodic triangular bump](#periodic-triangular-bump)
- [Periodization of a Schwartz function](fourier-analysis.md#periodization-of-a-schwartz-function)
- [Periodization of an integrable function](fourier-analysis.md#periodization-of-an-integrable-function)
- [Pointwise convergence of a piecewise smooth Fourier series](#pointwise-convergence-of-a-piecewise-smooth-fourier-series)
- [Product-to-sum formula](geometry-and-topology.md#product-to-sum-formula)
- [Rankin–Selberg integral for holomorphic cusp forms](modular-function.md#rankin-selberg-integral-for-holomorphic-cusp-forms)
- [Sinusoidal Cole-Hopf solution for negative-flux Burgers flow](partial-differential-equation.md#sinusoidal-cole-hopf-solution-for-negative-flux-burgers-flow)
- [Spectral accuracy](numerical-analysis.md#spectral-accuracy)
- [Spectral geometry](riemannian-geometry.md#spectral-geometry)
- [Spectrum of a flat torus](second-fundamental-form.md#spectrum-of-a-flat-torus)
- [Square wave](#square-wave)
- [Triangular weights count genuine four-term progressions](additive-combinatorics.md#triangular-weights-count-genuine-four-term-progressions)
- [Trigonometric integral](calculus.md#trigonometric-integral)
- [Uniform Poisson summability of continuous circle functions](partial-differential-equation.md#uniform-poisson-summability-of-continuous-circle-functions)
- [Wiener algebra](#wiener-algebra)
