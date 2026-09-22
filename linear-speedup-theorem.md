# Linear speedup theorem

↑ **Parent:** [Time complexity](time-complexity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_speedup_theorem)

For every constant $c>0$, a deterministic [multitape Turing machine](multitape-turing-machine.md) with more than one tape and [time complexity](time-complexity.md) bounded by $T(n)$ has an equivalent machine with the same tape count and bound $T(n)/c+n+O(1)$, allowing a larger finite control and tape [alphabet](alphabet.md). Blocks of old symbols become single new symbols, and finite control implements blocks of old steps. The linear overhead accounts for initial [input](input-computer-science.md) packing. If $T(n)/n\to\infty$, the overhead can be absorbed to obtain any fixed constant speed increase for sufficiently large [inputs](input-computer-science.md). This does not supply unlimited speed increases for operations on fixed hardware.[Slides 47–48, PDF pp. 62–63: formal statement and block-simulation construction](computational-complexity-slides-1-by-paul-w-goldberg-2023.md)

## ↑ Ancestors (6)

1. [Time complexity](time-complexity.md)
2. [Complexity class](complexity-class.md)
3. [Computational complexity theory](computational-complexity-theory.md)
4. [Theoretical computer science](theoretical-computer-science-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Computational Complexity, slides 1 by Paul W. Goldberg (2023)](computational-complexity-slides-1-by-paul-w-goldberg-2023.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-complexity/2/b/solution.md)
