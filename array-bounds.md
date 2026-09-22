# Array bounds

↑ **Parent:** [Array index](array-index.md)

The permitted [array indices](array-index.md) for a length-$n$ [array](array-data-structure.md) are $0,\ldots,n-1$ under zero-based indexing. A one-past-the-end index $n$ can describe an empty remaining segment but cannot be dereferenced. Proving bounds safety requires showing that every executed read and write uses a permitted index, including evaluations in a loop guard. A known target inside the array can sometimes supply a stronger [loop invariant](loop-invariant.md) than an explicit bounds test.

## ↑ Ancestors (5)

1. [Array index](array-index.md)
2. [Array (data structure)](array-data-structure.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/compilers/3/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/compilers/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/2/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/4/a/solution.md)
