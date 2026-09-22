# Verified Grover promise test

↑ **Parent:** [Grover's algorithm](grover-s-algorithm.md)

Under the promise of either no marked entry or one marked entry in an $N$-element [Boolean quantum oracle](boolean-quantum-oracle.md) search space, run the [Grover search algorithm](grover-s-algorithm.md) for the displayed number of iterations, measure a candidate, and make one additional oracle query to check it. Since $|(2k+1)\theta-\pi/2|\leq\theta$, the marked-entry success probability is at least $\cos^2\theta=1-1/N$. For $N\geq4$ this is at least $3/4$. If no entry is marked the verification never accepts, so there is no false positive. The query count is $k+1=O(\sqrt N)$ because $\theta\geq1/\sqrt N$. Measuring a candidate without verification would not determine whether a marked entry exists.

## ↑ Ancestors (5)

1. [Grover's algorithm](grover-s-algorithm.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/1/c/solution.md)
