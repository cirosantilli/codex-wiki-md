# Simultaneous minimum and maximum

↑ **Parent:** [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)

The minimum and maximum of a nonempty [array](array-data-structure.md) can be found with at most $\lceil3n/2\rceil-2$ pairwise comparisons. Compare consecutive pairs once, retaining smaller entries as minimum candidates and larger entries as maximum candidates. If an entry is unpaired, put it into both candidate sets. Each candidate set has $\lceil n/2\rceil$ entries, and finding one extremum on $r$ entries uses $r-1$ comparisons. Thus the total is $\lfloor n/2\rfloor+2(\lceil n/2\rceil-1)$, equal to the stated bound; the singleton case uses zero. Balanced [divide-and-conquer algorithms](divide-and-conquer-algorithm.md) can perform both candidate reductions. Pairing is important: arbitrary equal splitting with only a two-element base case does not attain this comparison count at every size.

## ↑ Ancestors (4)

1. [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/5/b/solution.md)
