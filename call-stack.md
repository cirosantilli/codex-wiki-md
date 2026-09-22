# Call stack

↑ **Parent:** [Stack (data structure)](stack-data-structure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Call_stack)

A [call stack](call-stack.md) stores active procedure calls and the information needed to resume each caller, such as its return location and local variables. A call adds a frame; returning removes that frame and resumes the previous call. When [depth-first search](depth-first-search.md) uses [recursion](recursion-computer-science.md), a frame also records where its [adjacency list](adjacency-list.md) scan paused. The active frames describe a [graph path](path-in-a-graph.md) from the starting [vertex](vertex-graph-theory.md) to the current [vertex](vertex-graph-theory.md); finished calls have left the [call stack](call-stack.md), although their [vertices](vertex-graph-theory.md) remain marked as discovered.

**Table of contents**

- [Display for lexical scope](display-for-lexical-scope.md)
- [Dynamic chain](dynamic-chain.md)
- [Static chain](static-chain.md)
- [Stack alignment](stack-alignment.md)
- [Stack frame](stack-frame.md)
  - [Frame pointer](frame-pointer.md)
  - [Dynamic link](dynamic-link.md)
  - [Static link](static-link.md)

## ↑ Ancestors (4)

1. [Stack (data structure)](stack-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (28)

- [Binary array sum by recursion](binary-array-sum-by-recursion.md)
- [Breadth-first search](breadth-first-search.md)
- [Cached cell value](cached-cell-value.md)
- [Call stack](call-stack.md)
- [Calling convention](calling-convention.md)
- [Depth-first search](depth-first-search.md)
- [Execution context](execution-context.md)
- [Factorial recursion and returning frames](factorial-recursion-and-returning-frames.md)
- [Memoization arithmetic and stack costs](memoization-arithmetic-and-stack-costs.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/compilers/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/1/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/3/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/3/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/3/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/2/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/2/e/solution.md)
- [Recursive process](recursive-process.md)
- [Stack frame](stack-frame.md)
- [Stack pointer](stack-pointer.md)
- [Tail recursion](tail-recursion.md)
- [Thread (computing)](thread-computing.md)
