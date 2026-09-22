# Paper 7

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper7.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper7.pdf)

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
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)

## 1

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For a nonempty [bounded set](../../../topological-analysis.md#bounded-set), let $N_\delta(E)$ be the least number of radius-$\delta$ balls covering $E$. The lower and upper [Minkowski dimensions](../../../geometry-and-topology.md#box-counting-dimension) are respectively

$$
\underline{\dim}_{\mathrm M}E=\liminf_{\delta\downarrow0}\frac{\log N_\delta(E)}{\log(1/\delta)},\qquad\overline{\dim}_{\mathrm M}E=\limsup_{\delta\downarrow0}\frac{\log N_\delta(E)}{\log(1/\delta)}.
$$

Using comparable cubes or ball diameters gives the same limits. For an unbounded set one must specify a local or bounded-piece convention; these are the usual bounded-set definitions used in the [Kakeya set](../../../combinatorics.md#kakeya-set) problem.

For the digit set, fixing the first $k$ digits gives exactly $3^k$ cylinders in intervals of length $9^{-k}$. They cover the set with at most $3^k$ balls of comparable radius. Their base-nine prefix integers are separated by at least two, so these containing intervals have gaps at least $9^{-k}$. Choosing one point in each cylinder shows that a radius-$9^{-k}$ ball meets at most a bounded number of chosen points. Hence $N_{9^{-k}}(Q)\asymp3^k$. For $9^{-(k+1)}<\delta\leq9^{-k}$, monotonicity sandwiches the [covering number](../../../topological-analysis.md#metric-covering-number) between constant multiples of $3^k$ and $3^{k+1}$. This proves the [box-counting dimension of separated digit sets](../../../geometry-and-topology.md#box-counting-dimension-of-separated-digit-sets) formula here:

$$
\boxed{\underline{\dim}_{\mathrm M}Q=\overline{\dim}_{\mathrm M}Q=\frac{\log3}{\log9}=\frac12.}
$$

A planar [Besicovitch set](../../../combinatorics.md#besicovitch-set) is a [bounded set](../../../topological-analysis.md#bounded-set) of zero [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) containing a unit line segment in every unoriented direction. The following proof in fact applies to every bounded planar [Kakeya set](../../../combinatorics.md#kakeya-set), whether its area is zero or positive.

Choose $M\asymp\delta^{-1}$ directions equally spaced in an angular interval of length, say, $\pi/2$, and one segment of the set in each direction. Let $T_j$ be its rectangle of length one and width comparable to $\delta$, lying in the $C\delta$ neighborhood $E_{C\delta}$. Put $F=\sum_j1_{T_j}$. Then $\int F\asymp M\delta\asymp1$. Two such [Kakeya tubes](../../../combinatorics.md#kakeya-tube) at angle $\alpha$ have overlap at most $C\delta^2/\alpha$, since the intersection of their supporting strips is a parallelogram of that area. The trivial bound $C\delta$ applies for nearly parallel tubes. Thus, uniformly over their translations,

$$
|T_j\cap T_k|\leq\frac{C\delta^2}{\delta+\alpha_{jk}}\lesssim\frac{\delta}{1+|j-k|}.
$$

Sum these intersections. Each row contributes at most $C\delta\log(2/\delta)$, so $\int F^2\lesssim\log(2/\delta)$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) on the union now gives the [planar Kakeya neighborhood lower bound](../../../fourier-analysis.md#planar-kakeya-neighborhood-lower-bound)

$$
|E_{C\delta}|\geq\left|\bigcup T_j\right|\geq\frac{(\int F)^2}{\int F^2}\gtrsim\frac1{\log(2/\delta)}.
$$

A cover of $E$ by $N_\delta(E)$ radius-$\delta$ balls covers $E_{C\delta}$ by their fixed-factor enlargements. Hence $N_\delta(E)\gtrsim\delta^{-2}/\log(2/\delta)$. Boundedness gives the matching upper exponent $N_\delta(E)\lesssim_E\delta^{-2}$. Taking the lower and upper limits proves

$$
\boxed{\underline{\dim}_{\mathrm M}E=\overline{\dim}_{\mathrm M}E=2.}
$$

The logarithmic neighborhood loss is compatible with zero area; it still forces full dimension.

## 2

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [finite-field Kakeya set](../../../vector-space.md#finite-field-kakeya-set), also called a finite-field Besicovitch set, is a subset containing a complete [affine line in a vector space](../../../vector-space.md#affine-line-in-a-vector-space) $a+\mathbb F_pv$ in every nonzero direction $v$, with scalar multiples counted as the same direction. The line's translate may depend on the direction.

For odd $p$, take the union of the lines $y=mx-m^2/4$, $m\in\mathbb F_p$. Completing the square gives $x^2-y=(m/2-x)^2$. Thus that union is exactly $K_0=\{(x,y):x^2-y\text{ is a square, including zero}\}$. For each fixed $x$ there are $(p+1)/2$ such $y$, so $|K_0|=p(p+1)/2$. It contains every nonvertical slope. Add the vertical line $x=0$, whose overlap with $K_0$ has $(p+1)/2$ points. The [tangent-line finite-field Kakeya construction](../../../vector-space.md#tangent-line-finite-field-kakeya-construction) consequently has

$$
\boxed{|K|=\frac{p^2+2p-1}{2}=\frac12p^2(1+o(1)).}
$$

The prime two is irrelevant to this asymptotic statement and can be handled by taking its whole plane.

For the high-dimensional lower bound, we give a direct [polynomial method in combinatorics](../../../combinatorics.md#polynomial-method-in-combinatorics) proof, which yields a stronger estimate. Suppose a finite-field Kakeya set $K\subseteq\mathbb F_p^n$ has fewer than $\binom{p+n-1}{n}$ points. That binomial coefficient is the [dimension of a bounded-total-degree polynomial space](../../../polynomial.md#dimension-of-a-bounded-total-degree-polynomial-space) of [polynomials](../../../polynomial.md) of total degree at most $p-1$. Evaluation at the points of $K$ imposes fewer linear conditions than this dimension. By the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem), there is a nonzero [polynomial](../../../polynomial.md) $P$ of total degree $d\leq p-1$ vanishing on $K$.

For every nonzero $v$ choose the line $a_v+tv\subseteq K$. The [polynomial](../../../polynomial.md) $P(a_v+tv)$ in $t$ has degree at most $d<p$ and vanishes at all $p$ field elements, so it vanishes identically. Its coefficient of $t^d$ is the leading [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) part $P_d(v)$. Thus $P_d(v)=0$ for every nonzero $v$. The case $d=0$ is already impossible for a nonzero constant vanishing on a nonempty set; for $d>0$, the absence of a constant term in this [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) also gives $P_d(0)=0$.

A [polynomial](../../../polynomial.md) of degree less than $p$ in each variable cannot vanish at every point of $\mathbb F_p^n$ unless it is zero. To see this, induct on $n$: fix the first $n-1$ variables, apply the one-variable root bound in the last variable, then apply the induction hypothesis to each resulting coefficient [polynomial](../../../polynomial.md). This forces $P_d=0$, contradicting the choice of the leading part. We have proved the [finite-field Kakeya polynomial bound](../../../vector-space.md#finite-field-kakeya-polynomial-bound)

$$
|K|\geq\binom{p+n-1}{n}\geq\frac{p^n}{n!}.
$$

At $n=15$ this implies the required bound with an explicit absolute constant:

$$
\boxed{|K|\geq\frac{p^{15}}{15!}\geq\frac{p^9}{15!},\qquad c=1/15!.}
$$

The argument is valid in every prime characteristic and does not invoke the lower bound as an unproved theorem.

## 3

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use $\widehat{f\sigma}(x)=\int_{S^1}f(\omega)e^{-2\pi ix\cdot\omega}\,d\sigma(\omega)$, with arclength measure. We first bound the transform for constant density. By rotational symmetry, $\widehat\sigma(x)=\int_0^{2\pi}e^{-2\pi ir\cos\theta}d\theta$, $r=|x|$. For $r\geq1$, remove neighborhoods of width $h=r^{-1/2}$ about the stationary points $0,\pi$. Their contribution is $O(h)$. On each remaining interval integrate by parts using the phase derivative $2\pi r\sin\theta$. The boundary terms are $O((rh)^{-1})$, and the integral of the derivative of its reciprocal is bounded by

$$
\frac Cr\int_h^{\pi-h}\frac{|\cos\theta|}{\sin^2\theta}d\theta\lesssim\frac1{rh}.
$$

Splitting at the stationary points gives the same bound on the other half of the circle. Together with the trivial estimate for bounded $r$, this proves $|\widehat\sigma(x)|\lesssim(1+|x|)^{-1/2}$.

For merely measurable $f$ there is no reason that its amplitude permits this [integration by parts](../../../calculus.md#integration-by-parts). Instead use [Gaussian positivity for even extension moments](../../../fourier-analysis.md#gaussian-positivity-for-even-extension-moments). Set

$$
I_R(f)=\int_{\mathbb R^2}|\widehat{f\sigma}(x)|^4e^{-\pi|x|^2/R^2}dx.
$$

Expand the fourth power and integrate first in $x$. The [Fourier transform of a Gaussian](../../../fourier-analysis.md#fourier-transform-of-a-gaussian) gives

$$
I_R(f)=R^2\int_{(S^1)^4} f(\omega_1)f(\omega_2)\overline{f(\omega_3)f(\omega_4)}\,e^{-\pi R^2|\omega_1+\omega_2-\omega_3-\omega_4|^2}\,d\sigma^4.
$$

All exchanges of integrals are justified by bounded amplitudes, finite surface measure and the integrable Gaussian. The kernel is nonnegative and $|f|\leq1$ almost everywhere. Taking the absolute value of the integral therefore gives $0\leq I_R(f)\leq I_R(1)$. The preceding scalar decay estimate and polar coordinates yield

$$
I_R(1)\lesssim\int_0^\infty\frac{r}{(1+r)^2}e^{-\pi r^2/R^2}dr\lesssim1+\log R\lesssim\log R\qquad(R\geq2).
$$

For the last bound split at $1$ and $R$; the tail becomes an integrable $e^{-\pi s^2}/s$ integral after $r=Rs$. Since the Gaussian is at least $e^{-\pi}$ on the radius-$R$ ball, the [local fourth-moment restriction estimate for the circle](../../../fourier-analysis.md#local-fourth-moment-restriction-estimate-for-the-circle) follows:

$$
\boxed{\|\widehat{f\sigma}\|_{L^4(B(0,R))}\leq C(\log R)^{1/4}.}
$$

Every constant here is independent of $f$ and $R$.

For the requested connection to [Besicovitch sets](../../../combinatorics.md#besicovitch-set), let $\delta$ be small and dilate the unit segments of a bounded planar Kakeya set by $\delta^{-2}$. Their $\delta$-neighborhoods become direction-separated rectangles of length $\delta^{-2}$ and width $\delta^{-1}$. A smooth circle cap of angular width $c\delta$ has a [Fourier extension operator](../../../fourier-analysis.md#fourier-extension-operator) of magnitude at least $c'\delta$ on such a rectangle: after removing the constant phase, the tangential phase variation is $O(c)$ and the normal variation is $O(c^2)$. A frequency modulation translates the rectangle to any desired location. Choose separated caps for the rectangle directions, and multiply their modulated densities by independent [Rademacher random variables](../../../probability-theory.md#rademacher-distribution). Because the caps are disjoint, the input remains bounded by one.

Apply the local fourth-moment estimate in a ball of radius $C_E\delta^{-2}$ containing the rectangles, then take expectation over the [Rademacher random variables](../../../probability-theory.md#rademacher-distribution). The fourth moment dominates the square of the sum of squared packet magnitudes, giving

$$
\delta^4\int\left(\sum_j1_{T_j}\right)^2\lesssim_E\log(1/\delta).
$$

There are $M\asymp\delta^{-1}$ rectangles, each of area $\asymp\delta^{-3}$, so the integral of their sum is $\asymp\delta^{-4}$. [Cauchy-Schwarz](../../../probability-and-statistics.md#cauchy-schwarz-inequality) forces their union area to be at least $c_E\delta^{-4}/\log(1/\delta)$. Scaling back gives $|E_{C\delta}|\gtrsim_E1/\log(1/\delta)$, the [planar Kakeya neighborhood lower bound](../../../fourier-analysis.md#planar-kakeya-neighborhood-lower-bound). The covering-number argument in Question 1 then gives both [Minkowski dimensions](../../../geometry-and-topology.md#box-counting-dimension) equal to two.

## 4

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For odd $p$, write $e_p(t)=e^{2\pi it/p}$ and use the [discrete paraboloid](../../../fourier-analysis.md#discrete-paraboloid)

$$
P=\{(u,v,u^2+v^2):u,v\in\mathbb F_p\},\qquad \sigma=p^{-2}1_P.
$$

Here surface integration means $p^{-2}\sum_P$, whereas ambient [norms](../../../functional-analysis.md#norm) below use unnormalized counting measure on $\mathbb F_p^3$. With the negative-phase transform convention,

$$
\widehat\sigma(x)=p^{-2}\sum_{u,v}e_p(-x_1u-x_2v-x_3(u^2+v^2)).
$$

When $x_3=0$, additive-[orthogonality of characters](../../../representation-theory.md#character-orthogonality) makes this one at $x=0$ and zero at all other points of that plane. When $x_3\ne0$, completing the two squares gives

$$
\widehat\sigma(x)=p^{-2}e_p\left(\frac{x_1^2+x_2^2}{4x_3}\right)G(-x_3)^2,\qquad G(t)=\sum_u e_p(tu^2).
$$

The [Quadratic Gauss sum](../../../number-theory.md#quadratic-gauss-sum) identity is $G(t)^2=\chi(-1)p$, where $\chi$ is the [Legendre symbol](../../../number-theory.md#legendre-symbol). For completeness, counting the preimages of a square gives $G(t)=\chi(t)G(1)$ for nonzero $t$. Also $|G(1)|^2=\sum_{u,v}e_p(u^2-v^2)=p$, by the invertible change $(u,v)\mapsto(u-v,u+v)$ and [orthogonality of characters](../../../representation-theory.md#character-orthogonality). Since $\overline{G(1)}=G(-1)=\chi(-1)G(1)$, the asserted square identity follows. Thus for $p\equiv3\pmod4$,

$$
\boxed{\widehat\sigma(x)=\begin{cases}1,&x=0,\\0,&x_3=0,\ x\ne0,\\-p^{-1}e_p((x_1^2+x_2^2)/(4x_3)),&x_3\ne0.\end{cases}}
$$

Using positive phase instead changes the sign inside the character, not the magnitude or any [norm](../../../functional-analysis.md#norm) estimate.

Define $Eg(x)=p^{-2}\sum_{\xi\in P}g(\xi)e_p(x\cdot\xi)$, and define $R^*(2\to q)$ as the smallest constant for

$$
\|Eg\|_{\ell^q(\mathbb F_p^3)}\leq R^*(2\to q)\left(p^{-2}\sum_{\xi\in P}|g(\xi)|^2\right)^{1/2}.
$$

The adjoint relative to these measures is $E^*h(\xi)=\sum_xh(x)e_p(-x\cdot\xi)$. Consequently $EE^*h=h*\widehat\sigma(-\cdot)$, where convolution is the unnormalized ambient sum. Put $K=\widehat\sigma(-\cdot)-1_{\{0\}}$. Its supremum is at most $p^{-1}$, so convolution by $K$ has $\ell^1\to\ell^\infty$ [norm](../../../functional-analysis.md#norm) at most $p^{-1}$.

Under the unnormalized ambient [Fourier transform on a finite group](../../../additive-combinatorics.md#fourier-transform-on-a-finite-group), the convolution multiplier of $\widehat\sigma(-\cdot)$ is $p^3\sigma=p1_P$, up to the harmless reflection convention. Thus the multiplier of $K$ is $p1_P-1$, with maximum absolute value at most $p$. The [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) gives $\ell^2\to\ell^2$ [norm](../../../functional-analysis.md#norm) at most $p$. The [Riesz-Thorin interpolation theorem](../../../continuous-dual-space.md#riesz-thorin-theorem) between these two bounds gives $\ell^{4/3}\to\ell^4$ [norm](../../../functional-analysis.md#norm) at most one for convolution by $K$. Convolution by $1_{\{0\}}$ is the identity, whose $\ell^{4/3}\to\ell^4$ [norm](../../../functional-analysis.md#norm) is at most one for counting measure. Hence $\|EE^*h\|_4\leq2\|h\|_{4/3}$.

By [Lp duality](../../../continuous-dual-space.md#lp-duality-on-an-arbitrary-measure-space) and [Hölder's inequality](../../../real-analysis.md#holder-s-inequality), $\|E^*h\|_{L^2(\sigma)}^2=\langle EE^*h,h\rangle\leq2\|h\|_{4/3}^2$. Taking adjoints proves the [finite-field paraboloid fourth-moment extension estimate](../../../fourier-analysis.md#finite-field-paraboloid-fourth-moment-extension-estimate)

$$
\boxed{R^*(2\to4)\leq\sqrt2<10.}
$$

In fact this argument works for both residue classes of odd primes.

If $p\equiv1\pmod4$, choose $i\in\mathbb F_p$ with $i^2=-1$. The complete line $\ell=\{(t,it,0):t\in\mathbb F_p\}$ lies in $P$. For $g=1_\ell$ the normalized surface $L^2$ [norm](../../../functional-analysis.md#norm) is $p^{-1/2}$, and [orthogonality of characters](../../../representation-theory.md#character-orthogonality) gives $Eg(x)=p^{-1}1_{\{x_1+ix_2=0\}}$. That annihilator plane has $p^2$ points, so the [isotropic-line obstruction to finite-field restriction](../../../fourier-analysis.md#isotropic-line-obstruction-to-finite-field-restriction) gives

$$
\boxed{R^*(2\to q)\geq\frac{p^{2/q-1}}{p^{-1/2}}=p^{2/q-1/2}.}
$$

This tends to infinity along these primes for every $q<4$, as required.

## 5

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

A [Boolean function](../../../combinatorics.md#boolean-function) takes each vector of bits to either zero or one. Use independent uniform input bits; the [influence of a variable](../../../combinatorics.md#influence-of-a-variable) is the probability that flipping that bit changes the value. A [quite fair Boolean function](../../../combinatorics.md#quite-fair-boolean-function) has $1/4\leq\mathbb Ef\leq3/4$. All logarithms in the estimates below are natural, except where a base is explicitly written.

Here is a [balanced tribes construction with unused coordinates](../../../combinatorics.md#balanced-tribes-construction-with-unused-coordinates) valid for every $n\geq2$. For each $w\geq1$ put $m_w=\lfloor(\log2)2^w\rfloor$, and choose the largest $w$ with $wm_w\leq n$. Partition $wm_w$ of the bits into $m=m_w$ blocks of size $w$. Let $f$ be one when at least one block is all ones, and ignore the other bits. This is a [tribes function](../../../combinatorics.md#tribes-function). With $s=2^{-w}$, its zero probability is $(1-s)^m$.

For $w=1$ the function is a single bit and has mean $1/2$. For $w\geq2$, $m s\leq\log2$ and $m s\geq\log2-s$. The elementary inequalities $-s/(1-s)\leq\log(1-s)\leq-s$ give

$$
(1-s)^m\geq\exp\left(-\frac{\log2}{1-s}\right)\geq\frac14,\qquad (1-s)^m\leq e^{-\log2+s}\leq\frac{e^{1/4}}2<\frac34.
$$

Thus both output probabilities are between one quarter and three quarters.

A used bit is pivotal exactly when the other $w-1$ bits of its block are one and every other block fails. Hence its influence is $2^{1-w}(1-2^{-w})^{m-1}\leq2^{1-w}$; unused bits have zero influence. Maximality of $w$ gives $n<(w+1)m_{w+1}\leq(w+1)(\log2)2^{w+1}$. Also $w\leq\log_2n$ for $n\geq2$: this is immediate for $w=1$, while for $w\geq2$ one has $wm_w\geq2^w$. Therefore

$$
\operatorname{Inf}_j(f)\leq2^{1-w}<\frac{4(\log2)(w+1)}n\leq\frac{4(\log n+\log2)}n\leq\boxed{\frac{8\log n}n<\frac{10\log n}n}.
$$

This proves the requested existence with room in the constant. The dimension-one boundary case cannot satisfy the printed logarithmic bound: a quite fair function of one bit is nonconstant and has influence one, whereas $10\log1=0$. Thus the statement requires the usual nontrivial range $n\geq2$ (or its intended large-$n$ interpretation).

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Use normalized [Fourier-Walsh transform](../../../combinatorics.md#fourier-walsh-transform) coefficients $\widehat g(\xi)=2^{-n}\sum_x g(x)(-1)^{x\cdot\xi}$. The Hamming weight $|\xi|$ counts the nonzero coordinates. Norms on the input cube use uniform probability, and a frequency integral here is counting over $\xi\in\mathbb F_2^n$. A common alternative normalization multiplies both sides of the requested comparison by the same factor and does not change it.

[Beckner's inequality](../../../combinatorics.md#beckner-s-inequality) states that for $1<p\leq q<\infty$ and $0\leq\rho\leq\sqrt{(p-1)/(q-1)}$, the [noise operator on the Boolean hypercube](../../../combinatorics.md#noise-operator-on-the-boolean-hypercube), with coefficients $\widehat{T_\rho g}(\xi)=\rho^{|\xi|}\widehat g(\xi)$, satisfies $\|T_\rho g\|_q\leq\|g\|_p$. In particular choose $q=2$, $p=4/3$, $\rho=1/\sqrt3$.

Let $g=1_A$ and $\alpha=|A|/2^n$. Then $\|g\|_{4/3}^2=\alpha^{3/2}$. On frequencies of weight at most two, $\rho^{2|\xi|}\geq1/9$, so [Beckner's inequality](../../../combinatorics.md#beckner-s-inequality) and [Parseval's identity](../../../fourier-analysis.md#parseval-identity) give the [low-degree Fourier mass of a sparse Boolean set](../../../combinatorics.md#low-degree-fourier-mass-of-a-sparse-boolean-set) estimate

$$
S_{\leq2}:=\sum_{|\xi|\leq2}\widehat g(\xi)^2\leq9\sum_\xi\rho^{2|\xi|}\widehat g(\xi)^2=9\|T_\rho g\|_2^2\leq9\alpha^{3/2}.
$$

The [indicator function](../../../measure-theory.md#indicator-function) is real and the cube characters are real, so the displayed squares equal the squared [absolute values](../../../real-analysis.md#absolute-value). Total [Fourier weight](../../../combinatorics.md#fourier-weight) is $\sum\widehat g(\xi)^2=\|g\|_2^2=\alpha$. If $2^n>2003$, then $0<\alpha\leq1/2003$ and $9\sqrt\alpha\leq9/\sqrt{2003}<1/2$, since $2003>18^2$. Therefore

$$
\boxed{S_{\leq2}<\frac\alpha2<\alpha-S_{\leq2}=\sum_{|\xi|>2}\widehat g(\xi)^2.}
$$

This establishes the strict comparison for every power $N=2^n>2003$, not merely for an unspecified very large threshold. The original PDF supplies the density condition and Beckner request, both missing from the converted TeX.

## 6

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

We use the [Bose-Chowla Sidon construction](../../../additive-combinatorics.md#bose-chowla-sidon-construction), deriving its difference property explicitly. Let $p$ be an odd prime and choose a generator $\theta$ of the [multiplicative group of a finite field](../../../algebra.md#multiplicative-group-of-a-finite-field) of the quadratic [finite field extension](../../../algebra.md#finite-field-extension) $\mathbb F_{p^2}$. Such a generator cannot belong to $\mathbb F_p$, so $1,\theta$ are linearly independent over the prime field. For each $t\in\mathbb F_p$, the nonzero field element $\theta+t$ has a unique exponent $a_t$ modulo $p^2-1$, with $\theta^{a_t}=\theta+t$. The $p$ exponents are distinct.

Suppose $a_s-a_t=a_u-a_v$ in the [cyclic group](../../../group.md#cyclic-group). Multiplying the corresponding field elements gives

$$
(\theta+s)(\theta+v)=(\theta+u)(\theta+t).
$$

Subtract the common $\theta^2$ term. Linear independence of $1,\theta$ gives $s+v=u+t$ and $sv=ut$. Thus the two unordered pairs are the roots of the same monic [quadratic polynomial](../../../polynomial.md#quadratic-polynomial), so $\{s,v\}=\{u,t\}$. Either $s=u,v=t$, giving the same ordered difference, or $s=t,v=u$, giving two zero differences. This is exactly the [Sidon set](../../../additive-combinatorics.md#sidon-set) property.

Choose the integer representatives in $\{1,\ldots,p^2-1\}$. Equality of integer differences implies equality modulo $p^2-1$, so their Sidon property persists in the integers. Now apply the given prime-gap hypothesis at $x=\sqrt N$ to get $\sqrt N-N^{3/8}\leq p\leq\sqrt N$ for large $N$. The representatives fit inside $\{1,\ldots,N\}$, because $p^2-1\leq N$, and their [cardinality](../../../set-theory.md#cardinality) is

$$
\boxed{|A|=p\geq\sqrt N-N^{3/8}=\sqrt N-o(\sqrt N).}
$$

Only the supplied short-interval prime existence and the elementary structure of a finite field are used.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Write $m=|A|$, choose $u=\lfloor N^{3/4}\rfloor$, and let $A_i$ count the points of $A$ in the length-$u$ window ending at $i$, for $1\leq i\leq N+u$. Each element occurs in precisely $u$ such windows, so $\sum_i A_i=um$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) consequently gives

$$
\sum_i\binom{A_i}2=\frac12\left(\sum_iA_i^2-um\right)\geq\frac12\left(\frac{u^2m^2}{N+u}-um\right).
$$

On the other hand, a pair $a<b$ of difference $d=b-a<u$ belongs to exactly $u-d$ windows; larger differences contribute none. The [Sidon set](../../../additive-combinatorics.md#sidon-set) condition permits at most one pair for each positive difference $d$. Therefore

$$
\sum_i\binom{A_i}2\leq\sum_{d=1}^{u-1}(u-d)=\frac{u(u-1)}2.
$$

Combining these two estimates proves the [sliding-window upper bound for Sidon sets](../../../additive-combinatorics.md#sliding-window-upper-bound-for-sidon-sets):

$$
m^2\leq(N+u)\left(1-\frac1u+\frac mu\right)\leq N+u+\frac{N+u}{u}m.
$$

If $D=(N+u)/u$, the final inequality for this [quadratic polynomial](../../../polynomial.md#quadratic-polynomial) implies $m\leq\sqrt{N+u}+D$; otherwise $m(m-D)>N+u$. With the chosen $u$, $D=O(N^{1/4})$ and $\sqrt{N+u}=\sqrt N+O(N^{1/4})$. Thus

$$
\boxed{|A|\leq\sqrt N+O(N^{1/4})=\sqrt N+o(\sqrt N).}
$$

Together with part (i)'s construction, this proves that the maximum [cardinality](../../../set-theory.md#cardinality) is **$\sqrt N+o(\sqrt N)$**. The lower and upper error terms need not have the same size to establish that asymptotic conclusion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
