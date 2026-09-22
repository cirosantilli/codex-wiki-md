<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

A single bucket holding about a quarter of all keys suggests **severely nonuniform hashing or a strongly skewed/adversarial key set**, rather than ordinary load growth alone. With one hundred well-used buckets the expected fraction in one fixed bucket is about one hundredth. Persistent concentration near one quarter is evidence to investigate, not a proof identifying one particular implementation bug.

Inspect the bucket histogram, raw hash outputs and patterns in the names. A hash depending only on an initial character, weak mixing of common prefixes, or an indexing rule using few possible buckets could create this behavior. Improve the hash so that it uses the complete key and spreads this workload across the table, then rehash every stored entry. Check the valid-index rule as well, including negative machine hash values.

Increasing the table size is useful if index reduction caused the concentration; **it cannot separate keys that all receive the same raw hash**. For maliciously chosen keys, randomized or keyed hashing and balanced collision structures may be appropriate. The observed occupancy does not justify assuming uniformly random hashes in a performance claim.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
