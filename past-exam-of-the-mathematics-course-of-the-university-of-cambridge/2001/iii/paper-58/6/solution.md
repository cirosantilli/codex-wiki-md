<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md) asserts that every real [continuous function](../../../../../continuous-function.md) on a [compact](../../../../../compact-space.md) [interval](../../../../../interval-mathematics.md) is a [uniform limit](../../../../../uniform-limit.md) of [polynomials](../../../../../polynomial-split.md). An affine change of variable reduces the interval to $[0,1]$. There are two complementary routes: construct positive approximation operators, or construct an algebra dense enough to approximate absolute values and hence pointwise maxima and minima.

For the first route, the [Korovkin theorem](../../../../../korovkin-theorem.md) reduces convergence of [positive linear operators on continuous functions](../../../../../positive-linear-operator-on-continuous-functions.md) $L_n$ to the three tests $1,t,t^2$. Here is its proof. Given $f\in C[0,1]$ and $\varepsilon>0$, [uniform continuity](../../../../../uniform-continuity.md) supplies a $\delta>0$ such that $|f(t)-f(x)|<\varepsilon$ for $|t-x|<\delta$. For all $t,x$ one then has

$$
|f(t)-f(x)|\le\varepsilon+M(t-x)^2,\qquad M=2\|f\|_\infty/\delta^2.
$$

Apply positivity to the two real inequalities obtained from this bound. At $x$ this gives

$$
|L_nf(x)-f(x)|\le |f(x)|\,|L_n1(x)-1|+\varepsilon L_n1(x)+M\bigl[L_nt^2(x)-2xL_nt(x)+x^2L_n1(x)\bigr].
$$

The expression in brackets is nonnegative and tends uniformly to zero by the three test assumptions. Also $L_n1\to1$ uniformly. Taking the upper limit of the [supremum norm](../../../../../supremum-norm.md) and then letting $\varepsilon\downarrow0$ proves convergence for every $f$. This is the [quadratic barrier estimate for positive approximation operators](../../../../../quadratic-barrier-estimate-for-positive-approximation-operators.md).

The [Bernstein polynomial](../../../../../bernstein-polynomial.md) supplies the constructive corollary

$$
B_nf(x)=\sum_{j=0}^nf(j/n)\binom nj x^j(1-x)^{n-j}.
$$

The [binomial theorem](../../../../../binomial-theorem.md) makes its nonnegative weights sum to one. Differentiating the [binomial theorem](../../../../../binomial-theorem.md), or using the first two [binomial distribution](../../../../../binomial-distribution.md) moments, gives

$$
B_n1=1,\qquad B_nt=x,\qquad B_nt^2=x^2+\frac{x(1-x)}n.
$$

The [Korovkin theorem](../../../../../korovkin-theorem.md) proves $B_nf\to f$ uniformly, and each $B_nf$ is a [polynomial](../../../../../polynomial-split.md), proving the [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md). The same criterion gives the [Schoenberg spline operator](../../../../../schoenberg-spline-operator.md) convergence in Solution 3. For periodic [functions](../../../../../function-split.md) its counterpart uses $1,\cos t,\sin t$: the nonnegative barrier $1-\cos(t-x)$ is bounded away from zero outside any fixed small arc. This [periodic Korovkin test set](../../../../../periodic-korovkin-test-set.md) gives convergence of the normalized [Fejér sums](../../../../../fejer-sum.md) and density of [trigonometric polynomials](../../../../../trigonometric-polynomial.md).

The [Lebesgue convergence criterion for approximation operators](../../../../../extension-of-approximation-operators-from-a-dense-subspace.md) addresses stability. Suppose bounded [linear operators](../../../../../linear-operator.md) $L_n:C[a,b]\to C[a,b]$ converge to the identity on every [polynomial](../../../../../polynomial-split.md). Then they converge on every [continuous function](../../../../../continuous-function.md) if and only if $\sup_n\|L_n\|<\infty$. Sufficiency is the [extension of approximation operators from a dense subspace](../../../../../extension-of-approximation-operators-from-a-dense-subspace.md): for a [polynomial](../../../../../polynomial-split.md) $p$ with $\|f-p\|<\eta$ and a common bound $M$,

$$
\|L_nf-f\|\le(M+1)\eta+\|L_np-p\|.
$$

First let $n\to\infty$, then $\eta\downarrow0$. Necessity follows from the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md), since a convergent $L_nf$ is bounded for every $f$. Applied to approximation [projectors](../../../../../projection-linear-algebra.md), the [Lebesgue inequality for approximation projectors](../../../../../polynomial-reproduction-error-bound.md) is

$$
\|f-P_nf\|_\infty\le(1+\|P_n\|)E_{V_n}(f),\qquad E_{V_n}(f)=\inf_{v\in V_n}\|f-v\|_\infty.
$$

Indeed $P_nv=v$ makes $f-P_nf=(f-v)-P_n(f-v)$; take the infimum. Thus density of the ranges and a uniform bound on the [Lebesgue constants of interpolation](../../../../../lebesgue-constant-of-interpolation.md) imply convergence. Density alone does not control a sequence of interpolation [projectors](../../../../../projection-linear-algebra.md).

