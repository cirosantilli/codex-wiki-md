# Finite-domain composition from relation predicates

↑ **Parent:** [Composition of relations](composition-of-relations.md)

If $R:X\times Y\to\{false,true\}$ and $S:Y\times Z\to\{false,true\}$ expose only membership predicates, composition requires finding whether some middle value satisfies both. A complete finite enumeration of $Y$ makes the query decidable by scanning until a witness is found or all values fail. Without an enumeration or equivalent access operation, generic membership oracles do not supply enough information: a finite query transcript can agree with an all-false case yet omit a fresh middle witness that makes composition true. Known finiteness is not the same as an available traversal. A separate carrier argument preserves the variance of the base predicate interfaces.

## ↑ Ancestors (8)

1. [Composition of relations](composition-of-relations.md)
2. [Binary relation](binary-relation.md)
3. [Finitary relation](finitary-relation.md)
4. [Set theory](set-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/8/d/solution.md)
