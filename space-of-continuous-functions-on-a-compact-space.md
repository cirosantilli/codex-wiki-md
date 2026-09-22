# Space of continuous functions on a compact space

↑ **Parent:** [Space of continuous functions vanishing at infinity](space-of-continuous-functions-vanishing-at-infinity.md)

For a [compact Hausdorff space](compact-hausdorff-space.md) $K$, $C(K)$ consists of continuous scalar-valued functions with the [supremum norm](supremum-norm.md). It is a [Banach space](banach-space-split.md) and, with complex scalars, pointwise multiplication and conjugation make it a commutative unital [C-star algebra](c-star-algebra.md).

Why does [completeness](completeness.md) hold? A [Cauchy sequence](cauchy-sequence.md) in the [supremum norm](supremum-norm.md) is Cauchy at every point, hence has a pointwise limit. The uniform Cauchy estimate passes to that limit, giving [uniform convergence](uniform-convergence.md); the [uniform limit theorem](uniform-limit-theorem.md) makes the limit continuous. Thus the [norm](norm.md) and the chosen regularity of the functions cooperate to keep every limit inside $C(K)$.

Changing to the [L2 norm](l2-norm.md) on $C([0,1])$ loses this property. For integers $n\geq2$, the [continuous functions](continuous-function.md) $h_n(x)=\min(1,\max(0,n(x-1/2)))$ approximate the [step function](step-function.md) $h(x)=0$ for $x\leq1/2$ and $h(x)=1$ for $x>1/2$. Direct integration gives

$$
\|h_n-h\|_2^2=\int_{1/2}^{1/2+1/n}\bigl(1-n(x-1/2)\bigr)^2\,dx=\frac1{3n}.
$$

The [triangle inequality](triangle-inequality.md) makes $(h_n)$ a [Cauchy sequence](cauchy-sequence.md), but no [continuous function](continuous-function.md) agrees with $h$ [almost everywhere](almost-everywhere.md): continuity would force value zero on the whole left open interval and one on the whole right open interval. Hence this [normed space](normed-vector-space-split.md) is incomplete. The missing limit exists in [L2 space](l2-space-is-a-hilbert-space.md), its [completion of a normed space](completion-of-a-normed-space.md), showing exactly what the larger space adds.

**Table of contents**

- [Planar logarithm factorization](planar-logarithm-factorization.md)
- [Character space of continuous functions on the circle](character-space-of-continuous-functions-on-the-circle.md)
- [Isometric evaluation embedding into continuous functions on a compact dual ball](isometric-evaluation-embedding-into-continuous-functions-on-a-compact-dual-ball.md)
- [Weakly null continuous functions converge in L1](weakly-null-continuous-functions-converge-in-l1.md)
- [Banach–Stone theorem](banach-stone-theorem.md)
  - [Extreme points of the dual unit ball of C(K)](extreme-points-of-the-dual-unit-ball-of-c-k.md)

## ↑ Ancestors (6)

1. [Space of continuous functions vanishing at infinity](space-of-continuous-functions-vanishing-at-infinity.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Discontinuous pointwise limit obstruction to weak compactness](discontinuous-pointwise-limit-obstruction-to-weak-compactness.md)
- [Extreme points of a real continuous-function unit ball](extreme-points-of-a-real-continuous-function-unit-ball.md)
- [Jordan decomposition of a bounded functional on C(K)](jordan-decomposition-of-a-bounded-functional-on-c-k.md)
- [Norm of a positive functional on C(K)](norm-of-a-positive-functional-on-c-k.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-5/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-106/5/solution.md)
