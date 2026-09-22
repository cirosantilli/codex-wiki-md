# Expected query count for Simon sampling

↑ **Parent:** [Simon's algorithm](simon-s-algorithm.md)

With a nonzero hidden period, [Simon's algorithm](simon-s-algorithm.md) samples uniformly from its $(n-1)$-dimensional [orthogonal complement over the binary field](orthogonal-complement-over-the-binary-field.md). At rank $k$, a new sample raises the rank with probability $1-2^{k-(n-1)}$. Summing the geometric waiting times gives an expected $n-1+\sum_{j=1}^{n-1}(2^j-1)^{-1}<n+1$ queries. After $n-1+c$ samples, the probability of insufficient rank is less than $2^{-c}$, by a [union bound](boole-s-inequality.md) over the nonzero linear functionals that could annihilate all samples.

## ↑ Ancestors (8)

1. [Simon's algorithm](simon-s-algorithm.md)
2. [Simon's problem](simon-s-problem.md)
3. [Hidden subgroup problem](hidden-subgroup-problem.md)
4. [Quantum Fourier transform](quantum-fourier-transform.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/2/5/solution.md)
