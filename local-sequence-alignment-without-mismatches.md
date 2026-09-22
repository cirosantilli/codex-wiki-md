# Local sequence alignment without mismatches

↑ **Parent:** [Sequence alignment](sequence-alignment.md)

Choose one contiguous [substring](substring.md) from each [string](string.md) and align them under the same matching and gap rules as [global sequence alignment without mismatches](global-sequence-alignment-without-mismatches.md). Let $L_{i,j}$ maximize the score over aligned suffixes of the two prefixes. Zero permits a fresh empty alignment; the other cases extend one ending at adjacent prefix indices. The answer is the largest table entry, which can occur before either input ends. Starting all boundaries at zero yields $O(mn)$ time for positive lengths. [Alignment traceback](alignment-traceback.md) stops on reaching zero.

## ↑ Ancestors (5)

1. [Sequence alignment](sequence-alignment.md)
2. [Molecular genetics](molecular-genetics-split.md)
3. [Genetics](genetics-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Alignment traceback](alignment-traceback.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/8/e/solution.md)
