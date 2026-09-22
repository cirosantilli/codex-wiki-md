# First-vertex degree in the LCD model

↑ **Parent:** [Linearized chord diagram model](linearized-chord-diagram-model.md)

In a [uniform linearized chord diagram](uniform-linearized-chord-diagram.md), $\Pr(\sqrt nR_1\ge x)=(1-x^2/n)^n\to e^{-x^2}$. Conditional on the right endpoints, $d_1(n)=2+\sum_{i=2}^n\mathbf1_{\{L_i\le R_1\}}$, with [independent](independent-random-variables.md) success [probabilities](probability.md) $R_1/R_i$. A [Chernoff bound](chernoff-bound.md) gives $R_i=(1+o(1))\sqrt{i/n}$ uniformly for $i\ge n^{1/10}$. The early indicators are $o(\sqrt n)$, and the remaining conditional [mean](expected-value.md) is $(2+o(1))nR_1$. Their conditional [variance](variance-split.md) is $O_{\mathbb P}(\sqrt n)$. Hence $d_1(n)/\sqrt n-2\sqrt nR_1\to0$ in [probability](probability.md), proving the displayed tail limit. A [self-loop](loop-graph-theory.md)'s contribution is included in the constant two.

## ↑ Ancestors (8)

1. [Linearized chord diagram model](linearized-chord-diagram-model.md)
2. [Preferential attachment](preferential-attachment.md)
3. [Random graph](random-graph.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12/6/c/solution.md)
