# Hilbert-Schmidt operators form a Hilbert space

↑ **Parent:** [Hilbert-Schmidt operator](hilbert-schmidt-operator.md)

On a [Hilbert space](hilbert-space-split.md) $X$ with a countable [Hilbertian basis](hilbertian-basis.md) $(e_k)$, the [Hilbert-Schmidt operators](hilbert-schmidt-operator.md) form a [Hilbert space](hilbert-space-split.md) under $\langle S,T\rangle=\sum_k\langle Se_k,Te_k\rangle$, using the same linearity convention as the [inner product](inner-product-split.md) on $X$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) proves convergence of this sum. The finite-sum [triangle inequality](triangle-inequality.md) and [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) give $\|T\|\leq\|T\|_2$. Thus a [Cauchy sequence](cauchy-sequence.md) $(T_n)$ in [Hilbert-Schmidt norm](hilbert-schmidt-norm.md) converges in [operator norm](operator-norm.md) to a [bounded linear operator](continuous-linear-operator.md) $T$. For $n,m\geq N$ with $\|T_n-T_m\|_2\leq\varepsilon$, taking $m\to\infty$ in each finite column sum gives $\sum_{k=1}^K\|(T_n-T)e_k\|^2\leq\varepsilon^2$ for every $K$. Taking the supremum over $K$ proves $T_n-T\in\mathcal S_2(X)$ and $\|T_n-T\|_2\leq\varepsilon$, so $T\in\mathcal S_2(X)$ and completeness follows.

## ↑ Ancestors (7)

1. [Hilbert-Schmidt operator](hilbert-schmidt-operator.md)
2. [Compact operator](compact-operator-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-functional-analysis-ii-course-of-the-university-of-oxford/2023/3/b/iii/solution.md)
