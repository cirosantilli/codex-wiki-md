# Sign-bracketing binary search

↑ **Parent:** [Binary search](binary-search.md)

Suppose [integer](integer-split.md) endpoints satisfy $l<r$ and $f(l)\leq0<f(r)$. Repeatedly test an interior midpoint and replace the endpoint with its matching sign. The [loop invariant](loop-invariant.md) is the ordered opposite-sign bracket. The positive [integer](integer-split.md) width is a [loop variant](loop-variant.md), and at termination $r=l+1$. Thus an adjacent sign transition can be located in $O(\log(r-l))$ evaluations without assuming that $f$ is monotone. If $f$ extends continuously between the endpoints, the [intermediate value theorem](intermediate-value-theorem.md) associates the sign bracket with a zero. This is different from finding the first true position of a globally monotone predicate.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Exponential sign bracketing](exponential-sign-bracketing.md)
