# Lower type bound

↑ **Parent:** [Subtyping](subtyping.md)

A lower bound requires an admissible [type argument](type-argument.md) to be a [supertype](supertype.md) of a specified type. In [Scala](scala.md), `[V >: U]` means $U<:V$. For an immutable [software class](class-programming.md) covariant in `U`, a method accepting a new output value cannot consume `U` directly in a contravariant method-parameter position. Instead, `add[V >: U](x: V)` accepts a possibly wider value and returns a fresh instance parameterized by `V`. The original narrower instance remains unchanged. The [variance-position rule](variance-position-rule.md) and [subtyping](subtyping.md) justify this widening; a bound alone does not authorize mutating an existing instance through a widened reference.[Variance Annotations, lower-bound widening in the Sequence.append example](scala-2-13-variance-annotations-specification.md)

## ↑ Ancestors (5)

1. [Subtyping](subtyping.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Covariant persistent multiset](covariant-persistent-multiset.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/8/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/8/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/6/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming-resit/6/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/8/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/7/e/solution.md)
- [Supertype](supertype.md)
