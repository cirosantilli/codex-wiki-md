# Information from two conditionally independent observations

↑ **Parent:** [Conditional mutual information](conditional-mutual-information.md)

If outputs $V,W$ are [conditionally independent](conditional-independence.md) given $U$, then $H(V,W\mid U)=H(V\mid U)+H(W\mid U)$. Expanding the [entropy](information-entropy-split.md) expressions proves the displayed [mutual information](mutual-information.md) identity. The chain rule also gives $I(U;V,W)\geq\max\{I(U;V),I(U;W)\}$, while the identity and nonnegativity give the upper bound by their [sum](sum.md). For two [channels](communication-channel.md) with common input and [independent](independent-random-variables.md) output noise conditional on that input, maximizing over the input law therefore bounds the joint-output [capacity](channel-capacity.md) between the larger marginal [capacity](channel-capacity.md) and the [sum](sum.md) of the two marginal capacities. Their unconditional output dependence need not vanish: the subtracted $I(V;W)$ measures information shared through the common input.

## ↑ Ancestors (7)

1. [Conditional mutual information](conditional-mutual-information.md)
2. [Mutual information](mutual-information.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2011/3/c/solution.md)
