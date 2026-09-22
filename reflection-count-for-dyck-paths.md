# Reflection count for Dyck paths

↑ **Parent:** [Dyck path](dyck-path.md)

There are $\binom{2n}{n}$ paths with $n$ up steps and $n$ down steps, ignoring the height constraint. For $n\geq1$, reflect the prefix of a bad path through its first visit to height $-1$, swapping its up and down steps. The resulting path has $n+1$ up steps and $n-1$ down steps, hence final height two. Its first visit to height one identifies the inverse reflection, so this is a [bijection](bijection.md). There are $\binom{2n}{n+1}$ bad paths. Subtracting gives

$$
C_n=\binom{2n}{n}-\binom{2n}{n+1}=\frac1{n+1}\binom{2n}{n}.
$$

This count connects a global nonnegative-height requirement to an unrestricted [binomial coefficient](binomial-coefficient-split.md). The case $n=0$ is separately the unique empty path.

## ↑ Ancestors (6)

1. [Dyck path](dyck-path.md)
2. [Lattice path](lattice-path.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
