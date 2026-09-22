# Monotonicity of normalized subset entropies

↑ **Parent:** [Normalized subset entropy](normalized-subset-entropy.md)

For discrete [random variables](random-variable-split.md), [normalized subset entropy](normalized-subset-entropy.md) decreases with subset size. For finite entropies, the [chain rule for information entropy](chain-rule-for-information-entropy.md) and [conditioning reduces entropy](conditioning-reduces-entropy.md) give $\sum_{i\in S}h(X_{S\setminus\{i\}})\geq(|S|-1)h(X_S)$. Sum this over all $k$-subsets $S$. Every $(k-1)$-subset occurs $n-k+1$ times, and $k\binom nk=(n-k+1)\binom n{k-1}$ cancels the normalization factors. This proves $h_k^{(n)}\leq h_{k-1}^{(n)}$. If a marginal entropy is infinite, every one of these subset averages is infinite; otherwise all entropies used in the proof are finite.

## ↑ Ancestors (9)

1. [Normalized subset entropy](normalized-subset-entropy.md)
2. [Han's entropy inequality](han-s-entropy-inequality.md)
3. [Han's inequality for relative entropy](han-s-inequality-for-relative-entropy.md)
4. [Kullback-Leibler divergence](kullback-leibler-divergence.md)
5. [f-divergence](f-divergence.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-33/2/solution.md)
