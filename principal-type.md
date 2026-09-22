# Principal type

↑ **Parent:** [Type inference](type-inference.md)

A [principal type](principal-type.md) is a most general valid type scheme: every other valid typing of the expression is obtained by substituting types for its quantified type variables, subject to any declared class constraints. For example, `\s x f y -> f (s y x)` has type `(u -> v -> w) -> v -> (w -> r) -> u -> r`; the application constraints require precisely these connections and no equality between the four type variables. A concrete typing is an instance, not evidence that the expression needs that particular type.

## ↑ Ancestors (5)

1. [Type inference](type-inference.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Hindley-Milner type inference](hindley-milner-type-inference.md)
- [K combinator](k-combinator.md)
- [Map (higher-order function)](map-higher-order-function.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/1/b/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/1/b/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/3/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/1/f/solution.md)
- [Principal type](principal-type.md)
