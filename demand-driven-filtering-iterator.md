# Demand-driven filtering iterator

↑ **Parent:** [Iterator](iterator.md)

An [iterator](iterator.md) adapter that consumes underlying values only far enough to find the next value passing a predicate. Store at most one passing value in an [optional value](optional-value.md). With no cached value, its abstract remainder is the filtered underlying remainder; with cached $x$, it is $x$ followed by that filtered remainder.

Construction performs no read. On `hasNext` or `next`, consume rejected values until one passes or the input is exhausted. Cache the passing value immediately and stop. Repeated availability tests reuse it. Returning it clears the cache without prefetching another value. This gives a precise demand boundary even when producing source values is expensive. Availability need not terminate on an infinite input with no further passing value.

## ↑ Ancestors (4)

1. [Iterator](iterator.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/imperative-programming/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/6/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/6/f/solution.md)
- [Prefix-dropping iterator](prefix-dropping-iterator.md)
