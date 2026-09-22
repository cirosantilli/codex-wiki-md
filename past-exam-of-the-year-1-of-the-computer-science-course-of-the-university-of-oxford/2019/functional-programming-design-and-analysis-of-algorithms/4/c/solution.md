<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**No universally correct sequential [Haskell](../../../../../haskell.md) implementation has that guarantee for [partial lists](../../../../../partial-list.md).** Compare `undefined` paired with `[v]`, and `[v]` paired with `undefined`, where the element type is arbitrary. A generic program cannot fabricate `v`; it must eventually inspect an input spine to obtain it. Whichever input it first demands can be chosen to be the undefined one, blocking access to the available element in the other input.

In particular, the implementation in part b can emit a defined prefix and then block when alternation reaches an undefined tail. [Lazy evaluation](../../../../../lazy-evaluation.md) postpones demands; it cannot recognize that a demanded computation will never finish. The result is the [partial-list interleaving obstruction](../../../../../partial-list-interleaving-obstruction.md), not an objection to fairness under the proper-input hypothesis. Additional concurrent primitives would change the computational model.[§3.1, errors and nontermination; §3.17, demands made by pattern matching](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
