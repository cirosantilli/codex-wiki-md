# Left scan

↑ **Parent:** [Left fold](left-fold.md)

Return the successive accumulator values of a [left fold](left-fold.md), including the initial accumulator: `scanl f e [] = [e]` and `scanl f e (x:xs) = e : scanl f (f e x) xs`. The $k$th result is the fold of the first $k$ elements, proved by the fold equation. Thus the scan equals `map (foldl f e) . inits`, but computes $n$ updates instead of $n(n+1)/2$ on a finite input of length $n$. Accumulator strictness and the cost of an update remain separate from this operation count.

## ↑ Ancestors (5)

1. [Left fold](left-fold.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/4/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/4/c/solution.md)
