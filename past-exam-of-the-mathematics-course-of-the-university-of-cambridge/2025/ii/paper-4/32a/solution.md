<h1 id="32a/solution">Solution</h1>

↑ **Parent:** [32A](../32a.md)

A map is [Devaney chaos](../../../../../devaney-chaos.md) when:

- every pair of nonempty open sets eventually overlap under an iterate, which is [topological transitivity](../../../../../topological-transitivity.md);
- it has [dense periodic points](../../../../../dense-periodic-points.md); and
- nearby initial conditions can eventually separate by a fixed amount, which is [sensitive dependence on initial conditions](../../../../../butterfly-effect.md).

Write a point as a binary expansion

$$
x=0.b_1b_2b_3\ldots{}_2.
$$

Apart from the harmless choice of expansion at dyadic rationals, the [binary shift representation of the doubling map](../../../../../binary-shift-representation-of-the-doubling-map.md) is

$$
F(x)=0.b_2b_3b_4\ldots{}_2.
$$

Every open interval contains a binary cylinder specified by a finite initial word. Given cylinders $U$ and $V$, choose a binary sequence beginning with the word for $U$ and place the word for $V$ after it. A suitable iterate shifts the second word to the front, proving topological transitivity.

Given any cylinder, repeat its defining word forever. The resulting point is periodic and lies in that cylinder, so periodic points are dense.

Finally, given $x$ and any neighbourhood, choose $N$ so large that changing only digits after the first $N$ stays inside that neighbourhood. Choose the later tail so that after $N$ shifts it is either $0$ or $3/4$, whichever is farther from $F^N(x)$. The separation is at least $3/8$, so any smaller fixed constant, for example $\delta=1/4$, proves sensitivity. Hence the [doubling map](../../../../../dyadic-transformation.md) is chaotic in Devaney's sense.

## ↑ Ancestors (10)

1. [32A](../32a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
