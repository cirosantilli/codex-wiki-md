# Global sequence alignment without mismatches

↑ **Parent:** [Sequence alignment](sequence-alignment.md)

Align two complete [strings](string.md) using matching letters or a letter opposite a gap, with no unequal-letter columns and no double-gap columns. Give each match score one and each gap penalty $g\geq0$. The [dynamic programming](dynamic-programming.md) table for prefixes starts with $D_{i,0}=-gi$ and $D_{0,j}=-gj$. Its last-column cases give the displayed recurrence, where the diagonal candidate is omitted on a mismatch. Construction takes $O(mn)$ time for positive lengths and $O(mn)$ space with full [alignment traceback](alignment-traceback.md).

An alignment with $\ell$ matches has $m+n-2\ell$ gaps and score $(1+2g)\ell-g(m+n)$. Therefore a [longest common subsequence](longest-common-subsequence.md) determines its optimum. A finite mismatch penalty would solve a different problem.

## ↑ Ancestors (5)

1. [Sequence alignment](sequence-alignment.md)
2. [Molecular genetics](molecular-genetics-split.md)
3. [Genetics](genetics-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Alignment traceback](alignment-traceback.md)
- [Local sequence alignment without mismatches](local-sequence-alignment-without-mismatches.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/8/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/8/b/solution.md)
