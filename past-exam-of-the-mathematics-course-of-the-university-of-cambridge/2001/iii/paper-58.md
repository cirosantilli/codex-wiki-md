# Paper 58

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper58.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper58.pdf)

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
- [7](#7)
  - [Solution](#7/solution)

## 1

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [cubic spline](../../../uniform-approximation.md#cubic-spline) is even, so the symmetry of the normalized [B-splines](../../../uniform-approximation.md#b-spline) gives $N_{j,4}(-x)=N_{6-j,4}(x)$. It therefore suffices to extract three [coefficients](../../../vector-space.md#coefficient). The two [polynomial](../../../polynomial.md) pieces join with matching values and first two [derivatives](../../../calculus.md#derivative) at zero, so the function belongs to the stated [cubic spline](../../../uniform-approximation.md#cubic-spline) space. At zero its right-hand [derivatives](../../../calculus.md#derivative) are

$$
f(0)=1,\qquad f'(0)=0,\qquad f''(0)=-27,\qquad f'''(0+)=81.
$$

Use the supplied [De Boor–Fix spline coefficient functional](../../../uniform-approximation.md#de-boor-fix-spline-coefficient-functional) with the unnormalized knot [polynomial](../../../polynomial.md) $\psi_j(x)=\prod_{r=j+1}^{j+3}(t_r-x)$. In this sign convention the [coefficient](../../../vector-space.md#coefficient) is

$$
c_j=\frac{\psi_jf'''-\psi_j'f''+\psi_j''f'-\psi_j'''f}{6}.
$$

For $j=1$, $\psi_1=(-1-x)^3$. Taking the right-hand limit at $-1$ kills the first three terms and gives $c_1=f(-1)=1$. For the next two [coefficients](../../../vector-space.md#coefficient) take the right-hand limit at zero. Their knot [polynomials](../../../polynomial.md) and [derivatives](../../../calculus.md#derivative) there are

$$
\begin{aligned}
\psi_2(x)&=-x(1+x)^2,&(\psi_2,\psi_2',\psi_2'',\psi_2''')(0)&=(0,-1,-4,-6),\\
\psi_3(x)&=x-x^3,&(\psi_3,\psi_3',\psi_3'',\psi_3''')(0)&=(0,1,0,-6).
\end{aligned}
$$

Consequently $c_2=(-27+6)/6=-7/2$ and $c_3=(27+6)/6=11/2$. Although the third [derivative](../../../calculus.md#derivative) jumps at zero, its multiplier $\psi_j(0)$ vanishes for these two [functionals](../../../calculus-of-variations.md#functional); taking either one-sided limit gives the same [coefficients](../../../vector-space.md#coefficient). Symmetry gives $c_4=c_2$ and $c_5=c_1$. Thus

$$
\boxed{(c_1,c_2,c_3,c_4,c_5)=(1,-7/2,11/2,-7/2,1).}
$$

For a normalized [B-spline](../../../uniform-approximation.md#b-spline) [basis](../../../vector-space.md#basis), define the synthesis [linear map](../../../vector-space.md#linear-map) $Tc=\sum_jc_jN_{j,4}$ from the maximum [coefficient](../../../vector-space.md#coefficient) [norm](../../../functional-analysis.md#norm) into the [spline](../../../uniform-approximation.md#spline-mathematics) space with its [supremum norm](../../../functional-analysis.md#supremum-norm). Nonnegativity and partition of unity give $\|T\|=1$, including equality on the all-ones [vector](../../../vector-space.md#vector). The [coefficient condition number of a normalized B-spline basis](../../../uniform-approximation.md#coefficient-condition-number-of-a-normalized-b-spline-basis) is

$$
\kappa(\mathcal S)=\|T\|\|T^{-1}\|=\sup_{0\ne s\in\mathcal S}\frac{\|c(s)\|_{\ell^\infty}}{\|s\|_\infty}.
$$

On $[0,1]$, $f'(x)=(27/2)x(3x-2)$. The only interior extremum is at $2/3$, where $f=-1$; at zero and one, $f=1$. Reflection therefore gives $\|f\|_\infty=1$. Its largest absolute [coefficient](../../../vector-space.md#coefficient) is $11/2$, proving

$$
\boxed{\kappa(\mathcal S)\ge\frac{11}{2}.}
$$

## 2

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write the [spline interpolation operator](../../../uniform-approximation.md#spline-interpolation-operator) as $P_{\mathbf x}=TA_{\mathbf x}^{-1}R$, where $R$ samples at the interpolation sites and $T$ synthesizes the normalized [B-spline](../../../uniform-approximation.md#b-spline) expansion. Sampling has [operator norm](../../../continuous-dual-space.md#operator-norm) at most one, and nonnegative [B-splines](../../../uniform-approximation.md#b-spline) with sum at most one give $\|T\|\le1$. Hence

$$
\|P_{\mathbf x}g\|_\infty\le\|A_{\mathbf x}^{-1}Rg\|_{\ell^\infty}\le\|A_{\mathbf x}^{-1}\|_{\ell^\infty}\|g\|_\infty,
\qquad\boxed{\|P_{\mathbf x}\|\le\|A_{\mathbf x}^{-1}\|_{\ell^\infty}.}
$$

Here the [matrix norm](../../../vector-space.md#matrix-norm) is the maximum absolute row sum. Existence of the [inverse matrix](../../../linear-algebra.md#matrix-inverse) requires the usual ordered distinct interpolation sites and the [Schoenberg–Whitney theorem](../../../uniform-approximation.md#schoenberg-whitney-theorem) support conditions, with endpoint values interpreted by their one-sided limits. If the displayed diagonal condition is read without the implicit ordering and distinctness, it is insufficient: all three sites equal to $1/2$ in the quadratic example give positive diagonal entries but three identical rows. The estimate applies whenever the interpolating [linear map](../../../vector-space.md#linear-map) in the question is defined uniquely.

For the quadratic [Bernstein basis](../../../functional-analysis.md#bernstein-basis), $N_1=(1-x)^2$, $N_2=2x(1-x)$ and $N_3=x^2$. Sampling and inverting give

$$
A=\begin{pmatrix}1&0&0\\1/4&1/2&1/4\\0&0&1\end{pmatrix},\qquad
A^{-1}=\begin{pmatrix}1&0&0\\-1/2&2&-1/2\\0&0&1\end{pmatrix},\qquad
\boxed{\|A^{-1}\|_{\ell^\infty}=3.}
$$

The three cardinal [Lagrange interpolation polynomials](../../../numerical-analysis.md#lagrange-polynomial) are

$$
\ell_0(x)=2x^2-3x+1,\qquad\ell_1(x)=4x(1-x),\qquad\ell_2(x)=2x^2-x.
$$

The [Lebesgue constant of interpolation](../../../uniform-approximation.md#lebesgue-constant-of-interpolation) gives the exact [operator norm](../../../continuous-dual-space.md#operator-norm): the upper bound follows from $|Pg(x)|\le\|g\|_\infty\sum_i|\ell_i(x)|$. To attain it at a maximizing point, prescribe at the three sites the signs of the corresponding cardinal [polynomials](../../../polynomial.md) and extend those values by a [continuous](../../../calculus.md#continuous-function) [piecewise linear function](../../../function.md#piecewise-linear-function) of [norm](../../../functional-analysis.md#norm) one.

On $0\le x\le1/2$, the first two cardinal [polynomials](../../../polynomial.md) are nonnegative and the last is nonpositive. Since their sum is one, their absolute sum is $1-2\ell_2(x)=1+2x-4x^2$. Its maximum is $5/4$ at $x=1/4$. Reflection gives the same maximum at $3/4$ on the other half. In particular the data $(1,1,-1)$ produce $1+2x-4x^2$, attaining $5/4$. Thus

$$
\boxed{\|P_{\mathbf x}\|=\frac54<3=\|A^{-1}\|_{\ell^\infty}.}
$$

The coefficient estimate loses cancellation among the [B-splines](../../../uniform-approximation.md#b-spline), which explains why it is not sharp for the resulting [function](../../../function.md) [norm](../../../functional-analysis.md#norm).

## 3

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [Korovkin theorem](../../../uniform-approximation.md#korovkin-theorem) says that a sequence of [positive linear operators on continuous functions](../../../topological-vector-space.md#positive-linear-operator-on-continuous-functions) on $[0,1]$ converges uniformly to the identity on every [continuous function](../../../calculus.md#continuous-function) if it does so on $1$, $x$ and $x^2$. Necessity is immediate; the quadratic barrier argument establishing sufficiency is given in Solution 6.

There is an endpoint misprint in the original PDF: the repeated knots at the right end must equal $1$, not $0$. Otherwise the advertised nondecreasing [spline knot sequence](../../../uniform-approximation.md#spline-knot-sequence) on $[0,1]$ does not exist. Use the corrected clamped [spline knot sequences](../../../uniform-approximation.md#spline-knot-sequence), with fixed order $k$ and maximum gap $h_n\to0$. Let $m_n$ denote the number of [B-splines](../../../uniform-approximation.md#b-spline) for the $n$th sequence. Nonnegativity and partition of unity show that the [Schoenberg spline operator](../../../uniform-approximation.md#schoenberg-spline-operator) $V_n$ is positive and $V_n1=1$.

The [monomial B-spline coefficients](../../../uniform-approximation.md#monomial-b-spline-coefficients) reproduce the first two nonconstant test [polynomials](../../../polynomial.md). Put

$$
a_{1,j}=\frac1{k-1}\sum_{r=j+1}^{j+k-1}t_r,\qquad
a_{2,j}=\binom{k-1}{2}^{-1}\sum_{j+1\le r<s\le j+k-1}t_rt_s.
$$

The pair sum uses $r<s$, as in the PDF; the converted TeX incorrectly includes $r=s$. Every sampling point $\tau_j$ and every knot entering these [coefficients](../../../vector-space.md#coefficient) lie in $[t_j,t_{j+k}]$, whose length is at most $kh_n$. Thus $|\tau_j-a_{1,j}|\le kh_n$. Also all these numbers belong to $[0,1]$, so

$$
|\tau_j^2-t_rt_s|\le|\tau_j(\tau_j-t_r)|+|t_r(\tau_j-t_s)|\le2kh_n,
\qquad |\tau_j^2-a_{2,j}|\le2kh_n.
$$

The positive [B-spline](../../../uniform-approximation.md#b-spline) weights give

$$
\|V_nx-x\|_\infty\le kh_n,\qquad\|V_nx^2-x^2\|_\infty\le2kh_n.
$$

Together with $V_n1=1$, the three limits prove

$$
\boxed{\|V_ng-g\|_\infty\longrightarrow0\quad\text{for every }g\in C[0,1].}
$$

Under the usual interior knot multiplicities at most $k-1$, the [splines](../../../uniform-approximation.md#spline-mathematics) are continuous and the quoted form of the [Korovkin theorem](../../../uniform-approximation.md#korovkin-theorem) applies directly. If full interior multiplicity is allowed, the output can be discontinuous. The same positive-operator quadratic barrier proof still works with bounded output [functions](../../../function.md) and the [supremum norm](../../../functional-analysis.md#supremum-norm), and proves exactly the stated uniform error limit without asserting continuity of each output. Indeed the stronger [local-support error bound for a Schoenberg spline operator](../../../uniform-approximation.md#local-support-error-bound-for-a-schoenberg-spline-operator), $\|V_ng-g\|_\infty\le\omega(g,kh_n)$, follows by comparing $g(x)$ with each active sample value. The restriction $k\ge3$ is needed for the displayed quadratic reproduction argument, not for this direct support estimate.

## 4

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Fix $\varepsilon>0$ and put $\eta=\varepsilon/2$. For each pair $s,t\in T$, choose $a_{s,t}\in A$ whose errors at these two points are smaller than $\eta$. By [continuity](../../../calculus.md#continuous-function), there is a neighborhood $U_{s,t}$ of $t$ on which $a_{s,t}>f-\eta$. For a fixed $s$, these neighborhoods cover the [compact space](../../../topology.md#compact-space) $T$. Choose a finite subcover $U_{s,t_1},\ldots,U_{s,t_m}$ and form

$$
b_s=\max_{1\le j\le m}a_{s,t_j}\in A.
$$

Then $b_s>f-\eta$ everywhere, while $b_s(s)<f(s)+\eta$, because every chosen [function](../../../function.md) has error smaller than $\eta$ at $s$. Since $b_s$ is continuous, there is a neighborhood $W_s$ of $s$ on which $b_s<f+\eta$.

A second use of [compactness](../../../topology.md#compact-space) supplies $W_{s_1},\ldots,W_{s_q}$ covering $T$. Set

$$
a=\min_{1\le i\le q}b_{s_i}\in A.
$$

Every $b_{s_i}$ is above $f-\eta$, so their minimum is also above it. At each point at least one $b_{s_i}$ is below $f+\eta$, and hence so is their minimum. This proves $\|a-f\|_\infty\le\eta<\varepsilon$. The two finite operations are the essential mechanism in [lattice approximation from two-point approximation](../../../functional-analysis.md#lattice-approximation-from-two-point-approximation); no closure under addition or multiplication has been assumed.

For the corollary take $A$ to consist of all [continuous](../../../calculus.md#continuous-function) [piecewise linear functions](../../../function.md#piecewise-linear-function) on $[0,1]$. On a common finite partition, the maximum or minimum of two affine pieces can change which piece it selects only at their crossing. Adding those finitely many crossings to the partition shows that $A$ is closed under both operations. For two distinct points, the affine [polynomial](../../../polynomial.md) through the two prescribed values belongs to $A$ and matches $f$ exactly there; for equal points use a [constant function](../../../function.md#constant-function). The proved criterion therefore gives **density of continuous piecewise linear functions in $C[0,1]$ in the supremum norm**. Concretely, interpolation on a partition of maximum gap $h$ also gives error at most $\omega(f,h)$ by [uniform continuity](../../../topological-analysis.md#uniform-continuity).

## 5

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The original PDF's kernel has an incorrect normalization. With ordinary $dt$, its integral is $\pi$, not one. Already at $n=1$ the printed kernel is the constant $1/2$. For $f\equiv1$, the printed operator therefore returns $\pi$, while $\omega(f,\delta)=0$ for every $\delta$. Thus **the literal inequality with the printed kernel is false**. The [Fejér kernel](../../../fourier-series.md#fejer-kernel) representing the stated average of [Fourier partial sums](../../../fourier-series.md#fourier-partial-sum) is

$$
K_n(t)=\frac1{2\pi n}\left(\frac{\sin(nt/2)}{\sin(t/2)}\right)^2,
\qquad \int_{-\pi}^{\pi}K_n(t)\,dt=1.
$$

The ratio at zero is interpreted by its limit. To verify the normalization and the averaging property, use the finite geometric sum:

$$
K_n(t)=\frac1{2\pi n}\left|\sum_{j=0}^{n-1}e^{ijt}\right|^2
=\frac1{2\pi}\sum_{|r|<n}\left(1-\frac{|r|}{n}\right)e^{irt}.
$$

[Fourier orthogonality](../../../fourier-series.md#fourier-orthogonality) gives unit integral; the displayed [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) are exactly the multipliers of the [Fejér sum](../../../fourier-series.md#fejer-sum). This also proves nonnegativity.

For the correctly normalized [Fejér sum](../../../fourier-series.md#fejer-sum), subtraction of $f(x)$ gives

$$
|\sigma_{n-1}f(x)-f(x)|\le\int_{-\pi}^{\pi}K_n(t)|f(x-t)-f(x)|\,dt.
$$

Take $0<\delta\le1$ and split at $|t|=\delta$. The inner part is at most $\omega(f,\delta)$, because the kernel is nonnegative and has mass one. The strict inequality in the definition of the [modulus of continuity](../../../topological-analysis.md#modulus-of-continuity) causes no endpoint issue: [continuity](../../../calculus.md#continuous-function) gives the same bound at distance exactly $\delta$.

On $0<|t|\le\pi$, $\sin(|t|/2)\ge|t|/\pi$, so

$$
K_n(t)\le\frac{\pi}{2nt^2},\qquad\int_{\delta\le|t|\le\pi}K_n(t)\,dt\le\frac{\pi}{n\delta}.
$$

Divide an arc of length $|t|$ into at most $1+|t|/\delta$ shorter arcs. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) then bounds $|f(x-t)-f(x)|$ by $(1+\pi/\delta)\omega(f,\delta)$. Consequently

$$
\|\sigma_{n-1}f-f\|_\infty\le\left[1+\frac{\pi}{n\delta}\left(1+\frac\pi\delta\right)\right]\omega(f,\delta).
$$

Choosing $\delta=n^{-1/2}$ proves the requested [fractional-scale Fejér approximation bound](../../../fourier-series.md#fractional-scale-fejer-approximation-bound) for the intended normalization, for example with the absolute constant $1+\pi+\pi^2$:

$$
\boxed{\|\sigma_{n-1}f-f\|_\infty\le(1+\pi+\pi^2)\,\omega(f,n^{-1/2}).}
$$

The same proof applies to complex-valued [continuous functions](../../../calculus.md#continuous-function), since the estimates use absolute values.

## 6

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The [Weierstrass approximation theorem](../../../functional-analysis.md#weierstrass-approximation-theorem) asserts that every real [continuous function](../../../calculus.md#continuous-function) on a [compact](../../../topology.md#compact-space) [interval](../../../real-analysis.md#interval-mathematics) is a [uniform limit](../../../real-analysis.md#uniform-limit) of [polynomials](../../../polynomial.md). An affine change of variable reduces the interval to $[0,1]$. There are two complementary routes: construct positive approximation operators, or construct an algebra dense enough to approximate absolute values and hence pointwise maxima and minima.

For the first route, the [Korovkin theorem](../../../uniform-approximation.md#korovkin-theorem) reduces convergence of [positive linear operators on continuous functions](../../../topological-vector-space.md#positive-linear-operator-on-continuous-functions) $L_n$ to the three tests $1,t,t^2$. Here is its proof. Given $f\in C[0,1]$ and $\varepsilon>0$, [uniform continuity](../../../topological-analysis.md#uniform-continuity) supplies a $\delta>0$ such that $|f(t)-f(x)|<\varepsilon$ for $|t-x|<\delta$. For all $t,x$ one then has

$$
|f(t)-f(x)|\le\varepsilon+M(t-x)^2,\qquad M=2\|f\|_\infty/\delta^2.
$$

Apply positivity to the two real inequalities obtained from this bound. At $x$ this gives

$$
|L_nf(x)-f(x)|\le |f(x)|\,|L_n1(x)-1|+\varepsilon L_n1(x)+M\bigl[L_nt^2(x)-2xL_nt(x)+x^2L_n1(x)\bigr].
$$

The expression in brackets is nonnegative and tends uniformly to zero by the three test assumptions. Also $L_n1\to1$ uniformly. Taking the upper limit of the [supremum norm](../../../functional-analysis.md#supremum-norm) and then letting $\varepsilon\downarrow0$ proves convergence for every $f$. This is the [quadratic barrier estimate for positive approximation operators](../../../uniform-approximation.md#quadratic-barrier-estimate-for-positive-approximation-operators).

The [Bernstein polynomial](../../../functional-analysis.md#bernstein-polynomial) supplies the constructive corollary

$$
B_nf(x)=\sum_{j=0}^nf(j/n)\binom nj x^j(1-x)^{n-j}.
$$

The [binomial theorem](../../../combinatorics.md#binomial-theorem) makes its nonnegative weights sum to one. Differentiating the [binomial theorem](../../../combinatorics.md#binomial-theorem), or using the first two [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) moments, gives

$$
B_n1=1,\qquad B_nt=x,\qquad B_nt^2=x^2+\frac{x(1-x)}n.
$$

The [Korovkin theorem](../../../uniform-approximation.md#korovkin-theorem) proves $B_nf\to f$ uniformly, and each $B_nf$ is a [polynomial](../../../polynomial.md), proving the [Weierstrass approximation theorem](../../../functional-analysis.md#weierstrass-approximation-theorem). The same criterion gives the [Schoenberg spline operator](../../../uniform-approximation.md#schoenberg-spline-operator) convergence in Solution 3. For periodic [functions](../../../function.md) its counterpart uses $1,\cos t,\sin t$: the nonnegative barrier $1-\cos(t-x)$ is bounded away from zero outside any fixed small arc. This [periodic Korovkin test set](../../../uniform-approximation.md#periodic-korovkin-test-set) gives convergence of the normalized [Fejér sums](../../../fourier-series.md#fejer-sum) and density of [trigonometric polynomials](../../../fourier-series.md#trigonometric-polynomial).

The [Lebesgue convergence criterion for approximation operators](../../../uniform-approximation.md#extension-of-approximation-operators-from-a-dense-subspace) addresses stability. Suppose bounded [linear operators](../../../vector-space.md#linear-operator) $L_n:C[a,b]\to C[a,b]$ converge to the identity on every [polynomial](../../../polynomial.md). Then they converge on every [continuous function](../../../calculus.md#continuous-function) if and only if $\sup_n\|L_n\|<\infty$. Sufficiency is the [extension of approximation operators from a dense subspace](../../../uniform-approximation.md#extension-of-approximation-operators-from-a-dense-subspace): for a [polynomial](../../../polynomial.md) $p$ with $\|f-p\|<\eta$ and a common bound $M$,

$$
\|L_nf-f\|\le(M+1)\eta+\|L_np-p\|.
$$

First let $n\to\infty$, then $\eta\downarrow0$. Necessity follows from the [Uniform boundedness principle](../../../banach-space.md#uniform-boundedness-principle), since a convergent $L_nf$ is bounded for every $f$. Applied to approximation [projectors](../../../vector-space.md#projection-linear-algebra), the [Lebesgue inequality for approximation projectors](../../../uniform-approximation.md#polynomial-reproduction-error-bound) is

$$
\|f-P_nf\|_\infty\le(1+\|P_n\|)E_{V_n}(f),\qquad E_{V_n}(f)=\inf_{v\in V_n}\|f-v\|_\infty.
$$

Indeed $P_nv=v$ makes $f-P_nf=(f-v)-P_n(f-v)$; take the infimum. Thus density of the ranges and a uniform bound on the [Lebesgue constants of interpolation](../../../uniform-approximation.md#lebesgue-constant-of-interpolation) imply convergence. Density alone does not control a sequence of interpolation [projectors](../../../vector-space.md#projection-linear-algebra).

There is also a kernel version of this stability criterion, useful for [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) approximation. If [integrable](../../../measure-theory.md#integrability) periodic kernels $K_n$ have uniformly bounded $L^1$ [norms](../../../functional-analysis.md#norm), their integrals tend to one, and $\int_{|t|\ge\delta}|K_n(t)|\,dt\to0$ for every $\delta>0$, then convolution with $K_n$ converges uniformly to every [continuous](../../../calculus.md#continuous-function) periodic [function](../../../function.md). Subtract $f(x)\int K_n$ and split the error into a small arc, bounded by $\omega(f,\delta)\sup_n\|K_n\|_1$, and its complement, bounded by $2\|f\|_\infty\int_{|t|\ge\delta}|K_n|$. The remaining mass error tends to zero. This [approximate identity](../../../fourier-analysis.md#approximate-identity) argument shows directly why nonnegative unit-mass [Fejér kernels](../../../fourier-series.md#fejer-kernel) work even though ordinary [Fourier partial sums](../../../fourier-series.md#fourier-partial-sum) need not converge uniformly for every continuous target.

Lebesgue's constructive approach to the [Weierstrass approximation theorem](../../../functional-analysis.md#weierstrass-approximation-theorem) starts instead with the [absolute value](../../../real-analysis.md#absolute-value). On $[-1,1]$ define the [polynomial recurrence for the absolute value](../../../functional-analysis.md#polynomial-recurrence-for-the-absolute-value)

$$
p_0(x)=0,\qquad p_{r+1}(x)=p_r(x)+\frac{x^2-p_r(x)^2}{2}.
$$

Induction gives $0\le p_r(x)\le|x|$, monotonicity, and

$$
|x|-p_{r+1}(x)=(|x|-p_r(x))\left(1-\frac{|x|+p_r(x)}2\right).
$$

The pointwise limit satisfies $p(x)^2=x^2$ and is nonnegative, hence equals $|x|$. [Dini's theorem](../../../real-analysis.md#dini-s-theorem) makes the convergence uniform. More explicitly, the continuous decreasing errors have, for any positive tolerance, open sublevel sets covering the [compact](../../../topology.md#compact-space) [interval](../../../real-analysis.md#interval-mathematics); a finite subcover supplies one index valid everywhere. Every [continuous](../../../calculus.md#continuous-function) [piecewise linear function](../../../function.md#piecewise-linear-function) has the form

$$
L(x)=a+bx+\sum_{j=1}^mc_j(x-t_j)_+,\qquad (x-t)_+=\frac{x-t+|x-t|}{2}.
$$

The $c_j$ are its changes in slope. Scaling and translating the absolute-value approximation shows that $L$ is uniformly approximable by [polynomials](../../../polynomial.md). Solution 4, or polygonal interpolation and [uniform continuity](../../../topological-analysis.md#uniform-continuity), makes these [piecewise linear functions](../../../function.md#piecewise-linear-function) dense in $C[a,b]$. Approximating $f$ first by $L$ and then by a [polynomial](../../../polynomial.md) is another complete proof of the [Weierstrass approximation theorem](../../../functional-analysis.md#weierstrass-approximation-theorem).

The [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem) generalizes from intervals to a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space) $K$: a real subalgebra $A\subseteq C(K,\mathbb R)$ containing the constants and separating points is uniformly dense. Its proof uses the same absolute-value mechanism. The [uniform closure of a function algebra](../../../uniform-approximation.md#uniform-closure-of-a-function-algebra) is an algebra. If $a$ belongs to this closure, approximation of $|t|$ by [polynomials](../../../polynomial.md) on a bounded interval containing its range proves that $|a|$ also belongs to the closure. Therefore the closure contains

$$
\max(a,b)=\frac{a+b+|a-b|}{2},\qquad\min(a,b)=\frac{a+b-|a-b|}{2}.
$$

Point separation and constants allow exact interpolation of any two real values: choose $h\in A$ with $h(s)\ne h(t)$ and solve for $\alpha,\beta$ in $\alpha h+\beta$. The [lattice approximation from two-point approximation](../../../functional-analysis.md#lattice-approximation-from-two-point-approximation) proved in Solution 4 now makes the closure all of $C(K,\mathbb R)$.

The complex version requires a unital, point-separating subalgebra closed under [complex conjugation](../../../complex-analysis.md#complex-conjugation). Its real-valued members separate points using real or imaginary parts, so the real result approximates both parts of every complex target. Conjugation closure is essential: [polynomials](../../../polynomial.md) in $z$ alone on the closed unit disk cannot approximate $\overline z$ uniformly, because $\int_{|z|=1}p(z)\,dz=0$ whereas $\int_{|z|=1}\overline z\,dz=2\pi i$.

Among the corollaries are **density of multivariate polynomials on compact subsets of real Euclidean space**, since coordinates separate points, and **density of trigonometric polynomials on the circle**, since sine and cosine separate points there. On a [compact](../../../topology.md#compact-space) [interval](../../../real-analysis.md#interval-mathematics), [polynomials](../../../polynomial.md) with rational [coefficients](../../../vector-space.md#coefficient) are a countable dense family, giving separability of $C[a,b]$. The real and complex approximation results above concern uniform approximation of continuous targets; neither asserts convergence of arbitrary interpolation schemes or arbitrary [Fourier series](../../../fourier-series.md).

## 7

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

Fix a clamped nondecreasing [spline knot sequence](../../../uniform-approximation.md#spline-knot-sequence) $t_1,\ldots,t_{n+k}$ on $[a,b]$, with $t_1=\cdots=t_k=a$ and $t_{n+1}=\cdots=t_{n+k}=b$. For continuous [splines](../../../uniform-approximation.md#spline-mathematics) assume interior multiplicities at most $k-1$, and assume $t_i<t_{i+k}$. An order-$k$ [spline](../../../uniform-approximation.md#spline-mathematics) has degree at most $k-1$ on each nonempty knot interval; at a knot of multiplicity $r$ it has $k-1-r$ continuous [derivatives](../../../calculus.md#derivative). Its dimension is $n$, and a normalized [B-spline](../../../uniform-approximation.md#b-spline) [basis](../../../vector-space.md#basis) $N_1,\ldots,N_n$ has local [support](../../../function.md#support), nonnegative values and sum one on $[a,b]$.

These properties are visible in the [Cox-de Boor recurrence](../../../uniform-approximation.md#cox-de-boor-recursion-formula). Starting with interval indicators at order one, set

$$
N_{i,k}(x)=\frac{x-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(x)+\frac{t_{i+k}-x}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(x),
$$

with a term of zero denominator defined to be zero. On each contributing [support](../../../function.md#support) the weights are nonnegative, and summing the recurrence makes the coefficients of each lower-order [B-spline](../../../uniform-approximation.md#b-spline) add to one. This gives partition of unity and $\operatorname{supp}N_{i,k}=[t_i,t_{i+k}]$, with endpoint values defined by limits.

At distinct ordered sites $x_1<\cdots<x_n$, interpolation is the [linear system](../../../linear-algebra.md#system-of-linear-equations)

$$
A_{\mathbf x}c=y,\qquad (A_{\mathbf x})_{ij}=N_j(x_i).
$$

It has a unique solution for every data [vector](../../../vector-space.md#vector) exactly when the [B-spline collocation matrix](../../../uniform-approximation.md#b-spline-collocation-matrix) is invertible. The [Schoenberg–Whitney theorem](../../../uniform-approximation.md#schoenberg-whitney-theorem) characterizes this by $N_i(x_i)>0$ for every $i$; away from clamped endpoints this is $t_i<x_i<t_{i+k}$. At the clamped endpoints the first and last [B-splines](../../../uniform-approximation.md#b-spline) have value one, so the endpoint version uses this positive-value formulation rather than the strict inequalities. Both ordering and the support conditions matter. A [spline](../../../uniform-approximation.md#spline-mathematics) space with interior knots is generally not a [Chebyshev system](../../../uniform-approximation.md#chebyshev-system) on the entire interval: a locally supported [B-spline](../../../uniform-approximation.md#b-spline) vanishes on an interval. Thus arbitrary distinct nodes need not permit interpolation. Merely specifying all data sites as knots also need not fix the remaining freedom; for example, cubic interpolation with simple interior knots at $m-2$ data sites has dimension $m+2$, and two extra boundary conditions are needed to interpolate $m$ values uniquely.

The positivity governing this existence theorem is [total nonnegativity of B-spline collocation matrices](../../../uniform-approximation.md#total-nonnegativity-of-b-spline-collocation-matrices): every square minor with increasing row and column indices is nonnegative. In spline terminology this is often called total positivity, but it permits zero minors caused by disjoint [supports](../../../function.md#support). It is not the stronger assertion that every minor is strictly positive. A useful proof uses [knot insertion](../../../uniform-approximation.md#knot-insertion). Each refinement step changes [coefficients](../../../vector-space.md#coefficient) by

$$
\widetilde c_j=\alpha_jc_j+(1-\alpha_j)c_{j-1},\qquad 0\le\alpha_j\le1,
$$

with the unchanged endpoint pieces. The refinement [matrix](../../../vector-space.md#matrix) is nonnegative bidiagonal, and its minors are nonnegative: any nonzero determinant has its allowed diagonal matching and is a product of nonnegative entries. Products preserve this property by the [Cauchy–Binet formula](../../../linear-algebra.md#cauchy-binet-formula). Insert each sampling site to full multiplicity, so evaluation at that site becomes selection of an ordered refined [coefficient](../../../vector-space.md#coefficient). The collocation [matrix](../../../vector-space.md#matrix) is then an ordered row submatrix of the refinement product, proving total nonnegativity. The strict support criterion is the strict part of this argument: an ordered path through the consecutive support intervals exists exactly when every diagonal [B-spline](../../../uniform-approximation.md#b-spline) value is positive, giving the [Schoenberg–Whitney theorem](../../../uniform-approximation.md#schoenberg-whitney-theorem) determinant criterion.

If $A$ is invertible, its determinant is positive and the [adjugate identity](../../../linear-algebra.md#adjugate-identity) yields

$$
(A^{-1})_{ij}=(-1)^{i+j}\frac{\det A_{\widehat j,\widehat i}}{\det A},\qquad(-1)^{i+j}(A^{-1})_{ij}\ge0.
$$

This [checkerboard inverse of a totally nonnegative matrix](../../../vector-space.md#checkerboard-inverse-of-a-totally-nonnegative-matrix) is the central stability fact. With alternating data $e_i=(-1)^i$, the absolute row sums satisfy

$$
|(A^{-1}e)_j|=\sum_i|(A^{-1})_{ji}|,\qquad\|A^{-1}\|_\infty=\|A^{-1}e\|_\infty.
$$

For general data, the cardinal [splines](../../../uniform-approximation.md#spline-mathematics) are $\ell_i(x)=\sum_jN_j(x)(A^{-1})_{ji}$. The [spline interpolation operator](../../../uniform-approximation.md#spline-interpolation-operator) and its exact [Lebesgue constant of interpolation](../../../uniform-approximation.md#lebesgue-constant-of-interpolation) are

$$
P_{\mathbf x}f=\sum_if(x_i)\ell_i,\qquad\|P_{\mathbf x}\|=\Lambda_{\mathbf x}:=\max_x\sum_i|\ell_i(x)|\le\|A_{\mathbf x}^{-1}\|_\infty.
$$

The equality for the [operator norm](../../../continuous-dual-space.md#operator-norm) follows by extending the signs at distinct sites to a continuous unit-norm data [function](../../../function.md), as in Solution 2. That solution also shows the last inequality can be very strict. Stability concerns the range [function](../../../function.md) as well as its [coefficients](../../../vector-space.md#coefficient).

An optimal interpolation set must be specified relative to an objective. For the normalized [B-spline](../../../uniform-approximation.md#b-spline) [coefficients](../../../vector-space.md#coefficient), every admissible sampling set satisfies

$$
\kappa(\mathcal S)\le\|A_{\mathbf x}^{-1}\|_\infty,
$$

since $c(s)=A_{\mathbf x}^{-1}(s(x_i))$ and sampling cannot increase the [supremum norm](../../../functional-analysis.md#supremum-norm). If a unit-norm [spline](../../../uniform-approximation.md#spline-mathematics) $s_*$ has $n$ ordered alternating extrema $s_*(x_i)=(-1)^i$ at admissible sites, the checkerboard identity gives

$$
|c_j(s_*)|=\sum_i|(A_{\mathbf x}^{-1})_{ji}|.
$$

Taking the largest row shows $\|A_{\mathbf x}^{-1}\|_\infty\le\kappa(\mathcal S)$, so equality holds. This proves the [optimal spline coefficient interpolation sites](../../../uniform-approximation.md#optimal-spline-coefficient-interpolation-sites) property and the [Chebyshev spline coefficient and dual norm equality](../../../uniform-approximation.md#chebyshev-spline-coefficient-and-dual-norm-equality). In particular, for the cubic space of Solution 1 the alternating extrema $-1,-2/3,0,2/3,1$ satisfy the support conditions. Its [coefficients](../../../vector-space.md#coefficient) have maximum magnitude $11/2$, so these sites are optimal for coefficient recovery and

$$
\boxed{\kappa(\mathcal S)=\frac{11}{2}=\|A_{\mathbf x}^{-1}\|_\infty\quad\text{at those five sites}.}
$$

The argument proves optimality whenever this admissible equioscillating [spline](../../../uniform-approximation.md#spline-mathematics) is available; it does not identify extrema of an arbitrary [spline](../../../uniform-approximation.md#spline-mathematics) as optimal sites, or transfer coefficient optimality automatically to the [Lebesgue constant of interpolation](../../../uniform-approximation.md#lebesgue-constant-of-interpolation).

For the intrinsic interpolation objective, minimize $\Lambda_{\mathbf x}$ itself. There is a minimizer for a fixed finite-dimensional continuous [spline](../../../uniform-approximation.md#spline-mathematics) space. Indeed the sites lie in a compact ordered simplex. On admissible sets, inverse entries and hence $\Lambda_{\mathbf x}$ vary continuously. As a collocation [matrix](../../../vector-space.md#matrix) tends to a singular one, its inverse [norm](../../../functional-analysis.md#norm) diverges. The [uniform-norm stability of a B-spline basis](../../../uniform-approximation.md#uniform-norm-stability-of-a-b-spline-basis) gives the complementary bound

$$
\|P_{\mathbf x}\|\ge\frac{\|A_{\mathbf x}^{-1}\|_\infty}{\kappa(\mathcal S)}:
$$

choose sample signs attaining a largest inverse row, extend them to a continuous unit-norm [function](../../../function.md), and use $\|Tc\|_\infty\ge\|c\|_\infty/\kappa(\mathcal S)$. Thus a minimizing sequence with bounded [Lebesgue constants of interpolation](../../../uniform-approximation.md#lebesgue-constant-of-interpolation) cannot approach a singular site set. A convergent subsequence has an admissible limit attaining the minimum.

[Fekete interpolation sites for a continuous function space](../../../uniform-approximation.md#fekete-interpolation-sites-for-a-continuous-function-space) offer another useful, constructive criterion: maximize the absolute evaluation determinant. A nonzero maximum exists by compactness and linear independence. Replacing one row by evaluation at $x$ multiplies the determinant by the corresponding cardinal [function](../../../function.md), so maximality gives $|\ell_i(x)|\le1$, and therefore $\Lambda_{\mathbf x}\le n$. These sites are determinant-optimal, with a proven interpolation bound; one should not claim without further argument that they minimize $\Lambda_{\mathbf x}$. [Greville abscissae](../../../uniform-approximation.md#greville-abscissa) provide inexpensive admissible sites for the usual continuous clamped [spline](../../../uniform-approximation.md#spline-mathematics) spaces of order at least two. Admissibility alone does not give the best stability bound.

Finally, the [coefficient condition number of a normalized B-spline basis](../../../uniform-approximation.md#coefficient-condition-number-of-a-normalized-b-spline-basis) is bounded by a constant depending only on order. To see the mechanism, for each [coefficient](../../../vector-space.md#coefficient) choose a longest nonempty knot cell in that [B-spline](../../../uniform-approximation.md#b-spline)'s support. If its length is $h$ and the support width is $W$, then $W/h\le k$. On that cell the [spline](../../../uniform-approximation.md#spline-mathematics) is a degree-at-most-$k-1$ [polynomial](../../../polynomial.md); repeated [Markov polynomial inequalities](../../../uniform-approximation.md#markov-inequality-for-polynomial-derivatives) bound its $r$th [derivative](../../../calculus.md#derivative) by $C_kh^{-r}\|s\|_\infty$. In the [De Boor–Fix spline coefficient functional](../../../uniform-approximation.md#de-boor-fix-spline-coefficient-functional), the accompanying derivative of the knot [polynomial](../../../polynomial.md) is bounded by $C_kW^r$. Each term is consequently at most $C_k(W/h)^r\|s\|_\infty$, yielding $\|c(s)\|_\infty\le C_k\|s\|_\infty$ independently of the number and spacing of knots. This is basis stability; it does not bound $\|A_{\mathbf x}^{-1}\|$ at arbitrarily poor sampling sites.

For approximation, reproduction gives the [Lebesgue inequality for approximation projectors](../../../uniform-approximation.md#polynomial-reproduction-error-bound)

$$
\|f-P_{\mathbf x}f\|_\infty\le(1+\Lambda_{\mathbf x})\inf_{s\in\mathcal S}\|f-s\|_\infty.
$$

As the maximum knot gap tends to zero with fixed order, [spline quasi-interpolation](../../../uniform-approximation.md#spline-quasi-interpolation) gives an approximant with error at most $\omega(f,kh)$, so the infimum tends to zero. A sequence of uniformly bounded interpolation [linear operators](../../../vector-space.md#linear-operator) therefore converges to every continuous target. Local [support](../../../function.md#support) and a stable choice of sites make [spline interpolation](../../../uniform-approximation.md#spline-interpolation) effective; mesh refinement without control of the interpolation [operator norm](../../../continuous-dual-space.md#operator-norm) is not by itself a convergence proof.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
