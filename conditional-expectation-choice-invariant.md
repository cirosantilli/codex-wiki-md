# Conditional expectation choice invariant

↑ **Parent:** [Method of conditional probabilities](method-of-conditional-probabilities.md)

Let $Z=Z(X_1,\ldots,X_n)$ be a real-valued [objective function](objective-function.md) of finitely many choices, with finite [expected value](expected-value-split.md). Suppose a prefix $P=(X_1=x_1,\ldots,X_i=x_i)$ has positive [probability](probability.md). Write $q(P)=\mathbb E[Z\mid P]$. If the next choice is a fair [bit](bit.md), the [law of total expectation](law-of-total-expectation.md) gives

$$
q(P)=\frac{q(P,0)+q(P,1)}2.
$$

At least one child is at least this average. Choose a child with the larger value, using a fixed rule for ties. The resulting [loop invariant](loop-invariant.md) is $q(P)\geq\mathbb E Z$. At a complete assignment $x$, there is only one completion left, so $q(x)=Z(x)$ and therefore $Z(x)\geq\mathbb E Z$.

For a biased choice or more than two possibilities, use the corresponding weighted average:

$$
q(P)=\sum_{a:\,p_a>0}p_aq(P,a),\qquad p_a=\mathbb P(X_{i+1}=a\mid P).
$$

Some positive-[probability](probability.md) child is at least the weighted average. For minimization, choose a child at most the current [conditional expectation](conditional-expectation.md) and reverse the invariant. The averaging identity is the same in both directions.[Jeff Erickson, Discrete Probability, §1.2.2, printed pp. 6–7: conditional expectation decomposition and linearity; authorship stated on the author's Algorithms notes page](discrete-probability-by-jeff-erickson.md)

The word "probabilities" in the method's name also covers an [indicator random variable](indicator-random-variable.md) for an undesirable outcome: keeping its [conditional expectation](conditional-expectation.md), which is its [conditional probability](conditional-probability.md), strictly below one eventually forces that indicator to be zero. Optimizing an ordinary numerical [objective function](objective-function.md) is the [method of conditional expectations](method-of-conditional-probabilities.md) formulation used below.

## ↑ Ancestors (6)

1. [Method of conditional probabilities](method-of-conditional-probabilities.md)
2. [Derandomization](derandomization.md)
3. [Randomized algorithm](randomized-algorithm.md)
4. [Algorithm](algorithm-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Conditional expectation cut formula](conditional-expectation-cut-formula.md)
