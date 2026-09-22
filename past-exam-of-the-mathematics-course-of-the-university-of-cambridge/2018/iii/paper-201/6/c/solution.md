<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose $X_n\to X$ with [convergence in probability](../../../../../../convergence-in-probability.md). For real $t$ and $\delta>0$, the elementary inequality $|e^{iu}-e^{iv}|\leq\min(2,|u-v|)$ gives

$$
\left|\mathbb E e^{itX_n}-\mathbb E e^{itX}\right|
\leq |t|\delta+2\mathbb P(|X_n-X|>\delta).
$$

First let $n\to\infty$, then let $\delta\downarrow0$. The [characteristic functions](../../../../../../characteristic-function.md) converge pointwise to that of $X$, which is continuous at zero. The [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) gives **[convergence in probability](../../../../../../convergence-in-probability.md) implies [convergence in distribution](../../../../../../convergence-in-distribution.md)**.

For the converse, let $Z$ have the fair [Bernoulli distribution](../../../../../../bernoulli-distribution.md), put $X=Z$, and set $X_n=1-Z$ for every $n$. All $X_n$ have the same [probability distribution](../../../../../../probability-distribution.md) as $X$, so $X_n\xrightarrow dX$. But $|X_n-X|=1$ always, hence

$$
\boxed{\mathbb P(|X_n-X|>1/2)=1\quad\text{for every }n.}
$$

There is no [convergence in probability](../../../../../../convergence-in-probability.md) to $X$. In this example $X_n$ does have [convergence in probability](../../../../../../convergence-in-probability.md) to $1-Z$: the counterexample concerns the converse with the specified limit $X$, as usual. If one interprets the question as denying [convergence in probability](../../../../../../convergence-in-probability.md) to any limit, take $X_n=Z$ for even $n$ and $X_n=1-Z$ for odd $n$. Its [probability distribution](../../../../../../probability-distribution.md) is still constant, while the two subsequences have distinct limits from [almost sure convergence](../../../../../../almost-sure-convergence.md), ruling out any common limit in probability by [uniqueness of a limit in probability](../../../../../../uniqueness-of-a-limit-in-probability.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
