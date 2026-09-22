# Recursion tree

↑ **Parent:** [Recursion (computer science)](recursion-computer-science.md)

A [recursion tree](recursion-tree.md) records recursive calls as nodes and their direct recursive subcalls as children. Its node labels can record the work done outside those subcalls. Summing the work over levels or charging it to nodes proves a total [running time](running-time.md) bound. For $T(n)=aT(n/b)+f(n)$, level $j$ has approximately $a^j$ instances of size $n/b^j$, so its nonrecursive work is $a^jf(n/b^j)$. Summing those quantities explains the cases of the [master theorem](master-theorem.md).

**Table of contents**

- [Entropy potential for a divide-and-conquer recurrence](entropy-potential-for-a-divide-and-conquer-recurrence.md)

## ↑ Ancestors (4)

1. [Recursion (computer science)](recursion-computer-science.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/6/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/5/a/solution.md)
- [Recursion tree](recursion-tree.md)
