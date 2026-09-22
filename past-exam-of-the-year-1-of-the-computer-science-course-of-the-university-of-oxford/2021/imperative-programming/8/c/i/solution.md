<h1 id="8/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The pipe [object interface](../../../../../../object-interface.md) supports **[command-query separation](../../../../../../command-query-separation.md)**: consuming an input changes state, while querying the result observes the current output without feeding another input. A client can inspect the result repeatedly, including an initial result when the concrete pipe defines one. That is useful for accumulated statistics.

The channel [object interface](../../../../../../object-interface.md) instead packages an input update and its associated output into one call. For request-and-result processing this is simpler: the caller cannot forget which update precedes a query. A pipe caller must respect the intended order of operations, and interleaving other callers between consume and result can change the observation. A single channel [object method](../../../../../../object-method.md) is not automatically thread-safe either; synchronization is a separate property.

**Neither [object interface](../../../../../../object-interface.md) is universally better.** The choice depends on whether clients need independent observation of state or a combined transformation step. The adapters below can reconcile their protocols, provided the initial-result policy is made explicit.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
