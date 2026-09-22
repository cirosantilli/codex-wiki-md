# Multiplicative block-count language

↑ **Parent:** [Pumping lemma for context-free languages](pumping-lemma-for-context-free-languages.md)

This [formal language](formal-language.md) is not a [context-free language](context-free-language.md). For [pumping length](pumping-length.md) $p$, use $a^p b^{p^2}c^p$. A pumpable window of length at most $p$ cannot meet both outer blocks. If pumping adds $\alpha,\beta,\gamma$ copies of $a,b,c$, then $\alpha\gamma=0$ and $1\leq\alpha+\beta+\gamma\leq p$. Preserving the product constraint would require $\beta=p(\alpha+\gamma)$, impossible both when $\alpha+\gamma=0$ and when it is positive. This contradicts the [pumping lemma for context-free languages](pumping-lemma-for-context-free-languages.md).

## ↑ Ancestors (6)

1. [Pumping lemma for context-free languages](pumping-lemma-for-context-free-languages.md)
2. [Formal language theory](formal-language-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/models-of-computation/3/c/ii/solution.md)
