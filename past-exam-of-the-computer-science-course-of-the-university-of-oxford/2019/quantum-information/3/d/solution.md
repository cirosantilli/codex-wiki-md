<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $N_0,N_1$ be the two output counts. Choose a known preparation unitary F with $F|0\rangle=N^{-1/2}\sum_x|x\rangle=:|s\rangle$. The [Deutsch-Jozsa algorithm](../../../../../deutsch-jozsa-algorithm.md) applies the supplied [phase oracle](../../../../../phase-oracle.md) $O_f|x\rangle=(-1)^{f(x)}|x\rangle$ and then $F^\dagger$, declaring constant exactly for outcome 0. Its amplitude on that outcome is

$$
\langle0|F^\dagger O_fF|0\rangle=\langle s|O_f|s\rangle=\frac{N_0-N_1}{N}.
$$

This is the [Deutsch-Jozsa test with an arbitrary uniform-state unitary](../../../../../deutsch-jozsa-test-with-an-arbitrary-uniform-state-unitary.md). For $N=2^m$, the usual preparation is $F=H^{\otimes m}$; the argument itself needs only a uniform preparation on the stated N-dimensional space.

For an actually constant-up-to-k function, the two counts are $k$ and $N-k$, so the outcome-0 [probability](../../../../../probability.md) is $(1-2k/N)^2$. The error is returning the other label. Therefore

$$
\boxed{P_{\rm error}=1-\left(1-\frac{2k}{N}\right)^2=\frac{4k}{N}\left(1-\frac{k}{N}\right).}
$$

Here the possible count k is nonnegative, and the supplied bound implies $0\le k/N\le1/8$. The error is consequently at most $7/16$; at $k=0$ it vanishes. This is the error conditional on the stated constant-up-to-k case, not an average over unspecified prior [probabilities](../../../../../probability.md). For comparison, the printed balanced-up-to-k definition has count _difference_ $\pm k$, so its outcome-0 [probability](../../../../../probability.md) would be $(k/N)^2$, not the expression for the constant-up-to-k case. No change to that promise definition is made.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
