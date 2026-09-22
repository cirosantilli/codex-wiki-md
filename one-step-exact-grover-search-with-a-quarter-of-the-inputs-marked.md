# One-step exact Grover search with a quarter of the inputs marked

↑ **Parent:** [Exact amplitude amplification](exact-amplitude-amplification.md)

Start from $|s\rangle=N^{-1/2}\sum_x|x\rangle$, negate amplitudes at marked indices, and apply $2|s\rangle\langle s|-I$. If the marked fraction is $r$, the oracle-state mean amplitude is $(1-2r)/\sqrt N$. [Inversion about the mean](inversion-about-the-mean.md) therefore gives amplitudes $(1-4r)/\sqrt N$ on unmarked indices and $(3-4r)/\sqrt N$ on marked ones. The marked success [probability](probability.md) is $r(3-4r)^2$. At $r=1/4$ it is exactly one: unmarked amplitudes vanish and each marked amplitude is $2/\sqrt N$. The output is uniform among the $N/4$ marked indices. This is an exact special case of [Grover's algorithm](grover-s-algorithm.md), using one [phase oracle](phase-oracle.md) call under the stated promise.

## ↑ Ancestors (6)

1. [Exact amplitude amplification](exact-amplitude-amplification.md)
2. [Amplitude amplification](amplitude-amplification.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/quantum-information/3/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/quantum-information/3/e/solution.md)
