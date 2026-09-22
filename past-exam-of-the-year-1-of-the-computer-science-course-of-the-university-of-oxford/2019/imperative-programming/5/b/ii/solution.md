<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Not automatically: the duplicate-value policy must implement a [multiset](../../../../../../multiset.md).** A strict [binary search tree](../../../../../../binary-search-tree.md) storing one entry per distinct key represents a [set](../../../../../../set-split.md); inserting a second equal value then loses a required occurrence. A fixed rule that puts all equal values on one side also needs care, because ordinary balancing rotations need not preserve that one-sided equality rule.

One valid refinement stores a multiplicity at each distinct key. Inserting an equal key increments its count; `delMin` decrements the minimum key's count and removes that node only at zero. Alternatively, use distinct internal keys such as `(value, uniqueSerial)` while ordering primarily by value and returning only the value. With an appropriate balanced representation either approach preserves every occurrence and the required operation bounds. A bare claim about balanced search trees, with no treatment of duplicates, does not establish the abstract specification.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
