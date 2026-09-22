# List unfold

↑ **Parent:** [Functional programming](functional-programming.md)

Generate a [list](list-abstract-data-type.md) from a state: a step returning `Nothing` terminates; `Just (x,s')` emits `x` and continues from `s'`. Thus `unfoldr step s = case step s of Nothing -> []; Just (x,s') -> x : unfoldr step s'`. A [list unfold](list-unfold.md) decomposes the evolving state, whereas a [list fold](list-fold.md) consumes existing constructors. [Productivity](stream-productivity.md) depends on each demanded constructor becoming available, not merely on using [lazy evaluation](lazy-evaluation.md).

**Table of contents**

- [Filtering a list by unfolding](filtering-a-list-by-unfolding.md)

## ↑ Ancestors (4)

1. [Functional programming](functional-programming.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [List unfold](list-unfold.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/d/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms-resit/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms-resit/4/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/3/d/solution.md)
