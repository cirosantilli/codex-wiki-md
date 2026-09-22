# Finite candidate elimination bound

↑ **Parent:** [Algorithm](algorithm-split.md)

Suppose a finite candidate [set](set-split.md) of size $N$ contains the truth, every query chooses a current candidate, and each wrong reply eliminates that candidate while retaining the truth. Then at most $N-1$ wrong queries occur. If a correct reply uniquely identifies the truth, an infinite strategy of this kind eventually repeats the true candidate; stopping when only one candidate remains takes at most $N-1$ replies. The proof is the strictly decreasing positive [cardinality](cardinality.md) of the surviving candidate set after every nonidentifying round.

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/3/e/solution.md)
