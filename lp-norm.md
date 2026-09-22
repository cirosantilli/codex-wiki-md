# Lp norm

↑ **Parent:** [Real analysis](real-analysis-split.md)

An [Lp norm](lp-norm.md) measures the size of a [measurable function](measurable-function.md) by averaging a power of its [absolute value](absolute-value.md) with respect to a specified [measure](measure-split.md). For $1\leq p<\infty$,

$$
\lVert f\rVert_p=\left(\int |f|^p\,d\mu\right)^{1/p},
$$

when the [integral](integral-split.md) is finite. The [exponent](exponent.md) $p$ controls how strongly large values influence the result. The [Lp space](lp-space.md) identifies [functions](function-split.md) equal [almost everywhere](almost-everywhere.md), so this becomes a [norm](norm.md) on the corresponding [equivalence classes](equivalence-class.md). For $p=\infty$, use the [essential supremum](essential-supremum.md) of $|f|$, as defined by the [L-infinity norm](l-infinity-norm.md). [Hunter, Measure Theory, Definitions 7.1 and 7.4: Lp spaces and norms](measure-theory-by-john-k-hunter/lp-spaces-chapter-7-of-measure-theory.md).

For a two-coordinate [vector](vector.md) $(3,4)$, treat the coordinates as a [function](function-split.md) on two inputs with [counting measure](counting-measure.md). Then $\lVert(3,4)\rVert_1=3+4=7$, $\lVert(3,4)\rVert_2=\sqrt{9+16}=5$, and $\lVert(3,4)\rVert_\infty=4$. The middle case is the [Euclidean norm](euclidean-norm.md); the first adds the coordinate magnitudes, and the last takes their largest value. These are different answers to different questions about size, all satisfying the [triangle inequality](triangle-inequality.md).

If instead each input has [probability](probability.md) $1/2$, the same values give $\lVert f\rVert_1=3.5$ and $\lVert f\rVert_2=\sqrt{12.5}$, while $\lVert f\rVert_\infty=4$ remains unchanged. Thus the [measure](measure-split.md) is not an optional label. On a [probability space](probability-space-split.md), the finite [Lp norms](lp-norm.md) are nondecreasing in $p$ whenever they are finite, by [Hölder's inequality](holder-s-inequality.md); the unnormalized two-coordinate example above decreases instead. Statements comparing different [exponents](exponent.md) must specify their [measure](measure-split.md) convention.

Why are these sizes useful? If $e$ is an error [function](function-split.md), its [L1 norm](l1-norm.md) measures aggregate [absolute error](absolute-error.md), its [L2 norm](l2-norm.md) measures the square root of aggregate [quadratic loss](squared-error-loss.md), and its [L-infinity norm](l-infinity-norm.md) bounds error [almost everywhere](almost-everywhere.md). Concentrating a large error on a [set](set-split.md) of small positive [measure](measure-split.md) can give a modest finite [Lp norm](lp-norm.md) but a large [L-infinity norm](l-infinity-norm.md). The three-point example and diagram in [L-infinity norm](l-infinity-norm.md) show this explicitly, including why a [null set](null-set.md) behaves differently from a rare event.

**Table of contents**

- [L-infinity norm](l-infinity-norm.md)
  - [Essentially bounded function](essentially-bounded-function.md)
- [Lq quasi-norm](lq-quasi-norm.md)
- [Minkowski inequality](minkowski-inequality.md)
  - [Minkowski inequality for finite vectors](minkowski-inequality-for-finite-vectors.md)
  - [Equality in Minkowski inequality](equality-in-minkowski-inequality.md)
  - [Minkowski inequality for error aggregation](minkowski-inequality-for-error-aggregation.md)
  - [Failure of Minkowski inequality below exponent one](failure-of-minkowski-inequality-below-exponent-one.md)
- [L2 norm](l2-norm.md)
- [Marcinkiewicz–Zygmund inequality](marcinkiewicz-zygmund-inequality.md)
- [Hölder's inequality](holder-s-inequality.md)
  - [Conjugate exponent](conjugate-exponent.md)
  - [Finite-vector example of Hölder's inequality](finite-vector-example-of-holder-s-inequality.md)
  - [Equality in Hölder's inequality](equality-in-holder-s-inequality.md)
  - [Probabilistic use of Hölder's inequality](probabilistic-use-of-holder-s-inequality.md)
  - [History of Hölder's inequality](history-of-holder-s-inequality.md)

## ↑ Ancestors (5)

1. [Real analysis](real-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (44)

- [Completeness of Lp spaces](completeness-of-lp-spaces.md)
- [Derivative supremum norm](derivative-supremum-norm.md)
- [Dual norm](dual-norm.md)
- [Dyadic increment chaining](dyadic-increment-chaining.md)
- [Equality in Minkowski inequality](equality-in-minkowski-inequality.md)
- [Essential range](essential-range.md)
- [Exponent](exponent.md)
- [Finite-vector example of Hölder's inequality](finite-vector-example-of-holder-s-inequality.md)
- [Fourier extension operator](fourier-extension-operator.md)
- [Free transport equation](free-transport-equation.md)
- [Hardy's integral inequality](hardy-s-integral-inequality.md)
- [Hölder's inequality](holder-s-inequality.md)
- [L-infinity norm](l-infinity-norm.md)
- [Ladyzhenskaya's inequality](ladyzhenskaya-s-inequality.md)
- [Littlewood interpolation inequality](littlewood-interpolation-inequality.md)
- [Local boundedness of weak elliptic subsolutions](local-boundedness-of-weak-elliptic-subsolutions.md)
- [Lp conservation for incompressible transport](lp-conservation-for-incompressible-transport.md)
- [Lp martingale convergence theorem](lp-martingale-convergence-theorem.md)
- [Lp norm](lp-norm.md)
- [Lyapunov moment inequality](lyapunov-moment-inequality.md)
- [Minkowski inequality](minkowski-inequality.md)
- [Minkowski inequality for error aggregation](minkowski-inequality-for-error-aggregation.md)
- [Minkowski inequality for finite vectors](minkowski-inequality-for-finite-vectors.md)
- [Mixed Lebesgue norm](mixed-lebesgue-norm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34/3/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/24j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3/3e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-76/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/23j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-10/2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-12/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-129/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/23f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-129/3/ii/solution.md)
- [Proof outline of Hardy's integral inequality](proof-outline-of-hardy-s-integral-inequality.md)
- [Sharp comparison of l1 and l2 norms](sharp-comparison-of-l1-and-l2-norms.md)
- [Translation of a function](translation-of-a-function.md)
