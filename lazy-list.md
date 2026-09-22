# Lazy list

↑ **Parent:** [Linked list](linked-list.md)

A [linked list](linked-list.md) whose future structure is obtained by calling a delayed computation. In [Standard ML](standard-ml.md), `unit -> node` delays a computation until demand. Filtering may need to force arbitrarily many rejected elements to produce its next retained element; filtering an infinite list need not produce a result. Delay alone does not imply [memoization](memoization.md).

// Destination: computer-science.bigb

**Table of contents**

- [Proper lazy list](proper-lazy-list.md)
- [Absence-detection obstruction for infinite lists](absence-detection-obstruction-for-infinite-lists.md)
- [Stream productivity](stream-productivity.md)
- [Partial list](partial-list.md)
  - [Partial-list interleaving obstruction](partial-list-interleaving-obstruction.md)
  - [Finite approximation of a lazy list](finite-approximation-of-a-lazy-list.md)

## ↑ Ancestors (4)

1. [Linked list](linked-list.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (31)

- [Continuation representation of a left fold](continuation-representation-of-a-left-fold.md)
- [Finite approximation of a lazy list](finite-approximation-of-a-lazy-list.md)
- [Fold factorisation criterion](fold-factorisation-criterion.md)
- [Lazy evaluation](lazy-evaluation.md)
- [Left-fold fusion law](left-fold-fusion-law.md)
- [Locally finite sorted-stream merge](locally-finite-sorted-stream-merge.md)
- [Memoized iterator snapshot](memoized-iterator-snapshot.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/6/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/6/a/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/2/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/6/c/solution.md)
- [Functional programming, design and analysis of algorithms](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms-split.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/2/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/2/h/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/1/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/2/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/1/f/solution.md)
- [Sorted multiplicative closure stream](sorted-multiplicative-closure-stream.md)
