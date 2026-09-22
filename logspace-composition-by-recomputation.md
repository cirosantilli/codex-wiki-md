# Logspace composition by recomputation

↑ **Parent:** [Logspace-computable function](logspace-computable-function.md)

To simulate $g$ on the virtual [input](input-computer-science.md) $f(x)$, store the simulated [input](input-computer-science.md)-head position and rerun the [logspace transducer](logspace-transducer.md) for $f$ whenever an [input](input-computer-science.md) symbol is requested. Count emitted symbols until the requested position is reached. The intermediate output has [polynomial](polynomial-split.md) length, so its positions take $O(\log n)$ [bits](bit.md), and the work space of $g$ is also $O(\log n)$. Storage used by successive recomputations is reused. This proves closure of [logspace-computable functions](logspace-computable-function.md) under composition and transitivity of [logspace many-one reductions](logspace-many-one-reduction.md).

## ↑ Ancestors (9)

1. [Logspace-computable function](logspace-computable-function.md)
2. [Logspace transducer](logspace-transducer.md)
3. [Logarithmic space](logarithmic-space.md)
4. [Space complexity](space-complexity.md)
5. [Complexity class](complexity-class.md)
6. [Computational complexity theory](computational-complexity-theory.md)
7. [Theoretical computer science](theoretical-computer-science-split.md)
8. [Computer science](computer-science-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Binary addition in logarithmic space](binary-addition-in-logarithmic-space.md)
- [Logspace-computable function](logspace-computable-function.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-complexity/3/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-complexity/3/f/solution.md)
