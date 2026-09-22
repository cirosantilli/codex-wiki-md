<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Test-driven development](../../../../../test-driven-development.md) uses a short cycle: write a test for the next behavior and observe its failure, implement enough to pass it, then refactor without changing the tested behavior. In a conventional implementation-then-test workflow, tests primarily assess code after it has been written; in TDD they also guide each small design increment. Tests accumulate into a regression suite, but passing them is not a universal correctness proof.[Definition: interleaved unit tests, implementation and refactoring](../../../../../test-driven-development-in-the-agile-alliance-glossary.md)

A good candidate is a deterministic [priority queue](../../../../../priority-queue.md) operation with a precise contract. Before implementation, test that inserting two equal values permits two minimum deletions and only then leaves an empty queue. The expected result is objective, cheap to check and useful for finding the duplicate-loss bug in a set-based representation.

An exploratory decision about whether an editor's toolbar feels usable is a poor candidate for TDD alone: the desired behavior and human evaluation criteria may not yet be settled, and an executable assertion does not replace user observation. Prototypes and usability evaluation can establish the design before stable behavioral properties are tested automatically. **The distinction is the availability of a useful repeatable test oracle**, not a claim that interface software is inherently untestable.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
