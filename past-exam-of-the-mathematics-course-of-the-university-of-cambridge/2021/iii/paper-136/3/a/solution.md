<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $a\in k$ and each $n$, choose a lift $x_n\in\mathcal O_K$ of the unique $p^n$th root $a^{p^{-n}}$, which exists because $k$ is a [perfect field](../../../../../../perfect-field.md). Define

$$
[a]=\lim_{n\to\infty}x_n^{p^n}.
$$

Changing $x_n$ by an element of the maximal ideal changes its $p^n$th power by an element whose valuation tends to infinity, so the limit exists and is independent of all choices. In characteristic $p$, the [Frobenius endomorphism](../../../../../../frobenius-endomorphism.md) satisfies $(x+y)^{p^n}=x^{p^n}+y^{p^n}$, making $[\mathord\cdot]$ a ring homomorphism lifting the identity on $k$. If $s:k\to\mathcal O_K$ is any other such section, then

$$
s(a)=s(a^{p^{-n}})^{p^n}
$$

for every $n$, and the same limiting construction forces $s(a)=[a]$. This proves uniqueness of the [Teichmuller lift](../../../../../../teichmuller-representative.md).

Choose a [uniformizer](../../../../../../uniformizer.md) $t$. Repeatedly subtracting the lift of the residue and dividing by $t$ gives every $x\in\mathcal O_K$ a unique convergent [Teichmuller expansion](../../../../../../teichmuller-expansion.md)

$$
x=\sum_{j\geq0}[a_j]t^j.
$$

Because the lift is a ring map, this identifies $\mathcal O_K$ with $k[[t]]$ and its fraction field with the [Laurent series field](../../../../../../laurent-series-field.md) $k((t))$. This is the [equal-characteristic complete discretely valued field](../../../../../../equal-characteristic-complete-discretely-valued-field.md) classification.

If $K$ is locally compact, its compact valuation ring has only finitely many disjoint residue-class balls. Thus $k$ is finite, as also follows from the [local compactness criterion for a complete non-Archimedean field](../../../../../../local-compactness-criterion-for-a-complete-non-archimedean-field.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
