<h1 id="25k/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Continue with $\sigma^2>0$. For each integer $K\geq1$, let $B_m(K)=\bigcup_{n\geq m}\{S_n/\sqrt n\geq K\}$. These events decrease with $m$, and their probabilities are at least $c_K>0$ by (iii). [Continuity from above of a measure](../../../../../../continuity-from-above-of-a-measure.md) gives

$$
\mathbb P\left(\frac{S_n}{\sqrt n}\geq K\text{ infinitely often}\right)\geq c_K.
$$

It is important not to assume that this exact threshold event is automatically a [tail event](../../../../../../tail-event.md): a vanishing change of partial sums can affect infinitely many exact comparisons at the threshold. Instead use

$$
L=\limsup_{n\to\infty}\frac{S_n}{\sqrt n}.
$$

For any fixed $m$, subtracting $S_m/\sqrt n\to0$ shows that $L=\limsup_{n\to\infty}(X_{m+1}+\cdots+X_n)/\sqrt n$. Thus $L$ is measurable with respect to every tail sigma-algebra. The event $\{L\geq K\}$ has positive probability by the preceding bound, so [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md) makes its probability one. Intersecting over all positive integers gives

$$
\boxed{\limsup_{n\to\infty}\frac{S_n}{\sqrt n}=+\infty\quad\text{almost surely}.}
$$

For any specified real $K>0$, this conclusion implies infinitely many $n$ with $S_n/\sqrt n\geq K$, completing both requests. In the excluded zero-variance case the limsup is zero.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [25K](../../25k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
