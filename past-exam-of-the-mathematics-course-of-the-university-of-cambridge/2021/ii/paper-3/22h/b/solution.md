<h1 id="22h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Taking the [Fourier transform of a derivative](../../../../../../fourier-transform-of-a-derivative.md) gives

$$
iξ\mathbin\cdot\widehat B=\widehat f,\qquad ξ\mathbin\times\widehat B=0.
$$

Thus, away from $ξ=0$,

$$
\widehat B_j(ξ)=-iξ_j|ξ|^{-2}\widehat f(ξ).
$$

This formula determines the $L^2$ solution uniquely; a distribution supported only at $ξ=0$ cannot belong to $L^2$ unless it is zero.

For $|ξ|\leq1$, the [Fourier transform](../../../../../../fourier-transform.md) estimate $|\widehat f(ξ)|\leq C\|f\|_1$ and local integrability of $|ξ|^{-2}$ in three dimensions control the squared norm. For $|ξ|>1$,

$$
(1+|ξ|^2)^{s+1}|\widehat B_j|^2\leq C(1+|ξ|^2)^s|\widehat f|^2.
$$

The [Plancherel theorem](../../../../../../plancherel-theorem.md) therefore yields $\|B_j\|_{H^{s+1}}\leq C(\|f\|_1+\|f\|_{H^s})$. Finally the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) in three dimensions gives $H^{s+1}\subset C^1$ when $s+1>1+3/2$, namely when $s>3/2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22H](../../22h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
