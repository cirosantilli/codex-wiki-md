<h1 id="rademacher-johnson-lindenstrauss-transform">Rademacher Johnson–Lindenstrauss transform</h1>

↑ **Parent:** [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)

If $A\in\{-1,1\}^{d\times p}$ has independent [Rademacher](rademacher-distribution.md) entries, then for fixed $u\ne0$ and $0<t<1$,

$$
\mathbb P\left(\left|\frac{\lVert Au\rVert_2^2}{d\lVert u\rVert_2^2}-1\right|\geq t\right)
\leq2e^{-dt^2/136}.
$$

Applying a [union bound](boole-s-inequality.md) to all pairwise differences embeds $n$ fixed points into dimension $O(t^{-2}\log(n/\varepsilon))$ while preserving every squared distance within a factor $1\pm t$ with probability at least $1-\varepsilon$.

## ↑ Ancestors (7)

1. [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)
2. [Metric embedding](metric-embedding.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-205/3/a/solution.md)
