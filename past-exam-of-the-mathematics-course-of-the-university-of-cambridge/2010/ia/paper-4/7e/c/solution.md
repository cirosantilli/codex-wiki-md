<h1 id="7e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\Omega$ be the [set](../../../../../../set-split.md) of all [functions](../../../../../../function-split.md) from the $n$-element domain to the $k$-element codomain, and let $C_j$ consist of the [functions](../../../../../../function-split.md) which omit codomain element $j$. A [function](../../../../../../function-split.md) is [surjective](../../../../../../surjective-function.md) precisely when it lies outside $\bigcup_jC_j$.

For $J\subseteq[k]$ of size $i$, the intersection $\bigcap_{j\in J}C_j$ consists of maps taking all their values in the remaining $k-i$ elements, so it has $(k-i)^n$ members. There are $\binom ki$ choices of $J$. Applying the complement form of the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) gives

$$
\boxed{\#\{\text{surjections}\}
=\sum_{i=0}^k(-1)^i\binom ki(k-i)^n\quad(n\ge k\ge1).}
$$

When $k=n$, every fibre of a [surjective function](../../../../../../surjective-function.md) has at least one member, and the $n$ fibres partition an $n$-element domain. Thus every fibre has exactly one member and the [function](../../../../../../function-split.md) is a [bijection](../../../../../../bijection.md). The count of these [bijections](../../../../../../bijection.md) is $n!$ by the successive distinct-image choices from part (a). Hence

$$
\boxed{n!=\sum_{i=0}^n(-1)^i\binom ni(n-i)^n.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7E](../../7e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
