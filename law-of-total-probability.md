# Law of total probability

↑ **Parent:** [Probability measure](probability-measure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_total_probability)

Let $(B_i)$ be a countable [measurable partition](measurable-partition.md) of the [sample space](sample-space.md), with positive [probabilities](probability.md). For any [event](event.md) $A$, the law of total probability gives

$$
\mathbb P(A)=\sum_i\mathbb P(A\mid B_i)\mathbb P(B_i).
$$

The pieces $A\cap B_i$ are [disjoint events](disjoint-events.md), so add their masses and use the definition of [conditional probability](conditional-probability.md). Zero-mass partition pieces can be omitted without changing the answer.

For the coin selection in [probability](probability.md), let $B$ mean the $3/4$-head coin was selected and let $H$ mean the first toss was heads. Then $\mathbb P(H)=\mathbb P(H\mid B)\mathbb P(B)+\mathbb P(H\mid B^c)\mathbb P(B^c)=11/20$. Each conditional answer describes one possible hidden situation; its weight describes how often that situation occurs under the model. This decomposition is useful whenever a simple conditional model sits behind a more complicated marginal [probability distribution](probability-distribution.md).

## ↑ Ancestors (7)

1. [Probability measure](probability-measure.md)
2. [Probability space](probability-space.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (29)

- [Bayes' theorem](bayes-theorem.md)
- [Conditional independence](conditional-independence.md)
- [Discrete-time Markov chain](discrete-time-markov-chain.md)
- [Input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md)
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
- [Phenotype](phenotype.md)
- [Probability](probability.md)
