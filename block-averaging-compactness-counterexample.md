# Block averaging compactness counterexample

↑ **Parent:** [Compact operator](compact-operator-split.md)

For $1<p<\infty$, let $q=p/(p-1)$ and partition the coordinates into consecutive finite blocks $B_k$ of lengths $m_k\to\infty$. The displayed map defines a norm-one operator on the [l-p sequence space](l-p-sequence-space.md). By [Hölder's inequality](holder-s-inequality.md), $|(Tx)_k|^p\leq\sum_{j\in B_k}|x_j|^p$, giving the upper [norm](norm.md) bound. For the unit [vector](vector.md) $e_j$ with $j\in B_k$, $Te_j=m_k^{-1/q}e_k$, so its [norm](norm.md) tends to zero as $j\to\infty$.

Nevertheless, $x^{(k)}=m_k^{-1/p}\mathbf1_{B_k}$ has [norm](norm.md) one and maps to $e_k$. Those images are pairwise distance $2^{1/p}$ apart. Thus $T$ is not a [compact operator](compact-operator-split.md), and has [norm](norm.md) exactly one. Vanishing images of a chosen basis do not alone test [compactness](compact-space.md) on $\ell^p$ for $p>1$. The map is the adjoint of the isometric block embedding $(Uy)_j=m_k^{-1/q}y_k$, $j\in B_k$, on $\ell^q$.

## ↑ Ancestors (6)

1. [Compact operator](compact-operator-split.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-functional-analysis-course-of-the-university-of-oxford/2011/1/b/ii/solution.md)
