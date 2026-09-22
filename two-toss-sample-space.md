# Two-toss sample space

↑ **Parent:** [Sample space](sample-space.md)

Model two fair [independent](independent-random-variables.md) coin tosses, recording their order. Here $H$ denotes heads and $T$ tails, and

$$
\Omega=\{HH,HT,TH,TT\},\qquad
\mathcal F=\mathcal P(\Omega),\qquad
\mathbb P(\{\omega\})=\frac14\quad(\omega\in\Omega).
$$

The [power set](power-set.md) $\mathcal P(\Omega)$ includes every question expressible as a [subset](subset.md) of these four outcomes. The mass $1/4=(1/2)(1/2)$ comes from the fairness and [independence](independent-random-variables.md) assumptions. These are exact model [probabilities](probability.md), rather than measured toss frequencies.

Let $A$ be the [event](event.md) that the first toss is heads and $B$ the [event](event.md) that the second toss is heads. Then

$$
A=\{HH,HT\},\qquad B=\{HH,TH\},\qquad
A\cup B=\{HH,HT,TH\},\qquad A\cap B=\{HH\}.
$$

The [union](set-union.md) means “at least one head,” while the [intersection](set-intersection.md) means “both heads.” Their [probabilities](probability.md) are $3/4$ and $1/4$. Counting the [union](set-union.md) through the [inclusion-exclusion principle](inclusion-exclusion-principle.md) gives $1/2+1/2-1/4=3/4$; alternatively its [complement of an event](complement-of-an-event.md) is $\{TT\}$, of [probability](probability.md) $1/4$.

<a id="image-four-ordered-outcomes-and-the-event-of-at-least-one-head"></a>
![](two-coin-outcomes-and-events.png)

**[Figure 1](#image-four-ordered-outcomes-and-the-event-of-at-least-one-head). Four ordered outcomes and the event of at least one head**. Rows record the first toss and columns the second. Each cell has [probability](probability.md) $1/4$ under fair [independent](independent-random-variables.md) tosses. The highlighted [union](set-union.md) $A\cup B$ includes $HH$, $HT$, and $TH$; the overlap $A\cap B$ contains only $HH$.

On the same [sample space](sample-space.md), assigning masses $3/8,1/8,1/8,3/8$ to $HH,HT,TH,TT$ would still make each toss fair: $\mathbb P(A)=\mathbb P(B)=1/2$. But $\mathbb P(A\cap B)=3/8\ne1/4$, so the tosses would be dependent. The [event](event.md) of at least one head would have [probability](probability.md) $5/8$. Changing the [probability measure](probability-measure.md) changes the answer even when the [sample space](sample-space.md) and the single-toss [probabilities](probability.md) stay the same.

**Table of contents**

- [Events determined by a random variable](events-determined-by-a-random-variable.md)

## ↑ Ancestors (7)

1. [Sample space](sample-space.md)
2. [Probability space](probability-space-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
