# Minkowski inequality for error aggregation

↑ **Parent:** [Minkowski inequality](minkowski-inequality.md)

Suppose an approximation $a$ is compared with a target $f$ through an intermediate approximation $b$, with both error [functions](function-split.md) in the same [Lp space](lp-space.md). The identity $f-a=(f-b)+(b-a)$ and the [Minkowski inequality](minkowski-inequality.md) combine two error budgets without any [independence](independent-random-variables.md) assumption. The [L1 norm](l1-norm.md) controls aggregate [absolute error](absolute-error.md), the [L2 norm](l2-norm.md) controls the square root of aggregate [quadratic loss](squared-error-loss.md), and the [L-infinity norm](l-infinity-norm.md) controls the largest error [almost everywhere](almost-everywhere.md). For equally weighted samples with the [probability measure](probability-measure.md) $1/n$ on each coordinate, the [L2 norm](l2-norm.md) is the [root mean square](root-mean-square.md) error; the inequality still applies when this normalization is used consistently.

For example, two signed error [vectors](vector.md) $e=(3,0)$ and $r=(0,4)$ have [Euclidean norms](euclidean-norm.md) $3$ and $4$, while $\lVert e+r\rVert_2=5\leq7$. Reinforcing errors $e=(3,0)$ and $r=(4,0)$ attain the bound $7$; opposing errors $e=(3,0)$ and $r=(-3,0)$ cancel completely. The [Minkowski inequality](minkowski-inequality.md) always allows reinforcement. A smaller combined budget requires additional information about the errors, not just their separate [norms](norm.md).

Iteration gives $\lVert\sum_{k=1}^N e_k\rVert_p\leq\sum_{k=1}^N\lVert e_k\rVert_p$ for every finite sum. For an infinite [series](series-mathematics.md), if all $e_k$ belong to one fixed [Lp space](lp-space.md) with $1\leq p\leq\infty$ and $\sum_{k=1}^\infty\lVert e_k\rVert_p<\infty$, its [partial sums](partial-sum.md) form a [Cauchy sequence](cauchy-sequence.md) in the full [Lp norm](lp-norm.md). [Completeness](completeness.md) of this [Banach space](banach-space-split.md) then gives [norm convergence](norm-convergence.md) to an element of the same [Lp space](lp-space.md). A finite sum bound alone does not establish convergence, and [completeness](completeness.md) is an additional ingredient beyond the [Minkowski inequality](minkowski-inequality.md). [Hunter, Measure Theory, §7.4, Lemma 7.9, pp. 81–82, and Theorem 7.10, pp. 82–83: norm summability and completeness](measure-theory-by-john-k-hunter/lp-spaces-chapter-7-of-measure-theory.md)

## ↑ Ancestors (7)

1. [Minkowski inequality](minkowski-inequality.md)
2. [Lp norm](lp-norm.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Minkowski inequality](minkowski-inequality.md)
