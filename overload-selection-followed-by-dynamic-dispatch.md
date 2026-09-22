# Overload selection followed by dynamic dispatch

↑ **Parent:** [Object-oriented programming](object-oriented-programming.md)

To analyze an ordinary overloaded instance call, first enumerate members visible through the receiver's [static type](static-type.md) and choose the applicable signature using argument [static types](static-type.md). Only then use the receiver's [runtime type](runtime-type.md) to select the effective override of that signature. This two-stage rule explains why changing a reference's declared type can change the selected overload even when every reference points to the same object. A `super` call selects the inherited implementation according to the language's superclass or linearization rules instead of recursively redispatching to the overriding body.

## ↑ Ancestors (4)

1. [Object-oriented programming](object-oriented-programming.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/7/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/imperative-programming/6/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/5/b/solution.md)
