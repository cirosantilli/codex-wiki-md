# Paper 8

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_8.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_8.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
  - [vii](#1/vii)
    - [Solution](#1/vii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use normalized [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) and the [inner product](../../../linear-algebra.md#inner-product)

$$
\widehat f(n)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)e^{-int}\,dt,\qquad
\langle f,g\rangle=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)\overline{g(t)}\,dt.
$$

The functions $e_n(t)=e^{int}$ are [orthonormal](../../../linear-algebra.md#orthonormal-set). Hence the [Fourier partial sum](../../../fourier-series.md#fourier-partial-sum) $S_Nf=\sum_{|n|\leq N}\widehat f(n)e_n$ is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the [trigonometric polynomials](../../../fourier-series.md#trigonometric-polynomial) of degree at most $N$. For any such polynomial $P$, [orthogonality](../../../linear-algebra.md#orthogonal-vectors) gives

$$
\|f-P\|_2^2=\|f-S_Nf\|_2^2+\|S_Nf-P\|_2^2,
$$

so $\|f-S_Nf\|_2\leq\|f-P\|_2$.

Given $\varepsilon>0$, the permitted density result supplies a [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) $P$ with $\|f-P\|_\infty<\varepsilon$. Once $N$ includes its degree,

$$
\|f-S_Nf\|_2\leq\|f-P\|_2\leq\|f-P\|_\infty<\varepsilon.
$$

Therefore **the [Fourier partial sums](../../../fourier-series.md#fourier-partial-sum) converge to $f$ in the normalized $L^2$ norm**, giving exactly the stated mean-square limit.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Apply part (i) to the continuous difference $h=f-g$. Every [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) of $h$ vanishes, so every [Fourier partial sum](../../../fourier-series.md#fourier-partial-sum) is zero. The [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) convergence from part (i) therefore gives $\|h\|_2=0$.

If $h(t_0)\ne0$, [continuity](../../../calculus.md#continuous-function) gives an interval on which $|h|$ is bounded below by a positive number. That interval would contribute positively to $\|h\|_2^2$, a contradiction. Hence

$$
\boxed{f=g\quad\text{at every point of the circle}.}
$$

The continuity hypothesis upgrades equality almost everywhere to pointwise equality.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

By the [Weierstrass M-test](../../../probability-and-statistics.md#weierstrass-m-test), absolute summability of the [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) makes $\sum_n\widehat f(n)e^{int}$ uniformly convergent to a continuous periodic function $H$. Termwise integration is justified by that [uniform convergence](../../../real-analysis.md#uniform-convergence), and [orthogonality](../../../linear-algebra.md#orthogonal-vectors) gives

$$
\widehat H(k)=\widehat f(k)\qquad(k\in\mathbb Z).
$$

Part (ii) then implies $H=f$. Thus **the [Fourier series](../../../fourier-series.md) converges uniformly to the original function**, not merely to some continuous limit. In particular,

$$
\boxed{\|S_Nf-f\|_\infty
\leq\sum_{|n|>N}|\widehat f(n)|\longrightarrow0.}
$$

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

The [absolute Fourier convergence from a square-integrable derivative](../../../fourier-series.md#absolute-fourier-convergence-from-a-square-integrable-derivative) uses more than the pointwise estimate $|\widehat f(n)|=O(1/|n|)$. Periodic [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\widehat{f'}(n)=in\widehat f(n).
$$

By [Bessel's inequality](../../../hilbert-space.md#bessel-s-inequality),

$$
\sum_{n\ne0}n^2|\widehat f(n)|^2
=\sum_{n\ne0}|\widehat{f'}(n)|^2
\leq\|f'\|_2^2.
$$

Now apply the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality):

$$
\boxed{\sum_{n\ne0}|\widehat f(n)|
\leq\left(\sum_{n\ne0}n^2|\widehat f(n)|^2\right)^{1/2}
\left(\sum_{n\ne0}\frac1{n^2}\right)^{1/2}
\leq\frac{\pi}{\sqrt3}\|f'\|_2.}
$$

Adding the finite constant coefficient proves absolute summability. Since a continuously differentiable periodic function has $f'\in L^2$, all hypotheses of part (iii) hold and its [Fourier series](../../../fourier-series.md) converges uniformly.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Part (i) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) show

$$
\langle f,g\rangle=\lim_{N\to\infty}\langle S_Nf,g\rangle.
$$

Direct integration of this finite [Fourier partial sum](../../../fourier-series.md#fourier-partial-sum) gives

$$
\langle S_Nf,g\rangle
=\sum_{|n|\leq N}\widehat f(n)\overline{\widehat g(n)}.
$$

Moreover [Bessel's inequality](../../../hilbert-space.md#bessel-s-inequality) puts both coefficient sequences in $\ell^2$, so their product series is absolutely convergent by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Consequently the cross form of [Parseval's identity](../../../fourier-analysis.md#parseval-identity) is

$$
\boxed{\frac1{2\pi}\int_{-\pi}^{\pi}f(t)\overline{g(t)}\,dt
=\sum_{n\in\mathbb Z}\widehat f(n)\overline{\widehat g(n)}.}
$$

Taking $g=f$ also gives equality of the squared function norm and the squared coefficient norm.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

For the [Hurwitz proof of the planar isoperimetric inequality](../../../geometry-and-topology.md#hurwitz-proof-of-the-planar-isoperimetric-inequality), take a positively oriented regular simple closed curve of length $L$ and enclosed area $A$. Write its complex position as $z(t)=x(t)+iy(t)$, with $0\leq t\leq2\pi$ proportional to [arc length](../../../riemannian-geometry.md#arc-length). Then $|z'(t)|=L/(2\pi)$. Translate the curve to make its mean position zero, and write its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) as $c_n$, with $c_0=0$.

[Green's theorem](../../../calculus.md#green-theorem) gives the signed area, and [Parseval's identity](../../../fourier-analysis.md#parseval-identity) computes it:

$$
A=\frac12\int_0^{2\pi}(xy'-yx')\,dt
=\frac12\operatorname{Im}\int_0^{2\pi}\overline z\,z'\,dt
=\pi\sum_{n\in\mathbb Z}n|c_n|^2.
$$

Periodic [integration by parts](../../../calculus.md#integration-by-parts) and [Parseval's identity](../../../fourier-analysis.md#parseval-identity) applied to $z'$ give

$$
\sum_n n^2|c_n|^2=\frac1{2\pi}\int_0^{2\pi}|z'|^2\,dt
=\frac{L^2}{4\pi^2}.
$$

Since $n\leq n^2$ for every integer $n$,

$$
\boxed{A\leq\pi\sum_n n^2|c_n|^2
=\frac{L^2}{4\pi},\qquad L^2\geq4\pi A.}
$$

The sums converge absolutely: $\sum|n||c_n|^2\leq(\sum|c_n|^2)^{1/2}(\sum n^2|c_n|^2)^{1/2}$. Equality forces $c_n=0$ unless $n=0$ or $1$; after the mean translation, $z(t)=c_1e^{it}$ is a circle. Conversely a circle attains equality. Thus **circles uniquely attain equality, up to translation and orientation**.

The same proof applies to a rectifiable simple closed curve using its Lipschitz [arc length](../../../riemannian-geometry.md#arc-length) parametrization. Its derivative exists almost everywhere and belongs to $L^2$; periodic [mollification](../../../distribution-theory.md#mollification) converges to the curve in the function and derivative $L^2$ norms. This justifies the derivative coefficient identity, [Parseval's identity](../../../fourier-analysis.md#parseval-identity) and area integral by approximation. Reversing orientation, if necessary, makes the enclosed area positive. The printed name “Hurewitz” is read as Hurwitz.

<h3 id="1/vii">vii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#1/vii)

Use the transform convention $F(\lambda)=\int_{\mathbb R}f(t)e^{-i\lambda t}\,dt$. The given [Fourier inversion theorem](../../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
f(t)=\frac1{2\pi}\int_{-\pi}^{\pi}F(\lambda)e^{it\lambda}\,d\lambda.
$$

Here $F$ is continuous, vanishes at both endpoints and belongs to $L^2[-\pi,\pi]$. It therefore defines a continuous periodic function. Its [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) at index $-n$ is $f(n)$. By part (i),

$$
P_N(\lambda)=\sum_{|n|\leq N}f(n)e^{-in\lambda}\longrightarrow F(\lambda)
\quad\text{in }L^2.
$$

Pair this convergence with $e^{it\lambda}$. Since that function has normalized $L^2$ norm one, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) yields, uniformly in $t$,

$$
\left|f(t)-\frac1{2\pi}\int_{-\pi}^{\pi}P_N(\lambda)e^{it\lambda}\,d\lambda\right|
\leq\|F-P_N\|_2\longrightarrow0.
$$

The elementary integral is the [sinc function](../../../analysis.md#sinc-function),

$$
\frac1{2\pi}\int_{-\pi}^{\pi}e^{i(t-n)\lambda}\,d\lambda
=D(t-n).
$$

Thus the [sampling expansion by periodic Fourier projection](../../../fourier-analysis.md#sampling-expansion-by-periodic-fourier-projection) is

$$
\boxed{f(t)=\sum_{n\in\mathbb Z}f(n)D(t-n).}
$$

There is no pointwise interchange with an unproved [Fourier series](../../../fourier-series.md): the calculation first uses finite sums and then an $L^2$ limit.

The convergence can also be made absolute. [Parseval's identity](../../../fourier-analysis.md#parseval-identity) gives $\sum_n|f(n)|^2=\|F\|_2^2$, and [Bessel's inequality](../../../hilbert-space.md#bessel-s-inequality) applied to $e^{it\lambda}$ gives $\sum_n|D(t-n)|^2\leq1$. Hence

$$
\sum_{|n|>N}|f(n)D(t-n)|
\leq\left(\sum_{|n|>N}|f(n)|^2\right)^{1/2}\longrightarrow0
$$

uniformly in $t$. At an integer argument, $D$ is one at zero and zero at the other integers, so the expansion interpolates the samples exactly.

## 2

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

We prove the [Kahane-Katznelson divergence theorem](../../../fourier-series.md#kahane-katznelson-divergence-theorem) through an explicit small-norm block construction. Let $\mu$ be normalized [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) on the circle.

First establish the [compact-set Fourier amplification lemma](../../../fourier-series.md#compact-set-fourier-amplification-lemma). If a compact set $K$ satisfies

$$
\mu(K)\leq\exp(-8\pi M/\varepsilon),\qquad0<\varepsilon\leq1,\quad M\geq1,
$$

we can make a [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) $q$ with $\|q\|_\infty\leq\varepsilon$, supported in any sufficiently high interval of positive frequencies, whose partial prefix has magnitude greater than $M$ on $K$.

To construct it, choose a smooth nonnegative function $u$ equal to one near $K$, with values at most one and mean

$$
0<\delta=\int u\,d\mu<\exp(-4\pi M/\varepsilon).
$$

[Outer regularity](../../../measure-theory.md#outer-regular-measure) and a smooth cutoff give this choice; the stipulated bound on $\mu(K)$ leaves room between the two exponentials. The [Schwarz integral on the unit disk](../../../partial-differential-equation.md#schwarz-integral-on-the-unit-disk)

$$
H(z)=\int_{\mathbb T}\frac{e^{it}+z}{e^{it}-z}\,u(t)\,d\mu(t)
$$

has positive real part in the disk, $H(0)=\delta$, and boundary real part $u$. Its [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm)

$$
W(z)=\log H(z)-\log\delta
$$

satisfies $W(0)=0$ and $|\operatorname{Im}W|<\pi/2$. On $K$, the boundary value has $\operatorname{Re}W\geq\log(1/\delta)>4\pi M/\varepsilon$. Smoothness of $u$ makes $H$ continuous at the boundary, and its positive boundary real part near $K$ makes $W$ continuous there.

Choose a radius just below one, then truncate the Taylor series of $W$ at that radius. This gives an analytic polynomial $R(e^{it})$ with zero constant term, degree $d$, and

$$
|\operatorname{Im}R(t)|<\pi,\qquad
\operatorname{Re}R(t)>4\pi M/\varepsilon-1\quad(t\in K).
$$

The radial function is analytic beyond the closed unit disk, so the Taylor truncation is uniform on the whole circle. For $L>d$, put

$$
q(t)=\frac{\varepsilon}{\pi}e^{iLt}\operatorname{Im}R(t).
$$

Its frequencies lie between $L-d$ and $L+d$, all positive. Its prefix through frequency $L$ includes exactly the negative-frequency half of $\operatorname{Im}R$ shifted into this interval:

$$
S_Lq(t)=-\frac{\varepsilon}{2\pi i}e^{iLt}\overline{R(t)}.
$$

Consequently $|S_Lq(t)|>\varepsilon(4\pi M/\varepsilon-1)/(2\pi)>M$ on $K$, whereas $\|q\|_\infty<\varepsilon$. Increasing $L$ places the entire block above any previously used frequency.

We next use [compact batching of a small open set](../../../measure-theory.md#compact-batching-of-a-small-open-set) to handle an arbitrary null set, without assuming that it is compact or a countable union of compact null sets. Set

$$
\varepsilon_{j,k}=2^{-j-k-2},\qquad j\geq1,\ k\geq0.
$$

For each $j$, choose an open $U_j\supseteq E$ with $\mu(U_j)<\exp(-8\pi j/\varepsilon_{j,0})$. Decompose $U_j$ into countably many closed subarcs with pairwise disjoint interiors: subdivide each open component into closed pieces accumulating only at its excluded endpoints. Group these subarcs into finite successive batches $K_{j,k}$. After batch $k$, include enough pieces that the remaining total length is less than $\exp(-8\pi j/\varepsilon_{j,k+1})$. Require each batch endpoint in the enumeration to increase. Then

$$
U_j=\bigcup_{k\geq0}K_{j,k},\qquad
\mu(K_{j,k})\leq\exp(-8\pi j/\varepsilon_{j,k}).
$$

Each batch is compact; endpoints shared by pieces have zero measure and do not affect the estimates.

Enumerate the pairs $(j,k)$ in diagonal order. Apply the block lemma with target $M=j$ to each $K_{j,k}$, and shift its spectrum above all preceding blocks. Denote the resulting polynomial by $q_{j,k}$ and set

$$
f=\sum_{j\geq1,\ k\geq0}q_{j,k}.
$$

Since $\sum_{j,k}\varepsilon_{j,k}=1/2$, this series is uniformly convergent and defines a continuous complex-valued function.

Fix $t\in E$. For every $j$ there is a $k$ with $t\in K_{j,k}$. The difference between the [Fourier partial sum](../../../fourier-series.md#fourier-partial-sum) just before that block and the sum at its midpoint has magnitude greater than $j$: previous blocks cancel in the difference, and future blocks have not yet entered. As $j\to\infty$, these cutoffs tend to infinity. At least one of the two partial sums therefore has magnitude greater than $j/2$. The [Fourier partial sums](../../../fourier-series.md#fourier-partial-sum) are unbounded, hence not Cauchy, at $t$. We have proved

$$
\boxed{E\subseteq\{t:\limsup_N|S_Nf(t)|=\infty\}.}
$$

This establishes divergence on every prescribed null set, including dense nonclosed null sets; it does not assert that the divergence set is exactly $E$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Use the [uniform bound for harmonic sine polynomials](../../../fourier-series.md#uniform-bound-for-harmonic-sine-polynomials)

$$
P_m(t)=\sum_{k=1}^m\frac{\sin kt}{k},\qquad
\|P_m\|_\infty\leq C_0,\quad C_0=1+\pi.
$$

For completeness, reduce to $0<t\leq\pi$ and split at $K=\min(m,\lfloor1/t\rfloor)$. The first part is bounded by $Kt\leq1$. Geometric-series summation bounds every interval sum of $\sin kt$ by $1/\sin(t/2)\leq\pi/t$. [Summation by parts](../../../analytic-number-theory.md#abel-s-summation-formula) bounds the remaining harmonic-weighted tail by $\pi/[t(K+1)]\leq\pi$. Negative $t$ follows by oddness and $t=0$ is immediate.

Let $H_m=\sum_{k=1}^m1/k$. Choose $m_j$ so large that $H_{m_j}\geq C_0\,2^{j+2}$, and positive integers $L_j>m_j$ such that the intervals $[L_j-m_j,L_j+m_j]$ are strictly separated and increase. Define

$$
Q_j(t)=e^{iL_jt}\frac{P_{m_j}(t)}{H_{m_j}},\qquad
\boxed{g(t)=\frac12\sum_{j=1}^{\infty}Q_j(t).}
$$

The bound $\|Q_j\|_\infty\leq2^{-j-2}$ makes this a continuous function with $g(0)=0$.

Each [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) of $P_m$ has modulus $1/(2k)$, so the sum of the absolute coefficients is $H_m$. Therefore every prefix of a normalized block $Q_j$ has norm at most one. At any Fourier cutoff, all earlier blocks are complete, at most one block is partial and all later blocks are absent. Hence

$$
\boxed{\|S_ng\|_\infty
\leq\frac12\left(\sum_{j\geq1}2^{-j-2}+1\right)
=\frac58<1.}
$$

At zero, a completed block contributes zero, but its prefix through frequency $L_j$ consists of the negative-frequency sine coefficients and equals $i/2$. Thus

$$
S_{L_j}g(0)=\frac i4,\qquad
S_{L_j+m_j}g(0)=0.
$$

Both index sequences tend to infinity. **The uniformly bounded partial sums fail to converge at the origin**, even though the function is continuous and zero there.

## 3

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For [infinite products](../../../real-analysis.md#infinite-product), a nonzero limiting product requires that its factors tend to one. A useful sufficient condition is

$$
\sum_j|u_j|<\infty,\qquad 1+u_j\ne0.
$$

After finitely many factors, $|u_j|<1/2$ and the principal [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm) satisfies $|\log(1+u_j)|\leq2|u_j|$. Therefore the sum of logarithms converges, and exponentiating it gives a finite nonzero product. The same argument on compact sets proves [infinite product convergence from logarithmic tails](../../../real-analysis.md#infinite-product-convergence-from-logarithmic-tails): a locally uniformly absolutely convergent tail of [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) logarithms gives a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) nonvanishing tail product. Finite factors then determine all zeros and their orders.

The [Weierstrass elementary factors](../../../real-analysis.md#weierstrass-elementary-factor) are

$$
E_p(w)=(1-w)\exp\left(w+\frac{w^2}{2}+\cdots+\frac{w^p}{p}\right),\quad
E_0(w)=1-w.
$$

For $|w|<1$,

$$
\log E_p(w)=-\sum_{\nu=p+1}^{\infty}\frac{w^\nu}{\nu},
\qquad
|\log E_p(w)|\leq2|w|^{p+1}\quad(|w|\leq1/2).
$$

Their only zero is a simple zero at $w=1$.

Work with [entire functions](../../../complex-analysis.md#entire-function) on $\mathbb C$. As usual for prescribed exact zero orders, the distinct zero locations must have consistent multiplicities. The literal statement allows repeated locations with conflicting orders; that cannot be true, for example if the same point is prescribed order one and order two. Remove consistent repetitions rather than adding their orders, and separate a possible zero at the origin.

List the distinct nonzero locations as $a_j$, with prescribed orders $n_j$, and write $m$ for the prescribed order at zero, or zero if the origin is not prescribed. Choose $p_j$ large enough that

$$
n_j2^{-p_j}\leq2^{-j}.
$$

Then the [Weierstrass factorization theorem](../../../complex-analysis.md#weierstrass-factorization-theorem) construction is

$$
\boxed{F(z)=z^m\prod_j E_{p_j}(z/a_j)^{n_j}.}
$$

On every compact set, $|z/a_j|\leq1/2$ for all sufficiently large $j$ because $|a_j|\to\infty$. Its logarithmic tail is bounded by

$$
\sum_j n_j|\log E_{p_j}(z/a_j)|\leq\sum_j n_j2^{-p_j}
\leq\sum_j2^{-j}.
$$

Thus the product converges locally uniformly, is entire, and has exactly the specified zeros with exactly their orders. At a prescribed zero, only its own finite factor vanishes; all other finite factors and the tail product are nonzero.

Without escape to infinity the conclusion fails in general. Distinct proposed zeros $1/j$ accumulate at zero. The [identity theorem](../../../complex-analysis.md#identity-theorem) would force an [entire function](../../../complex-analysis.md#entire-function) with those zeros to vanish identically, which does not have precisely the prescribed isolated zeros. A finite zero set can of course be realized by a polynomial.

For [entire functions with the same zero divisor](../../../complex-analysis.md#entire-functions-with-the-same-zero-divisor), the quotient $q=f/g$ extends through every common zero by cancelling equal local powers. It is entire and nowhere zero. Hence $q'/q$ is entire and has a primitive on the [simply connected](../../../algebraic-topology.md#simply-connected-space) plane. Choose $h(0)$ with $e^{h(0)}=q(0)$ and put

$$
h(z)=h(0)+\int_0^z\frac{q'(\zeta)}{q(\zeta)}\,d\zeta.
$$

The derivative of $qe^{-h}$ vanishes, and its value at zero is one. Therefore

$$
\boxed{f=e^h g.}
$$

If also $f=e^k g$, then $e^{h-k}=1$ everywhere. The continuous difference $h-k$ takes values in the discrete set $2\pi i\mathbb Z$ and so is constant on the [connected](../../../geometry-and-topology.md#connected-space) plane:

$$
\boxed{h-k=2\pi i\ell\quad\text{for one fixed }\ell\in\mathbb Z.}
$$

The whole-plane hypothesis matters: a zero-free [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) quotient on a multiply [connected](../../../geometry-and-topology.md#connected-space) domain need not possess a global [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write the [finite abelian group](../../../group.md#finite-abelian-group) additively. A [character of a finite abelian group](../../../group.md#character-of-a-finite-abelian-group) is a [group homomorphism](../../../group-theory.md#group-homomorphism) $\chi:G\to\{z:|z|=1\}$. We first prove that there are exactly $|G|$ such [characters of a finite abelian group](../../../group.md#character-of-a-finite-abelian-group), without assuming a structure theorem.

Use [extension of a character across a cyclic quotient](../../../group.md#extension-of-a-character-across-a-cyclic-quotient). Given a [subgroup](../../../group.md#subgroup) $H$ and $a\notin H$, let $k$ be the least positive integer with $ka\in H$. The [subgroup](../../../group.md#subgroup) $K=H+\langle a\rangle$ has $k$ cosets of $H$. If $\phi$ is a [character of a finite abelian group](../../../group.md#character-of-a-finite-abelian-group) on $H$, choose any of the $k$ roots $\lambda^k=\phi(ka)$ and define

$$
\widetilde\phi(h+ja)=\phi(h)\lambda^j.
$$

This is well-defined: two representations differ by an integer multiple of $ka$, and the root equation exactly cancels that difference. It is a [character of a finite abelian group](../../../group.md#character-of-a-finite-abelian-group), and every extension arises from one of the $k$ choices of $\lambda$. Build a chain from the trivial [subgroup](../../../group.md#subgroup) to $G$ by adjoining elements. The [character of a finite abelian group](../../../group.md#character-of-a-finite-abelian-group) count multiplies by the same factor as the [subgroup](../../../group.md#subgroup) order at every step, so $|\widehat G|=|G|$.

For a nontrivial [character of a finite abelian group](../../../group.md#character-of-a-finite-abelian-group) $\eta$, choose $a$ with $\eta(a)\ne1$. Translating the group sum shows

$$
\sum_{x\in G}\eta(x)
=\eta(a)\sum_{x\in G}\eta(x),
$$

so the sum is zero. Applied to $\chi\overline\psi$, this proves

$$
\sum_{x\in G}\chi(x)\overline{\psi(x)}
=\begin{cases}|G|,&\chi=\psi,\\0,&\chi\ne\psi.\end{cases}
$$

The $|G|$ [orthogonal](../../../linear-algebra.md#orthogonal-vectors) nonzero [characters of a finite abelian group](../../../group.md#character-of-a-finite-abelian-group) therefore form a [basis](../../../vector-space.md#basis) of all complex [functions](../../../function.md) on $G$, a [vector space](../../../vector-space.md) of [dimension](../../../vector-space.md#dimension-vector-space) $|G|$.

With the unnormalized [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) $\widehat f(\chi)=\sum_{x\in G}f(x)\overline{\chi(x)}$, expansion in that basis gives the [Fourier inversion on a finite group](../../../additive-combinatorics.md#fourier-inversion-on-a-finite-group)

$$
\boxed{f(x)=\frac1{|G|}\sum_{\chi\in\widehat G}\widehat f(\chi)\chi(x).}
$$

Under a normalized forward-transform convention the prefactor would instead be one. Thus the unspecified constant is determined by the convention, and the inversion itself follows directly from [character of a finite abelian group](../../../group.md#character-of-a-finite-abelian-group) counting and [orthogonality](../../../linear-algebra.md#orthogonal-vectors).

## 4

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use the [Chebyshev estimate from central binomial coefficients](../../../number-theory.md#chebyshev-estimate-from-central-binomial-coefficients). Define

$$
\vartheta(x)=\sum_{p\leq x}\log p,\qquad
\psi(x)=\sum_{p^k\leq x}\log p.
$$

The first is the [Chebyshev theta function](../../../number-theory.md#chebyshev-theta-function); the second counts prime powers with the same logarithmic prime weight. For a positive integer $m$, every prime $m<p\leq2m$ divides $\binom{2m}{m}$, hence

$$
\vartheta(2m)-\vartheta(m)\leq\log\binom{2m}{m}\leq2m\log2.
$$

Summing over dyadic intervals yields $\vartheta(2^j)\leq2^{j+1}\log2$. By monotonicity and rounding $x$ upward to a power of two,

$$
\vartheta(x)\leq Cx,\qquad C=4\log2.
$$

For the lower bound, the central [binomial coefficient](../../../combinatorics.md#binomial-coefficient) is the largest of the $2m+1$ coefficients whose sum is $4^m$, so

$$
\log\binom{2m}{m}\geq2m\log2-\log(2m+1).
$$

The exponent of a prime in the central coefficient is

$$
\sum_{k\geq1}\left(\left\lfloor\frac{2m}{p^k}\right\rfloor
-2\left\lfloor\frac m{p^k}\right\rfloor\right).
$$

Each summand is zero or one. Therefore $\log\binom{2m}{m}\leq\psi(2m)$. Higher prime powers contribute only

$$
0\leq\psi(x)-\vartheta(x)
=\sum_{k=2}^{\lfloor\log_2x\rfloor}\vartheta(x^{1/k})
\leq C\sqrt x\,\log_2x=o(x).
$$

Combining the lower bound with $2m$ just below $x$ shows $\vartheta(x)\geq cx$ for sufficiently large $x$, with, for example, $c=(\log2)/2$.

Let $\pi(x)$ denote the number of primes at most $x$. Since every prime weight is at most $\log x$,

$$
\pi(x)\geq\frac{\vartheta(x)}{\log x}\geq c\frac{x}{\log x}.
$$

For the upper bound, separate the primes at $\sqrt x$. The small ones number at most $\sqrt x$, and every larger one has weight at least $(\log x)/2$, giving

$$
\pi(x)\leq\sqrt x+\frac{2\vartheta(x)}{\log x}
\leq\sqrt x+2C\frac{x}{\log x}.
$$

Since $\sqrt x=o(x/\log x)$, this proves

$$
\boxed{A\frac n{\log n}\leq N(n)\leq B\frac n{\log n}}
$$

for all sufficiently large $n$, for instance with $A=(\log2)/2$ and $B=8\log2+1$. This elementary [Chebyshev estimate](../../../number-theory.md#chebyshev-estimate) does not assume the [Prime number theorem](../../../analytic-number-theory.md#prime-number-theorem).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The printed differential in the transform integral is $dz$; it must be $dt$, since $z$ is the transform parameter. We prove the [Newman Tauberian theorem](../../../analysis.md#newman-tauberian-theorem) in this corrected interpretation. Set

$$
F_T(z)=\int_0^T f(t)e^{-tz}\,dt,\qquad |f(t)|\leq M
$$

almost everywhere. The finite-interval transform $F_T$ is entire.

Fix $R>0$. Because the analytic domain contains the whole imaginary axis, compactness supplies a $\delta>0$ such that the thin rectangle $-\delta\leq\operatorname{Re}z\leq0$, $|\operatorname{Im}z|\leq R$ lies in the domain. Let $C_+$ be the right semicircle of radius $R$, oriented from $-iR$ to $iR$. Join its endpoints by a leftward path $L$ along the other three sides of that rectangle. This is a closed positively oriented contour.

Use [contour damping for bounded Laplace transforms](../../../analysis.md#contour-damping-for-bounded-laplace-transforms) with

$$
K_T(z)=e^{Tz}\left(1+\frac{z^2}{R^2}\right)\frac1z.
$$

The [residue theorem](../../../analysis.md#residue-theorem) gives

$$
F(0)-F_T(0)=\frac1{2\pi i}
\left[\int_{C_+}(F-F_T)K_T\,dz
+\int_L FK_T\,dz-\int_L F_TK_T\,dz\right].
$$

On $C_+$, with $x=\operatorname{Re}z>0$,

$$
|e^{Tz}(F-F_T)(z)|\leq M/x,\qquad
\left|1+z^2/R^2\right|=2x/R.
$$

Thus the integrand has modulus at most $2M/R^2$, and this half-circle contributes at most $M/R$ after division by $2\pi$.

On $L$, the $F$ term tends to zero as $T\to\infty$: every interior point of the path has negative real part, $F$ is bounded on this fixed compact path, and the remaining kernel factor is bounded because the path avoids zero. [Dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) applies, with the two endpoints irrelevant to the path integral.

For the $F_T$ term, deform $L$ to the left semicircle $C_-$ of radius $R$. This deformation uses only the [entire function](../../../complex-analysis.md#entire-function) $F_T$; it does not demand that $F$ extend across a large left half-disk. Both paths lie to the left of zero and their enclosed deformation region avoids the kernel pole. On $C_-$, for $x<0$,

$$
|e^{Tz}F_T(z)|
\leq M\int_0^T e^{(T-t)x}\,dt\leq M/|x|.
$$

The same circle factor gives another bound $M/R$. Consequently

$$
\limsup_{T\to\infty}|F_T(0)-F(0)|\leq\frac{2M}{R}.
$$

The radius $R$ is arbitrary, so

$$
\boxed{\int_0^\infty f(t)\,dt=\lim_{T\to\infty}F_T(0)=F(0).}
$$

This proves convergence of the ordinary improper integral, not merely a damped limit.

For the weakened domain hypothesis, take $f(t)=1$. Its [Laplace transform](../../../analysis.md#laplace-transform) is $F(z)=1/z$, analytic on the open right half-plane, but $\int_0^T f(t)\,dt=T$ diverges. **Analyticity only in the open right half-plane is insufficient.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
