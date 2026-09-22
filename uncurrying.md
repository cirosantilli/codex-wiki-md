# Uncurrying

↑ **Parent:** [Currying](currying.md)

Convert a curried [function](function-split.md) into one taking a [tuple](finite-tuple.md): `uncurry f (x,y) = f x y`. Conversely, `curry f x y = f (x,y)`. The two conversions undo each other on total arguments. Uncurrying lets `map` apply a curried [binary operation](binary-operation.md) to each [tuple](finite-tuple.md) in a zipped [list](list-abstract-data-type.md).

## ↑ Ancestors (10)

1. [Currying](currying.md)
2. [Exponential object](exponential-object.md)
3. [Cartesian closed category](cartesian-closed-category.md)
4. [Adjoint functors](adjoint-functors.md)
5. [Category](category-split.md)
6. [Category theory](category-theory-split.md)
7. [Foundations of mathematics](foundations-of-mathematics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Curried function](curried-function.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/1/a/solution.md)
