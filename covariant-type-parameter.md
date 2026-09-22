# Covariant type parameter

↑ **Parent:** [Parametric polymorphism](parametric-polymorphism.md)

A parameter position for which $S<:T$ implies $F[S]<:F[T]$. In [Scala](scala.md), it is annotated `+`. An immutable producer can return narrower values where broader values are expected. A method consuming that parameter directly would generally make covariance unsafe, since a widened reference could then receive unsupported inputs.

**Table of contents**

- [Covariance failure for a mutable collection](covariance-failure-for-a-mutable-collection.md)

## ↑ Ancestors (5)

1. [Parametric polymorphism](parametric-polymorphism.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Covariant persistent multiset](covariant-persistent-multiset.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/8/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/8/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/8/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/6/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming-resit/6/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/7/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/6/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/6/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/8/a/solution.md)
- [Type variance](type-variance.md)
