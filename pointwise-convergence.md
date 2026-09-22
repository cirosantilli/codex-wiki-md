# Pointwise convergence

↑ **Parent:** [Sequence and series](sequence-and-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pointwise_convergence)

For a [sequence](sequence.md) of [functions](function-split.md) $f_n:X\to\mathbb R$ and a [function](function-split.md) $f:X\to\mathbb R$ on the same [domain of a function](domain-of-a-function.md), [pointwise convergence](pointwise-convergence.md) to $f$ means

$$
\forall x\in X\;\forall\varepsilon>0\;\exists N\in\mathbb N_{>0}\;\forall n\geq N:\quad |f_n(x)-f(x)|<\varepsilon.
$$

At each fixed input, this is the ordinary [limit of a sequence](limit-of-a-sequence.md). The index may depend on both the input and the requested accuracy: $N=N(x,\varepsilon)$. It therefore certifies each input separately, with no promise about the worst error across the [domain of a function](domain-of-a-function.md). This is a useful first way to identify a candidate [pointwise limit](pointwise-limit.md): hold the input still and study a numerical [sequence](sequence.md). See [MIT 18.100A, Lecture 23, definition 7](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/mit18_100af20_lec23.pdf).

Consider the [polynomial functions](polynomial-function.md) $f_n(x)=x^n$, with positive [integer](integer.md) index $n$, on the [interval](interval-mathematics.md) $[0,1]$. For $0\leq x<1$ the [geometric sequence](geometric-progression.md) $(x^n)$ tends to zero, while $f_n(1)=1$. Thus its [pointwise limit](pointwise-limit.md) is

$$
f(x)=\begin{cases}0,&0\leq x<1,\\1,&x=1.\end{cases}
$$

Each $f_n$ is a [continuous function](continuous-function.md), but this [pointwise limit](pointwise-limit.md) fails [continuity](continuous-function.md) at one: its nearby values from the left are zero while its value at one is one. At any fixed $0<x<1$ and $0<\varepsilon<1$, the [logarithm](logarithm.md) gives the sufficient choice $N>\log(\varepsilon)/\log(x)$. For example, at $x=1/2$ and $\varepsilon=0.01$, $N=7$ works because $2^{-7}=0.0078125$, whereas $2^{-6}=0.015625$. As the input approaches one from below, the required index grows without bound. A common tolerance needs increasingly late indices at different inputs.

An even sharper warning concerns [integration](integral.md). On $[0,1]$, define the [continuous functions](continuous-function.md)

$$
g_n(x)=\begin{cases}2n^2x,&0\leq x\leq1/(2n),\\2n-2n^2x,&1/(2n)\leq x\leq1/n,\\0,&1/n\leq x\leq1.\end{cases}
$$

Their [supports](support.md) are $[0,1/n]$, with height $n$ at $1/(2n)$ and value zero at both ends. Every fixed $x>0$ eventually lies beyond the [support](support.md), and $g_n(0)=0$ always, so [pointwise convergence](pointwise-convergence.md) gives the zero [function](function-split.md). Nevertheless, each [integral](integral.md) is the area of a [triangle](triangle.md): $\int_0^1g_n(x)\,dx=\tfrac12(1/n)n=\tfrac12$. Shrinking width exactly compensates increasing height. Hence the [limit](limit-of-a-function.md) of these [integrals](integral.md) differs from the [integral](integral.md) of the [pointwise limit](pointwise-limit.md); interchanging them requires additional conditions, such as [uniform convergence preserves integrals on a compact interval](uniform-convergence-preserves-integrals-on-a-compact-interval.md).

<a id="image-shrinking-continuous-tents-have-pointwise-convergence-to-zero-while-retaining-integral-one-half"></a>
![](convergence-moving-peaks.png)

**[Figure 24](#image-shrinking-continuous-tents-have-pointwise-convergence-to-zero-while-retaining-integral-one-half). Shrinking continuous tents have pointwise convergence to zero while retaining integral one half**.

**Table of contents**

- [Factorial cosine iterated limit detects rationality](factorial-cosine-iterated-limit-detects-rationality.md)
- [Shrinking continuous spikes with vanishing integral](shrinking-continuous-spikes-with-vanishing-integral.md)
- [Pointwise limit](pointwise-limit.md)

## ↑ Ancestors (6)

1. [Sequence and series](sequence-and-series.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (38)

- [Convergence in a product space](convergence-in-a-product-space.md)
- [Fourier series](fourier-series-split.md)
- [Geometric power-series remainder](geometric-power-series-remainder.md)
- [Gibbs phenomenon](gibbs-phenomenon.md)
- [Moving an exterior pole to obtain pointwise polynomial approximation](moving-an-exterior-pole-to-obtain-pointwise-polynomial-approximation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/16e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-1/1e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1/4g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/2g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/3h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/2f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/2f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/2f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-7/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-7/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/2g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/3g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/22f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/2f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/3e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/2h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/2f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3/11f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3/26g/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1/27h/a/solution.md)
- [Pointwise approximation by uniformly continuous functions](pointwise-approximation-by-uniformly-continuous-functions.md)
- [Pointwise closure of the bounded Lipschitz unit ball](pointwise-closure-of-the-bounded-lipschitz-unit-ball.md)
- [Pointwise convergence](pointwise-convergence.md)
- [Pointwise polynomial approximation of a half-plane sign](pointwise-polynomial-approximation-of-a-half-plane-sign.md)
- [Real analysis](real-analysis-split.md)
- [Uniform convergence](uniform-convergence.md)
