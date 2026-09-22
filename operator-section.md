# Operator section

↑ **Parent:** [Haskell](haskell.md)

A partially applied infix operator: `(a op)` means `\x -> a op x`, and `(op b)` means `\x -> x op b`, subject to [Haskell](haskell.md)'s syntax rules. In particular, `(f .)` maps a [function](function-split.md) `g` to the [function composition](function-composition.md) `f . g`. Composing such a section with a curried binary [function](function-split.md) composes at two argument levels: `((f .) . g) x y = f (g x y)` on total inputs.[§3.5, Sections](haskell-2010-language-report.md)

## ↑ Ancestors (4)

1. [Haskell](haskell.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/1/b/solution.md)
