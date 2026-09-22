# Space-bound discovery by exit reachability

↑ **Parent:** [Savitch's theorem](savitch-s-theorem.md)

For a bounded-space machine, start with a logarithmic work budget and test accepting reachability and reachability of a transition leaving the budget. Accept if acceptance is found, double the budget if an exit is reachable, and otherwise reject. If all paths use at most $Cs(n)$ space, doubling stops at $O(s(n))$. Each budget test uses the [Savitch theorem](savitch-s-theorem.md) recursion and the storage is reused. The method discovers a sufficient bound without computing $s(n)$.

## ↑ Ancestors (8)

1. [Savitch's theorem](savitch-s-theorem.md)
2. [Nondeterministic space complexity class](nondeterministic-space-complexity-class.md)
3. [Space complexity](space-complexity.md)
4. [Complexity class](complexity-class.md)
5. [Computational complexity theory](computational-complexity-theory.md)
6. [Theoretical computer science](theoretical-computer-science.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-59/2/a/solution.md)
- [Savitch's theorem](savitch-s-theorem.md)
