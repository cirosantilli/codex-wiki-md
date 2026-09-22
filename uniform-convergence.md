# Uniform convergence

↑ **Parent:** [Sequence and series](sequence-and-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_convergence)

A [sequence](sequence.md) of [functions](function-split.md) $f_n:X\to Y$ [converges uniformly](uniform-convergence.md) to $f:X\to Y$, where $Y$ is a [metric space](metric-space.md) with [metric](metric.md) $d$, precisely when

$$
\forall\varepsilon>0\;\exists N\in\mathbb N_{>0}\;\forall x\in X\;\forall n\geq N:\quad d(f_n(x),f(x))<\varepsilon.
$$

For [real numbers](real-number.md), use $d(u,v)=|u-v|$, the [absolute value](absolute-value.md) of the difference. The [universal quantification](universal-quantification.md) over inputs and [existential quantification](existential-quantification.md) of the index change order: [pointwise convergence](pointwise-convergence.md) allows $\forall x\,\forall\varepsilon>0\,\exists N(x,\varepsilon)$, whereas [uniform convergence](uniform-convergence.md) requires $\forall\varepsilon>0\,\exists N(\varepsilon)\,\forall x$. Every later approximation must meet the same prescribed accuracy everywhere. This is valuable when the input is unknown beforehand or changes with the approximation index. [Uniform convergence](uniform-convergence.md) implies [pointwise convergence](pointwise-convergence.md); the converse fails. [Jiří Lebl, Basic Analysis I, section 6.1, pointwise and uniform convergence](https://www.jirka.org/ra/html/sec_puconv.html).

For [functions](function-split.md) taking values in [real numbers](real-number.md) on a nonempty [domain of a function](domain-of-a-function.md), the [supremum error](supremum-error.md) is $E_n=\sup_{x\in X}|f_n(x)-f(x)|$, allowing $+\infty$. Then [uniform convergence](uniform-convergence.md) is equivalent to $E_n\to0$, using the [supremum norm](supremum-norm.md) when the difference is a [bounded function](bounded-function.md). A [supremum](supremum.md) need not be attained, so bounds $|f_n(x)-f(x)|<\varepsilon$ at every input give $E_n\leq\varepsilon$; applying them with $\varepsilon/2$ gives the strict bound needed for the [limit of a sequence](limit-of-a-sequence.md).

For an easy [uniform convergence](uniform-convergence.md) example, let $h_n(x)=x/(n+1)$ on the [interval](interval-mathematics.md) $[0,1]$, for [integers](integer.md) $n\geq1$. Its [uniform limit](uniform-limit.md) is zero and its [supremum error](supremum-error.md) is exactly $1/(n+1)$, attained at $x=1$. For every $\varepsilon>0$, the explicit choice $N=\max\{1,\lceil1/\varepsilon\rceil\}$ works, where the [ceiling function](ceiling-function.md) rounds upward: if $n\geq N$ then $1/(n+1)<\varepsilon$. For $\varepsilon=0.01$, choose $N=100$, giving $E_n\leq1/101\approx0.00990099$. This provides a finite stopping rule before the input is known.

For $f_n(x)=x^n$ and its [pointwise limit](pointwise-limit.md) on $[0,1]$, the error is zero at one but approaches one as $x\to1$ from below. Consequently

$$
\sup_{x\in[0,1]}|f_n(x)-f(x)|=1
$$

for every positive [integer](integer.md) $n$. This [supremum](supremum.md) is not attained: at $x<1$ the error is $x^n<1$, and at $x=1$ it is zero. Even deleting the endpoint leaves [supremum error](supremum-error.md) one on $[0,1)$. The [supremum error](supremum-error.md) persists although every fixed input eventually becomes accurate. Indeed, $x_n=2^{-1/n}<1$ gives error exactly $1/2$ at every index. On the smaller [interval](interval-mathematics.md) $[0,a]$, for any fixed $0\leq a<1$,

$$
\sup_{x\in[0,a]}|f_n(x)|=a^n\longrightarrow0.
$$

For $a=0.8$ and $n=20$, the exact bound is $0.8^{20}=0.01152921504606846976$. A tolerance of $0.01$ needs $n\geq21$, since $0.8^{21}=0.009223372036854775808$. Taking the [logarithm](logarithm.md) gives $n>\log(0.01)/\log(0.8)\approx20.6377$; the [ceiling function](ceiling-function.md) gives $21$ here because the ratio is not an [integer](integer.md). If the ratio were an [integer](integer.md), the strict tolerance would require the next [integer](integer.md). The [domain of a function](domain-of-a-function.md) determines whether this approximation gives a common accuracy guarantee. [MIT 18.100A, Lecture 24, theorem 1](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/mit18_100af20_lec242.pdf).

<a id="image-pointwise-convergence-and-uniform-convergence-compared-through-supremum-error"></a>
![](pointwise-versus-uniform-convergence.png)

**[Figure 29](#image-pointwise-convergence-and-uniform-convergence-compared-through-supremum-error). Pointwise convergence and uniform convergence compared through supremum error**. Left: the [polynomial functions](polynomial-function.md) $x^n$ approach a [pointwise limit](pointwise-limit.md) with an open endpoint at $(1,0)$ and a filled point at $(1,1)$. Right: their [supremum error](supremum-error.md) stays at one on the [interval](interval-mathematics.md) $[0,1]$ but tends to zero on the [interval](interval-mathematics.md) $[0,0.8]$; the [functions](function-split.md) $x/(n+1)$ also have vanishing [supremum error](supremum-error.md) on the [interval](interval-mathematics.md) $[0,1]$.

The [uniform limit theorem](uniform-limit-theorem.md) explains why [uniform convergence](uniform-convergence.md) of [continuous functions](continuous-function.md) preserves [continuity](continuous-function.md). Its proof is short: fix $x$ and $\varepsilon>0$, choose one $f_N$ with [supremum error](supremum-error.md) below $\varepsilon/3$, and use its [continuity](continuous-function.md) to make $|f_N(y)-f_N(x)|<\varepsilon/3$ for $y$ close enough to $x$. The [triangle inequality](triangle-inequality.md) then gives $|f(y)-f(x)|<\varepsilon$. The same $f_N$ must control both inputs. No [compactness](compact-space.md) assumption is needed. [MIT 18.100A, Lecture 25, theorem 2 and its proof](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/mit18_100af20_lec25.pdf).

On a fixed finite [interval](interval-mathematics.md) $[a,b]$, [uniform convergence preserves integrals on a compact interval](uniform-convergence-preserves-integrals-on-a-compact-interval.md): if each $f_n$ is [Riemann integrable](riemann-integrable-function.md), so is $f$, and $|\int_a^b f_n-\int_a^b f|\leq(b-a)E_n\to0$. For $h_n(x)=x/(n+1)$ on the [interval](interval-mathematics.md) $[0,1]$, the [integral](integral.md) is $1/[2(n+1)]\to0$, agreeing with the [integral](integral.md) of its zero [uniform limit](uniform-limit.md). [Jiří Lebl, Basic Analysis I, theorem 6.2.4](https://www.jirka.org/ra/html/sec_liminter.html).

However, [uniform convergence](uniform-convergence.md) of [functions](function-split.md) does not imply convergence of their [derivatives](derivative.md). On the [interval](interval-mathematics.md) $[0,\pi]$, take $q_n(x)=\sin(nx)/n$, using the [sine](sine.md) [function](function-split.md). Its [supremum error](supremum-error.md) from zero is $1/n\to0$, attained at $x=\pi/(2n)$. But its [derivative](derivative.md) is $q_n'(x)=\cos(nx)$, using the [cosine](cosine.md) [function](function-split.md), and $q_n'(\pi)=(-1)^n$ alternates between one and minus one. Thus the [derivatives](derivative.md) fail even [pointwise convergence](pointwise-convergence.md), despite [uniform convergence](uniform-convergence.md) of the original [functions](function-split.md). Here the [derivatives](derivative.md) mean those of the same formulas defined on the [real line](real-line.md) and then restricted to the [interval](interval-mathematics.md) $[0,\pi]$. To exchange [differentiation](differentiation.md) and a [limit of a sequence](limit-of-a-sequence.md), additional control such as [uniform derivative convergence with an anchored value](uniform-derivative-convergence-with-an-anchored-value.md) is needed. [Jiří Lebl, Basic Analysis I, section 6.2.3 and theorem 6.2.10](https://www.jirka.org/ra/html/sec_liminter.html).

<a id="image-uniform-convergence-of-functions-does-not-force-convergence-of-derivatives"></a>
![](uniform-convergence-with-oscillating-derivatives.png)

**[Figure 30](#image-uniform-convergence-of-functions-does-not-force-convergence-of-derivatives). Uniform convergence of functions does not force convergence of derivatives**. On the [interval](interval-mathematics.md) $[0,\pi]$, the [functions](function-split.md) $\sin(nx)/n$ have [supremum error](supremum-error.md) $1/n$ from zero. Their [derivatives](derivative.md) $\cos(nx)$ keep oscillating with size one; at $\pi$, even [integer](integer.md) indices give one and odd [integer](integer.md) indices give minus one.

**Table of contents**

- [Supremum error](supremum-error.md)
- [Uniformly vanishing functions can retain a nonzero integral](uniformly-vanishing-functions-can-retain-a-nonzero-integral.md)
- [Uniform convergence preserves integrals on a compact interval](uniform-convergence-preserves-integrals-on-a-compact-interval.md)
- [Uniform convergence at moving evaluation points](uniform-convergence-at-moving-evaluation-points.md)
- [Uniform derivative convergence with an anchored value](uniform-derivative-convergence-with-an-anchored-value.md)
- [Egorov's theorem](egorov-s-theorem.md)
- [Uniform limit theorem](uniform-limit-theorem.md)
- [Dini's theorem](dini-s-theorem.md)
- [Uniformly Cauchy sequence](uniformly-cauchy-sequence.md)
- [Locally uniform convergence](locally-uniform-convergence.md)
  - [Compact-open topology](compact-open-topology.md)
    - [Weighted metric for local uniform convergence](weighted-metric-for-local-uniform-convergence.md)
  - [Local uniform convergence on compact subsets](local-uniform-convergence-on-compact-subsets.md)

## ↑ Ancestors (6)

1. [Sequence and series](sequence-and-series.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (149)

- [Area theorem (conformal mapping)](area-theorem-conformal-mapping.md)
- [Bernstein monomial recurrence](bernstein-monomial-recurrence.md)
- [Bernstein polynomial](bernstein-polynomial.md)
- [Compact Korovkin test space](compact-korovkin-test-space.md)
- [Compactness of normalized weak elliptic solutions](compactness-of-normalized-weak-elliptic-solutions.md)
- [Continuous functions on the p-adic integers](continuous-functions-on-the-p-adic-integers.md)
- [Derivative seminorms on a compact interval](derivative-seminorms-on-a-compact-interval.md)
- [Dirichlet test](dirichlet-test.md)
- [Egorov's theorem](egorov-s-theorem.md)
- [Fejér first-moment approximation bound](fejer-first-moment-approximation-bound.md)
- [Geometric power-series remainder](geometric-power-series-remainder.md)
- [Gibbs phenomenon](gibbs-phenomenon.md)
- [Kolmogorov-Arnold representation theorem](kolmogorov-arnold-representation-theorem.md)
- [Local-support error bound for a Schoenberg spline operator](local-support-error-bound-for-a-schoenberg-spline-operator.md)
- [Local uniform Cauchy control for pointwise convergent continuous functions](local-uniform-cauchy-control-for-pointwise-convergent-continuous-functions.md)
- [Moving an exterior pole to obtain pointwise polynomial approximation](moving-an-exterior-pole-to-obtain-pointwise-polynomial-approximation.md)
- [Multiplication semigroup](multiplication-semigroup.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/10a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4/10a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-1/1e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-61/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4/4e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-11/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-11/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-69/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1/4g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-9/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/11b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-30/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-86/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/3f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/3f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/11g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-28/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-28/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-67/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-67/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-7/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-7/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-9/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-9/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-2/13h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/13h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/3h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/3h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/23f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/2f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-19/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-29/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-32/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-2/13f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-2/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/16a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/5a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-9/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4/3e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/2f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-28/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-7/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/2f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/2f/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-5/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/11e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/2f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/11d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4/12f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-60/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-61/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-8/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/19g/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/30e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-7/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-70/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/2g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/2g/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/5a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-107/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/7d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/11g/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/3g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/3g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/22f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/2f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/2f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-107/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-136/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/12f/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/3e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/2h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3/21h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/10g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/2g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/2f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/2f/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3/11f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-2/12/12-1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-1/10g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-1/10g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-1/10g/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2/2i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3/28l/c/solution.md)
- [Periodic Korovkin test set](periodic-korovkin-test-set.md)
- [Periodization of a Schwartz function](periodization-of-a-schwartz-function.md)
- [Picard iteration](picard-iteration.md)
- [Pointwise limit](pointwise-limit.md)
- [Polynomial recurrence for the absolute value](polynomial-recurrence-for-the-absolute-value.md)
- [Real analysis](real-analysis-split.md)
- [Residue](residue.md)
- [Shrinking continuous spikes with vanishing integral](shrinking-continuous-spikes-with-vanishing-integral.md)
- [Smooth convergence on a compact interval](smooth-convergence-on-a-compact-interval.md)
- [Space of continuous functions on a compact space](space-of-continuous-functions-on-a-compact-space.md)
- [Spectral-radius maximum principle](spectral-radius-maximum-principle.md)
- [Summable absolute-value cusp series](summable-absolute-value-cusp-series.md)
- [Supremum error](supremum-error.md)
- [Termwise differentiation of a power series](termwise-differentiation-of-a-power-series.md)
- [Test-function inductive limit topology](test-function-inductive-limit-topology.md)
- [Uniform approximation](uniform-approximation-split.md)
- [Uniform convergence](uniform-convergence.md)
- [Uniform convergence preserves integrals on a compact interval](uniform-convergence-preserves-integrals-on-a-compact-interval.md)
- [Uniform derivative convergence with an anchored value](uniform-derivative-convergence-with-an-anchored-value.md)
- [Uniform half-line Schrodinger representation by boundary lifting](uniform-half-line-schrodinger-representation-by-boundary-lifting.md)
- [Uniform metric](uniform-metric.md)
- [Uniform Poisson summability of continuous circle functions](uniform-poisson-summability-of-continuous-circle-functions.md)
- [Uniformly vanishing functions can retain a nonzero integral](uniformly-vanishing-functions-can-retain-a-nonzero-integral.md)
- [Weierstrass approximation does not preserve derivatives](weierstrass-approximation-does-not-preserve-derivatives.md)
