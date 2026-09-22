# Reference aliasing

↑ **Parent:** [Memory reference](memory-reference.md)

Two program references designate the same mutable object or overlapping mutable state. Binary-update contracts must account for this possibility: an update intended to combine two old values should snapshot both operands before modifying the receiver. A frame condition preserving a distinct operand cannot literally preserve a second reference that aliases the modified receiver.

## ↑ Ancestors (4)

1. [Memory reference](memory-reference.md)
2. [Computer memory](computer-memory-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/object-oriented-programming/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming-resit/7/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/7/b/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/imperative-programming-resit/8/e/i/solution.md)
- [Prototype pattern](prototype-pattern.md)
- [Software object](software-object.md)
