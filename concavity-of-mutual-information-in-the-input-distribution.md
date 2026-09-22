# Concavity of mutual information in the input distribution

↑ **Parent:** [Mutual information](mutual-information.md)

For a fixed finite [discrete memoryless channel](discrete-memoryless-channel.md) $W$, the function $p\mapsto I_p(X;Y)$ is concave on the input probability simplex. Indeed, the induced output law $q=pW$ is linear in $p$, the output [Shannon entropy](information-entropy-split.md) $H(q)$ is concave, and $H(Y\mid X)=\sum_xp(x)H(W(\cdot\mid x))$ is linear. Their difference is therefore concave. Equivalently, at a mixture $p=\lambda p_1+(1-\lambda)p_2$, the concavity gap is $\lambda D(q_1\Vert q)+(1-\lambda)D(q_2\Vert q)\geq0$ by [Gibbs inequality](gibbs-inequality.md). Thus every local maximum is a global maximum, and averaging over symmetries of the fixed channel cannot decrease [mutual information](mutual-information.md).

## ↑ Ancestors (6)

1. [Mutual information](mutual-information.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2010/3/b/solution.md)
