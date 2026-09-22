# Events determined by a random variable

↑ **Parent:** [Two-toss sample space](two-toss-sample-space.md)

Define the head-count [random variable](random-variable-split.md) $X:\Omega\to\{0,1,2\}$ by

$$
X(TT)=0,\qquad X(HT)=X(TH)=1,\qquad X(HH)=2.
$$

The four [elementary outcomes](elementary-outcome.md) are inputs to this [function](function-split.md); its three numerical values are outputs. Each [fiber of a function](fiber-of-a-function.md) collects all outcomes giving one value. Under the fair [independent](independent-random-variables.md) model, adding the masses in each [fiber](fiber-of-a-function.md) gives the [probability mass function](probability-mass-function.md)

$$
\mathbb P(X=0)=\frac14,\qquad
\mathbb P(X=1)=\frac14+\frac14=\frac12,\qquad
\mathbb P(X=2)=\frac14.
$$

Consequently the output values are not equally likely, although the inputs are. Using the reduced [sample space](sample-space.md) $\{0,1,2\}$ with these masses gives the same head-count [probability distribution](probability-distribution-split.md); assigning $1/3$ to each value would describe a different model.

A question about a [random variable](random-variable-split.md)'s value becomes an [event](event.md) on the original [sample space](sample-space.md) by taking an [inverse image](preimage.md):

$$
\{X\in D\}=X^{-1}(D)=\{\omega\in\Omega:X(\omega)\in D\}.
$$

For a real-valued [random variable](random-variable-split.md), this is an [event](event.md) whenever $D$ is a [Borel set](borel-set.md), by [measurability](measurability.md). In this finite example every [subset](subset.md) of $\{0,1,2\}$ is allowed. In particular,

$$
\{X\geq1\}=X^{-1}(\{1,2\})=\{HH,HT,TH\},\qquad
\mathbb P(X\geq1)=\frac12+\frac14=\frac34.
$$

This is the same “at least one head” [event](event.md) counted above, expressed through an observable.[Probability Spaces, §2 Events and Random Variables, Random Variables: measurable functions and the inverse-image notation for value events](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist.md)

<a id="image-head-count-merges-outcomes-into-fibers-and-adds-their-probabilities"></a>
![](two-coin-head-count-fibers.png)

**[Figure 2](#image-head-count-merges-outcomes-into-fibers-and-adds-their-probabilities). Head count merges outcomes into fibers and adds their probabilities**. The [random variable](random-variable-split.md) sends $TT$ to zero, both $HT$ and $TH$ to one, and $HH$ to two. The [inverse image](preimage.md) of $\{1,2\}$ is the highlighted [event](event.md) of at least one head. Two arrows meeting at one explain its [probability](probability.md) $1/2$.

Every [event](event.md) determined by $X$ is a [union](set-union.md) of complete [fibers](fiber-of-a-function.md). There are $2^3=8$ such [events](event.md), whereas the full [power set](power-set.md) of $\Omega$ has $2^4=16$. In particular, the first-head [event](event.md) $A=\{HH,HT\}$ is not determined by $X$: it contains $HT$ but excludes $TH$, although both give $X=1$. Choosing an observable makes calculations simpler precisely by forgetting distinctions; the useful choice is one that retains the distinctions the question needs.

## ↑ Ancestors (8)

1. [Two-toss sample space](two-toss-sample-space.md)
2. [Sample space](sample-space.md)
3. [Probability space](probability-space-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
