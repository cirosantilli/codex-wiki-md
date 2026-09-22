# Arc-consistency closure

↑ **Parent:** [Arc consistency](arc-consistency.md)

The greatest componentwise subdomains of given finite initial [constraint domains](constraint-domain.md) satisfying every directed [arc consistency](arc-consistency.md) condition, allowing empty subdomains. Repeated sound revisions to a fixed point produce this same closure regardless of revision order, provided every affected arc is eventually reconsidered.

For the proof, fix subdomains $E_i$ of the initial $D_i$ satisfying [arc consistency](arc-consistency.md). If all current $D_i$ contain $E_i$, every value in $E_i$ has a support in $E_j\subseteq D_j$, so revising $i\to j$ preserves $E_i$. [Mathematical induction](mathematical-induction.md) shows that every revision preserves every such family $E$. At termination the current domains themselves satisfy [arc consistency](arc-consistency.md), so they are the greatest such family. Algorithms that stop immediately on the first empty [constraint domain](constraint-domain.md) need not finish computing the closure, but correctly establish that no complete solution exists.

## ↑ Ancestors (8)

1. [Arc consistency](arc-consistency.md)
2. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
3. [Search problem](search-problem.md)
4. [Computational problem](computational-problem.md)
5. [Computational complexity theory](computational-complexity-theory.md)
6. [Theoretical computer science](theoretical-computer-science-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Full-sweep arc consistency](full-sweep-arc-consistency.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/3/b/solution.md)
