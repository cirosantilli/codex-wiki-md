# Memento pattern

↑ **Parent:** [Object-oriented programming](object-oriented-programming.md)

A design in which an originator creates an opaque snapshot of its state, a caretaker retains it, and the originator can later restore it. [Encapsulation](encapsulation-computer-programming.md) prevents the caretaker from depending on internal state representation. A memento must freeze the relevant state: references to mutable objects can require a [deep copy](deep-copy.md), while immutable values can safely be shared. [Scala](scala.md)'s access controls and [path-dependent types](path-dependent-type.md) can restrict snapshot construction and associate it with its originating instance.

## ↑ Ancestors (4)

1. [Object-oriented programming](object-oriented-programming.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Command pattern](command-pattern.md)
- [Deep copy](deep-copy.md)
- [Inverse command correctness](inverse-command-correctness.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/6/c/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/6/c/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/7/a/solution.md)
- [Software design pattern](software-design-pattern.md)