There is also a kernel version of this stability criterion, useful for [trigonometric polynomial](../../../../../trigonometric-polynomial.md) approximation. If [integrable](../../../../../integrability.md) periodic kernels $K_n$ have uniformly bounded $L^1$ [norms](../../../../../norm.md), their integrals tend to one, and $\int_{|t|\ge\delta}|K_n(t)|\,dt\to0$ for every $\delta>0$, then convolution with $K_n$ converges uniformly to every [continuous](../../../../../continuous-function.md) periodic [function](../../../../../function-split.md). Subtract $f(x)\int K_n$ and split the error into a small arc, bounded by $\omega(f,\delta)\sup_n\|K_n\|_1$, and its complement, bounded by $2\|f\|_\infty\int_{|t|\ge\delta}|K_n|$. The remaining mass error tends to zero. This [approximate identity](../../../../../approximate-identity.md) argument shows directly why nonnegative unit-mass [Fejér kernels](../../../../../fejer-kernel.md) work even though ordinary [Fourier partial sums](../../../../../fourier-partial-sum.md) need not converge uniformly for every continuous target.

Lebesgue's constructive approach to the [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md) starts instead with the [absolute value](../../../../../absolute-value.md). On $[-1,1]$ define the [polynomial recurrence for the absolute value](../../../../../polynomial-recurrence-for-the-absolute-value.md)

$$
p_0(x)=0,\qquad p_{r+1}(x)=p_r(x)+\frac{x^2-p_r(x)^2}{2}.
$$

Induction gives $0\le p_r(x)\le|x|$, monotonicity, and

$$
|x|-p_{r+1}(x)=(|x|-p_r(x))\left(1-\frac{|x|+p_r(x)}2\right).
$$

The pointwise limit satisfies $p(x)^2=x^2$ and is nonnegative, hence equals $|x|$. [Dini's theorem](../../../../../dini-s-theorem.md) makes the convergence uniform. More explicitly, the continuous decreasing errors have, for any positive tolerance, open sublevel sets covering the [compact](../../../../../compact-space.md) [interval](../../../../../interval-mathematics.md); a finite subcover supplies one index valid everywhere. Every [continuous](../../../../../continuous-function.md) [piecewise linear function](../../../../../piecewise-linear-function.md) has the form

$$
L(x)=a+bx+\sum_{j=1}^mc_j(x-t_j)_+,\qquad (x-t)_+=\frac{x-t+|x-t|}{2}.
$$

The $c_j$ are its changes in slope. Scaling and translating the absolute-value approximation shows that $L$ is uniformly approximable by [polynomials](../../../../../polynomial-split.md). Solution 4, or polygonal interpolation and [uniform continuity](../../../../../uniform-continuity.md), makes these [piecewise linear functions](../../../../../piecewise-linear-function.md) dense in $C[a,b]$. Approximating $f$ first by $L$ and then by a [polynomial](../../../../../polynomial-split.md) is another complete proof of the [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md).

The [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) generalizes from intervals to a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) $K$: a real subalgebra $A\subseteq C(K,\mathbb R)$ containing the constants and separating points is uniformly dense. Its proof uses the same absolute-value mechanism. The [uniform closure of a function algebra](../../../../../uniform-closure-of-a-function-algebra.md) is an algebra. If $a$ belongs to this closure, approximation of $|t|$ by [polynomials](../../../../../polynomial-split.md) on a bounded interval containing its range proves that $|a|$ also belongs to the closure. Therefore the closure contains

$$
\max(a,b)=\frac{a+b+|a-b|}{2},\qquad\min(a,b)=\frac{a+b-|a-b|}{2}.
$$

Point separation and constants allow exact interpolation of any two real values: choose $h\in A$ with $h(s)\ne h(t)$ and solve for $\alpha,\beta$ in $\alpha h+\beta$. The [lattice approximation from two-point approximation](../../../../../lattice-approximation-from-two-point-approximation.md) proved in Solution 4 now makes the closure all of $C(K,\mathbb R)$.

The complex version requires a unital, point-separating subalgebra closed under [complex conjugation](../../../../../complex-conjugation.md). Its real-valued members separate points using real or imaginary parts, so the real result approximates both parts of every complex target. Conjugation closure is essential: [polynomials](../../../../../polynomial-split.md) in $z$ alone on the closed unit disk cannot approximate $\overline z$ uniformly, because $\int_{|z|=1}p(z)\,dz=0$ whereas $\int_{|z|=1}\overline z\,dz=2\pi i$.

Among the corollaries are **density of multivariate polynomials on compact subsets of real Euclidean space**, since coordinates separate points, and **density of trigonometric polynomials on the circle**, since sine and cosine separate points there. On a [compact](../../../../../compact-space.md) [interval](../../../../../interval-mathematics.md), [polynomials](../../../../../polynomial-split.md) with rational [coefficients](../../../../../coefficient.md) are a countable dense family, giving separability of $C[a,b]$. The real and complex approximation results above concern uniform approximation of continuous targets; neither asserts convergence of arbitrary interpolation schemes or arbitrary [Fourier series](../../../../../fourier-series-split.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
