# Finite cross entropy bounds countable information entropy

↑ **Parent:** [Information entropy](information-entropy-split.md)

Let $p$ and $g$ be [probability mass functions](probability-mass-function.md) on a countable [alphabet](alphabet.md), with $g_i>0$ whenever $p_i>0$. If the [cross-entropy](cross-entropy.md) $C=-\sum_i p_i\log_2g_i$ is finite, then $H(p)$ is finite, $H(p)\leq C$, and $D(p\|g)=C-H(p)$. To avoid assuming the desired finiteness, first apply $\ln u\leq u-1$ with $u=g_i/p_i$ to each positive $p_i$. For a finite initial segment,

$$
\sum_{i=0}^N-p_i\log_2p_i\leq\sum_{i=0}^N-p_i\log_2g_i+\frac{\sum_{i=0}^N(g_i-p_i)}{\ln2}.
$$

Zero coordinates satisfy this inequality too. [Monotone convergence](monotone-convergence-theorem.md) of the nonnegative [information entropy](information-entropy-split.md) summands and convergence of both total masses give $H(p)\leq C<\infty$. Both logarithmic sums are then finite, justifying their difference and the [relative entropy](kullback-leibler-divergence.md) identity. This supplies a rigorous route to the [maximum entropy distribution on the nonnegative integers](maximum-entropy-distribution-on-the-nonnegative-integers.md) without presupposing finite [information entropy](information-entropy-split.md) for every competing law.

## ↑ Ancestors (6)

1. [Information entropy](information-entropy-split.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/1/c/solution.md)
