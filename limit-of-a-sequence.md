# Limit of a sequence

↑ **Parent:** [Convergent sequence](convergent-sequence.md)

A [sequence](sequence.md) $(x_n)_{n\geq1}$ of [real numbers](real-number.md) has [limit of a sequence](limit-of-a-sequence.md) $L\in\mathbb R$, written $x_n\to L$, precisely when

$$
\forall\varepsilon>0\;\exists N\in\mathbb N_{>0}\;\forall n\geq N:\quad |x_n-L|<\varepsilon.
$$

The [absolute value](absolute-value.md) measures the error. The tolerance $\varepsilon$ is chosen first; $N$ may depend on it, but must control every later term. Infinitely many accurate terms alone do not suffice. For example, $x_n=(-1)^n$ repeatedly equals one but also repeatedly differs from one by two. The definition and uniqueness of the [limit of a sequence](limit-of-a-sequence.md) are discussed in [MIT 18.100A, Lecture 6, definitions 13 and theorem 15](https://ocw.mit.edu/courses/18-100a-real-analysis-fall-2020/mit18_100af20_lec62.pdf).

For a worked error estimate, let $x_n=3+2/n$. Then $|x_n-3|=2/n$, so any positive integer $N>2/\varepsilon$ works. With $\varepsilon=0.01$, choose $N=201$; every later error is at most $2/201<0.01$. The strict inequality matters: $N=200$ would give equality at its first term. A [limit of a sequence](limit-of-a-sequence.md) turns the informal instruction “take enough terms” into an explicit accuracy guarantee.

The [limit of a sequence](limit-of-a-sequence.md) is unique: two distinct proposed answers cannot both be within arbitrarily small error of every late term, by the [triangle inequality](triangle-inequality.md). Changing finitely many initial terms does not change it. For an [extended real number](extended-real-number-line.md), $x_n\to+\infty$ means $\forall M\in\mathbb R\;\exists N\;\forall n\geq N:\ x_n>M$; convergence to $-\infty$ similarly requires $x_n<M$. These describe escape rather than a finite answer. The [extended-real Fekete lemma](fekete-s-lemma.md) is an example where the [limit of a sequence](limit-of-a-sequence.md) need not be finite.

**Table of contents**

- [Reciprocal limits and escape in absolute value](reciprocal-limits-and-escape-in-absolute-value.md)

## ↑ Ancestors (7)

1. [Convergent sequence](convergent-sequence.md)
2. [Sequence and series](sequence-and-series.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (62)

- [Assumptions of the bounded monotone sequence theorem](assumptions-of-the-bounded-monotone-sequence-theorem.md)
- [Attainment of the limit of a monotone sequence](attainment-of-the-limit-of-a-monotone-sequence.md)
- [Bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md)
- [Bounded monotone sequences have no universal convergence rate](bounded-monotone-sequences-have-no-universal-convergence-rate.md)
- [Cauchy sequence](cauchy-sequence.md)
- [Cesàro sum](cesaro-sum.md)
- [Cesàro summation](cesaro-summation.md)
- [Cesàro theorem for convergent sequences](cesaro-theorem-for-convergent-sequences.md)
- [Closed real interval](closed-real-interval.md)
- [Closed set](closed-set.md)
- [Closure (topology)](closure-topology.md)
- [Compact space](compact-space.md)
- [Completeness of the real numbers](completeness-of-the-real-numbers.md)
- [Connection decay rate in a percolation strip](connection-decay-rate-in-a-percolation-strip.md)
- [Continuity of probability](continuity-of-probability.md)
- [Convergence from fixed-length series blocks](convergence-from-fixed-length-series-blocks.md)
- [Divergent series](divergent-series.md)
- [Error bounds for bounded monotone sequences](error-bounds-for-bounded-monotone-sequences.md)
- [Fekete's lemma](fekete-s-lemma.md)
- [Finite-seed local extinction in the voter model](finite-seed-local-extinction-in-the-voter-model.md)
- [Generalized limit](generalized-limit.md)
- [Geometric series](geometric-series.md)
- [Heine-Borel theorem](heine-borel-theorem.md)
- [Increasing and decreasing approximations to a common limit](increasing-and-decreasing-approximations-to-a-common-limit.md)
- [Infinite-volume wired random-cluster measure](infinite-volume-wired-random-cluster-measure.md)
- [Kolmogorov axioms](kolmogorov-axioms.md)
- [Limit inferior and limit superior](limit-inferior-and-limit-superior.md)
- [Limit of a sequence](limit-of-a-sequence.md)
- [Matrix summability method](matrix-summability-method.md)
- [Partial sum](partial-sum.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/3d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/12c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/3c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/4c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/9c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-1/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/4e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/4e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/1/b/iii/solution.md)
- [Percolation one-arm decay rate](percolation-one-arm-decay-rate.md)
- [Pointwise convergence](pointwise-convergence.md)
- [Random-cluster inverse correlation length](random-cluster-inverse-correlation-length.md)
- [Reciprocal limits and escape in absolute value](reciprocal-limits-and-escape-in-absolute-value.md)
- [Sequence](sequence.md)
- [Series (mathematics)](series-mathematics.md)
- [Tail of a sequence](tail-of-a-sequence.md)
- [Telescoping series](telescoping-series.md)
- [Topological vector space](topological-vector-space-split.md)
- [Topologist's sine curve](topologist-s-sine-curve.md)
- [Uniform convergence](uniform-convergence.md)
- [Uniform spanning tree of a recurrent infinite graph](uniform-spanning-tree-of-a-recurrent-infinite-graph.md)
