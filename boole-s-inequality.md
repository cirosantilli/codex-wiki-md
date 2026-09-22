<h1 id="boole-s-inequality">Boole's inequality</h1>

↑ **Parent:** [Probability inequality](probability-inequality-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boole's_inequality)

[Boole's inequality](boole-s-inequality.md), also called the [union bound](boole-s-inequality.md), bounds the [probability](probability.md) that at least one of several [events](event.md) occurs by adding their individual [probabilities](probability.md). For a finite or [countable](countable-set.md) family of [events](event.md) $A_i$ in the same [probability space](probability-space.md),

$$
\mathbb P\left(\bigcup_i A_i\right)\leq\min\left\{1,\sum_i\mathbb P(A_i)\right\}.
$$

The [union](set-union.md) includes outcomes where several [events](event.md) occur together. There is no [independence](independent-random-variables.md) assumption: adding the individual [probabilities](probability.md) counts such outcomes repeatedly, which can only make the sum larger. The cap at one uses the total mass of a [probability measure](probability-measure.md). For infinitely many [events](event.md), the sum is a nonnegative [series](series-mathematics.md), possibly infinite; an infinite sum gives only the bound one. This is [countable subadditivity of a measure](countable-subadditivity-of-a-measure.md) specialized to a [probability measure](probability-measure.md). See [Probability: Theory and Examples (fifth edition) by Rick Durrett](probability-theory-and-examples-fifth-edition-by-rick-durrett.md) (Section 1.1, Theorem 1.1.1(ii), printed p. 2).

For example, choose uniformly from the twelve outcomes $\Omega=\{1,\ldots,12\}$, using the [discrete uniform distribution](discrete-uniform-distribution.md). Put $A=\{1,2,3,4\}$. If $B=\{5,6,7,8\}$, these are [disjoint events](disjoint-events.md) and their [union](set-union.md) has [probability](probability.md) $8/12=2/3$, exactly the [union bound](boole-s-inequality.md). If $B=\{3,4,5,6\}$, the [union](set-union.md) has only six outcomes, so its exact [probability](probability.md) is $1/2$, although both individual [probabilities](probability.md) are still $1/3$ and the bound is still $2/3$. If $B=A$, the exact [probability](probability.md) falls to $1/3$ with the same bound. These examples isolate [overlap in the union bound](overlap-in-the-union-bound.md) by keeping the individual [probabilities](probability.md) fixed.

<a id="image-the-same-individual-event-probabilities-give-different-exact-union-probabilities-as-overlap-increases"></a>
![](union-bound-finite-events-overlap.png)

**[Figure 8](#image-the-same-individual-event-probabilities-give-different-exact-union-probabilities-as-overlap-increases). The same individual event probabilities give different exact union probabilities as overlap increases**. Each panel is a fully specified [discrete uniform distribution](discrete-uniform-distribution.md) on twelve numbered outcomes. Blue means $A$ only, orange means $B$ only, purple means their [intersection](set-intersection.md), and white means neither. The bottom bars compare the exact [union](set-union.md) [probability](probability.md) with the sum of the individual [probabilities](probability.md). The three [unions](set-union.md) contain eight, six, and four outcomes; the sum counts eight in every panel.

The [union bound](boole-s-inequality.md) is useful when each [event](event.md) is easy to control but their joint behavior is difficult to determine. A short proof uses [indicator functions](indicator-function.md): at every outcome,

$$
\mathbf 1_{\bigcup_{i=1}^n A_i}\leq\sum_{i=1}^n\mathbf 1_{A_i}.
$$

Taking [expected values](expected-value.md) and using [linearity of expectation](linearity-of-expectation.md) proves the finite bound.[6.2.1 The Union Bound and Extension](introduction-to-probability-statistics-and-random-processes-by-hossein-pishro-nik/6-2-1-the-union-bound-and-extension.md) For a [countable](countable-set.md) family, the finite [unions](set-union.md) increase to the full [union](set-union.md); [continuity of probability](continuity-of-probability.md) passes the finite inequalities to the limit. The closure of a [sigma-algebra](sigma-algebra.md) under [countable unions](countable-union.md) ensures that this limiting [union](set-union.md) is an [event](event.md). For the [continuity of probability](continuity-of-probability.md) step, see [Probability: Theory and Examples (fifth edition) by Rick Durrett](probability-theory-and-examples-fifth-edition-by-rick-durrett.md) (Section 1.1, Theorem 1.1.1(iii), printed p. 2).

**Table of contents**

- [Equality in Boole's inequality](equality-in-boole-s-inequality.md)
- [Overlap in the union bound](overlap-in-the-union-bound.md)
- [Failure-probability budget](failure-probability-budget.md)
- [Positive common intersection from pair-intersection probabilities](positive-common-intersection-from-pair-intersection-probabilities.md)

## ↑ Ancestors (6)

1. [Probability inequality](probability-inequality-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Boole's inequality](boole-s-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-2/9f/solution.md)
