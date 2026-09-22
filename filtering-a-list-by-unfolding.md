# Filtering a list by unfolding

↑ **Parent:** [List unfold](list-unfold.md)

For a [predicate](predicate.md) $p$, normalize the state to the first remaining passing element with `seek = dropWhile (not . p)`. Stop on an empty state, otherwise emit its head and continue from `seek (tail state)`. The invariant is that every nonempty state starts with a passing element. An initial `seek` establishes it; removing the emitted head and seeking again preserves it. Each rejected run is traversed once, giving [linear time](linear-time.md) in the examined input prefix under constant-cost predicate tests.

## ↑ Ancestors (5)

1. [List unfold](list-unfold.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms-resit/4/f/solution.md)
