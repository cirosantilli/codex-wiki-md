# Structural induction on lazy lists

↑ **Parent:** [Structural induction](structural-induction.md)

For an [admissible predicate on lazy lists](admissible-predicate-on-lazy-lists.md) $P$, prove $P(\bot)$ and $P([])$, and prove $P(xs)\Rightarrow P(x:xs)$ for every possibly partial head $x$. Constructor induction then establishes $P$ on every finite partial approximation, and admissibility extends it to limits, including infinite [lists](list-abstract-data-type.md). Without the [bottom value](bottom-value.md) case and the limit condition, ordinary finite [structural induction](structural-induction.md) does not justify a claim about infinite data.[Recursive Functions on Lazy Lists, ITP 2014 presentation, slide 7: admissibility restriction on induction over lazy lists](https://ethz.ch/content/dam/ethz/special-interest/infk/inst-infsec/information-security-group-dam/people/andreloc/lochbihler14itps.pdf)

## ↑ Ancestors (6)

1. [Structural induction](structural-induction.md)
2. [Mathematical proof](mathematical-proof.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms-resit/1/b/solution.md)
