# Mutual recursion

↑ **Parent:** [Recursion (computer science)](recursion-computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mutual_recursion)

Two or more functions are mutually recursive when their definitions call one another in a cycle. Two [algebraic data types](algebraic-data-type.md) can likewise be mutually recursive when constructors of each refer to the other. For alternating sequences `Zig a b` and `Zag b a`, descending one constructor exchanges the [type parameters](type-parameter.md); a pair of mapping functions must exchange its arguments correspondingly. A mutually recursive fold may have two independent result types $r,s$: its handlers have types `a -> s -> r` and `b -> r -> s`, with empty results of types `r` and `s`. Equality of the two result types is not required by [type inference](type-inference.md).

## ↑ Ancestors (4)

1. [Recursion (computer science)](recursion-computer-science.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/principles-of-programming-languages/3/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/3/d/solution.md)
