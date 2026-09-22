# Conditioned entropic Ruzsa distance of a summand

↑ **Parent:** [Conditional entropic Ruzsa distance](conditional-entropic-ruzsa-distance.md)

If $U,V,X$ are independent random variables in $\mathbb F_2^n$, then

$$
d_R(U\mid U+V;X)
\leq\frac12\bigl(d_R(U;X)+d_R(V;X)+d_R(U;V)\bigr).
$$

Indeed, [conditioning reduces entropy](conditioning-reduces-entropy.md) and independence give

$$
d_R(U\mid U+V;X)
\leq H(U+X)-\frac12H(U)-\frac12H(V)
+\frac12H(U+V)-\frac12H(X).
$$

In $\mathbb F_2^n$, $V=U+(U+V)$, so [conditional entropy under a deterministic change of variables](conditional-entropy-under-a-deterministic-change-of-variables.md) shows that the left-hand side is unchanged when $U$ and $V$ are exchanged. Averaging the displayed bound with its exchanged version gives the result.

## ↑ Ancestors (7)

1. [Conditional entropic Ruzsa distance](conditional-entropic-ruzsa-distance.md)
2. [Entropic Ruzsa distance](entropic-ruzsa-distance.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/4/ii/solution.md)
