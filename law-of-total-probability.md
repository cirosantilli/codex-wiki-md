# Law of total probability

↑ **Parent:** [Probability measure](probability-measure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_total_probability)

Let $(B_i)$ be a countable [measurable partition](measurable-partition.md) of the [sample space](sample-space.md), with positive [probabilities](probability.md). For any [event](event.md) $A$, the law of total probability gives

$$
\mathbb P(A)=\sum_i\mathbb P(A\mid B_i)\mathbb P(B_i).
$$

The pieces $A\cap B_i$ are [disjoint events](disjoint-events.md), so add their masses and use the definition of [conditional probability](conditional-probability.md). Zero-mass partition pieces can be omitted without changing the answer.

For the coin selection in [probability](probability.md), let $B$ mean the $3/4$-head coin was selected and let $H$ mean the first toss was heads. Then $\mathbb P(H)=\mathbb P(H\mid B)\mathbb P(B)+\mathbb P(H\mid B^c)\mathbb P(B^c)=11/20$. Each conditional answer describes one possible hidden situation; its weight describes how often that situation occurs under the model. This decomposition is useful whenever a simple conditional model sits behind a more complicated marginal [probability distribution](probability-distribution-split.md).

The [law of total probability](law-of-total-probability.md) combines local [conditional probabilities](conditional-probability.md) into one overall [probability](probability.md). The [measurable partition](measurable-partition.md) must cover the [sample space](sample-space.md) with pairwise [disjoint events](disjoint-events.md): every [elementary outcome](elementary-outcome.md) belongs to exactly one part. Its [probabilities](probability.md) are the weights of a [weighted mean](weighted-arithmetic-mean.md), and they sum to one.[Probability Spaces, §4 Conditional Probability, Basic Theory, Conditioning and Bayes' Theorem: countable partition formula and weighted-average interpretation](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist.md)

For an original constructed example, make a [finite set](finite-set.md) of 1,000 items: 600 belong to $B_1$ and 400 to $B_2$. Mark exactly 60 items in $B_1$ and 100 in $B_2$, and let the [event](event.md) $A$ mean that the selected item is marked. Select an item using the [uniform distribution on a finite set](discrete-uniform-distribution.md). These are prescribed counts, so the resulting [probabilities](probability.md) are exact properties of this construction:

$$
\begin{aligned}
\mathbb P(B_1)&=\frac{600}{1000}=0.6,&\mathbb P(A\mid B_1)&=\frac{60}{600}=0.1,\\
\mathbb P(B_2)&=\frac{400}{1000}=0.4,&\mathbb P(A\mid B_2)&=\frac{100}{400}=0.25.
\end{aligned}
$$

The [conditional probability](conditional-probability.md) $0.1$ uses only the 600 items in $B_1$ as its denominator. The [probability](probability.md) of the [intersection](set-intersection.md) $A\cap B_1$ uses all 1,000 items instead: $0.6\times0.1=0.06$. Similarly, $\mathbb P(A\cap B_2)=0.4\times0.25=0.10$. Adding the two [disjoint events](disjoint-events.md) gives

$$
\mathbb P(A)=0.6(0.1)+0.4(0.25)=0.06+0.10=0.16=\frac{60+100}{1000}.
$$

<a id="image-a-partition-turns-within-group-rates-into-whole-population-areas"></a>
![](total-probability-partition-population.png)

**[Figure 5](#image-a-partition-turns-within-group-rates-into-whole-population-areas). A partition turns within-group rates into whole-population areas**. An original constructed [finite set](finite-set.md) with 1,000 items, represented by area rather than measured data. The two widths encode [probabilities](probability.md) $0.6$ and $0.4$; the shaded heights encode [conditional probabilities](conditional-probability.md) $0.1$ and $0.25$. The shaded [intersection](set-intersection.md) areas encode 60 and 100 marked items, totaling 160.

An unweighted [arithmetic mean](arithmetic-mean.md) of the two [conditional probabilities](conditional-probability.md) would give $(0.1+0.25)/2=0.175$. That is the answer to a different selection rule: choose either group with [probability](probability.md) $1/2$, then select uniformly within that group. Here the first group contains more items, so selecting uniformly among all items gives it weight $0.6$. In fact, if its weight were $w$, the overall [probability](probability.md) would be $0.1w+0.25(1-w)=0.25-0.15w$. Moving the weight from $1/2$ to $0.6$ lowers the result by $0.015$, explaining exactly why $0.175$ is too large for the original model.

The same construction is a [mixture distribution](mixture-distribution.md): first select a group with its [mixture weight](mixture-weight.md), then select an item within that group. Multiplying the weight by its [conditional probability](conditional-probability.md) gives the [probability](probability.md) of reaching $A$ through that group; adding the contributions gives the [law of total probability](law-of-total-probability.md). For example, an item in $B_1$ has selection [probability](probability.md) $0.6/600=1/1000$, and an item in $B_2$ has selection [probability](probability.md) $0.4/400=1/1000$, recovering the original [uniform distribution on a finite set](discrete-uniform-distribution.md).

<a id="image-multiply-along-each-route-and-add-the-routes-ending-in-the-event"></a>
![](total-probability-weighted-routes.png)

**[Figure 6](#image-multiply-along-each-route-and-add-the-routes-ending-in-the-event). Multiply along each route and add the routes ending in the event**. The original constructed model expressed through group selection and a marked-or-unmarked result. First-stage weights are [probabilities](probability.md); second-stage weights are [conditional probabilities](conditional-probability.md). The four final [probabilities](probability.md) sum to one. The two routes to the [event](event.md) $A$ contribute $0.06+0.10=0.16$.

No assumption of [independent events](independent-events.md) is needed. In this construction $\mathbb P(A\mid B_1)=0.1$ differs from $\mathbb P(A)=0.16$, so $A$ and $B_1$ are not [independent events](independent-events.md). Also $B_1$ and $B_2$ are [disjoint events](disjoint-events.md) with positive [probabilities](probability.md), so they cannot be [independent events](independent-events.md): their [intersection](set-intersection.md) has [probability](probability.md) zero, whereas $\mathbb P(B_1)\mathbb P(B_2)=0.24$. The [measurable partition](measurable-partition.md) supplies exclusive alternatives, not an [independence](independent-random-variables.md) assumption.

For a short proof, the [intersection](set-intersection.md) pieces $A\cap B_i$ have [union](set-union.md) $A$ and are pairwise [disjoint events](disjoint-events.md). Apply [countable additivity](countable-additivity.md), then substitute the definition of [conditional probability](conditional-probability.md) on every positive-mass part:

$$
\mathbb P(A)=\sum_i\mathbb P(A\cap B_i)
=\sum_{i:\,\mathbb P(B_i)>0}\mathbb P(A\mid B_i)\mathbb P(B_i).
$$

A [zero-probability event](zero-probability-event.md) $B_i$ has $\mathbb P(A\cap B_i)=0$. Omit it: writing $\mathbb P(A\mid B_i)$ would divide by zero. Countability ensures that the [union](set-union.md) of the omitted [zero-probability events](zero-probability-event.md) also has [probability](probability.md) zero. Overlapping parts would double-count their [intersections](set-intersection.md), and incomplete coverage would omit the [probability](probability.md) of $A$ in the uncovered region.[Probability Spaces, §4 Conditional Probability: The Basic Definition requires a positive conditioning probability; Conditioning and Bayes' Theorem proves total probability by partition intersections](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist.md)

Reversing the question gives one compact application of [Bayes' theorem](bayes-theorem.md). Among the 160 marked items, 100 belong to $B_2$, so its [conditional probability](conditional-probability.md) after observing $A$ is

$$
\mathbb P(B_2\mid A)=\frac{\mathbb P(A\cap B_2)}{\mathbb P(A)}=\frac{0.10}{0.16}=\frac{100}{160}=0.625.
$$

The [law of total probability](law-of-total-probability.md) supplied the denominator by collecting every way that $A$ can occur. Its usefulness lies in choosing a [measurable partition](measurable-partition.md) where the [conditional probabilities](conditional-probability.md) are simple, then combining them without losing the relative sizes of the alternatives.

**Table of contents**

- [Sharp bounds from binary conditional probabilities](sharp-bounds-from-binary-conditional-probabilities.md)

## ↑ Ancestors (7)

1. [Probability measure](probability-measure.md)
2. [Probability space](probability-space-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (54)

- [Bayes' theorem](bayes-theorem.md)
- [Conditional independence](conditional-independence.md)
- [Discrete-time Markov chain](discrete-time-markov-chain.md)
- [IceCube starting-event veto](icecube-starting-event-veto.md)
- [Input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md)
- [Law of total probability](law-of-total-probability.md)
- [Mixture allocation indicator](mixture-allocation-indicator.md)
- [Neutrino event classification model](neutrino-event-classification-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-2/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/9f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/9f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-35/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-45/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47/2/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2/12f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2/9f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2/9f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-41/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-2/12f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-322/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/9f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-207/5/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-320/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-221/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-356/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2/11/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/7/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/section-b/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2/11/d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-2/17/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/17/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/17/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/17/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/18/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/18/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/18/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/11/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/16/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/10/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2/14/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/16/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/14/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/12/e/iii/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1/section-a/4/solution.md)
- [Phenotype](phenotype.md)
- [Probability](probability.md)
- [Sharp bounds from binary conditional probabilities](sharp-bounds-from-binary-conditional-probabilities.md)
