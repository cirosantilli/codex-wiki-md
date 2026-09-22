# Entropy potential for a divide-and-conquer recurrence

↑ **Parent:** [Recursion tree](recursion-tree.md)

If $0<m<n$, the displayed identity expresses the decrease of the potential $n\log_2n$ across a split. Here $H_2(a)=-a\log_2a-(1-a)\log_2(1-a)$ is the [binary entropy function](binary-entropy-function.md). If every split fraction stays in $[\delta,1-\delta]$ for a fixed $0<\delta\leq1/2$, the potential decreases by at least $nH_2(\delta)>0$. Consequently, for a [recurrence relation](recurrence-relation.md) with linear work at each split, the [inductive hypothesis](induction-hypothesis.md) $T(n)\leq A n\log_2n+B n$ closes when $A H_2(\delta)\geq1$ and $B$ covers the base cases. This is a proof by the [substitution method for a recurrence](substitution-method-for-a-recurrence.md) of an $O(n\log n)$ [time complexity](time-complexity.md) bound without requiring equal subproblem sizes.

## ↑ Ancestors (5)

1. [Recursion tree](recursion-tree.md)
2. [Recursion (computer science)](recursion-computer-science.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Integer rounding in a divide-and-conquer recurrence](integer-rounding-in-a-divide-and-conquer-recurrence.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/discrete-mathematics-continuous-mathematics-and-probability/3/e/i/solution.md)
- [Substitution method for a recurrence](substitution-method-for-a-recurrence.md)
