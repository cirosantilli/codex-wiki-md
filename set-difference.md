# Set difference

↑ **Parent:** [Set](set-split.md)

The set difference $A\setminus B$ keeps the [set elements](element-of-a-set.md) of $A$ that do not belong to $B$:

$$
A\setminus B=\{x\in A:x\notin B\},\qquad x\in A\setminus B\iff(x\in A)\wedge\neg(x\in B).
$$

Thus [set difference](set-difference.md) combines [logical conjunction](logical-conjunction.md) (AND) with [logical negation](negation.md) (NOT): pass the first condition and fail the second. The definition applies to any two [sets](set-split.md); $B$ need not be a [subset](subset.md) of $A$.

For $A=\{1,2,3\}$ and $B=\{3,4\}$, the two orders give different answers:

$$
A\setminus B=\{1,2\},\qquad B\setminus A=\{4\}.
$$

The common member $3$ is removed in both directions. A database filter illustrates the usefulness: if $A$ is the [set](set-split.md) of records matching the first condition and $B$ the [set](set-split.md) matching the second, $A\setminus B$ selects records matching the first but not the second. The [Venn diagram](venn-diagram.md) in [set union](set-union.md) shades both directions separately.

The name [relative complement](set-difference.md) emphasizes that the ambient [set](set-split.md) is $A$: $A\setminus B$ is the [complement](complement-of-a-set.md) of $A\cap B$ within $A$. If a larger [universal set](universal-set.md) $U$ contains $A$ and $B$, then $A\setminus B=A\cap(U\setminus B)$. Changing that larger [universal set](universal-set.md) does not change the [set difference](set-difference.md), because membership still requires belonging to $A$. In [ZF](zermelo-fraenkel-set-theory.md) the [set difference](set-difference.md) exists by the [axiom schema of separation](axiom-schema-of-specification.md). It also gives [relative complements](set-difference.md) within a fixed [tuple](finite-tuple.md) [domain](domain-mathematical-analysis.md) in [finite relation closure for set-theoretic coding](finite-relation-closure-for-set-theoretic-coding.md).

## ↑ Ancestors (6)

1. [Set](set-split.md)
2. [Set theory](set-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Continuity of probability](continuity-of-probability.md)
- [Difference set](difference-set.md)
- [Finite relation closure for set-theoretic coding](finite-relation-closure-for-set-theoretic-coding.md)
- [Kolmogorov axioms](kolmogorov-axioms.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-11/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-121/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121/2/iii/solution.md)
- [Set difference](set-difference.md)
- [Set union](set-union.md)
- [Union and intersection of set families](union-and-intersection-of-set-families.md)
- [Venn diagram](venn-diagram.md)
