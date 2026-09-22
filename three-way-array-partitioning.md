# Three-way array partitioning

↑ **Parent:** [Two-way array partition](two-way-array-partition.md)

Maintain consecutive regions less than a saved pivot value, equal to it, unclassified, and greater than it. Compare the first unclassified entry: move a smaller one into the lower region, advance over an equal one, or exchange a greater one with the final unclassified entry. In the last case the incoming entry still needs classification. Each step shortens the unclassified interval by one. The final equality interval is nonempty when the pivot was selected from the input; [Quickselect](quickselect.md) can discard that entire interval when searching another rank. Saving the value avoids accidentally comparing against a pivot index whose contents have moved.

## ↑ Ancestors (4)

1. [Two-way array partition](two-way-array-partition.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/4/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/2/a/solution.md)
