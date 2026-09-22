# Capacity of a disjoint sum of channels

↑ **Parent:** [Channel capacity](channel-capacity.md)

Combine finitely many [discrete memoryless channels](discrete-memoryless-channel.md) with disjoint input [alphabets](alphabet.md) and disjoint output [alphabets](alphabet.md) into a block-diagonal [channel](communication-channel.md). The block label $B$ is determined by both input and output. If it has law $\alpha$, the [mutual information](mutual-information.md) is at most $H(\alpha)+\sum_i\alpha_iC_i$, attained by using each block's capacity-achieving conditional input law. Put $S=\sum_i2^{C_i}$ and $r_i=2^{C_i}/S$. The expression equals $\log_2S-d(\alpha,r)$, so [Gibbs inequality](gibbs-inequality.md) proves the displayed [capacity](channel-capacity.md), attained for block [probabilities](probability.md) $\alpha_i=r_i$. Even blocks of [capacity](channel-capacity.md) zero contribute distinguishable block choices; three disjoint zero-capacity blocks give [capacity](channel-capacity.md) $\log_2 3$.

## ↑ Ancestors (6)

1. [Channel capacity](channel-capacity.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2011/3/b/i/solution.md)
