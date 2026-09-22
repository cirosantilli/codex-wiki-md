# Mutual conditional expectation rigidity in L2

↑ **Parent:** [Conditional expectation](conditional-expectation.md)

Let $A,B$ belong to [L2 space](l2-space-is-a-hilbert-space.md), and suppose $B=\mathbb E[A\mid\mathcal H]$ and $A=\mathbb E[B\mid\mathcal G]$ [almost surely](almost-sure-convergence.md), for two possibly nonnested [sigma-algebras](sigma-algebra.md). Then $A=B$ [almost surely](almost-sure-convergence.md). No [independence](independent-random-variables.md) or inclusion between the [sigma-algebras](sigma-algebra.md) is required.

The identities supply $\mathcal H$-[measurable](measurability.md) and $\mathcal G$-[measurable](measurability.md) versions of $B$ and $A$. The [measurable-factor rule for conditional expectation](measurable-factor-rule-for-conditional-expectation.md) and [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) give

$$
\mathbb E[AB]=\mathbb E[B^2]=\mathbb E[A^2].
$$

Expanding the square shows $\mathbb E[(A-B)^2]=0$, and hence the required [almost sure equality](almost-sure-equality.md). Equivalently, each [conditional expectation](conditional-expectation.md) is an [orthogonal projection](orthogonal-projection.md) in [L2 space](l2-space-is-a-hilbert-space.md), and the two projection identities force equality in the [equality case for conditional second moments](equality-case-for-conditional-second-moments.md).

Equality after applying a [function](function-split.md) need not identify its original input. For instance, on four equally likely outcomes let $X$ take $-2,-1,1,2$ and set $Y=-X$. Their squares are the same nonconstant [random variable](random-variable-split.md), even though $X$ and $Y$ differ everywhere. Injectivity of the [function](function-split.md) would rule out this loss of information.

## ↑ Ancestors (7)

1. [Conditional expectation](conditional-expectation.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-measure-and-martingales-course-of-the-university-of-oxford/2021/1/a/ii/solution.md)
