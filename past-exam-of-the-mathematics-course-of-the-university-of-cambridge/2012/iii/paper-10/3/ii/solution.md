<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Yes.** Use the sequence $x_j=2\cdot10^{j-1}$, $j\geq1$. Every nonempty finite sum has only digits $0$ and $2$ in decimal notation, with leading digit $2$, so none is a power of $10$, including $10^0=1$.

We still need an [idempotent ultrafilter](../../../../../../idempotent-ultrafilter.md) containing these sums; merely exhibiting an infinite set is insufficient. Put

$$
F_r=\operatorname{FS}(x_r,x_{r+1},\ldots),\qquad
K=\bigcap_{r\geq1}\overline{F_r},\qquad
\overline{F_r}=\{p:F_r\in p\}.
$$

The nonempty clopen sets $\overline{F_r}$ are nested, so compactness gives a nonempty compact $K$. This is the [tail finite-sums semigroup](../../../../../../tail-finite-sums-semigroup.md). To verify closure under addition, take $p,q\in K$ and fix $r$. For any $s\in F_r$, choose a finite representation of $s$ and then an index $t$ beyond every index in that representation. Disjointness of supports gives $F_t\subseteq F_r-s$, so $F_r-s\in q$. Consequently

$$
\{s:F_r-s\in q\}\supseteq F_r\in p,
$$

and $F_r\in p+q$. This holds for every $r$, proving $p+q\in K$. The [Ellis–Numakura lemma](../../../../../../ellis-numakura-lemma.md) now supplies an [idempotent ultrafilter](../../../../../../idempotent-ultrafilter.md) in $K$. It contains $F_1$, a subset of the non-powers of $10$, so by upward closure it contains **the whole set of non-powers of $10$**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
