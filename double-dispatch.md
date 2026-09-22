# Double dispatch

↑ **Parent:** [Dynamic dispatch](dynamic-dispatch.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double_dispatch)

Select behavior using the runtime types of two participating [software objects](software-object.md), typically through two virtual method calls. A method on the first participant calls a virtual method on the second, passing `this` with the concrete static type established in that second method's class. [Method overloading](method-overloading.md) there selects a signature, after which [dynamic dispatch](dynamic-dispatch.md) selects the implementation on the other runtime receiver. This differs from expecting ordinary overload resolution to inspect a method argument's runtime class.

## ↑ Ancestors (5)

1. [Dynamic dispatch](dynamic-dispatch.md)
2. [Object-oriented programming](object-oriented-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/7/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming-resit/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming-resit/8/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/7/d/solution.md)
- [Visitor pattern](visitor-pattern.md)
