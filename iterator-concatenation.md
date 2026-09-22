# Iterator concatenation

↑ **Parent:** [Iterator](iterator.md)

Consume the first [iterator](iterator.md) until it is exhausted, then consume the second. Short-circuit availability testing avoids polling the second producer while the first still has entries. Construction need not request any entry. If both wrappers share an underlying cursor, however, draining the first may also consume entries the second would otherwise have returned.

## ↑ Ancestors (4)

1. [Iterator](iterator.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/6/d/solution.md)
