<h1 id="fekete-s-lemma">Fekete's lemma</h1>

↑ **Parent:** [Sequence and series](sequence-and-series.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fekete's_lemma)

For a real [subadditive sequence](subadditive-sequence.md) $(x_n)_{n\geq1}$, the normalized [sequence](sequence.md) has the extended-real [limit of a sequence](limit-of-a-sequence.md)

$$
\lim_{n\to\infty}\frac{x_n}{n}=\inf_{k\geq1}\frac{x_k}{k}\in[-\infty,\infty).
$$

No lower-bound hypothesis is needed for this conclusion. The [limit of a sequence](limit-of-a-sequence.md) is finite precisely when the ratios are bounded below. The example $x_n=-n^2$ is a [subadditive sequence](subadditive-sequence.md) with normalized [limit of a sequence](limit-of-a-sequence.md) $-\infty$.

To prove the result, fix $k\geq1$ and, for $n\geq k$, write $n=qk+r$ with $q\geq1$ and $0\leq r<k$. Iterating [subadditivity](subadditive-sequence.md) gives $x_n\leq qx_k+C_k$, where $C_k=\max(0,x_1,\ldots,x_{k-1})$ and $C_1=0$. Hence $\limsup_n x_n/n\leq x_k/k$ for every $k$. Every ratio is at least their [infimum](infimum.md). If that [infimum](infimum.md) is finite these bounds identify the [limit of a sequence](limit-of-a-sequence.md); if it is $-\infty$, choosing $k$ with an arbitrarily negative ratio gives convergence to $-\infty$.

## ↑ Ancestors (6)

1. [Sequence and series](sequence-and-series.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Almost-additive partition-function limit](almost-additive-partition-function-limit.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-55/4/ii/solution.md)
