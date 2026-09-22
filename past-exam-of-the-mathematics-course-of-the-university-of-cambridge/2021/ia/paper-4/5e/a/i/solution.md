<h1 id="5e/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define the [binomial coefficient](../../../../../../../binomial-coefficient.md) $\binom nr$ as the number of $r$-element [subsets](../../../../../../../subset.md) of an $n$-element set, equivalently as $n!/[r!(n-r)!]$. Partitioning the $r$-element subsets of $\{1,\ldots,n+1\}$ according to whether they contain $n+1$ proves [Pascal's identity](../../../../../../../pascal-s-rule.md)

$$
\binom{n+1}r=\binom nr+\binom n{r-1}.
$$

Thus the [forward difference operator](../../../../../../../forward-difference-operator.md) satisfies

$$
\boxed{(\delta f_r)(n)=\binom{n+1}r-\binom nr=\binom n{r-1}=f_{r-1}(n).}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [5E](../../../5e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
