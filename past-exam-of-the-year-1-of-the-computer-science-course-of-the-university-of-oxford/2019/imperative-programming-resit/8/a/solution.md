<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Test-driven development](../../../../../test-driven-development.md) interleaves three small steps: write a test expressing the next required behavior and observe that it fails, implement enough behavior to make it pass, then improve the code's structure while keeping the tests passing. The retained tests become a regression suite. For example, before implementing a book deletion, test that deleting an existing contact removes it and returns true; later add the absent-name case. Each test guides a small implementation step rather than waiting for a finished component.[What is TDD?: interleaving unit tests, implementation and refactoring in a short cycle](../../../../../test-driven-development-in-the-agile-alliance-glossary.md)

Compared with a traditional write-the-component-then-test workflow, **tests guide the design before each increment is implemented**. This does not imply that all non-TDD testing is postponed until a whole product is finished, or that TDD eliminates broader integration testing.

The test-first behavioral core is naturally [black-box testing](../../../../../black-box-testing.md): expected outcomes come from the operation's contract. Later tests can use internal control flow or representation cases, becoming [white-box testing](../../../../../white-box-testing.md). Thus a complete practice can use **a mixture, with mainly contract-based black-box tests driving the next behavior**. The classification depends on how test cases are chosen, not on whether the programmer personally knows the implementation. Passing a finite suite is not a proof of universal correctness.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
