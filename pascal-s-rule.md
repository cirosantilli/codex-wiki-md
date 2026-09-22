<h1 id="pascal-s-rule">Pascal's rule</h1>

↑ **Parent:** [Binomial coefficient](binomial-coefficient-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pascal's_rule)

Pascal's identity is

$$
\binom nk=\binom{n-1}k+\binom{n-1}{k-1}.
$$

For an [integer](integer-split.md) $n\geq1$ and any [integer](integer-split.md) $k$, [Pascal's rule](pascal-s-rule.md) holds with the convention $\binom nk=0$ outside $0\leq k\leq n$. The boundary values are $\binom n0=\binom nn=1$, including $\binom00=1$. Initialize row zero separately: the [recurrence relation](recurrence-relation.md) does not require [binomial coefficients](binomial-coefficient-split.md) with top index $-1$.[§1.2, Recurrence relation for binomial coefficients and Pascal's Triangle: edge values and the two-parent rule](discrete-mathematics-an-open-introduction-3rd-edition-by-oscar-levin.md)

**Proof by a marked element.** Count the $k$-element [subsets](subset.md) of $\{1,\ldots,n\}$, marking the element $n$ as special. Those omitting $n$ are exactly the $k$-element [subsets](subset.md) of $\{1,\ldots,n-1\}$. From those containing $n$, delete $n$ to obtain the $(k-1)$-element [subsets](subset.md) of that same smaller [set](set-split.md); adjoining $n$ reverses this operation. The [rule of sum](addition-principle.md) adds these two disjoint counts. The proof includes $k=0$ and $k=n$ because the impossible class contributes zero.

For an original worked instance, choose three labels from $\{1,2,3,4,5,6,7\}$ and mark $7$. Omitting it gives $\binom63=20$ selections. Including it leaves two labels to choose from the other six, giving $\binom62=15$. Therefore $\binom73=20+15=35$. Under the [bijection](bijection.md) with [north-east lattice paths](north-east-lattice-path.md) to $(4,3)$, membership of position seven says whether the final step is north: the marked-element split becomes the last-step split.

This makes [Pascal's rule](pascal-s-rule.md) useful beyond an algebraic identity. A counting problem may have an obvious yes-or-no decision even when its [factorial](factorial.md) formula is obscure; splitting at that decision exposes a [recurrence relation](recurrence-relation.md). When the smaller counts are shared between many cases, [dynamic programming](dynamic-programming.md) reuses them. The beauty of [Pascal's triangle](pascal-s-triangle.md) is that one local addition rule simultaneously organizes [subsets](subset.md), [binary strings](binary-string.md), [north-east lattice paths](north-east-lattice-path.md), and the [binomial theorem](binomial-theorem.md).

## ↑ Ancestors (5)

1. [Binomial coefficient](binomial-coefficient-split.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Lattice path](lattice-path.md)
- [Pascal's rule](pascal-s-rule.md)
- [Pascal's triangle](pascal-s-triangle.md)
