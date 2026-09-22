# Array local maximum

↑ **Parent:** [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)

An entry of a finite [array](array-data-structure.md) which strictly exceeds each existing immediate neighbour. At either endpoint only one neighbour is tested, and the unique entry of a singleton qualifies vacuously. For distinct entries, a [divide-and-conquer algorithm](divide-and-conquer-algorithm.md) finds such an entry in $O(\log n)$ time. Maintain an index interval whose left endpoint exceeds the excluded entry immediately to its left, if any, and whose right endpoint exceeds the excluded entry immediately to its right, if any. If a midpoint has a larger internal neighbour, recurse towards it; the comparison supplies the new boundary inequality. Otherwise the midpoint exceeds its internal neighbours and the boundary inequalities cover any external neighbour. Halving the interval and preserving this [recursion invariant](recursion-invariant.md) proves correctness and the bound.

## ↑ Ancestors (4)

1. [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/5/d/solution.md)
