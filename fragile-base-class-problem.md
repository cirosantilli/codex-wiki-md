# Fragile base class problem

↑ **Parent:** [Class inheritance](class-inheritance.md)

A subclass may depend on its superclass's internal calls to overridable [object methods](object-method.md). A base implementation change that preserves the base abstraction can then change subclass behavior. For example, a set subclass may count insertion attempts by overriding insertion. If a revised deletion operation rebuilds the set by dynamically dispatched clear and insert calls, it unexpectedly resets and increases that counter. [Object composition](object-composition.md) can isolate the counting wrapper from the component's internal dispatch, provided only wrapper operations can mutate the owned component.

## ↑ Ancestors (5)

1. [Class inheritance](class-inheritance.md)
2. [Object-oriented programming](object-oriented-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/7/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/imperative-programming/6/e/solution.md)
