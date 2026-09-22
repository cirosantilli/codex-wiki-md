# Sample space

↑ **Parent:** [Probability space](probability-space-split.md)

The [sample space](sample-space.md) is the [set](set-split.md) $\Omega$ of outcomes represented by a [probability](probability.md) model. One [elementary outcome](elementary-outcome.md) $\omega\in\Omega$ specifies a complete result at the level of detail the model keeps. An [event](event.md) is a [subset](subset.md) belonging to the model's [sigma-algebra](sigma-algebra.md) $\mathcal F$; it occurs when the actual outcome lies in that [subset](subset.md). Together with a [probability measure](probability-measure.md) $\mathbb P$, these form a [probability space](probability-space-split.md) $(\Omega,\mathcal F,\mathbb P)$, with $\mathbb P(\Omega)=1$.[§1.3.1 Random Experiments: definitions of outcome, sample space, and event; three-toss example](introduction-to-probability-statistics-and-random-processes-by-hossein-pishro-nik.md)

Choosing a [sample space](sample-space.md) means deciding which distinctions matter. For two tosses, recording the ordered head-or-tail sequence distinguishes $HT$ from $TH$; recording only the number of heads merges them. Neither representation is automatically wrong, but the second cannot answer a question about which toss was heads. Keeping a detailed [sample space](sample-space.md) and defining a [random variable](random-variable-split.md) for the desired observation lets several questions share one model.

A [sample space](sample-space.md) alone assigns no [probabilities](probability.md). Even writing $\Omega=\{H,T\}^2$ as a [Cartesian product](cartesian-product.md) does not establish [independence](independent-random-variables.md): that requires a condition on the [probability measure](probability-measure.md). On a finite [sample space](sample-space.md) with all [subsets](subset.md) admitted as [events](event.md),

$$
\mathbb P(A)=\sum_{\omega\in A}\mathbb P(\{\omega\}).
$$

Only when all elementary [probabilities](probability.md) are equal does this become $\mathbb P(A)=|A|/|\Omega|$, where the bars denote [cardinality](cardinality.md). This is the [uniform distribution on a finite set](discrete-uniform-distribution.md), an additional modelling choice.

[Sample spaces](sample-space.md) can also be infinite. For example, take $\Omega=[0,1]$, its [Borel sigma-algebra](borel-sigma-algebra.md), and the [continuous uniform distribution](continuous-uniform-distribution.md). Then $\mathbb P([a,b])=b-a$ for $0\leq a\leq b\leq1$, so each [singleton](singleton-mathematics.md) has [probability](probability.md) zero while $\mathbb P(\Omega)=1$. Thus an [elementary outcome](elementary-outcome.md) need not carry positive [probability](probability.md), and a continuous model cannot be understood by counting equally likely points. The distinction is developed in [zero-probability event](zero-probability-event.md) and [countable additivity](countable-additivity.md).

**Table of contents**

- [Elementary outcome](elementary-outcome.md)
- [Two-toss sample space](two-toss-sample-space.md)
  - [Events determined by a random variable](events-determined-by-a-random-variable.md)

## ↑ Ancestors (6)

1. [Probability space](probability-space-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (44)

- [A shared coin prevents a zero-one conclusion](a-shared-coin-prevents-a-zero-one-conclusion.md)
- [Bayes factor](bayes-factor.md)
- [Bernoulli sample sum as a sufficient statistic](bernoulli-sample-sum-as-a-sufficient-statistic.md)
- [Boolean operations on events](boolean-operations-on-events.md)
- [Complement rule of probability](complement-rule-of-probability.md)
- [Conditioning on a sum can create dependence](conditioning-on-a-sum-can-create-dependence.md)
- [Constant random variable](constant-random-variable.md)
- [Continuity of probability](continuity-of-probability.md)
- [Elementary outcome](elementary-outcome.md)
- [Equality in Boole's inequality](equality-in-boole-s-inequality.md)
- [Events determined by a random variable](events-determined-by-a-random-variable.md)
- [Failure-probability budget](failure-probability-budget.md)
- [Fisher-Neyman factorization theorem](fisher-neyman-factorization-theorem.md)
- [Infinitely many heads as a tail event](infinitely-many-heads-as-a-tail-event.md)
- [Kolmogorov axioms](kolmogorov-axioms.md)
- [Law of total probability](law-of-total-probability.md)
- [Normalization of a probability distribution](normalization-of-a-probability-distribution.md)
- [Pairwise independent events](pairwise-independent-events.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/9f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2/9f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/18/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2/14/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/16/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/16/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/16/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/16/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/16/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/14/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/10/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/10/b/solution.md)
- [Probability](probability.md)
- [Probability measure](probability-measure.md)
- [Probability space](probability-space-split.md)
- [Probability theory](probability-theory-split.md)
- [Random variable](random-variable-split.md)
- [Sample path](sample-path.md)
- [Sample space](sample-space.md)
- [Stochastic process](stochastic-process-split.md)
- [Tail probability](tail-probability.md)
- [Two-toss sample space](two-toss-sample-space.md)
