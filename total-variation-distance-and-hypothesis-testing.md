# Total variation distance and hypothesis testing

↑ **Parent:** [Total variation distance](total-variation-distance.md)

Suppose one observation comes from either $P$ or $Q$, each with prior [probability](probability.md) $1/2$. A [decision rule](decision-rule.md) that chooses $P$ on an [event](event.md) $E$ and $Q$ otherwise has success [probability](probability.md)

$$
\frac12P(E)+\frac12Q(E^c)=\frac12\bigl(1+P(E)-Q(E)\bigr).
$$

On a [finite set](finite-set.md), choosing $E=\{x:P(x)>Q(x)\}$ therefore gives $\tfrac12(1+d_{\mathrm{TV}}(P,Q))$. This is the equal-prior version of [minimum sum of errors in a simple hypothesis test](minimum-sum-of-errors-in-a-simple-hypothesis-test.md); allowing a [statistical test](statistical-test.md) to use an auxiliary [random variable](random-variable-split.md) cannot improve it, because for each outcome the better of the two decisions already maximizes its contribution.

For the four-outcome example, choose $P$ after $A$ and $Q$ after $B$ or $C$, with either decision allowed after $D$. Choosing $Q$ after $D$ yields $\tfrac12(0.4+0.9)=0.65$. **The best success probability is 65%, with a 35% error probability.** A smaller [total variation distance](total-variation-distance.md) means the two sources are harder to distinguish from one observation. Unequal prior [probabilities](probability.md), unequal costs, or multiple observations change this particular decision problem; the $65\%$ figure is not a universal bound for every experiment.

## ↑ Ancestors (5)

1. [Total variation distance](total-variation-distance.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
