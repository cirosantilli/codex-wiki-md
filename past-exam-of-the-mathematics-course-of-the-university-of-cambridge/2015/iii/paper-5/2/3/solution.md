<h1 id="2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the assumed separability of the [Hilbert space](../../../../../../hilbert-space-split.md) to choose a countable [Hilbertian basis](../../../../../../hilbertian-basis.md) $(e_j)$. For $\|f_n\|\le M$, every scalar sequence $\langle f_n,e_j\rangle$ is bounded. Repeated extraction followed by the [diagonal subsequence argument](../../../../../../diagonal-subsequence-argument.md) gives one subsequence with all these coordinates converging, say to $a_j$. The [Bessel inequality](../../../../../../bessel-s-inequality.md) gives $\sum_{j\le N}|a_j|^2\le M^2$ for every $N$, so $g=\sum_ja_je_j$ exists and $\|g\|\le M$.

For $h\in H$, let $h_N$ be its finite basis truncation. Coordinate convergence gives $\langle f_{\varphi(n)}-g,h_N\rangle\to0$, while the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) bounds the remaining inner product by $2M\|h-h_N\|$, uniformly in $n$. First choose $N$ large, then $n$ large. Thus

$$
\boxed{f_{\varphi(n)}\rightharpoonup g.}
$$

This proves the asserted sequential conclusion. To obtain actual compactness for the [weak topology](../../../../../../weak-topology-split.md), note that on a bounded ball it is induced by the metric

$$
d(v,w)=\sum_{j=1}^\infty2^{-j}\frac{|\langle v-w,e_j\rangle|}{1+|\langle v-w,e_j\rangle|}.
$$

Finite coordinates and the uniformly small tail show that $d$ gives coordinate convergence; uniform boundedness of the ball extends this to every inner product as above. Hence this metric induces exactly the restricted [weak topology](../../../../../../weak-topology-split.md). In a [metric space](../../../../../../metric-space.md), sequential compactness implies compactness. The closed unit ball is therefore **weakly compact**, and the limit remains inside it.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
