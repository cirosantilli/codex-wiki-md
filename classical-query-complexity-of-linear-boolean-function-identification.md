# Classical query complexity of linear Boolean function identification

↑ **Parent:** [Query complexity](query-complexity.md)

In exact classical identification of an unknown [linear Boolean function](linear-boolean-function.md) $f_a(x)=a\cdot x$, a [function oracle](function-oracle.md) call returns one [bit](bit.md) $f_a(x)$. The [query complexity](query-complexity.md) is exactly $n$ for $n\ge1$. Queries on the [standard basis](standard-basis.md) inputs $e_j$ reveal $a_j$, proving sufficiency. For necessity, a depth-$k$ [decision tree](decision-tree.md) has at most $2^k$ answer histories and must distinguish $2^n$ hidden [binary strings](binary-string.md); hence $k\ge n$, even with adaptive inputs. A [reversible circuit](reversible-circuit.md) that preserves $x$ and updates a known target by [exclusive or](exclusive-or.md) reveals the same one [bit](bit.md) per call.

There is also a useful [linear algebra](linear-algebra-split.md) proof. Along a fixed history, the chosen inputs form the rows of a [matrix](matrix.md) $M$ over the two-element [finite field](finite-field.md), and the replies specify $Ma$. If there are $k<n$ queries, the [rank-nullity theorem](rank-nullity-theorem.md) gives a nonzero [vector](vector.md) $v$ with $Mv=0$. Then $a$ and $a+v$ give identical replies throughout this history. This also explains why adaptive choices cannot evade the bound: equal earlier replies force the same later choices.

## ↑ Ancestors (5)

1. [Query complexity](query-complexity.md)
2. [Computational complexity theory](computational-complexity-theory.md)
3. [Theoretical computer science](theoretical-computer-science-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/6/1/solution.md)
