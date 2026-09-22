<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By assumption the set of [combinators](../../../../../../combinator.md) is [recursively enumerable](../../../../../../recursively-enumerable-set.md). Finite [beta reduction](../../../../../../beta-reduction.md) sequences, and hence finite certificates of [beta equivalence](../../../../../../beta-equivalence.md), are also recursively enumerable.

For a closed term $Y$, choose a fresh variable $f$. The term $Y$ is a fixed-point combinator exactly when

$$
Yf\equiv_\beta f(Yf).
$$

Indeed, substitution then gives the required equivalence for every $F$, and the forward direction follows by taking $F=f$. [Dovetail](../../../../../../dovetailing.md) the enumeration of closed terms with all finite beta-equivalence certificates. Whenever a certificate of the displayed equivalence is found, output $Y$. This enumerates exactly the fixed-point combinators, proving [recursively enumerable fixed-point combinators](../../../../../../recursively-enumerable-fixed-point-combinators.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
