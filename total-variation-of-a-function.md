# Total variation of a function

↑ **Parent:** [Riemann integration](riemann-integration.md)

The total variation of a [function](function-split.md) $f:[a,b]\to\mathbb R$ measures its accumulated rises and falls, rather than just its change between the endpoints. For each [partition of an interval](partition-of-an-interval.md) $\Pi=(a=t_0<\cdots<t_n=b)$, add the [absolute values](absolute-value.md) of its sampled increments. Then take the [supremum](supremum.md) over all such [partitions of an interval](partition-of-an-interval.md):

$$
S_\Pi(f)=\sum_{k=1}^n|f(t_k)-f(t_{k-1})|,\qquad
V_a^b(f)=\sup_\Pi S_\Pi(f).
$$

The [function](function-split.md) has bounded variation when $V_a^b(f)<\infty$. This definition uses its value at every point of the [interval](interval-mathematics.md), including both endpoints.[§3.5.1, Definition 1, printed pp. 1–2: partition definition and pointwise convention](real-analysis-lecture-notes-3-5-functions-of-bounded-variation-by-christopher-e-heil.md)

For a [nondecreasing function](nondecreasing-function.md), all increments are nonnegative and the sum telescopes to $f(b)-f(a)$. More generally, the [triangle inequality](triangle-inequality.md) gives $|f(b)-f(a)|\leq V_a^b(f)$. Equality can fail dramatically when the [function](function-split.md) changes direction: an object can travel a long distance and finish near its starting position. Here we measure movement of the function's value; [arc length](arc-length.md) of its [function graph](graph-of-a-function.md) also includes horizontal movement.

**Table of contents**

- [Partition example of total variation](partition-example-of-total-variation.md)
- [Uniformly small functions with nonvanishing total variation](uniformly-small-functions-with-nonvanishing-total-variation.md)
- [Integration error controlled by total variation](integration-error-controlled-by-total-variation.md)
- [History of total variation of a function](history-of-total-variation-of-a-function.md)
- [p-variation of a path](p-variation-of-a-path.md)
- [Dyadic approximation of total variation](dyadic-approximation-of-total-variation.md)
- [Weak convergence of bounded-variation integrators](weak-convergence-of-bounded-variation-integrators.md)
- [Jordan decomposition of a function of bounded variation](jordan-decomposition-of-a-function-of-bounded-variation.md)

## ↑ Ancestors (6)

1. [Riemann integration](riemann-integration.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Dyadic approximation of total variation](dyadic-approximation-of-total-variation.md)
- [Finite-variation process](finite-variation-process.md)
- [Haar approximation error for a function of bounded variation](haar-approximation-error-for-a-function-of-bounded-variation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-33/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-202/3/b/solution.md)
- [Stieltjes bilinear functional under a variation constraint](stieltjes-bilinear-functional-under-a-variation-constraint.md)
- [Weak convergence of bounded-variation integrators](weak-convergence-of-bounded-variation-integrators.md)
