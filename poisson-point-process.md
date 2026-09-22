# Poisson point process

↑ **Parent:** [Probability theory](probability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_point_process)

A Poisson point process has independent counts on disjoint sets and Poisson count in each set with mean given by its intensity measure.

**Table of contents**

- [Poisson line process](#poisson-line-process)
  - [Intersection point process of a Poisson line process](#intersection-point-process-of-a-poisson-line-process)
    - [Strict disk-void bound for a Poisson line process](#strict-disk-void-bound-for-a-poisson-line-process)
- [Poisson factorial moment measure](#poisson-factorial-moment-measure)
- [Poisson mapping theorem](#poisson-mapping-theorem)
  - [Poisson polar projections share their total count](#poisson-polar-projections-share-their-total-count)
- [Symmetric inverse-power Poisson field on a line](#symmetric-inverse-power-poisson-field-on-a-line)
- [Poisson germ-grain model](#poisson-germ-grain-model)
  - [Void probability for growing Poisson rain patches](#void-probability-for-growing-poisson-rain-patches)
- [Poisson random measure](#poisson-random-measure)
  - [Mecke formula for a Poisson random measure](#mecke-formula-for-a-poisson-random-measure)
  - [Existence of a Poisson random measure on a standard Borel space](#existence-of-a-poisson-random-measure-on-a-standard-borel-space)
  - [L2 construction of compensated Poisson integrals](#l2-construction-of-compensated-poisson-integrals)
  - [Laplace functional of a Poisson random measure](#laplace-functional-of-a-poisson-random-measure)
    - [Count-weighted Laplace functional of a Poisson random measure](#count-weighted-laplace-functional-of-a-poisson-random-measure)
      - [Small-ball conditioning for a Poisson random measure](#small-ball-conditioning-for-a-poisson-random-measure)
  - [Exponential void probabilities characterize a Poisson random measure](#exponential-void-probabilities-characterize-a-poisson-random-measure)
  - [Inverse-power sum over Poisson arrivals](#inverse-power-sum-over-poisson-arrivals)
  - [Poisson stochastic integral with finite intensity](#poisson-stochastic-integral-with-finite-intensity)
- [Superposition theorem for Poisson point processes](#superposition-theorem-for-poisson-point-processes)
- [Campbell's theorem](#campbell-s-theorem)
  - [Campbell first-moment formula](#campbell-first-moment-formula)
- [Non-homogeneous Poisson point process](#non-homogeneous-poisson-point-process)
  - [Power-law boundary accumulation of a Poisson point process](#power-law-boundary-accumulation-of-a-poisson-point-process)
  - [Two-sided order statistics of a boundary-singular Poisson process](#two-sided-order-statistics-of-a-boundary-singular-poisson-process)
  - [Intensity function of a point process](#intensity-function-of-a-point-process)
- [Mapping theorem (point process)](#mapping-theorem-point-process)
  - [Radial volume transform of a homogeneous Poisson point process](#radial-volume-transform-of-a-homogeneous-poisson-point-process)
    - [Kth-nearest-neighbour distance in a homogeneous Poisson point process](#kth-nearest-neighbour-distance-in-a-homogeneous-poisson-point-process)
- [Independent marking theorem for Poisson point processes](#independent-marking-theorem-for-poisson-point-processes)
  - [Moments of a marked Poisson integral](#moments-of-a-marked-poisson-integral)
- [Poisson thinning theorem](#poisson-thinning-theorem)
  - [Joint red and green Poisson count formula](#joint-red-and-green-poisson-count-formula)

## Poisson line process

↑ **Parent:** [Poisson point process](poisson-point-process.md)

Identify an unoriented line not through the origin by $L(p,\theta)=\{z:z\cdot(\cos\theta,\sin\theta)=p\}$, with $p>0$. A [Poisson point process](poisson-point-process.md) on this parameter space is a random collection of lines. The [measure](measure.md) $c\,dp\,d\theta$ is invariant under rotations and translations; signed coordinates $t\in\mathbb R$, $0\leq\theta<\pi$ give the same [measure](measure.md) $c\,dt\,d\theta$. The number of lines meeting a disk of radius $r$ is [Poisson](discrete-probability-distribution.md#poisson-distribution) with [mean](expected-value.md) $2\pi cr$.

### Intersection point process of a Poisson line process

↑ **Parent:** [Poisson line process](#poisson-line-process)

For an isotropic [Poisson line process](#poisson-line-process) of intensity $c\,dp\,d\theta$, its pair intersections form a locally finite [point process](probability-theory.md#point-process). Coincident intersections and parallel pairs have [probability](probability-theory.md#probability) zero. Its [intensity measure](probability-theory.md#intensity-measure-of-a-point-process) is $\pi c^2$ times area. Indeed the [Poisson factorial moment measure](#poisson-factorial-moment-measure) and the [change of variables](multivariable-calculus.md#change-of-variables-formula) from signed distances to intersection location give

$$
\mathbb E\#(\Phi\cap A)=\frac{c^2|A|}{2}\int_0^\pi\int_0^\pi|\sin(\theta-\phi)|\,d\theta\,d\phi=\pi c^2|A|.
$$

The factor $1/2$ counts unordered line pairs. Shared lines create dependence between intersections; this process is not a [Poisson point process](poisson-point-process.md).

#### Strict disk-void bound for a Poisson line process

↑ **Parent:** [Intersection point process of a Poisson line process](#intersection-point-process-of-a-poisson-line-process)

For $c,r>0$, an intersection inside a disk requires at least two lines to meet that disk. The latter count is [Poisson](discrete-probability-distribution.md#poisson-distribution) with [mean](expected-value.md) $2\pi cr$, giving the non-strict bound first. It is strict because two lines with nearby normal angles but separated perpendicular distances can both hit the disk while intersecting outside. Choose two positive-measure parameter boxes forcing this configuration; the event of exactly one line in each box and no other disk-hitting line has positive [probability](probability-theory.md#probability). This also yields a void [probability](probability-theory.md#probability) too large to equal that of a [Poisson point process](poisson-point-process.md) with the intersection process's [intensity measure](probability-theory.md#intensity-measure-of-a-point-process).

## Poisson factorial moment measure

↑ **Parent:** [Poisson point process](poisson-point-process.md)

For a [Poisson point process](poisson-point-process.md) with [intensity measure](probability-theory.md#intensity-measure-of-a-point-process) $\mu$, ordered tuples of distinct atoms have factorial moment [measure](measure.md) $\mu^{\otimes k}$. Thus for any nonnegative [measurable](measure-theory.md#measurability) function $g$,

$$
\mathbb E\sum_{z_1,\ldots,z_k\text{ distinct}}g(z_1,\ldots,z_k)=\int g\,d\mu^{\otimes k}.
$$

For $k=2$, separating diagonal terms from distinct pairs gives the second moment of a [Poisson](discrete-probability-distribution.md#poisson-distribution) sum. Dividing by two instead counts unordered pairs, which is essential for geometric intersection intensities.

## Poisson mapping theorem

↑ **Parent:** [Poisson point process](poisson-point-process.md)

For a [measurable](measure-theory.md#measurability) map $f$ and a [Poisson random measure](#poisson-random-measure) of intensity $\nu$, image counts in disjoint sets equal original counts in their disjoint preimages. They are therefore [independent](random-variable.md#independent-random-variables) Poisson variables with the pushforward intensity. The result is a [Poisson random measure](#poisson-random-measure) even if images collide; diffuse pushforward intensity gives a simple point process.

### Poisson polar projections share their total count

↑ **Parent:** [Poisson mapping theorem](#poisson-mapping-theorem)

For unit volume intensity in the unit ball of $\mathbb R^d$, polar coordinates give intensity $r^{d-1}dr\,\sigma(d\omega)$. The separate radius and direction images are Poisson processes, but each counts the same random total number of original points. Their count [covariance](variance.md#covariance) is the displayed intensity of the intersection of their two preimages. Conditional on the total count, radii and directions are [independent](random-variable.md#independent-random-variables) samples, which does not imply unconditional [independence](random-variable.md#independent-random-variables) of the two point processes.

## Symmetric inverse-power Poisson field on a line

↑ **Parent:** [Poisson point process](poisson-point-process.md)

Place equal masses at points of a homogeneous [Poisson point process](poisson-point-process.md) of intensity $\rho$ on the line, and truncate their signed inverse-power forces symmetrically at radius $R$. For force $m\operatorname{sign}(x)/|x|^p$, with $\alpha=1/p\in(0,2)$, the characteristic exponent tends to $-2\rho\int_0^\infty(1-\cos(mt/x^p))\,dx$. The [cosine integral for a symmetric stable exponent](probability-distribution.md#cosine-integral-for-a-symmetric-stable-exponent) evaluates it as displayed. Thus the weak limit is a [symmetric stable distribution](probability-distribution.md#symmetric-stable-distribution). Symmetric truncation is important when the far-field force series is not absolutely summable.

## Poisson germ-grain model

↑ **Parent:** [Poisson point process](poisson-point-process.md)

A [Poisson germ-grain model](#poisson-germ-grain-model) assigns a measurable region to each point of a [Poisson point process](poisson-point-process.md) and takes the union of those regions. A location remains uncovered exactly when no Poisson point has a region containing it, so its coverage [probability](probability-theory.md#probability) is determined by the intensity of the corresponding set of germs and marks.

### Void probability for growing Poisson rain patches

↑ **Parent:** [Poisson germ-grain model](#poisson-germ-grain-model)

For drops with intensity $\lambda(x,t,v)$, impact time $t$ and nonnegative [volume](geometry-and-topology.md#volume) $v$, let their radius at time $\tau$ be $r(\tau-t,v)$. The dry [probability](probability-theory.md#probability) at $\xi$ is

$$
\exp\left[-\int_{t\le\tau}\int_{v\ge0}\int_{|x-\xi|\le r(\tau-t,v)}\lambda(x,t,v)\,dx\,dv\,dt\right].
$$

The exponent is the intensity of drops whose patch covers the point by that time. An infinite exponent means zero dry [probability](probability-theory.md#probability). No spatial-homogeneity assumption is needed.

## Poisson random measure

↑ **Parent:** [Poisson point process](poisson-point-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_random_measure)

A Poisson random measure $N$ with intensity measure $\mu$ assigns independent Poisson random variables to disjoint measurable sets, with $N(A)$ having mean $\mu(A)$. Its compensated version is $\widetilde N=N-\mu$ on sets of finite intensity.

### Mecke formula for a Poisson random measure

↑ **Parent:** [Poisson random measure](#poisson-random-measure)

For nonnegative [measurable](measure-theory.md#measurability) $H$ and a [Poisson random measure](#poisson-random-measure) of sigma-finite intensity $\rho$, removing the selected point from a sum leaves an [independent](random-variable.md#independent-random-variables) copy of the original process under the integral. For finite intensity, condition on the Poisson count, represent the points as [independent](random-variable.md#independent-random-variables) samples from normalized $\rho$, and shift the count index using $n/n!=1/(n-1)!$. For sigma-finite intensity, first select points in a finite-intensity set, condition on the [independent](random-variable.md#independent-random-variables) outside process and then exhaust the space. Repetition gives the corresponding formula for ordered distinct tuples of points.

### Existence of a Poisson random measure on a standard Borel space

↑ **Parent:** [Poisson random measure](#poisson-random-measure)

A [sigma-finite measure](measure.md#sigma-finite-measure) on a [standard Borel space](measure-theory.md#standard-borel-space) is the [intensity measure of a point process](probability-theory.md#intensity-measure-of-a-point-process) with Poisson counts. Partition the space into sets of finite intensity, draw an independent Poisson count on each piece, and conditional on that count draw independent points from its normalized intensity measure. The sum of their [Dirac measures](measure.md#dirac-measure) is the required [Poisson random measure](#poisson-random-measure). Non-atomic intensity gives simplicity; local finiteness of the intensity gives local finiteness of the point configuration.

### L2 construction of compensated Poisson integrals

↑ **Parent:** [Poisson random measure](#poisson-random-measure)

For deterministic square-integrable $f$ and a [Poisson random measure](#poisson-random-measure) of intensity $\nu$, first define the integral for simple functions on disjoint finite-intensity sets. [Independence](random-variable.md#independent-random-variables) and the equality of [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) mean and [variance](variance.md) prove the displayed [isometry](riemannian-geometry.md#isometry). Completion defines the integral for all $f\in L^2(\nu)$, even when $\int|f|d\nu=\infty$. A small-jump compensated [martingale](martingale.md) is thereby defined through [convergence in Lp](convergence-of-random-variables.md#convergence-in-lp), not by subtracting two divergent ordinary integrals.

### Laplace functional of a Poisson random measure

↑ **Parent:** [Poisson random measure](#poisson-random-measure)

For nonnegative measurable $f$, independent Poisson counts first prove this formula for simple functions on disjoint measurable sets. Monotone approximation gives the general formula, allowing infinite integrals with $e^{-\infty}=0$. Conversely, the formula evaluated at $f=\sum_ju_j\mathbf1_{A_j}$ for disjoint finite-intensity sets gives the joint Laplace transform of independent Poisson counts, so characterizes the law of a [Poisson random measure](#poisson-random-measure).

#### Count-weighted Laplace functional of a Poisson random measure

↑ **Parent:** [Laplace functional of a Poisson random measure](#laplace-functional-of-a-poisson-random-measure)

Let $M$ be a [Poisson random measure](#poisson-random-measure) of intensity $\mu$, let $\mu(A)<\infty$, and let $f\geq0$ be [measurable](measure-theory.md#measurability). Apply the [Laplace functional of a Poisson random measure](#laplace-functional-of-a-poisson-random-measure) to $f+t\mathbf1_A$ and differentiate from the right at $t=0$. On the random side, differentiation is dominated by the [integrable random variable](expected-value.md#integrable-random-variable) $M(A)$; on the intensity side, by $\mathbf1_A$. This proves the displayed identity when $\int(1-e^{-f})d\mu$ is finite. When this integral is infinite, $e^{-M(f)}=0$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence), and the same identity holds with both sides zero.

##### Small-ball conditioning for a Poisson random measure

↑ **Parent:** [Count-weighted Laplace functional of a Poisson random measure](#count-weighted-laplace-functional-of-a-poisson-random-measure)

For a [Poisson random measure](#poisson-random-measure) on $\mathbb R^d$ with [Lebesgue measure](measure-theory.md#lebesgue-measure) intensity and a nonnegative compactly supported [continuous function](calculus.md#continuous-function) $f$, put $m_r=\mu(B(0,r))$ and $a_r=\int_{B(0,r)}e^{-f}d\mu$. Continuity gives $a_r/m_r\to e^{-f(0)}$. With $L=\mathbb E e^{-M(f)}$, the [count-weighted Laplace functional of a Poisson random measure](#count-weighted-laplace-functional-of-a-poisson-random-measure) and independent inside/outside counts give respectively

$$
\frac{\mathbb E[M(B(0,r))e^{-M(f)}]}{\mathbb P(M(B(0,r))\geq1)}=L\frac{a_r}{1-e^{-m_r}},\qquad
\mathbb E[e^{-M(f)}\mid M(B(0,r))\geq1]=L\frac{1-e^{-a_r}}{1-e^{-m_r}}.
$$

Both converge to the displayed value. The conditioning is meaningful for every $r>0$; it is not conditioning on a positive-probability point at the origin.

### Exponential void probabilities characterize a Poisson random measure

↑ **Parent:** [Poisson random measure](#poisson-random-measure)

A [simple locally finite point measure](probability-theory.md#simple-locally-finite-point-measure) on $[0,\infty)$ with void [probability](probability-theory.md#probability) $e^{-\lambda(A)}$ on finite unions of bounded intervals is a [Poisson random measure](#poisson-random-measure) with [Lebesgue measure](measure-theory.md#lebesgue-measure) intensity. Void-event intersections factor, hence the occupation indicators on disjoint cells are independent. The [dyadic occupancy approximation of a simple point measure](probability-theory.md#dyadic-occupancy-approximation-of-a-simple-point-measure) is binomial with rare-event [probability](probability-theory.md#probability) $1-e^{-2^{-n}}$ and converges to a Poisson count of mean the interval length. [Independence](random-variable.md#independent-random-variables) survives joint convergence for disjoint intervals. Extension of the mean [measure](measure.md) and the [Laplace functional of a Poisson random measure](#laplace-functional-of-a-poisson-random-measure) to Borel functions identifies all Borel counts, not just intervals.

### Inverse-power sum over Poisson arrivals

↑ **Parent:** [Poisson random measure](#poisson-random-measure)

For unit-rate [Poisson process](poisson-process.md) arrivals $Z_i$, $X_p$ is finite almost surely when $p>1$. There are finitely many positive arrivals before time one; the expected contribution afterwards is $\int_1^\infty z^{-p}\,dz<\infty$, by the Poisson [expectation](expected-value.md) identity proved on simple functions and extended by [monotone convergence](measure-theory.md#monotone-convergence-theorem). Merging [independent](random-variable.md#independent-random-variables) processes of rates $1$ and $\rho$ produces rate $1+\rho$; rescaling their arrivals by $1+\rho$ restores unit rate. Hence the sum of their inverse-power contributions has law $(1+\rho)^pX_p$. In particular two [independent](random-variable.md#independent-random-variables) unit-rate inverse-square sums add to a variable with law $4X_2$.

### Poisson stochastic integral with finite intensity

↑ **Parent:** [Poisson random measure](#poisson-random-measure)

For a [Poisson random measure](#poisson-random-measure) on $E$ with finite intensity $\nu(E)$, its integral of a finite-valued measurable mark function is the finite sum of the marks at its random atoms. Its [characteristic function](characteristic-function.md) is $\mathbb E\exp(iu\int f\,dN)=\exp(\int(e^{iuf}-1)\,d\nu)$. On a time-mark space with intensity $ds\,\nu(dz)$ and finite mark intensity, restriction to each bounded time interval has finite intensity and defines a [Compound Poisson process](stochastic-process.md#compound-poisson-process). Zero-valued marks do not affect the integral and need not appear in its [Lévy measure](stochastic-process.md#levy-measure).

## Superposition theorem for Poisson point processes

↑ **Parent:** [Poisson point process](poisson-point-process.md)

The union of independent Poisson point processes with diffuse intensity measures $\mu_1,\ldots,\mu_m$ is a Poisson point process with intensity measure

$$
\mu_1+\cdots+\mu_m.
$$

On every finite collection of disjoint measurable sets, this follows by adding independent [Poisson counts](discrete-probability-distribution.md#poisson-distribution) and checking that the resulting counts remain independent.

<h2 id="campbell-s-theorem">Campbell's theorem</h2>

↑ **Parent:** [Poisson point process](poisson-point-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Campbell's_theorem_(probability))

For a Poisson point process $\Pi$ with intensity measure $\mu$ and a square-integrable measurable function $g$,

$$
\mathbb E\sum_{x\in\Pi}g(x)=\int g\,d\mu,
\qquad
\operatorname{Var}\left(\sum_{x\in\Pi}g(x)\right)=\int g^2\,d\mu.
$$

The second identity follows because distinct points contribute the square of the mean, while the diagonal contribution is $\int g^2\,d\mu$.

The expectation identity holds for a general [point process](probability-theory.md#point-process) with intensity measure $\mu$ whenever the sum is integrable. The stated variance identity uses the additional [Poisson point process](poisson-point-process.md) assumption.

### Campbell first-moment formula

↑ **Parent:** [Campbell's theorem](#campbell-s-theorem)

For a [Poisson random measure](#poisson-random-measure) $\Pi$ with intensity $\mu$ and measurable nonnegative $h$, $\mathbb E\int h\,d\Pi=\int h\,d\mu$, allowing both sides to be infinite. For signed $h$, the same identity holds if $\int|h|d\mu<\infty$. This first-moment statement does not require square integrability. Applying it to a nonnegative [volume](geometry-and-topology.md#volume) mark gives the expected total [volume](geometry-and-topology.md#volume) in a marked Poisson model.

## Non-homogeneous Poisson point process

↑ **Parent:** [Poisson point process](poisson-point-process.md)

Let $\lambda$ be a nonnegative measurable intensity function on a space with reference measure $dx$. A Non-homogeneous Poisson point process has independent counts on disjoint measurable sets and

$$
N(A)\sim\operatorname{Poisson}\left(\int_A\lambda(x)\,dx\right)
$$

whenever the integral is finite.

### Power-law boundary accumulation of a Poisson point process

↑ **Parent:** [Non-homogeneous Poisson point process](#non-homogeneous-poisson-point-process)

If an [intensity function of a point process](#intensity-function-of-a-point-process) has $\lambda(x)\sim c(b-x)^{-\alpha}$ at a finite endpoint, with $c>0$ and $\alpha>1$, the cumulative intensity satisfies $F(x)\sim c(b-x)^{1-\alpha}/(\alpha-1)$. The [Poisson mapping theorem](#poisson-mapping-theorem) turns $F(X_n)$ into unit-rate arrivals. The [strong law for Poisson arrival times](poisson-process.md#strong-law-for-poisson-arrival-times) gives $F(X_n)/n\to1$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence), hence the displayed accumulation rate. Reversing the coordinate gives the same argument at a left endpoint. Different singularity exponents produce different powers of the index.

### Two-sided order statistics of a boundary-singular Poisson process

↑ **Parent:** [Non-homogeneous Poisson point process](#non-homogeneous-poisson-point-process)

For intensity $x^{-2}(1-x)^{-1}$ on $(0,1)$, the cumulative-intensity maps based at $1/2$ are

$$
L(x)=x^{-1}-2-\log\frac{x}{1-x},\qquad F(x)=2-x^{-1}+\log\frac{x}{1-x}.
$$

The left and right images are independent unit-rate [Poisson processes](poisson-process.md). Labeling the original points by $X_{-k}<1/2<X_n$, with $k\ge1,n\ge0$, gives $L(X_{-k})/k\to1$ and $F(X_n)/n\to1$. Since $xL(x)\to1$ at zero and $F(x)=1-\log(1-x)+o(1)$ at one, $kX_{-k}\to1$ and $\log(1-X_n)/n\to-1$.

### Intensity function of a point process

↑ **Parent:** [Non-homogeneous Poisson point process](#non-homogeneous-poisson-point-process)

The intensity function $\lambda$ is the density of the expected counting measure: $\mathbb E[N(A)]=\int_A\lambda(x)\,dx$.

## Mapping theorem (point process)

↑ **Parent:** [Poisson point process](poisson-point-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mapping_theorem_(point_process))

Let $\Pi$ be a Poisson point process with intensity measure $\mu$ and let $f$ be measurable. If the pushforward

$$
f_*\mu(B)=\mu(f^{-1}(B))
$$

is locally finite, then the image counting measure is Poisson with intensity $f_*\mu$. If one requires a simple point process, the pushforward must also be diffuse, so distinct source points do not produce coincident image points with positive probability.

### Radial volume transform of a homogeneous Poisson point process

↑ **Parent:** [Mapping theorem (point process)](#mapping-theorem-point-process)

For a homogeneous Poisson point process of intensity $\lambda$ in $\mathbb R^d$, mapping $x$ to $v_d|x|^d$, where $v_d$ is the unit-ball volume, gives a rate-$\lambda$ Poisson process on $[0,\infty)$. Mapping to $|x|^d$ instead gives rate $\lambda v_d$.

#### Kth-nearest-neighbour distance in a homogeneous Poisson point process

↑ **Parent:** [Radial volume transform of a homogeneous Poisson point process](#radial-volume-transform-of-a-homogeneous-poisson-point-process)

For intensity $\lambda$ in $\mathbb R^d$, let $R_k$ be the distance to the $k$th closest point and put $\rho=\lambda v_d$. Then $R_k^d$ is the $k$th arrival time of a rate-$\rho$ Poisson process, so

$$
f_{R_k}(r)=\frac{d\rho^k}{(k-1)!}\,
r^{dk-1}e^{-\rho r^d},
\qquad r>0.
$$

## Independent marking theorem for Poisson point processes

↑ **Parent:** [Poisson point process](poisson-point-process.md)

Independently assigning a mark to each point of a [Poisson point process](poisson-point-process.md), with mark probabilities allowed to depend measurably on the point, produces independent Poisson point processes for the different marks. If the original intensity is $\lambda(x)\,dx$ and mark $j$ has probability $p_j(x)$, its intensity is $\lambda(x)p_j(x)\,dx$.

### Moments of a marked Poisson integral

↑ **Parent:** [Independent marking theorem for Poisson point processes](#independent-marking-theorem-for-poisson-point-processes)

Attach conditionally [independent](random-variable.md#independent-random-variables) nonnegative marks to a [Poisson point process](poisson-point-process.md), with a [measurable](measure-theory.md#measurability) mark law depending only on location. If a mark at $z$ has [mean](expected-value.md) $m(z)$ and [variance](variance.md) $v(z)$, and the displayed [integrals](integral.md) are finite, their total $W$ is finite [almost surely](convergence-of-random-variables.md#almost-sure-convergence) and has the displayed moments. The [Campbell first-moment formula](#campbell-first-moment-formula) gives the first moment and finiteness. The [Poisson factorial moment measure](#poisson-factorial-moment-measure) formula gives the square of that first moment for distinct pairs; the diagonal contributes $\int(v+m^2)\,d\mu$. Their difference is the [variance](variance.md). Signed marks require absolute first-moment integrability.

## Poisson thinning theorem

↑ **Parent:** [Poisson point process](poisson-point-process.md)

Independently retaining a point at $x$ with probability $p(x)$ thins a Poisson point process of intensity $\lambda(x)$ to one of intensity $p(x)\lambda(x)$; retained and rejected processes are independent.

### Joint red and green Poisson count formula

↑ **Parent:** [Poisson thinning theorem](#poisson-thinning-theorem)

For a finite-intensity set of mean $m$, independent red marking with [probability](probability-theory.md#probability) $r$ gives counts $R,G$ with

$$
\mathbb P(R=a,G=b)=e^{-m}\frac{m^{a+b}}{(a+b)!}\binom{a+b}{a}r^a(1-r)^b=\left[e^{-rm}\frac{(rm)^a}{a!}\right]\left[e^{-(1-r)m}\frac{((1-r)m)^b}{b!}\right].
$$

Disjoint source sets give independent pairs of these counts. Refining overlapping test sets into disjoint cells then proves independence of the two whole [Poisson point processes](poisson-point-process.md), not only their counts on one set.

## ↑ Ancestors (5)

1. [Probability theory](probability-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (27)

- [Campbell's theorem](#campbell-s-theorem)
- [Constant intensity does not imply independence](probability-theory.md#constant-intensity-does-not-imply-independence)
- [Galaxy power spectrum shot noise](large-scale-structure-of-the-universe.md#galaxy-power-spectrum-shot-noise)
- [Independent marking theorem for Poisson point processes](#independent-marking-theorem-for-poisson-point-processes)
- [Intersection point process of a Poisson line process](#intersection-point-process-of-a-poisson-line-process)
- [Joint red and green Poisson count formula](#joint-red-and-green-poisson-count-formula)
- [Moments of a marked Poisson integral](#moments-of-a-marked-poisson-integral)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-31.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-31.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-31.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-29.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-39.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#27k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#28k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-201.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#27j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4.md#27k/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4.md#27k/b/solution)
- [Poisson defect yield](electrical-circuit.md#poisson-defect-yield)
- [Poisson factorial moment measure](#poisson-factorial-moment-measure)
- [Poisson germ-grain model](#poisson-germ-grain-model)
- [Poisson line process](#poisson-line-process)
- [Randomly shifted lattice point process](probability-theory.md#randomly-shifted-lattice-point-process)
- [Shared random rate gives dependent point counts](probability-theory.md#shared-random-rate-gives-dependent-point-counts)
- [Strict disk-void bound for a Poisson line process](#strict-disk-void-bound-for-a-poisson-line-process)
- [Symmetric inverse-power Poisson field on a line](#symmetric-inverse-power-poisson-field-on-a-line)
- [Thinning of a point process](probability-theory.md#thinning-of-a-point-process)
