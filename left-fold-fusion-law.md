# Left-fold fusion law

↑ **Parent:** [Left fold](left-fold.md)

If $f$ is a [strict function](strict-function.md) and $f(g(a,x))=h(f(a),x)$ for every $a,x$, then `f (foldl g a xs) = foldl h (f a) xs`. Prove the equation simultaneously for all accumulators by [structural induction](structural-induction.md) on the [list](list-abstract-data-type.md). The empty case is immediate; at a cons, apply the hypothesis with accumulator `g a x` and then rewrite its image using the assumed equation. At the [bottom value](bottom-value.md), strictness supplies the required equality. For pure definable [functions](function-split.md), equality on finite [partial lists](partial-list.md) extends to infinite [lazy lists](lazy-list.md) by finite approximations. For finite terminating spines alone, strictness is unnecessary.

## ↑ Ancestors (5)

1. [Left fold](left-fold.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/1/c/solution.md)
