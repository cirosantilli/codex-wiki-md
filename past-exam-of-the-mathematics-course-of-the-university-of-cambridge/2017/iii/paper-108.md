# Paper 108

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_108.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_108.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 108](paper-108.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A continuous transformation $T$ of a compact [metric space](../../../topological-analysis.md#metric-space) $X$ is [uniquely ergodic](../../../measure-theory.md#unique-ergodicity) when there is exactly one $T$-invariant [Borel probability measure](../../../measure-theory.md#borel-probability-measure) on $X$. We use the usual compact-space convention for [unique ergodicity](../../../measure-theory.md#unique-ergodicity); the compactness and continuity hypotheses matter in the assertion about all starting points.

Let $R_\alpha(x)=x+\alpha\pmod1$ on the [circle group](../../../lie-theory.md#circle-group), with $\alpha$ irrational. Normalized [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) $m$ is invariant under this [irrational rotation of the circle](../../../measure-theory.md#irrational-rotation). If $\nu$ is any invariant [Borel probability measure](../../../measure-theory.md#borel-probability-measure), define its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) by $c_k=\int e^{2\pi ikx}\,d\nu(x)$. Invariance gives

$$
c_k=\int e^{2\pi ikR_\alpha(x)}\,d\nu(x)=e^{2\pi ik\alpha}c_k.
$$

For $k\ne0$, irrationality makes $e^{2\pi ik\alpha}\ne1$, so $c_k=0$; also $c_0=1$. These are the [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) of $m$. Hence $\nu$ and $m$ have the same integrals against every [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial). Such polynomials are uniformly dense in the continuous functions by the [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem), so the measures agree on every continuous test function and therefore agree as [Borel measures](../../../measure-theory.md#borel-measure). Thus

$$
\boxed{R_\alpha\text{ is uniquely ergodic, with invariant measure }m}.
$$

For the general [uniquely ergodic](../../../measure-theory.md#unique-ergodicity) system, fix $x\in X$ and form the [empirical measures](../../../probability-theory.md#empirical-measure)

$$
\nu_{N,x}=\frac1N\sum_{n=0}^{N-1}\delta_{T^nx}.
$$

On a compact [metric space](../../../topological-analysis.md#metric-space), the [Borel probability measures](../../../measure-theory.md#borel-probability-measure) are compact for [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures). Any subsequential limit $\nu$ is invariant: for every continuous $g$,

$$
\int(g\circ T-g)\,d\nu_{N,x}=\frac{g(T^Nx)-g(x)}N\longrightarrow0.
$$

Here $g$ is bounded and $g\circ T$ is continuous, so the identity passes to the limit. Uniqueness of the invariant [Borel probability measure](../../../measure-theory.md#borel-probability-measure) gives $\nu=\mu$. Every subsequential limit is therefore $\mu$, and compactness implies convergence of the entire sequence. Testing against $f$ proves

$$
\boxed{\lim_{N\to\infty}\frac1N\sum_{n=0}^{N-1}f(T^nx)=\int f\,d\mu\quad\text{for every }x\in X}.
$$

In fact this proves [uniform ergodic convergence for uniquely ergodic systems](../../../measure-theory.md#uniform-ergodic-convergence-for-uniquely-ergodic-systems): if convergence were not uniform in $x$, choose $N_j\to\infty$ and $x_j$ where the discrepancy stays above a fixed positive number. The same compactness and telescoping argument applied to $\nu_{N_j,x_j}$ forces a subsequence to converge to $\mu$, a contradiction. This also makes clear why an almost-everywhere [Birkhoff ergodic theorem](../../../measure-theory.md#birkhoff-ergodic-theorem) alone would not establish the requested everywhere assertion. Without the compact-space hypothesis the assertion need not hold: on the discrete space $\{p\}\sqcup\mathbb Z_{\ge0}$, set $T(p)=p$ and $T(n)=n+1$. The only invariant probability is $\delta_p$, but the continuous bounded function which is zero at $p$ and one on the integer orbit has orbit average one there.

For the decimal application put $\alpha=\log_{10}2$. This is irrational: if $\alpha=p/q$ with positive integers $p,q$, then $2^q=10^p=2^p5^p$, contradicting [unique prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic). Writing $n\alpha=m_n+t_n$ with $m_n=\lfloor n\alpha\rfloor$ and $t_n\in[0,1)$ gives $2^n=10^{m_n}10^{t_n}$. Its leading decimal digit is seven exactly when

$$
t_n\in I=[\log_{10}7,\log_{10}8).
$$

The half-open upper endpoint correctly excludes powers whose leading digit is eight, including $2^3=8$.

The indicator of $I$ is not continuous, so an extra step is needed. For any $\varepsilon>0$, choose continuous functions $a_\varepsilon,b_\varepsilon$ on the circle with $0\le a_\varepsilon\le\mathbf1_I\le b_\varepsilon\le1$ and $\int(b_\varepsilon-a_\varepsilon)\,dm<\varepsilon$, by tapering in small neighbourhoods of the two endpoints. Applying the everywhere averaging result to these functions traps the lower and upper limits of the interval frequency between their integrals. Letting $\varepsilon\downarrow0$ proves [everywhere interval frequency under an irrational rotation](../../../measure-theory.md#everywhere-interval-frequency-under-an-irrational-rotation). Consequently

$$
\boxed{\lim_{N\to\infty}\frac{|S\cap[0,N-1]|}{N}=m(I)=\log_{10}8-\log_{10}7=\frac{\log8-\log7}{\log10}}.
$$

This is the leading-seven case of [Benford frequencies for powers of an integer](../../../discrete-probability-distribution.md#benford-frequencies-for-powers-of-an-integer).

## 2

↑ **Parent:** [Paper 108](paper-108.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a probability [measure-preserving system](../../../measure-theory.md#measure-preserving-system), [strong mixing](../../../measure-theory.md#strong-mixing) means that for every pair of measurable sets $A,B$,

$$
\mu(T^{-n}A\cap B)\longrightarrow\mu(A)\mu(B).
$$

A sequence $a_n$ has [convergence in density of a sequence](../../../measure-theory.md#convergence-in-density-of-a-sequence) to $a$ when for each $\varepsilon>0$ the exceptional set $\{n:|a_n-a|\ge\varepsilon\}$ has [natural density](../../../number-theory.md#natural-density) zero. A [weakly mixing measure-preserving transformation](../../../measure-theory.md#weakly-mixing-measure-preserving-transformation) has convergence in density of $\mu(T^{-n}A\cap B)$ to $\mu(A)\mu(B)$ for every $A,B$. Equivalently, because these correlations are bounded,

$$
\frac1N\sum_{n=0}^{N-1}|\mu(T^{-n}A\cap B)-\mu(A)\mu(B)|\longrightarrow0.
$$

Indeed the mean of the absolute discrepancy is at least $\varepsilon$ times the exceptional frequency, while it is at most $\varepsilon$ plus a uniform bound times that frequency. A signed [Cesaro convergence of a sequence](../../../measure-theory.md#cesaro-convergence-of-a-sequence) without absolute values is insufficient to define weak mixing.

The standard three-cut [Chacon map](../../../measure-theory.md#chacon-transformation) is obtained by [cutting and stacking](../../../measure-theory.md#cutting-and-stacking). Start on $[0,1)$ with normalized [Lebesgue measure](../../../measure-theory.md#lebesgue-measure), an initial tower consisting of $[0,2/3)$, and a reservoir $[2/3,1)$ for spacers. At stage $j$, cut every level of the current tower into three equal subintervals, producing three subcolumns. Add one new interval of the same width above the middle subcolumn. Stack the first subcolumn at the bottom, then the middle subcolumn with its spacer, then the third at the top. Define the partial transformation by translation from each level to the next, leaving the current top unmapped. These assignments extend the earlier partial transformation. Repeat indefinitely.

If $h_j$ is the number of levels and $w_j$ their width, then

$$
\boxed{h_0=1,\quad w_0=\frac23,\quad h_{j+1}=3h_j+1,\quad w_{j+1}=\frac{w_j}{3}}.
$$

Hence $h_j=(3^{j+1}-1)/2$, $w_j=2/3^{j+1}$, and the stage-$j$ tower has measure $1-3^{-j-1}$. The spacers consume total measure $\sum_{j\ge0}w_{j+1}=1/3$, precisely the reservoir. The increasing partial maps give the [Chacon map](../../../measure-theory.md#chacon-transformation) modulo null sets. The tower tops and unused reservoir have measures tending to zero, and the construction yields an invertible [measure-preserving transformation](../../../measure-theory.md#measure-preserving-transformation). With $0$ marking an original level and $1$ a spacer, the tower words satisfy $W_0=0$ and $W_{j+1}=W_jW_j1W_j$, so the first new word is $0010$. This describes the spacer placement without needing a proof of well-definedness. The three-cut convention agrees with the classical constant spacer vector $(0,1,0)$ described in [Ryzhikov's construction](https://arxiv.org/html/1311.4524v3).

For the correlation assertion, take the [L2 inner product](../../../measure-theory.md#l2-inner-product) to be $\langle u,v\rangle=\int u\overline v\,d\mu$, linear in its first argument, and put $U=U_T$. The [Koopman operator](../../../measure-theory.md#koopman-operator) is an [isometry](../../../riemannian-geometry.md#isometry) on $L^2$, even when $T$ is not invertible. For $n\ge k$ the hint gives

$$
\langle U^nf,U^kf\rangle=\langle U^{n-k}f,f\rangle\longrightarrow|a|^2,\qquad a=\int f\,d\mu.
$$

To extend rigorously to all test functions, centre the observable: $v=f-a\mathbf1$. Invariance of the integral gives $\langle U^nv,v\rangle=\langle U^nf,f\rangle-|a|^2\to0$. Let

$$
M=\overline{\operatorname{span}}\{U^kv:k\ge0\}\subset L^2.
$$

For each fixed $k$, $\langle U^nv,U^kv\rangle\to0$ by the same [isometry](../../../riemannian-geometry.md#isometry) identity. Therefore the limit is zero for every finite [linear combination](../../../vector-space.md#linear-combination) of these orbit vectors. By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and $\|U^nv\|_2=\|v\|_2$, approximation extends this conclusion to every $g\in M$: the approximation error in the correlation is bounded by $\|v\|_2\|g-g_0\|_2$ uniformly in $n$. For $g\in M^\perp$, the correlation is identically zero because $U^nv\in M$. The [orthogonal decomposition by a closed subspace](../../../hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace) now gives the result for all $g\in L^2$. Thus

$$
\boxed{\langle U_T^nf,g\rangle\longrightarrow a\int\overline g\,d\mu=\left(\int f\,d\mu\right)\left(\int\overline g\,d\mu\right)}.
$$

This is [decay of autocorrelation implies weak convergence of an observable](../../../measure-theory.md#decay-of-autocorrelation-implies-weak-convergence-of-an-observable); no assumption that $T$ is an [ergodic transformation](../../../measure-theory.md#ergodicity), and no invertibility hypothesis was used, and $a=0$ is included.

Finally, [strong mixing](../../../measure-theory.md#strong-mixing) immediately implies the stated diagonal limit by taking $B=A$. Conversely, suppose that limit holds for every $A$. Apply the correlation result with $f=\mathbf1_A$ and $g=\mathbf1_B$. Its hypothesis is exactly $\langle U^n\mathbf1_A,\mathbf1_A\rangle\to\mu(A)^2$, and its conclusion is

$$
\boxed{\mu(T^{-n}A\cap B)\longrightarrow\mu(A)\mu(B)\quad\text{for every }A,B}.
$$

Hence [strong mixing](../../../measure-theory.md#strong-mixing) is equivalent to [diagonal set-correlation criterion for mixing](../../../measure-theory.md#diagonal-set-correlation-criterion-for-mixing). Using the orbit-span proof avoids an invalid polarization argument that would recover only the sum of the two directed cross-correlations from diagonal correlations.

## 3

↑ **Parent:** [Paper 108](paper-108.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

On a probability [measure-preserving system](../../../measure-theory.md#measure-preserving-system), for a finite [measurable partition](../../../measure-theory.md#measurable-partition) $\xi=\{A_1,\ldots,A_r\}$, the [entropy of a finite measurable partition](../../../measure-theory.md#entropy-of-a-finite-measurable-partition) is

$$
H_\mu(\xi)=-\sum_{i=1}^r\mu(A_i)\log\mu(A_i),\qquad0\log0=0.
$$

Use natural logarithms, so [information entropy](../../../information-theory.md#information-entropy) is measured in nats; another fixed logarithm base rescales all answers. The [join of measurable partitions](../../../measure-theory.md#join-of-measurable-partitions) is their common refinement, and write $\xi_a^b=\bigvee_{j=a}^bT^{-j}\xi$, with an empty join the trivial partition. The [entropy rate of a measurable partition](../../../measure-theory.md#entropy-rate-of-a-measurable-partition) and [Kolmogorov-Sinai entropy](../../../measure-theory.md#kolmogorov-sinai-entropy) are respectively

$$
\boxed{h_\mu(T,\xi)=\lim_{N\to\infty}\frac1NH_\mu(\xi_0^{N-1}),\qquad h_\mu(T)=\sup_{\xi\text{ finite}}h_\mu(T,\xi)}.
$$

The block entropies form a [subadditive sequence](../../../real-analysis.md#subadditive-sequence), so the first limit exists by the [Fekete lemma](../../../real-analysis.md#fekete-s-lemma). For finite partitions the [conditional entropy of finite measurable partitions](../../../measure-theory.md#conditional-entropy-of-finite-measurable-partitions) is $H(\eta\mid\zeta)=H(\eta\vee\zeta)-H(\zeta)$.

Put $c_0=H(\xi)$ and $c_k=H(\xi\mid\xi_1^k)$ for $k\ge1$. The [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy), applied from the last coordinate backwards, and measure preservation give

$$
H(\xi_0^{N-1})=\sum_{j=0}^{N-1}H(T^{-j}\xi\mid\xi_{j+1}^{N-1})=\sum_{k=0}^{N-1}c_k.
$$

The second equality uses invariance of the joint [partition atom](../../../measure-theory.md#partition-atom) probabilities under the common pullback $T^{-j}$; invertibility is unnecessary. Since [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy), $c_k$ decreases to a nonnegative limit $c$. The [Cesaro convergence of a sequence](../../../measure-theory.md#cesaro-convergence-of-a-sequence) of this convergent sequence has the same limit. Therefore

$$
\boxed{h_\mu(T,\xi)=\lim_{k\to\infty}H_\mu(\xi\mid\xi_1^k)}.
$$

Equivalently $h_\mu(T,\xi)=H_\mu(\xi\mid\mathcal F_1)$, where $\mathcal F_1=\sigma(\bigvee_{j\ge1}T^{-j}\xi)$. Here [conditional entropy of a countable measurable partition](../../../measure-theory.md#conditional-entropy-of-a-countable-measurable-partition) conditioned on a [sigma-algebra](../../../measure-theory.md#sigma-algebra) is computed using conditional [partition atom](../../../measure-theory.md#partition-atom) probabilities; the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) gives continuity under increasing conditioning [sigma-algebras](../../../measure-theory.md#sigma-algebra). This is the [infinite-future formula for partition entropy rate](../../../measure-theory.md#infinite-future-formula-for-partition-entropy-rate).

The [Kolmogorov-Sinai generator theorem](../../../measure-theory.md#kolmogorov-sinai-generator-theorem) states that if a finite or countable [measurable partition](../../../measure-theory.md#measurable-partition) $\eta$ has finite [entropy of a countable measurable partition](../../../measure-theory.md#entropy-of-a-countable-measurable-partition) and its iterates generate the whole completed [sigma-algebra](../../../measure-theory.md#sigma-algebra) modulo null sets, then $h_\mu(T)=h_\mu(T,\eta)$. For an invertible system, generating means $\sigma(\bigvee_{j\in\mathbb Z}T^{-j}\eta)=\mathcal B$ modulo null sets. For a noninvertible system a [one-sided generator](../../../measure-theory.md#one-sided-generator), using $j\ge0$, suffices. The two-sided and one-sided versions must not be confused.

For a [Bernoulli shift](../../../measure-theory.md#bernoulli-shift) with discrete symbol probabilities $(p_i)$, the coordinate-zero [measurable partition](../../../measure-theory.md#measurable-partition) has independent coordinate iterates. Thus

$$
H(\eta_0^{N-1})=N\left(-\sum_i p_i\log p_i\right),\qquad\boxed{h_\mu(T)=-\sum_i p_i\log p_i}.
$$

For a finite alphabet the coordinate partition is a generator of finite [entropy of a finite measurable partition](../../../measure-theory.md#entropy-of-a-finite-measurable-partition); on the two-sided sequence space use all integer coordinate iterates, and on the one-sided space use the nonnegative ones. The [Kolmogorov-Sinai generator theorem](../../../measure-theory.md#kolmogorov-sinai-generator-theorem) proves the displayed answer in both cases. The same calculation applies to countably many symbols when their [Shannon entropy](../../../information-theory.md#information-entropy) is finite, using the countable finite-entropy version of the theorem. If the [Shannon entropy](../../../information-theory.md#information-entropy) is infinite, merge all but the first $r$ symbols into one cell. These finite coordinate partitions have entropy rate $-\sum_{i\le r}p_i\log p_i-p_{>r}\log p_{>r}\to\infty$, so the system entropy is infinite. Zero-probability symbols contribute zero. In particular a fair $r$-symbol shift has entropy $\log r$.

For the final assertion, let $\mathcal F_0=\sigma(\bigvee_{j\ge0}T^{-j}\xi)$ and complete it modulo null sets. The approximation property forces $\mathcal F_0=\mathcal B$ modulo null sets. Indeed for each $A\in\mathcal B$, choose approximating sets from finite blocks with error tending to zero. Their indicators approach $\mathbf1_A$ in $L^2$, and $L^2(\mathcal F_0)$ is a closed [vector subspace](../../../vector-space.md#vector-subspace), so $A$ is $\mathcal F_0$-measurable modulo a null set.

Invertibility now gives $\mathcal F_1=T^{-1}\mathcal F_0=T^{-1}\mathcal B=\mathcal B$ modulo null sets. In particular the present partition $\xi$ is measurable with respect to its entire future, so $H(\xi\mid\mathcal F_1)=0$. The infinite-future formula gives $h_\mu(T,\xi)=0$. Since the given [one-sided generator](../../../measure-theory.md#one-sided-generator) is also a two-sided generator, the [Kolmogorov-Sinai generator theorem](../../../measure-theory.md#kolmogorov-sinai-generator-theorem) finishes the proof:

$$
\boxed{h_\mu(T)=0}.
$$

This is [finite one-sided generator of an invertible system forces zero entropy](../../../measure-theory.md#finite-one-sided-generator-of-an-invertible-system-forces-zero-entropy). Invertibility is essential: a fair binary one-sided [Bernoulli shift](../../../measure-theory.md#bernoulli-shift) has a finite [one-sided generator](../../../measure-theory.md#one-sided-generator) and [Kolmogorov-Sinai entropy](../../../measure-theory.md#kolmogorov-sinai-entropy) $\log2$.

## 4

↑ **Parent:** [Paper 108](paper-108.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a probability [measure-preserving system](../../../measure-theory.md#measure-preserving-system), the hypothesis is [completely positive entropy](../../../measure-theory.md#completely-positive-entropy): every finite [measurable partition](../../../measure-theory.md#measurable-partition) with positive static [entropy of a finite measurable partition](../../../measure-theory.md#entropy-of-a-finite-measurable-partition) has positive [entropy rate of a measurable partition](../../../measure-theory.md#entropy-rate-of-a-measurable-partition). Fix a finite partition $\xi$ and put

$$
\mathcal F_N=\sigma\left(\bigvee_{j\ge N}T^{-j}\xi\right),\qquad\mathcal T(\xi)=\bigcap_{N\ge0}\mathcal F_N.
$$

All [sigma-algebras](../../../measure-theory.md#sigma-algebra) are interpreted modulo null sets. We will prove that every finite partition $\alpha$ measurable with respect to this [tail sigma-algebra of a measurable partition](../../../measure-theory.md#tail-sigma-algebra-of-a-measurable-partition) has $h_\mu(T,\alpha)=0$. Applying this to a binary partition will force the required triviality. This proves the needed direction of the [Tail characterization of the Pinsker sigma-algebra](../../../measure-theory.md#tail-characterization-of-the-pinsker-sigma-algebra) directly, including noninvertible transformations.

Write $h=h_\mu(T,\xi)$. The infinite-future entropy formula and the backwards [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) give, for every $L\ge1$, the [block conditional entropy given the infinite future](../../../measure-theory.md#block-conditional-entropy-given-the-infinite-future) identity

$$
\boxed{H_\mu(\xi_0^{L-1}\mid\mathcal F_L)=\sum_{j=0}^{L-1}H_\mu(T^{-j}\xi\mid\mathcal F_{j+1})=Lh}.
$$

Each term equals $h$ by invariance of the joint probabilities under a common pullback and continuity of [conditional entropy](../../../information-theory.md#conditional-entropy) under increasing finite future blocks. Invertibility is not needed for this identity.

Fix $\varepsilon>0$. Since $\alpha$ is $\mathcal F_0$-measurable and finite, the [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) and continuity of finite-partition [conditional entropy](../../../information-theory.md#conditional-entropy) allow an $r\ge0$ with

$$
H_\mu(\alpha\mid\xi_0^r)<\varepsilon.
$$

To see the continuity explicitly, for each [partition atom](../../../measure-theory.md#partition-atom) $A$ of $\alpha$ the conditional probabilities $\mathbb E[\mathbf1_A\mid\sigma(\xi_0^r)]$ tend to $\mathbf1_A$ almost everywhere; apply [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) to the bounded continuous function $-t\log t$ on $[0,1]$ and sum over the finitely many [partition atoms](../../../measure-theory.md#partition-atom).

For $n\ge1$ set $\gamma=\alpha_0^{n-1}$, $L=n+r$, and $\beta=\xi_0^{L-1}$. The [conditional entropy of finite measurable partitions](../../../measure-theory.md#conditional-entropy-of-finite-measurable-partitions) satisfies

$$
H(\gamma\mid\beta)\le\sum_{j=0}^{n-1}H(T^{-j}\alpha\mid\beta)\le\sum_{j=0}^{n-1}H(T^{-j}\alpha\mid T^{-j}\xi_0^r)=nH(\alpha\mid\xi_0^r)<n\varepsilon.
$$

The second inequality uses [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy), since $\beta$ refines each block $T^{-j}\xi_0^r$; the final equality uses measure preservation.

Moreover $\gamma$ is $\mathcal F_L$-measurable. For each $j\ge0$, tail measurability gives $\alpha$ measurable with respect to $\mathcal F_L$, hence $T^{-j}\alpha$ measurable with respect to $T^{-j}\mathcal F_L=\mathcal F_{L+j}\subseteq\mathcal F_L$. Thus [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy) and the displayed block identity imply

$$
H(\beta\mid\gamma)\ge H(\beta\mid\mathcal F_L)=Lh.
$$

Use the symmetric entropy identity $H(\gamma)=H(\beta)-H(\beta\mid\gamma)+H(\gamma\mid\beta)$ to obtain

$$
0\le\frac1nH(\alpha_0^{n-1})\le\frac{H(\xi_0^{n+r-1})-(n+r)h}{n}+\varepsilon.
$$

The fraction on the right tends to zero: $r$ is fixed and $H(\xi_0^{n+r-1})/(n+r)\to h$ by the definition of [entropy rate of a measurable partition](../../../measure-theory.md#entropy-rate-of-a-measurable-partition). Taking $n\to\infty$ and then $\varepsilon\downarrow0$ gives

$$
\boxed{h_\mu(T,\alpha)=0\quad\text{for every finite }\mathcal T(\xi)\text{-measurable partition }\alpha}.
$$

Now let $A\in\mathcal T(\xi)$ and take $\alpha=\{A,X\setminus A\}$. If $0<\mu(A)<1$, its [binary entropy](../../../information-theory.md#binary-entropy) is $-\mu(A)\log\mu(A)-(1-\mu(A))\log(1-\mu(A))>0$, while its entropy rate is zero, contradicting [completely positive entropy](../../../measure-theory.md#completely-positive-entropy). Therefore

$$
\boxed{\mu(A)\in\{0,1\}\quad\text{for every }A\in\mathcal T(\xi)}.
$$

Since $\xi$ was arbitrary, every finite-partition tail is trivial. The argument needs only that $\xi$ is finite and the measure is a probability; it does not assume a finite generator, finite total system entropy, or invertibility.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
