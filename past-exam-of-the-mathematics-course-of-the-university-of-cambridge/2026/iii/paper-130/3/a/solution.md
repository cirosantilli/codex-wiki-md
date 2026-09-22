<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The cofinite subsets of $\mathbb N$ form a proper filter. By [Zorn lemma](../../../../../../zorn-s-lemma.md), it extends to an [ultrafilter](../../../../../../ultrafilter.md) $\mathcal U$. Since $\mathcal U$ contains every cofinite set, it cannot contain a finite set, so it is nonprincipal.

Define the [Stone-Čech compactification of the natural numbers](../../../../../../stone-cech-compactification-of-the-natural-numbers.md) $\beta\mathbb N$ to be the set of ultrafilters on $\mathbb N$, with basic sets

$$
\bar A=\{\mathcal V:A\in\mathcal V\}.
$$

Since $\beta\mathbb N\setminus\bar A=\overline{\mathbb N\setminus A}$, these sets are clopen. If $\mathcal U\ne\mathcal V$, choose $A\in\mathcal U\setminus\mathcal V$; then $\bar A$ and $\overline{\mathbb N\setminus A}$ are disjoint neighbourhoods, proving Hausdorffness. For compactness, a family of basic closed sets with the finite-intersection property corresponds to a family of subsets of $\mathbb N$ with the finite-intersection property. Extend that family to an ultrafilter; the resulting point belongs to every closed set. The Alexander subbase theorem now proves compactness.

The [Hindman theorem](../../../../../../hindman-theorem.md) states that every finite colouring of $\mathbb N$ admits an infinite sequence $x_1,x_2,\ldots$ for which every nonempty finite sum of distinct terms has one colour. Let $\mathcal U\in\beta\mathbb N$ be an additive idempotent, and choose a colour class $A\in\mathcal U$. Put

$$
A^*=\{x\in A:A-x\in\mathcal U\}.
$$

Idempotence gives $A^*\in\mathcal U$, and $A^*-x\in\mathcal U$ whenever $x\in A^*$. Having selected $x_1,ldots,x_n$ with all finite sums in $A^*$, choose

$$
x_{n+1}\in A^*\cap
\bigcap_{s\in\operatorname{FS}(x_1,ldots,x_n)}(A^*-s).
$$

This finite intersection belongs to $\mathcal U$ and is nonempty. Induction keeps every finite sum in $A^*\subseteq A$, proving Hindman's theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
