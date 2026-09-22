# Finite column sum does not imply boundedness

↑ **Parent:** [Hilbert-Schmidt operator](hilbert-schmidt-operator.md)

An everywhere-defined [linear operator](linear-operator.md) $T$ on an infinite-dimensional [separable Hilbert space](separable-hilbert-space.md) need not be bounded merely because $\sum_k\|Te_k\|^2<\infty$ for a [Hilbertian basis](hilbertian-basis.md) $(e_k)$. Let $v=\sum_{k\geq1}2^{-k}e_k$, extend $\{e_k:k\geq1\}\cup\{v\}$ to a [Hamel basis](basis.md), and let the [linear functional](linear-functional.md) $\phi$ equal one on $v$ and zero on every other basis vector. Then $Tx=\phi(x)e_1$ has $Te_k=0$ for every $k$ but $Tv=e_1$. For $v_N=\sum_{k=1}^N2^{-k}e_k$, $v-v_N\to0$ while $T(v-v_N)=e_1$, proving discontinuity. Thus the definition of a [Hilbert-Schmidt operator](hilbert-schmidt-operator.md) must require boundedness, or first define the operator on finite [linear combinations](linear-combination.md) and take its unique continuous extension.

## ↑ Ancestors (7)

1. [Hilbert-Schmidt operator](hilbert-schmidt-operator.md)
2. [Compact operator](compact-operator-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-functional-analysis-ii-course-of-the-university-of-oxford/2023/3/b/i/solution.md)
