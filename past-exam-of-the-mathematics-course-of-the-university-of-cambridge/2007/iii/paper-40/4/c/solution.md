<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [imputation](../../../../../../imputation-in-a-coalitional-game.md) $y$, the [excess of a coalition](../../../../../../excess-of-a-coalition.md) is $e(S,y)=v(S)-\sum_{i\in S}y_i$. Arrange these excesses in decreasing order. The [nucleolus](../../../../../../nucleolus.md) is the [imputation](../../../../../../imputation-in-a-coalitional-game.md) that lexicographically minimizes this ordered vector: minimize the largest complaint first, then the next largest among ties, and so on. The empty and grand-coalition excesses are fixed at zero for every efficient allocation, so they can be omitted without changing the lexicographic comparison.

For every efficient $y$ the three pair excesses have sum

$$
e(\{1,2\},y)+e(\{1,3\},y)+e(\{2,3\},y)=6+9+11-2(15)=-4.
$$

Hence at least one pair has excess at least $-4/3$, and the largest proper-coalition excess is at least $-4/3$. At the proposed allocation all three pair excesses equal $-4/3$, while all three singleton excesses equal $-8/3$. It therefore attains the best possible largest proper-coalition excess.

Moreover, any allocation attaining this bound must have all three pair excesses equal $-4/3$, since they are individually at most that value and sum to $-4$. This forces

$$
y_1+y_2=\frac{22}3,\qquad y_1+y_3=\frac{31}3,\qquad y_2+y_3=\frac{37}3,
$$

whose unique solution is $y=x$. It is already an [imputation](../../../../../../imputation-in-a-coalitional-game.md), so the first nonconstant lexicographic stage has a unique minimizer; there are no later choices to resolve. Therefore

$$
\boxed{\operatorname{nuc}(v)=x:\quad\text{(c) is true.}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
