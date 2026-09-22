# Dirac measure

↑ **Parent:** [Measure](measure-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac_measure)

On a [measurable space](measurable-space.md) $(X,\mathcal F)$, the [Dirac measure](dirac-measure.md) at $x\in X$ assigns unit mass according to whether a [measurable set](measurable-set.md) contains that point:

$$
\delta_x(A)=\mathbf1_A(x)=\begin{cases}1,&x\in A,\\0,&x\notin A,\end{cases}\qquad A\in\mathcal F.
$$

Here $\mathbf1_A$ is the [indicator function](indicator-function.md). This is a [probability measure](probability-measure.md), since $\delta_x(X)=1$. For pairwise disjoint [measurable sets](measurable-set.md) $A_n$, at most one contains $x$, so $\delta_x(\bigcup_nA_n)=\sum_n\delta_x(A_n)$: [countable additivity](countable-additivity.md) reduces to a membership test. The definition works even when the [singleton](singleton-mathematics.md) $\{x\}$ is not a [measurable set](measurable-set.md). [Terence Tao, 245B notes 0, Example 7: Dirac measures](https://terrytao.wordpress.com/2009/01/01/245b-notes-0-a-quick-review-of-measure-and-integration-theory/)

To assert that its [support of a measure](support-of-a-measure.md) is exactly $\{x\}$, assume that $X$ is a [metric space](metric-space.md) and $\mathcal F$ is its [Borel sigma-algebra](borel-sigma-algebra.md). The [singleton](singleton-mathematics.md) $\{x\}$ is then a [closed set](closed-set.md) and a [Borel set](borel-set.md), with $\delta_x(\{x\})=1$. Every open [neighbourhood](neighbourhood-mathematics.md) of $x$ has mass one; every other point $y$ has an open [ball](ball-mathematics.md) of radius less than its distance from $x$, with mass zero. Thus $\operatorname{supp}\delta_x=\{x\}$. An abstract [measurable space](measurable-space.md) has no specified [topology](topology-split.md), so this topological conclusion is not part of the bare definition. Indeed, on the [sigma-algebra](sigma-algebra.md) $\{\varnothing,X\}$, all [Dirac measures](dirac-measure.md) coincide: the available [measurable sets](measurable-set.md) cannot distinguish points.

The [Lebesgue integral](lebesgue-integral.md) against a [Dirac measure](dirac-measure.md) is evaluation:

$$
\int_X f\,d\delta_x=f(x).
$$

This holds for every nonnegative [measurable function](measurable-function.md), allowing an infinite value, and for real or complex [measurable functions](measurable-function.md) satisfying $|f(x)|<\infty$, which are precisely the [integrable functions](lebesgue-integrable-function.md) for $\delta_x$. For a nonnegative [simple function](simple-function.md), only the cell containing $x$ contributes to its [integral](integral-split.md); increasing [simple functions](simple-function.md) and the [monotone convergence theorem](monotone-convergence-theorem.md) extend the identity. Splitting into positive and negative parts, and then real and imaginary parts, gives the remaining cases. This is why a [Dirac measure](dirac-measure.md) turns [integration](integral-split.md) into a point query.

For a [measurable function](measurable-function.md) $T:(X,\mathcal F)\to(Y,\mathcal G)$, its [pushforward measure](pushforward-measure.md) satisfies

$$
(T_*\delta_x)(B)=\delta_x(T^{-1}(B))=\mathbf1_B(T(x)),\qquad T_*\delta_x=\delta_{T(x)}.
$$

Consequently $\int_Y g\,d(T_*\delta_x)=g(T(x))$ for nonnegative or integrable [measurable functions](measurable-function.md) $g$. For example, on the [real numbers](real-number.md) with their [Borel sigma-algebra](borel-sigma-algebra.md), $T(t)=2t+1$ sends $\delta_1$ to $\delta_3$, so integrating $g(y)=y^2$ against that [pushforward measure](pushforward-measure.md) gives $9$. [Terence Tao, 245B notes 0, Example 10 and Theorem 2(8): pushforward and change of variables](https://terrytao.wordpress.com/2009/01/01/245b-notes-0-a-quick-review-of-measure-and-integration-theory/)

Finite weighted sums of [Dirac measures](dirac-measure.md) give useful [measures](measure-split.md) with finitely many point masses. For finite nonnegative weights $w_j$,

$$
\mu=\sum_{j=1}^m w_j\delta_{x_j},\qquad\mu(A)=\sum_{j=1}^m w_j\mathbf1_A(x_j),\qquad\int f\,d\mu=\sum_{j=1}^m w_jf(x_j)
$$

for nonnegative [measurable functions](measurable-function.md) $f$, or whenever $\sum_jw_j|f(x_j)|<\infty$, with zero-weight terms omitted. Repeated locations have their weights added. On the [real numbers](real-number.md), this is the finite version of the [measure](measure-split.md) underlying the [left-continuous cumulative function of an atomic measure](left-continuous-cumulative-function-of-an-atomic-measure.md); a positive-weight [singleton](singleton-mathematics.md) is an [atom of a measure](atom-measure-theory.md). Unit weights at the distinct points of a [finite set](finite-set.md) recover [counting measure](counting-measure.md) on that [set](set-split.md). [Terence Tao, 245A notes 3, Exercises 21 and 25: representation by weighted Dirac measures](https://terrytao.wordpress.com/2010/09/25/245a-notes-3-integration-on-abstract-measure-spaces-and-the-convergence-theorems/)

The same [function](function-split.md) can have sharply different [integrals](integral-split.md) for different [measures](measure-split.md). On $[0,2]$ with its [Borel sigma-algebra](borel-sigma-algebra.md), define

$$
f(t)=\begin{cases}5,&t=1,\\t+1,&t\ne1.\end{cases}\qquad\int_{[0,2]}f\,d\delta_1=5,\qquad\int_{[0,2]}f\,d\lambda=4,\qquad\int_{[0,2]}f\,d\#=\infty.
$$

Here $\lambda$ is [Lebesgue measure](lebesgue-measure.md) and $\#$ is [counting measure](counting-measure.md). The [singleton](singleton-mathematics.md) $\{1\}$ is a [Lebesgue null set](lebesgue-null-set.md), so its changed value leaves the [Lebesgue integral](lebesgue-integral.md) equal to $\int_0^2(t+1)\,dt=4$. For [counting measure](counting-measure.md) on the whole [interval](interval-mathematics.md), $f\geq1$ on an [infinite set](infinite-set.md), forcing an infinite [integral](integral-split.md). On the smaller [measure space](measure-space.md) $D=\{0,1,2\}$ with its [power set](power-set.md) and [counting measure](counting-measure.md), the restricted [function](function-split.md) instead has [integral](integral-split.md) $1+5+3=9$.

<a id="image-an-isolated-value-contributes-differently-to-dirac-measure-counting-measure-and-lebesgue-measure"></a>
![](counting-dirac-measures-evaluation-and-integration.png)

**[Figure 1](#image-an-isolated-value-contributes-differently-to-dirac-measure-counting-measure-and-lebesgue-measure). An isolated value contributes differently to Dirac measure, counting measure, and Lebesgue measure**. Original analytical illustration of the specified [function](function-split.md), with an open circle at the excluded value $2$ and a filled point at the actual value $f(1)=5$. The finite sum uses $D=\{0,1,2\}$; the other three [integrals](integral-split.md) use the same ambient [interval](interval-mathematics.md) $[0,2]$. The drawn area is the [Lebesgue integral](lebesgue-integral.md), and no density curve is assigned to the [Dirac measure](dirac-measure.md).

This also explains the [almost everywhere](almost-everywhere.md) convention in [Lp spaces](lp-space.md): equality [almost everywhere](almost-everywhere.md) for $\delta_x$ requires equality at $x$, whereas equality [almost everywhere](almost-everywhere.md) for [Lebesgue measure](lebesgue-measure.md) allows different values at that [singleton](singleton-mathematics.md). A point value therefore cannot be read unambiguously from an equivalence class in an [Lp space](lp-space.md) formed using [Lebesgue measure](lebesgue-measure.md).

On the [real numbers](real-number.md), a [Dirac measure](dirac-measure.md) gives the [Dirac delta distribution](dirac-delta-function.md) by $\langle\delta_x,\varphi\rangle=\int\varphi\,d\delta_x=\varphi(x)$ for every [test function](test-function.md). The name [Dirac delta function](dirac-delta-function.md) does not mean an ordinary [function](function-split.md) that is zero away from $x$ and infinitely high at $x$. Such a nonnegative [measurable function](measurable-function.md) still has [Lebesgue integral](lebesgue-integral.md) zero, because its nonzero values occur on a [Lebesgue null set](lebesgue-null-set.md). More generally, no nonnegative density $h$ with respect to [Lebesgue measure](lebesgue-measure.md) can represent $\delta_x$: it would give $\delta_x(\{x\})=\int_{\{x\}}h\,d\lambda=0$, contradicting unit mass. The [measure](measure-split.md) and its associated [distribution](distribution-mathematical-analysis.md) act on different kinds of inputs, namely [measurable sets](measurable-set.md) and [test functions](test-function.md), but express the same point evaluation. [Terence Tao, 245C notes 3: Radon measures, test functions, and the Dirac delta distribution](https://terrytao.wordpress.com/2009/04/19/245c-notes-3-distributions/)

## ↑ Ancestors (7)

1. [Measure](measure-split.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (34)

- [Bootstrapping (statistics)](bootstrapping-statistics.md)
- [Conditioning and differential entropy](conditioning-and-differential-entropy.md)
- [Counting measure](counting-measure.md)
- [Cure model](cure-model.md)
- [Dirac measure](dirac-measure.md)
- [Essential infimum and essential supremum](essential-infimum-and-essential-supremum.md)
- [Essential supremum](essential-supremum.md)
- [Existence of a Poisson random measure on a standard Borel space](existence-of-a-poisson-random-measure-on-a-standard-borel-space.md)
- [Expected utility representation on a finite measurable space](expected-utility-representation-on-a-finite-measurable-space.md)
- [Extreme points of the dual unit ball of C(K)](extreme-points-of-the-dual-unit-ball-of-c-k.md)
- [Gaussian random variable](gaussian-random-variable.md)
- [Influence function](influence-function.md)
- [Intensity measure of a point process](intensity-measure-of-a-point-process.md)
- [Invariant measures of the two-dimensional voter model](invariant-measures-of-the-two-dimensional-voter-model.md)
- [Large Fourier coefficient criterion for pretentiousness](large-fourier-coefficient-criterion-for-pretentiousness.md)
- [Measure](measure-split.md)
- [Mixture distribution](mixture-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-30/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-44/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/30b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-44/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/5/d/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/26k/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-108/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-348/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-348/1/c/solution.md)
- [Point process](point-process.md)
- [Simple locally finite point measure](simple-locally-finite-point-measure.md)
- [Support of a measure](support-of-a-measure.md)
